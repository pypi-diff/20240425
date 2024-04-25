# Comparing `tmp/libmsiecf-python-20240209.tar.gz` & `tmp/libmsiecf-python-20240425.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmsiecf-python-20240209.tar", last modified: Fri Feb  9 06:20:51 2024, max compression
+gzip compressed data, was "libmsiecf-python-20240425.tar", last modified: Thu Apr 25 05:44:30 2024, max compression
```

## Comparing `libmsiecf-python-20240209.tar` & `libmsiecf-python-20240425.tar`

### file list

```diff
@@ -1,849 +1,849 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:50.000000 libmsiecf-20240209/libfole/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-02-09 04:59:07.000000 libmsiecf-20240209/libfole/libfole_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-09 04:59:07.000000 libmsiecf-20240209/libfole/libfole_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      665 2024-02-09 04:59:07.000000 libmsiecf-20240209/libfole/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1555 2024-02-09 04:59:07.000000 libmsiecf-20240209/libfole/libfole_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-09 04:59:07.000000 libmsiecf-20240209/libfole/libfole_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-02-09 04:59:07.000000 libmsiecf-20240209/libfole/libfole_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1407 2024-02-09 04:59:07.000000 libmsiecf-20240209/libfole/libfole_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-02-09 04:59:07.000000 libmsiecf-20240209/libfole/libfole_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3793 2024-02-09 04:59:07.000000 libmsiecf-20240209/libfole/libfole_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-09 04:59:07.000000 libmsiecf-20240209/libfole/libfole_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-09 04:59:07.000000 libmsiecf-20240209/libfole/libfole_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28462 2024-02-09 04:59:19.000000 libmsiecf-20240209/libfole/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-09 04:59:07.000000 libmsiecf-20240209/libfole/libfole_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      713 2024-02-09 04:49:21.000000 libmsiecf-20240209/libmsiecf.pc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-02-09 04:49:21.000000 libmsiecf-20240209/COPYING
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3278 2024-02-09 04:49:21.000000 libmsiecf-20240209/libmsiecf.spec.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-02-09 04:59:18.000000 libmsiecf-20240209/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 04:49:21.000000 libmsiecf-20240209/NEWS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:50.000000 libmsiecf-20240209/libmsiecf/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13908 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_leak_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1546 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_allocation_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1896 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1785 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_directory_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2764 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1729 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2072 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2133 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_property_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2477 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1608 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1674 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_item_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11972 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_redirected_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/msiecf_cache_directory_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1093 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2561 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_cache_directory_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2766 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42605 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_url.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16295 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_cache_directory_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1091 2024-02-09 04:59:27.000000 libmsiecf-20240209/libmsiecf/libmsiecf.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10392 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_file_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1565 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/msiecf_redr_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4711 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_hash.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1794 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_libfvalue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1595 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2023-12-03 09:11:36.000000 libmsiecf-20240209/libmsiecf/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4565 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_url.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2386 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/msiecf_file_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1839 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19708 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2141 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_redirected_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2211 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_redirected.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/msiecf_hash_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3824 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2154 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_file_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9416 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1932 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5642 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/msiecf_url_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3822 2024-02-09 04:59:27.000000 libmsiecf-20240209/libmsiecf/libmsiecf_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1406 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_hash_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8707 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_hash_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5787 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_directory_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43357 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_url_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5588 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2438 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_leak.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1215 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_hash.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2697 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57225 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3100 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_item_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2159 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_leak_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1309 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/msiecf_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7872 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_allocation_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3563 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_property_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2380 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/msiecf_leak_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13164 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_redirected.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37083 2024-02-09 04:59:19.000000 libmsiecf-20240209/libmsiecf/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16308 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_leak.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16919 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8439 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2987 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_url_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1278 2024-02-09 04:49:23.000000 libmsiecf-20240209/libmsiecf/libmsiecf_libfole.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:50.000000 libmsiecf-20240209/pymsiecf/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16625 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_datetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_libmsiecf.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4156 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33969 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8473 2024-02-09 04:51:50.000000 libmsiecf-20240209/pymsiecf/pymsiecf_leak.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1637 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_item_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1645 2024-02-09 04:51:50.000000 libmsiecf-20240209/pymsiecf/pymsiecf_leak.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9063 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_items.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1148 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1837 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_datetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2036 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44879 2024-02-09 04:51:50.000000 libmsiecf-20240209/pymsiecf/pymsiecf_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1574 2023-12-03 09:11:34.000000 libmsiecf-20240209/pymsiecf/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3326 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10689 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_cache_directories.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5844 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_item_types.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6849 2024-02-09 04:51:50.000000 libmsiecf-20240209/pymsiecf/pymsiecf_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9566 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2363 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_items.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1553 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18096 2024-02-09 04:51:50.000000 libmsiecf-20240209/pymsiecf/pymsiecf.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5448 2024-02-09 04:51:50.000000 libmsiecf-20240209/pymsiecf/pymsiecf_redirected.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1839 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1434 2024-02-09 04:51:50.000000 libmsiecf-20240209/pymsiecf/pymsiecf_redirected.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9567 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_url_types.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3110 2024-02-09 04:51:50.000000 libmsiecf-20240209/pymsiecf/pymsiecf_url.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29857 2024-02-09 04:51:50.000000 libmsiecf-20240209/pymsiecf/pymsiecf_url.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8894 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1528 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6182 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_item_flags.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1549 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1873 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1637 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_item_flags.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55745 2024-02-09 04:59:19.000000 libmsiecf-20240209/pymsiecf/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_cache_directories.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-02-09 04:49:23.000000 libmsiecf-20240209/pymsiecf/pymsiecf_url_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4568 2024-02-09 04:51:50.000000 libmsiecf-20240209/pymsiecf/pymsiecf_file.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-02-09 04:59:19.000000 libmsiecf-20240209/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:50.000000 libmsiecf-20240209/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-09 04:59:06.000000 libmsiecf-20240209/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-02-09 04:59:06.000000 libmsiecf-20240209/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-02-09 04:59:06.000000 libmsiecf-20240209/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-09 04:59:06.000000 libmsiecf-20240209/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      681 2024-02-09 04:59:06.000000 libmsiecf-20240209/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-09 04:59:06.000000 libmsiecf-20240209/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-09 04:59:06.000000 libmsiecf-20240209/libfguid/libfguid_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-02-09 04:59:06.000000 libmsiecf-20240209/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-02-09 04:59:06.000000 libmsiecf-20240209/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-02-09 04:59:06.000000 libmsiecf-20240209/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-02-09 04:59:06.000000 libmsiecf-20240209/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28539 2024-02-09 04:59:19.000000 libmsiecf-20240209/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-09 04:59:06.000000 libmsiecf-20240209/libfguid/libfguid_error.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:49.000000 libmsiecf-20240209/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3956 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/libfole.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-02-09 04:59:14.000000 libmsiecf-20240209/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-02-09 04:59:14.000000 libmsiecf-20240209/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-02-09 04:59:14.000000 libmsiecf-20240209/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-02-09 04:59:14.000000 libmsiecf-20240209/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-02-09 04:59:14.000000 libmsiecf-20240209/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 10:23:50.000000 libmsiecf-20240209/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19791 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/libfvalue.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:11:38.000000 libmsiecf-20240209/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:49.000000 libmsiecf-20240209/include/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:49.000000 libmsiecf-20240209/include/libmsiecf/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2668 2024-02-09 04:49:22.000000 libmsiecf-20240209/include/libmsiecf/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2666 2024-02-09 04:59:27.000000 libmsiecf-20240209/include/libmsiecf/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4986 2024-02-09 04:49:22.000000 libmsiecf-20240209/include/libmsiecf/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4855 2024-02-09 04:59:27.000000 libmsiecf-20240209/include/libmsiecf/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-09 04:49:22.000000 libmsiecf-20240209/include/libmsiecf/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-02-09 04:49:22.000000 libmsiecf-20240209/include/libmsiecf/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1436 2024-02-09 04:49:22.000000 libmsiecf-20240209/include/libmsiecf/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1499 2024-02-09 04:59:27.000000 libmsiecf-20240209/include/libmsiecf/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5422 2024-02-09 04:49:22.000000 libmsiecf-20240209/include/libmsiecf/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23293 2024-02-09 04:59:27.000000 libmsiecf-20240209/include/libmsiecf.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      489 2024-02-09 04:49:21.000000 libmsiecf-20240209/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23293 2024-02-09 04:49:22.000000 libmsiecf-20240209/include/libmsiecf.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27104 2024-02-09 04:59:18.000000 libmsiecf-20240209/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:49.000000 libmsiecf-20240209/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-02-09 04:49:22.000000 libmsiecf-20240209/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-02-09 04:49:22.000000 libmsiecf-20240209/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-02-09 04:49:22.000000 libmsiecf-20240209/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-02-09 04:49:22.000000 libmsiecf-20240209/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-09 04:49:22.000000 libmsiecf-20240209/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-02-09 04:49:22.000000 libmsiecf-20240209/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-02-09 04:49:22.000000 libmsiecf-20240209/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-02-09 04:49:21.000000 libmsiecf-20240209/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-02-09 04:49:22.000000 libmsiecf-20240209/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-02-09 04:59:27.000000 libmsiecf-20240209/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15639 2024-02-09 04:59:18.000000 libmsiecf-20240209/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16577 2024-02-09 04:59:27.000000 libmsiecf-20240209/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-02-09 04:49:22.000000 libmsiecf-20240209/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-02-09 04:49:22.000000 libmsiecf-20240209/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-02-09 04:49:22.000000 libmsiecf-20240209/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24092 2024-02-09 04:59:18.000000 libmsiecf-20240209/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:49.000000 libmsiecf-20240209/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-02-09 04:58:58.000000 libmsiecf-20240209/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-02-09 04:58:58.000000 libmsiecf-20240209/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-02-09 04:58:58.000000 libmsiecf-20240209/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-02-09 04:58:58.000000 libmsiecf-20240209/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-09 04:58:58.000000 libmsiecf-20240209/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-09 04:58:58.000000 libmsiecf-20240209/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-02-09 04:58:58.000000 libmsiecf-20240209/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-02-09 04:58:58.000000 libmsiecf-20240209/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-02-09 04:58:58.000000 libmsiecf-20240209/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-02-09 04:58:58.000000 libmsiecf-20240209/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29095 2024-02-09 04:59:18.000000 libmsiecf-20240209/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-09 04:58:58.000000 libmsiecf-20240209/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-02-09 04:58:58.000000 libmsiecf-20240209/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-02-09 04:58:58.000000 libmsiecf-20240209/libclocale/libclocale_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2304 2023-12-03 10:25:10.000000 libmsiecf-20240209/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:50.000000 libmsiecf-20240209/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32554 2024-02-09 04:59:18.000000 libmsiecf-20240209/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-02-09 04:58:52.000000 libmsiecf-20240209/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:11:33.000000 libmsiecf-20240209/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-02-09 04:59:18.000000 libmsiecf-20240209/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:49.000000 libmsiecf-20240209/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1028 2024-02-09 04:49:23.000000 libmsiecf-20240209/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:49.000000 libmsiecf-20240209/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-02-09 04:49:21.000000 libmsiecf-20240209/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2143 2024-02-09 04:49:21.000000 libmsiecf-20240209/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-02-09 04:49:21.000000 libmsiecf-20240209/dpkg/libmsiecf-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      777 2024-02-09 04:49:21.000000 libmsiecf-20240209/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-02-09 04:49:21.000000 libmsiecf-20240209/dpkg/libmsiecf.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      122 2024-02-09 04:49:21.000000 libmsiecf-20240209/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      141 2024-02-09 04:59:27.000000 libmsiecf-20240209/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-02-09 04:49:21.000000 libmsiecf-20240209/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-02-09 04:49:21.000000 libmsiecf-20240209/dpkg/libmsiecf-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-02-09 04:49:21.000000 libmsiecf-20240209/dpkg/libmsiecf-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      485 2024-02-09 04:59:27.000000 libmsiecf-20240209/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-02-09 04:49:21.000000 libmsiecf-20240209/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1826070 2024-02-09 04:59:17.000000 libmsiecf-20240209/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-02-09 04:59:18.000000 libmsiecf-20240209/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-02-09 04:59:18.000000 libmsiecf-20240209/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecf_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5584 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/msiecf_test_error/msiecf_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/libfole/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4605 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/libfole/libfole.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38509 2024-02-09 04:51:09.000000 libmsiecf-20240209/msvscpp/libmsiecf.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecf_test_property_type/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5857 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/msiecf_test_property_type/msiecf_test_property_type.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecf_test_allocation_table/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6203 2024-02-09 04:51:09.000000 libmsiecf-20240209/msvscpp/msiecf_test_allocation_table/msiecf_test_allocation_table.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/libmsiecf/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10873 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/libmsiecf/libmsiecf.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecf_test_cache_directory_table/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6134 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/msiecf_test_cache_directory_table/msiecf_test_cache_directory_table.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/pymsiecf/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7930 2024-02-09 04:51:09.000000 libmsiecf-20240209/msvscpp/pymsiecf/pymsiecf.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecf_test_leak_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6104 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/msiecf_test_leak_values/msiecf_test_leak_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecf_test_file/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6336 2024-02-09 04:51:09.000000 libmsiecf-20240209/msvscpp/msiecf_test_file/msiecf_test_file.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1946 2024-02-09 04:51:09.000000 libmsiecf-20240209/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecfinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6455 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/msiecfinfo/msiecfinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecf_test_file_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6104 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/msiecf_test_file_header/msiecf_test_file_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecf_test_hash_table/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6185 2024-02-09 04:51:09.000000 libmsiecf-20240209/msvscpp/msiecf_test_hash_table/msiecf_test_hash_table.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecf_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5781 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/msiecf_test_tools_signal/msiecf_test_tools_signal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecf_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6510 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/msiecf_test_support/msiecf_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecf_test_redirected_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6122 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/msiecf_test_redirected_values/msiecf_test_redirected_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecf_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5672 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/msiecf_test_notify/msiecf_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecf_test_item/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5830 2024-02-09 04:51:09.000000 libmsiecf-20240209/msvscpp/msiecf_test_item/msiecf_test_item.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecf_test_tools_info_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5946 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/msiecf_test_tools_info_handle/msiecf_test_tools_info_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecf_test_url/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5663 2024-02-09 04:51:09.000000 libmsiecf-20240209/msvscpp/msiecf_test_url/msiecf_test_url.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecf_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5781 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/msiecf_test_tools_output/msiecf_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecf_test_leak/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5666 2024-02-09 04:51:09.000000 libmsiecf-20240209/msvscpp/msiecf_test_leak/msiecf_test_leak.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecf_test_url_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6101 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/msiecf_test_url_values/msiecf_test_url_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23006 2024-02-09 04:59:19.000000 libmsiecf-20240209/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8010 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/libfvalue/libfvalue.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecf_test_item_descriptor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5863 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/msiecf_test_item_descriptor/msiecf_test_item_descriptor.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecf_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5845 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/msiecf_test_io_handle/msiecf_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecfexport/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6625 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/msiecfexport/msiecfexport.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/libfdatetime/libfdatetime.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecf_test_redirected/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5684 2024-02-09 04:51:09.000000 libmsiecf-20240209/msvscpp/msiecf_test_redirected/msiecf_test_redirected.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/msvscpp/msiecf_test_directory_descriptor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5878 2024-02-09 04:49:42.000000 libmsiecf-20240209/msvscpp/msiecf_test_directory_descriptor/msiecf_test_directory_descriptor.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      378 2024-02-09 04:49:22.000000 libmsiecf-20240209/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:50.000000 libmsiecf-20240209/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-09 04:58:56.000000 libmsiecf-20240209/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-02-09 04:58:56.000000 libmsiecf-20240209/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-09 04:58:56.000000 libmsiecf-20240209/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-09 04:58:56.000000 libmsiecf-20240209/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-02-09 04:58:56.000000 libmsiecf-20240209/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-02-09 04:58:56.000000 libmsiecf-20240209/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-02-09 04:58:56.000000 libmsiecf-20240209/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-09 04:58:56.000000 libmsiecf-20240209/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-09 04:58:56.000000 libmsiecf-20240209/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-02-09 04:58:56.000000 libmsiecf-20240209/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-09 04:58:56.000000 libmsiecf-20240209/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-09 04:58:56.000000 libmsiecf-20240209/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-09 04:58:56.000000 libmsiecf-20240209/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-09 04:58:56.000000 libmsiecf-20240209/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-02-09 04:58:56.000000 libmsiecf-20240209/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-09 04:58:56.000000 libmsiecf-20240209/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-02-09 04:58:56.000000 libmsiecf-20240209/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29859 2024-02-09 04:59:18.000000 libmsiecf-20240209/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-09 04:58:56.000000 libmsiecf-20240209/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-09 04:58:56.000000 libmsiecf-20240209/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-02-09 04:58:56.000000 libmsiecf-20240209/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-02-09 04:58:56.000000 libmsiecf-20240209/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      381 2024-02-09 04:49:21.000000 libmsiecf-20240209/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-02-09 04:59:18.000000 libmsiecf-20240209/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:49.000000 libmsiecf-20240209/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31543 2024-02-09 04:59:18.000000 libmsiecf-20240209/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-09 04:58:54.000000 libmsiecf-20240209/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-02-09 04:49:21.000000 libmsiecf-20240209/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      486 2024-02-09 04:49:21.000000 libmsiecf-20240209/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-02-09 04:59:18.000000 libmsiecf-20240209/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-02-09 04:49:21.000000 libmsiecf-20240209/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-02-09 04:49:21.000000 libmsiecf-20240209/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:11:33.000000 libmsiecf-20240209/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:49.000000 libmsiecf-20240209/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31949 2024-02-09 04:59:19.000000 libmsiecf-20240209/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-02-09 04:59:03.000000 libmsiecf-20240209/libcthreads/libcthreads_queue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2024-02-09 04:59:27.000000 libmsiecf-20240209/libmsiecf.spec
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-02-09 04:59:19.000000 libmsiecf-20240209/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:50.000000 libmsiecf-20240209/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-02-09 04:59:01.000000 libmsiecf-20240209/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-09 04:59:01.000000 libmsiecf-20240209/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-02-09 04:59:01.000000 libmsiecf-20240209/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-02-09 04:59:01.000000 libmsiecf-20240209/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-09 04:59:01.000000 libmsiecf-20240209/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-09 04:59:01.000000 libmsiecf-20240209/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-09 04:59:01.000000 libmsiecf-20240209/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-02-09 04:59:01.000000 libmsiecf-20240209/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-02-09 04:59:01.000000 libmsiecf-20240209/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-09 04:59:01.000000 libmsiecf-20240209/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-09 04:59:01.000000 libmsiecf-20240209/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-09 04:59:01.000000 libmsiecf-20240209/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29137 2024-02-09 04:59:18.000000 libmsiecf-20240209/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-09 04:59:01.000000 libmsiecf-20240209/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-09 04:59:01.000000 libmsiecf-20240209/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-02-09 04:59:01.000000 libmsiecf-20240209/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-02-09 04:59:01.000000 libmsiecf-20240209/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7753 2023-12-03 09:11:33.000000 libmsiecf-20240209/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:50.000000 libmsiecf-20240209/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10780 2024-02-09 04:49:23.000000 libmsiecf-20240209/manuals/libmsiecf.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2514 2024-02-09 04:49:23.000000 libmsiecf-20240209/manuals/msiecfexport.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      198 2023-12-03 09:11:34.000000 libmsiecf-20240209/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1890 2024-02-09 04:49:23.000000 libmsiecf-20240209/manuals/msiecfinfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26102 2024-02-09 04:59:19.000000 libmsiecf-20240209/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2003 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_redirected.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1821 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7407 2024-02-09 04:51:50.000000 libmsiecf-20240209/tests/pymsiecf_test_file.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15088 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_redirected_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13465 2024-02-09 04:51:09.000000 libmsiecf-20240209/tests/msiecf_test_file_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1468 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1557 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8291 2024-02-09 04:51:09.000000 libmsiecf-20240209/tests/msiecf_test_io_handle.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4071 2024-02-09 04:51:50.000000 libmsiecf-20240209/tests/test_tools.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6365 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_item_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14515 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4215 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_tools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1914 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_property_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3179 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_error.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3327 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/test_msiecfinfo.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3340 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/test_msiecfexport.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10375 2024-02-09 04:51:09.000000 libmsiecf-20240209/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2917 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_url.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30553 2024-02-09 04:51:09.000000 libmsiecf-20240209/tests/msiecf_test_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9739 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_directory_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2094 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_leak.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3456 2024-02-09 04:51:50.000000 libmsiecf-20240209/tests/pymsiecf_test_support.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4084 2024-02-09 04:52:24.000000 libmsiecf-20240209/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30868 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_hash_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2970 2024-02-09 04:51:09.000000 libmsiecf-20240209/tests/msiecf_test_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1745 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15890 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_leak_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4747 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17885 2024-02-09 04:51:09.000000 libmsiecf-20240209/tests/msiecf_test_cache_directory_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1713 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5678 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_tools_info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6034 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_allocation_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2469 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_tools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18714 2024-02-09 04:51:09.000000 libmsiecf-20240209/tests/msiecf_test_url_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      989 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_libmsiecf.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    72034 2024-02-09 04:59:19.000000 libmsiecf-20240209/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4539 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4370 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8609 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1712 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13271 2024-02-09 04:49:23.000000 libmsiecf-20240209/tests/msiecf_test_functions.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4237 2024-02-09 04:51:50.000000 libmsiecf-20240209/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:51.000000 libmsiecf-20240209/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      977 2024-02-09 04:49:23.000000 libmsiecf-20240209/ossfuzz/ossfuzz_libmsiecf.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1398 2023-12-03 09:11:37.000000 libmsiecf-20240209/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-02-09 04:49:23.000000 libmsiecf-20240209/ossfuzz/ossfuzz_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2641 2024-02-09 04:49:23.000000 libmsiecf-20240209/ossfuzz/item_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2229 2024-02-09 04:49:23.000000 libmsiecf-20240209/ossfuzz/file_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33122 2024-02-09 04:59:19.000000 libmsiecf-20240209/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-02-09 04:59:14.000000 libmsiecf-20240209/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:50.000000 libmsiecf-20240209/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-02-09 04:59:02.000000 libmsiecf-20240209/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-02-09 04:59:02.000000 libmsiecf-20240209/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-02-09 04:59:02.000000 libmsiecf-20240209/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-02-09 04:59:02.000000 libmsiecf-20240209/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-09 04:59:02.000000 libmsiecf-20240209/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-02-09 04:59:02.000000 libmsiecf-20240209/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-09 04:59:02.000000 libmsiecf-20240209/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-02-09 04:59:02.000000 libmsiecf-20240209/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-09 04:59:02.000000 libmsiecf-20240209/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-02-09 04:59:02.000000 libmsiecf-20240209/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-09 04:59:02.000000 libmsiecf-20240209/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-02-09 04:59:02.000000 libmsiecf-20240209/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-09 04:59:02.000000 libmsiecf-20240209/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-09 04:59:02.000000 libmsiecf-20240209/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-09 04:59:02.000000 libmsiecf-20240209/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-02-09 04:59:02.000000 libmsiecf-20240209/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29917 2024-02-09 04:59:19.000000 libmsiecf-20240209/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-02-09 04:59:02.000000 libmsiecf-20240209/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-02-09 04:59:02.000000 libmsiecf-20240209/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:50.000000 libmsiecf-20240209/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:11:36.000000 libmsiecf-20240209/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:11:36.000000 libmsiecf-20240209/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:11:36.000000 libmsiecf-20240209/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:11:36.000000 libmsiecf-20240209/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:11:36.000000 libmsiecf-20240209/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:11:36.000000 libmsiecf-20240209/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:11:36.000000 libmsiecf-20240209/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:11:36.000000 libmsiecf-20240209/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:11:36.000000 libmsiecf-20240209/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1855 2024-02-09 04:59:27.000000 libmsiecf-20240209/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:11:36.000000 libmsiecf-20240209/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:11:36.000000 libmsiecf-20240209/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:50.000000 libmsiecf-20240209/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4197 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52661 2024-02-09 04:59:19.000000 libmsiecf-20240209/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-02-09 04:59:11.000000 libmsiecf-20240209/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40188 2024-02-09 04:59:18.000000 libmsiecf-20240209/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:50.000000 libmsiecf-20240209/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_split_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_split_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1684 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_split_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_binary_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_value_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_split_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_floating_point.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_binary_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_value_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34374 2024-02-09 04:59:19.000000 libmsiecf-20240209/libfvalue/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_floating_point.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-02-09 04:59:08.000000 libmsiecf-20240209/libfvalue/libfvalue_libuna.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:49.000000 libmsiecf-20240209/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-09 04:58:59.000000 libmsiecf-20240209/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-09 04:58:59.000000 libmsiecf-20240209/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-02-09 04:58:59.000000 libmsiecf-20240209/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-02-09 04:58:59.000000 libmsiecf-20240209/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-02-09 04:58:59.000000 libmsiecf-20240209/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-09 04:58:59.000000 libmsiecf-20240209/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-02-09 04:58:59.000000 libmsiecf-20240209/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-02-09 04:58:59.000000 libmsiecf-20240209/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-02-09 04:58:59.000000 libmsiecf-20240209/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-02-09 04:58:59.000000 libmsiecf-20240209/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-02-09 04:58:59.000000 libmsiecf-20240209/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28971 2024-02-09 04:59:18.000000 libmsiecf-20240209/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-09 04:58:59.000000 libmsiecf-20240209/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-02-09 04:58:59.000000 libmsiecf-20240209/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:50.000000 libmsiecf-20240209/msiecftools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-02-09 04:49:23.000000 libmsiecf-20240209/msiecftools/msiecftools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1216 2024-02-09 04:49:23.000000 libmsiecf-20240209/msiecftools/msiecftools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4539 2024-02-09 04:49:23.000000 libmsiecf-20240209/msiecftools/msiecftools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2298 2024-02-09 04:51:50.000000 libmsiecf-20240209/msiecftools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1486 2024-02-09 04:49:23.000000 libmsiecf-20240209/msiecftools/msiecftools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-02-09 04:49:23.000000 libmsiecf-20240209/msiecftools/msiecftools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1784 2024-02-09 04:49:23.000000 libmsiecf-20240209/msiecftools/msiecftools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2005 2023-12-03 09:11:34.000000 libmsiecf-20240209/msiecftools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12400 2024-02-09 04:51:50.000000 libmsiecf-20240209/msiecftools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41188 2024-02-09 04:49:23.000000 libmsiecf-20240209/msiecftools/export_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-09 04:49:23.000000 libmsiecf-20240209/msiecftools/msiecftools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7414 2024-02-09 04:51:50.000000 libmsiecf-20240209/msiecftools/msiecfinfo.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5776 2024-02-09 04:49:23.000000 libmsiecf-20240209/msiecftools/msiecftools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1751 2024-02-09 04:49:23.000000 libmsiecf-20240209/msiecftools/msiecftools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9132 2024-02-09 04:49:23.000000 libmsiecf-20240209/msiecftools/msiecfexport.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1507 2024-02-09 04:49:23.000000 libmsiecf-20240209/msiecftools/msiecftools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5939 2024-02-09 04:49:23.000000 libmsiecf-20240209/msiecftools/log_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1481 2024-02-09 04:49:23.000000 libmsiecf-20240209/msiecftools/msiecftools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3736 2024-02-09 04:49:23.000000 libmsiecf-20240209/msiecftools/export_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32430 2024-02-09 04:59:19.000000 libmsiecf-20240209/msiecftools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1675 2024-02-09 04:49:23.000000 libmsiecf-20240209/msiecftools/log_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3965 2024-02-09 04:49:23.000000 libmsiecf-20240209/msiecftools/msiecftools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      989 2024-02-09 04:49:23.000000 libmsiecf-20240209/msiecftools/msiecftools_libmsiecf.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1774 2024-02-09 04:49:23.000000 libmsiecf-20240209/msiecftools/msiecftools_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-02-09 04:49:23.000000 libmsiecf-20240209/msiecftools/msiecftools_libcnotify.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:49.000000 libmsiecf-20240209/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-02-09 04:58:55.000000 libmsiecf-20240209/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-02-09 04:58:55.000000 libmsiecf-20240209/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-09 04:58:55.000000 libmsiecf-20240209/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-02-09 04:58:55.000000 libmsiecf-20240209/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-02-09 04:58:55.000000 libmsiecf-20240209/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-09 04:58:55.000000 libmsiecf-20240209/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-02-09 04:58:55.000000 libmsiecf-20240209/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-02-09 04:58:55.000000 libmsiecf-20240209/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-02-09 04:58:55.000000 libmsiecf-20240209/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-09 04:58:55.000000 libmsiecf-20240209/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-09 04:58:55.000000 libmsiecf-20240209/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28484 2024-02-09 04:59:18.000000 libmsiecf-20240209/libcerror/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-09 06:20:50.000000 libmsiecf-20240209/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1148 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31710 2024-02-09 04:59:19.000000 libmsiecf-20240209/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-02-09 04:59:04.000000 libmsiecf-20240209/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56797 2024-02-09 04:59:16.000000 libmsiecf-20240209/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7505 2024-02-09 04:49:21.000000 libmsiecf-20240209/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      417 2024-02-09 06:20:51.717468 libmsiecf-20240209/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:27.000000 libmsiecf-20240425/libfole/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-25 05:26:06.000000 libmsiecf-20240425/libfole/libfole_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-25 05:26:06.000000 libmsiecf-20240425/libfole/libfole_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      661 2024-04-25 05:26:06.000000 libmsiecf-20240425/libfole/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1555 2024-04-25 05:26:06.000000 libmsiecf-20240425/libfole/libfole_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-25 05:26:06.000000 libmsiecf-20240425/libfole/libfole_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-04-25 05:26:06.000000 libmsiecf-20240425/libfole/libfole_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1407 2024-04-25 05:26:06.000000 libmsiecf-20240425/libfole/libfole_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-04-25 05:26:06.000000 libmsiecf-20240425/libfole/libfole_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3793 2024-04-25 05:26:06.000000 libmsiecf-20240425/libfole/libfole_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-25 05:26:06.000000 libmsiecf-20240425/libfole/libfole_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-25 05:26:06.000000 libmsiecf-20240425/libfole/libfole_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28609 2024-04-25 05:26:21.000000 libmsiecf-20240425/libfole/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-25 05:26:06.000000 libmsiecf-20240425/libfole/libfole_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      713 2024-04-25 04:44:23.000000 libmsiecf-20240425/libmsiecf.pc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-04-25 04:44:23.000000 libmsiecf-20240425/COPYING
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3278 2024-04-25 04:44:23.000000 libmsiecf-20240425/libmsiecf.spec.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-04-25 05:26:21.000000 libmsiecf-20240425/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 04:44:23.000000 libmsiecf-20240425/NEWS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:28.000000 libmsiecf-20240425/libmsiecf/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13908 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_leak_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1546 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_allocation_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1896 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1785 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_directory_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2764 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1729 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2072 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2133 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_property_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2477 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1608 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1674 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_item_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11972 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_redirected_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/msiecf_cache_directory_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1093 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2561 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_cache_directory_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2766 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42605 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_url.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16295 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_cache_directory_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1091 2024-04-25 05:26:39.000000 libmsiecf-20240425/libmsiecf/libmsiecf.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10392 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_file_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1565 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/msiecf_redr_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4711 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_hash.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1794 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_libfvalue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1595 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2865 2024-04-25 04:55:53.000000 libmsiecf-20240425/libmsiecf/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4565 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_url.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2386 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/msiecf_file_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1839 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19708 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2141 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_redirected_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2211 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_redirected.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/msiecf_hash_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3824 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2154 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_file_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9416 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1932 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5642 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/msiecf_url_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3822 2024-04-25 05:26:38.000000 libmsiecf-20240425/libmsiecf/libmsiecf_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1406 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_hash_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8707 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_hash_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5787 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_directory_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43357 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_url_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5588 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2438 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_leak.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1215 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_hash.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2697 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57225 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3100 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_item_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2159 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_leak_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1309 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/msiecf_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7872 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_allocation_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3563 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_property_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2380 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/msiecf_leak_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13164 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_redirected.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38073 2024-04-25 05:26:21.000000 libmsiecf-20240425/libmsiecf/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16308 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_leak.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16919 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8439 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2987 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_url_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1278 2024-04-25 04:44:27.000000 libmsiecf-20240425/libmsiecf/libmsiecf_libfole.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:28.000000 libmsiecf-20240425/pymsiecf/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16625 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_datetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_libmsiecf.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4156 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33969 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8473 2024-04-25 04:45:59.000000 libmsiecf-20240425/pymsiecf/pymsiecf_leak.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1637 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_item_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1645 2024-04-25 04:45:59.000000 libmsiecf-20240425/pymsiecf/pymsiecf_leak.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9063 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_items.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1148 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1837 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_datetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2036 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44879 2024-04-25 04:45:59.000000 libmsiecf-20240425/pymsiecf/pymsiecf_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1570 2024-04-25 04:55:39.000000 libmsiecf-20240425/pymsiecf/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3326 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10689 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_cache_directories.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5844 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_item_types.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6849 2024-04-25 04:45:59.000000 libmsiecf-20240425/pymsiecf/pymsiecf_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9566 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2363 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_items.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1553 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18096 2024-04-25 04:45:59.000000 libmsiecf-20240425/pymsiecf/pymsiecf.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5448 2024-04-25 04:45:59.000000 libmsiecf-20240425/pymsiecf/pymsiecf_redirected.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1839 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1434 2024-04-25 04:45:59.000000 libmsiecf-20240425/pymsiecf/pymsiecf_redirected.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9567 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_url_types.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3110 2024-04-25 04:45:59.000000 libmsiecf-20240425/pymsiecf/pymsiecf_url.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29857 2024-04-25 04:45:59.000000 libmsiecf-20240425/pymsiecf/pymsiecf_url.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8894 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1528 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6182 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_item_flags.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1549 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1873 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1637 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_item_flags.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56631 2024-04-25 05:26:21.000000 libmsiecf-20240425/pymsiecf/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_cache_directories.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-04-25 04:44:28.000000 libmsiecf-20240425/pymsiecf/pymsiecf_url_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4568 2024-04-25 04:45:59.000000 libmsiecf-20240425/pymsiecf/pymsiecf_file.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-04-25 05:26:21.000000 libmsiecf-20240425/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:27.000000 libmsiecf-20240425/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-25 05:26:05.000000 libmsiecf-20240425/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-04-25 05:26:05.000000 libmsiecf-20240425/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-04-25 05:26:05.000000 libmsiecf-20240425/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-25 05:26:05.000000 libmsiecf-20240425/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-04-25 05:26:05.000000 libmsiecf-20240425/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-25 05:26:05.000000 libmsiecf-20240425/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-25 05:26:05.000000 libmsiecf-20240425/libfguid/libfguid_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-04-25 05:26:05.000000 libmsiecf-20240425/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-04-25 05:26:05.000000 libmsiecf-20240425/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-04-25 05:26:05.000000 libmsiecf-20240425/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-04-25 05:26:05.000000 libmsiecf-20240425/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28689 2024-04-25 05:26:21.000000 libmsiecf-20240425/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-25 05:26:05.000000 libmsiecf-20240425/libfguid/libfguid_error.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:25.000000 libmsiecf-20240425/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-04-25 04:44:30.000000 libmsiecf-20240425/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18489 2024-04-25 04:44:30.000000 libmsiecf-20240425/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:11:38.000000 libmsiecf-20240425/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-04-25 04:44:30.000000 libmsiecf-20240425/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:11:38.000000 libmsiecf-20240425/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:11:38.000000 libmsiecf-20240425/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-04-25 04:44:30.000000 libmsiecf-20240425/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:11:38.000000 libmsiecf-20240425/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:11:38.000000 libmsiecf-20240425/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4187 2024-04-25 04:44:30.000000 libmsiecf-20240425/m4/libfole.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-04-25 04:44:30.000000 libmsiecf-20240425/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-04-25 04:44:30.000000 libmsiecf-20240425/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-04-25 04:44:30.000000 libmsiecf-20240425/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-04-25 04:44:30.000000 libmsiecf-20240425/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-04-25 04:44:30.000000 libmsiecf-20240425/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-04-25 05:26:16.000000 libmsiecf-20240425/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-04-25 05:26:15.000000 libmsiecf-20240425/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:11:38.000000 libmsiecf-20240425/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-04-25 05:26:15.000000 libmsiecf-20240425/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:11:38.000000 libmsiecf-20240425/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-04-25 04:44:30.000000 libmsiecf-20240425/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-04-25 04:44:30.000000 libmsiecf-20240425/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-04-25 04:44:30.000000 libmsiecf-20240425/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-04-25 04:44:30.000000 libmsiecf-20240425/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:11:38.000000 libmsiecf-20240425/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-04-25 05:26:16.000000 libmsiecf-20240425/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:11:38.000000 libmsiecf-20240425/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:11:38.000000 libmsiecf-20240425/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-04-25 05:26:15.000000 libmsiecf-20240425/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:11:38.000000 libmsiecf-20240425/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-04-25 04:44:30.000000 libmsiecf-20240425/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20032 2024-04-25 04:44:30.000000 libmsiecf-20240425/m4/libfvalue.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:11:38.000000 libmsiecf-20240425/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-04-25 04:44:30.000000 libmsiecf-20240425/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:25.000000 libmsiecf-20240425/include/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:25.000000 libmsiecf-20240425/include/libmsiecf/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2668 2024-04-25 04:44:26.000000 libmsiecf-20240425/include/libmsiecf/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2666 2024-04-25 05:26:38.000000 libmsiecf-20240425/include/libmsiecf/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4986 2024-04-25 04:44:26.000000 libmsiecf-20240425/include/libmsiecf/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4855 2024-04-25 05:26:38.000000 libmsiecf-20240425/include/libmsiecf/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-25 04:44:26.000000 libmsiecf-20240425/include/libmsiecf/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-04-25 04:44:26.000000 libmsiecf-20240425/include/libmsiecf/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1436 2024-04-25 04:44:26.000000 libmsiecf-20240425/include/libmsiecf/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1499 2024-04-25 05:26:38.000000 libmsiecf-20240425/include/libmsiecf/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5422 2024-04-25 04:44:26.000000 libmsiecf-20240425/include/libmsiecf/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23293 2024-04-25 05:26:38.000000 libmsiecf-20240425/include/libmsiecf.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      440 2024-04-25 04:54:18.000000 libmsiecf-20240425/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23293 2024-04-25 04:44:26.000000 libmsiecf-20240425/include/libmsiecf.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27084 2024-04-25 05:26:21.000000 libmsiecf-20240425/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:25.000000 libmsiecf-20240425/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-25 04:44:26.000000 libmsiecf-20240425/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-04-25 04:44:26.000000 libmsiecf-20240425/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-04-25 04:44:26.000000 libmsiecf-20240425/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-04-25 04:44:26.000000 libmsiecf-20240425/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-25 04:44:26.000000 libmsiecf-20240425/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-25 04:44:26.000000 libmsiecf-20240425/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-04-25 04:44:26.000000 libmsiecf-20240425/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-04-25 04:54:18.000000 libmsiecf-20240425/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-04-25 04:44:26.000000 libmsiecf-20240425/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-04-25 05:26:38.000000 libmsiecf-20240425/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15639 2024-04-25 05:26:20.000000 libmsiecf-20240425/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16577 2024-04-25 05:26:39.000000 libmsiecf-20240425/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-04-25 04:44:26.000000 libmsiecf-20240425/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-04-25 04:44:26.000000 libmsiecf-20240425/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-04-25 04:44:26.000000 libmsiecf-20240425/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24099 2024-04-25 05:26:21.000000 libmsiecf-20240425/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:26.000000 libmsiecf-20240425/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-04-25 05:25:57.000000 libmsiecf-20240425/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-04-25 05:25:57.000000 libmsiecf-20240425/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-04-25 05:25:57.000000 libmsiecf-20240425/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-04-25 05:25:57.000000 libmsiecf-20240425/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-25 05:25:57.000000 libmsiecf-20240425/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-25 05:25:57.000000 libmsiecf-20240425/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-04-25 05:25:57.000000 libmsiecf-20240425/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-04-25 05:25:57.000000 libmsiecf-20240425/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-04-25 05:25:57.000000 libmsiecf-20240425/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-04-25 05:25:57.000000 libmsiecf-20240425/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29297 2024-04-25 05:26:21.000000 libmsiecf-20240425/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-25 05:25:57.000000 libmsiecf-20240425/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-04-25 05:25:57.000000 libmsiecf-20240425/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-04-25 05:25:57.000000 libmsiecf-20240425/libclocale/libclocale_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2112 2024-04-25 04:56:37.000000 libmsiecf-20240425/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:27.000000 libmsiecf-20240425/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33149 2024-04-25 05:26:21.000000 libmsiecf-20240425/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-04-25 05:25:51.000000 libmsiecf-20240425/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:11:33.000000 libmsiecf-20240425/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-04-25 05:26:21.000000 libmsiecf-20240425/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:25.000000 libmsiecf-20240425/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1028 2024-04-25 04:44:30.000000 libmsiecf-20240425/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:25.000000 libmsiecf-20240425/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-04-25 04:44:23.000000 libmsiecf-20240425/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2143 2024-04-25 04:44:23.000000 libmsiecf-20240425/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-04-25 04:44:23.000000 libmsiecf-20240425/dpkg/libmsiecf-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      777 2024-04-25 04:44:23.000000 libmsiecf-20240425/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-04-25 04:44:23.000000 libmsiecf-20240425/dpkg/libmsiecf.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      122 2024-04-25 04:44:23.000000 libmsiecf-20240425/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      141 2024-04-25 05:26:39.000000 libmsiecf-20240425/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-04-25 04:44:23.000000 libmsiecf-20240425/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-04-25 04:44:23.000000 libmsiecf-20240425/dpkg/libmsiecf-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-04-25 04:44:23.000000 libmsiecf-20240425/dpkg/libmsiecf-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      485 2024-04-25 05:26:39.000000 libmsiecf-20240425/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-04-25 04:44:23.000000 libmsiecf-20240425/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1828532 2024-04-25 05:26:19.000000 libmsiecf-20240425/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-04-25 05:26:21.000000 libmsiecf-20240425/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-04-25 05:26:21.000000 libmsiecf-20240425/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecf_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5584 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/msiecf_test_error/msiecf_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/libfole/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4605 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/libfole/libfole.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38509 2024-04-25 04:45:09.000000 libmsiecf-20240425/msvscpp/libmsiecf.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecf_test_property_type/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5857 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/msiecf_test_property_type/msiecf_test_property_type.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecf_test_allocation_table/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6203 2024-04-25 04:45:09.000000 libmsiecf-20240425/msvscpp/msiecf_test_allocation_table/msiecf_test_allocation_table.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/libmsiecf/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10873 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/libmsiecf/libmsiecf.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecf_test_cache_directory_table/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6134 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/msiecf_test_cache_directory_table/msiecf_test_cache_directory_table.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/pymsiecf/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7930 2024-04-25 04:45:09.000000 libmsiecf-20240425/msvscpp/pymsiecf/pymsiecf.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecf_test_leak_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6104 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/msiecf_test_leak_values/msiecf_test_leak_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecf_test_file/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6336 2024-04-25 04:45:09.000000 libmsiecf-20240425/msvscpp/msiecf_test_file/msiecf_test_file.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1917 2024-04-25 04:55:29.000000 libmsiecf-20240425/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecfinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6455 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/msiecfinfo/msiecfinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecf_test_file_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6104 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/msiecf_test_file_header/msiecf_test_file_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecf_test_hash_table/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6185 2024-04-25 04:45:09.000000 libmsiecf-20240425/msvscpp/msiecf_test_hash_table/msiecf_test_hash_table.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecf_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5781 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/msiecf_test_tools_signal/msiecf_test_tools_signal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecf_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6510 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/msiecf_test_support/msiecf_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecf_test_redirected_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6122 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/msiecf_test_redirected_values/msiecf_test_redirected_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecf_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5672 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/msiecf_test_notify/msiecf_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecf_test_item/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5830 2024-04-25 04:45:09.000000 libmsiecf-20240425/msvscpp/msiecf_test_item/msiecf_test_item.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecf_test_tools_info_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5946 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/msiecf_test_tools_info_handle/msiecf_test_tools_info_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecf_test_url/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5663 2024-04-25 04:45:09.000000 libmsiecf-20240425/msvscpp/msiecf_test_url/msiecf_test_url.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecf_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5781 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/msiecf_test_tools_output/msiecf_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecf_test_leak/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5666 2024-04-25 04:45:09.000000 libmsiecf-20240425/msvscpp/msiecf_test_leak/msiecf_test_leak.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecf_test_url_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6101 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/msiecf_test_url_values/msiecf_test_url_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23006 2024-04-25 05:26:21.000000 libmsiecf-20240425/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8010 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/libfvalue/libfvalue.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecf_test_item_descriptor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5863 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/msiecf_test_item_descriptor/msiecf_test_item_descriptor.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecf_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5845 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/msiecf_test_io_handle/msiecf_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecfexport/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6625 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/msiecfexport/msiecfexport.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/libfdatetime/libfdatetime.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecf_test_redirected/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5684 2024-04-25 04:45:09.000000 libmsiecf-20240425/msvscpp/msiecf_test_redirected/msiecf_test_redirected.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/msvscpp/msiecf_test_directory_descriptor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5878 2024-04-25 04:44:51.000000 libmsiecf-20240425/msvscpp/msiecf_test_directory_descriptor/msiecf_test_directory_descriptor.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      378 2024-04-25 04:44:26.000000 libmsiecf-20240425/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:26.000000 libmsiecf-20240425/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-25 05:25:56.000000 libmsiecf-20240425/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-04-25 05:25:56.000000 libmsiecf-20240425/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-25 05:25:56.000000 libmsiecf-20240425/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-25 05:25:56.000000 libmsiecf-20240425/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-04-25 05:25:56.000000 libmsiecf-20240425/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-04-25 05:25:56.000000 libmsiecf-20240425/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-04-25 05:25:56.000000 libmsiecf-20240425/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-25 05:25:56.000000 libmsiecf-20240425/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-04-25 05:25:56.000000 libmsiecf-20240425/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-04-25 05:25:56.000000 libmsiecf-20240425/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-25 05:25:56.000000 libmsiecf-20240425/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-04-25 05:25:56.000000 libmsiecf-20240425/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-25 05:25:56.000000 libmsiecf-20240425/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-25 05:25:56.000000 libmsiecf-20240425/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-04-25 05:25:56.000000 libmsiecf-20240425/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-25 05:25:56.000000 libmsiecf-20240425/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-04-25 05:25:56.000000 libmsiecf-20240425/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30130 2024-04-25 05:26:21.000000 libmsiecf-20240425/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-25 05:25:56.000000 libmsiecf-20240425/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-25 05:25:56.000000 libmsiecf-20240425/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-04-25 05:25:56.000000 libmsiecf-20240425/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-04-25 05:25:56.000000 libmsiecf-20240425/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      381 2024-04-25 04:44:23.000000 libmsiecf-20240425/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-04-25 05:26:21.000000 libmsiecf-20240425/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:26.000000 libmsiecf-20240425/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32043 2024-04-25 05:26:21.000000 libmsiecf-20240425/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-25 05:25:53.000000 libmsiecf-20240425/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-25 04:44:23.000000 libmsiecf-20240425/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      486 2024-04-25 04:44:23.000000 libmsiecf-20240425/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-04-25 05:26:21.000000 libmsiecf-20240425/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-04-25 04:44:23.000000 libmsiecf-20240425/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-04-25 04:44:23.000000 libmsiecf-20240425/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:11:33.000000 libmsiecf-20240425/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:26.000000 libmsiecf-20240425/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32482 2024-04-25 05:26:21.000000 libmsiecf-20240425/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-04-25 05:26:02.000000 libmsiecf-20240425/libcthreads/libcthreads_queue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2024-04-25 05:26:39.000000 libmsiecf-20240425/libmsiecf.spec
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-04-25 05:26:21.000000 libmsiecf-20240425/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:26.000000 libmsiecf-20240425/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-04-25 05:26:00.000000 libmsiecf-20240425/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-25 05:26:00.000000 libmsiecf-20240425/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-04-25 05:26:00.000000 libmsiecf-20240425/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-04-25 05:26:00.000000 libmsiecf-20240425/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-25 05:26:00.000000 libmsiecf-20240425/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-25 05:26:00.000000 libmsiecf-20240425/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-04-25 05:26:00.000000 libmsiecf-20240425/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-04-25 05:26:00.000000 libmsiecf-20240425/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-04-25 05:26:00.000000 libmsiecf-20240425/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-04-25 05:26:00.000000 libmsiecf-20240425/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-25 05:26:00.000000 libmsiecf-20240425/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-25 05:26:00.000000 libmsiecf-20240425/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29328 2024-04-25 05:26:21.000000 libmsiecf-20240425/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-25 05:26:00.000000 libmsiecf-20240425/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-25 05:26:00.000000 libmsiecf-20240425/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-04-25 05:26:00.000000 libmsiecf-20240425/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-04-25 05:26:00.000000 libmsiecf-20240425/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7753 2023-12-03 09:11:33.000000 libmsiecf-20240425/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10780 2024-04-25 04:44:30.000000 libmsiecf-20240425/manuals/libmsiecf.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2514 2024-04-25 04:44:30.000000 libmsiecf-20240425/manuals/msiecfexport.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      169 2024-04-25 04:55:17.000000 libmsiecf-20240425/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1890 2024-04-25 04:44:30.000000 libmsiecf-20240425/manuals/msiecfinfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26102 2024-04-25 05:26:21.000000 libmsiecf-20240425/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2003 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_redirected.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1821 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7407 2024-04-25 04:45:59.000000 libmsiecf-20240425/tests/pymsiecf_test_file.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15088 2024-04-25 04:44:30.000000 libmsiecf-20240425/tests/msiecf_test_redirected_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13465 2024-04-25 04:45:09.000000 libmsiecf-20240425/tests/msiecf_test_file_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1468 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1557 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8291 2024-04-25 04:45:09.000000 libmsiecf-20240425/tests/msiecf_test_io_handle.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4040 2024-04-25 04:52:20.000000 libmsiecf-20240425/tests/test_tools.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6365 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_item_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14515 2024-04-25 04:44:30.000000 libmsiecf-20240425/tests/msiecf_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4215 2024-04-25 04:44:30.000000 libmsiecf-20240425/tests/msiecf_test_tools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1914 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_property_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3179 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_error.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/test_msiecfinfo.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3309 2024-04-25 05:10:22.000000 libmsiecf-20240425/tests/test_msiecfexport.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10392 2024-04-25 04:55:06.000000 libmsiecf-20240425/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2917 2024-04-25 04:44:30.000000 libmsiecf-20240425/tests/msiecf_test_url.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30553 2024-04-25 04:45:09.000000 libmsiecf-20240425/tests/msiecf_test_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9739 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_directory_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2094 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_leak.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3456 2024-04-25 04:45:59.000000 libmsiecf-20240425/tests/pymsiecf_test_support.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4412 2024-04-25 04:51:56.000000 libmsiecf-20240425/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-04-25 04:44:30.000000 libmsiecf-20240425/tests/msiecf_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30868 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_hash_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2970 2024-04-25 04:45:09.000000 libmsiecf-20240425/tests/msiecf_test_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1745 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15890 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_leak_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4747 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17885 2024-04-25 04:45:09.000000 libmsiecf-20240425/tests/msiecf_test_cache_directory_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1713 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5678 2024-04-25 04:44:30.000000 libmsiecf-20240425/tests/msiecf_test_tools_info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6034 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_allocation_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2469 2024-04-25 04:44:30.000000 libmsiecf-20240425/tests/msiecf_test_tools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18714 2024-04-25 04:45:09.000000 libmsiecf-20240425/tests/msiecf_test_url_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      989 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_libmsiecf.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73397 2024-04-25 05:26:21.000000 libmsiecf-20240425/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4539 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4370 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8609 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1712 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13271 2024-04-25 04:44:29.000000 libmsiecf-20240425/tests/msiecf_test_functions.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4206 2024-04-25 04:51:35.000000 libmsiecf-20240425/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      977 2024-04-25 04:44:27.000000 libmsiecf-20240425/ossfuzz/ossfuzz_libmsiecf.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1394 2024-04-25 04:54:40.000000 libmsiecf-20240425/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-04-25 04:44:27.000000 libmsiecf-20240425/ossfuzz/ossfuzz_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2641 2024-04-25 04:44:27.000000 libmsiecf-20240425/ossfuzz/item_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2229 2024-04-25 04:44:27.000000 libmsiecf-20240425/ossfuzz/file_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33218 2024-04-25 05:26:21.000000 libmsiecf-20240425/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-04-25 05:26:15.000000 libmsiecf-20240425/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:26.000000 libmsiecf-20240425/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-04-25 05:26:01.000000 libmsiecf-20240425/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-04-25 05:26:01.000000 libmsiecf-20240425/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-04-25 05:26:01.000000 libmsiecf-20240425/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-04-25 05:26:01.000000 libmsiecf-20240425/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-25 05:26:01.000000 libmsiecf-20240425/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-04-25 05:26:01.000000 libmsiecf-20240425/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-25 05:26:01.000000 libmsiecf-20240425/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-04-25 05:26:01.000000 libmsiecf-20240425/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-25 05:26:01.000000 libmsiecf-20240425/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-04-25 05:26:01.000000 libmsiecf-20240425/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-25 05:26:01.000000 libmsiecf-20240425/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-04-25 05:26:01.000000 libmsiecf-20240425/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-25 05:26:01.000000 libmsiecf-20240425/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-25 05:26:01.000000 libmsiecf-20240425/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-25 05:26:01.000000 libmsiecf-20240425/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-04-25 05:26:01.000000 libmsiecf-20240425/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30225 2024-04-25 05:26:21.000000 libmsiecf-20240425/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-04-25 05:26:01.000000 libmsiecf-20240425/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-04-25 05:26:01.000000 libmsiecf-20240425/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:29.000000 libmsiecf-20240425/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:11:36.000000 libmsiecf-20240425/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:11:36.000000 libmsiecf-20240425/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:11:36.000000 libmsiecf-20240425/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:11:36.000000 libmsiecf-20240425/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:11:36.000000 libmsiecf-20240425/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:11:36.000000 libmsiecf-20240425/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:11:36.000000 libmsiecf-20240425/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:11:36.000000 libmsiecf-20240425/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:11:36.000000 libmsiecf-20240425/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1855 2024-04-25 05:26:38.000000 libmsiecf-20240425/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:11:36.000000 libmsiecf-20240425/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:11:36.000000 libmsiecf-20240425/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:26.000000 libmsiecf-20240425/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55809 2024-04-25 05:26:21.000000 libmsiecf-20240425/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-04-25 05:26:10.000000 libmsiecf-20240425/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40070 2024-04-25 05:26:21.000000 libmsiecf-20240425/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:27.000000 libmsiecf-20240425/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-04-25 05:26:08.000000 libmsiecf-20240425/libfvalue/libfvalue_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_split_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_split_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-04-25 05:26:08.000000 libmsiecf-20240425/libfvalue/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_split_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_binary_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_value_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_split_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_floating_point.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_binary_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_value_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35118 2024-04-25 05:26:21.000000 libmsiecf-20240425/libfvalue/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_floating_point.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-04-25 05:26:07.000000 libmsiecf-20240425/libfvalue/libfvalue_libuna.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:26.000000 libmsiecf-20240425/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-25 05:25:58.000000 libmsiecf-20240425/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-25 05:25:58.000000 libmsiecf-20240425/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-04-25 05:25:58.000000 libmsiecf-20240425/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-04-25 05:25:58.000000 libmsiecf-20240425/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-04-25 05:25:58.000000 libmsiecf-20240425/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-25 05:25:58.000000 libmsiecf-20240425/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-04-25 05:25:58.000000 libmsiecf-20240425/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-04-25 05:25:58.000000 libmsiecf-20240425/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-04-25 05:25:58.000000 libmsiecf-20240425/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-04-25 05:25:58.000000 libmsiecf-20240425/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-04-25 05:25:58.000000 libmsiecf-20240425/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29166 2024-04-25 05:26:21.000000 libmsiecf-20240425/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-25 05:25:58.000000 libmsiecf-20240425/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-04-25 05:25:58.000000 libmsiecf-20240425/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:28.000000 libmsiecf-20240425/msiecftools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-04-25 04:44:29.000000 libmsiecf-20240425/msiecftools/msiecftools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1216 2024-04-25 04:44:28.000000 libmsiecf-20240425/msiecftools/msiecftools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4539 2024-04-25 04:44:28.000000 libmsiecf-20240425/msiecftools/msiecftools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2298 2024-04-25 04:45:59.000000 libmsiecf-20240425/msiecftools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1486 2024-04-25 04:44:28.000000 libmsiecf-20240425/msiecftools/msiecftools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-04-25 04:44:29.000000 libmsiecf-20240425/msiecftools/msiecftools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1784 2024-04-25 04:44:29.000000 libmsiecf-20240425/msiecftools/msiecftools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2001 2024-04-25 04:54:32.000000 libmsiecf-20240425/msiecftools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12400 2024-04-25 04:45:59.000000 libmsiecf-20240425/msiecftools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41188 2024-04-25 04:44:28.000000 libmsiecf-20240425/msiecftools/export_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-25 04:44:28.000000 libmsiecf-20240425/msiecftools/msiecftools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7414 2024-04-25 04:45:59.000000 libmsiecf-20240425/msiecftools/msiecfinfo.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5776 2024-04-25 04:44:29.000000 libmsiecf-20240425/msiecftools/msiecftools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1751 2024-04-25 04:44:28.000000 libmsiecf-20240425/msiecftools/msiecftools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9132 2024-04-25 04:44:28.000000 libmsiecf-20240425/msiecftools/msiecfexport.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1507 2024-04-25 04:44:28.000000 libmsiecf-20240425/msiecftools/msiecftools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5939 2024-04-25 04:44:28.000000 libmsiecf-20240425/msiecftools/log_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1481 2024-04-25 04:44:29.000000 libmsiecf-20240425/msiecftools/msiecftools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3736 2024-04-25 04:44:28.000000 libmsiecf-20240425/msiecftools/export_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32758 2024-04-25 05:26:21.000000 libmsiecf-20240425/msiecftools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1675 2024-04-25 04:44:28.000000 libmsiecf-20240425/msiecftools/log_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3965 2024-04-25 04:44:29.000000 libmsiecf-20240425/msiecftools/msiecftools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      989 2024-04-25 04:44:29.000000 libmsiecf-20240425/msiecftools/msiecftools_libmsiecf.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1774 2024-04-25 04:44:29.000000 libmsiecf-20240425/msiecftools/msiecftools_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-04-25 04:44:29.000000 libmsiecf-20240425/msiecftools/msiecftools_libcnotify.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:25.000000 libmsiecf-20240425/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-04-25 05:25:54.000000 libmsiecf-20240425/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-04-25 05:25:54.000000 libmsiecf-20240425/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-25 05:25:54.000000 libmsiecf-20240425/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-04-25 05:25:54.000000 libmsiecf-20240425/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-25 05:25:54.000000 libmsiecf-20240425/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-25 05:25:54.000000 libmsiecf-20240425/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-04-25 05:25:54.000000 libmsiecf-20240425/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-04-25 05:25:54.000000 libmsiecf-20240425/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-04-25 05:25:54.000000 libmsiecf-20240425/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-25 05:25:54.000000 libmsiecf-20240425/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-25 05:25:54.000000 libmsiecf-20240425/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28633 2024-04-25 05:26:21.000000 libmsiecf-20240425/libcerror/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-25 05:44:27.000000 libmsiecf-20240425/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32217 2024-04-25 05:26:21.000000 libmsiecf-20240425/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-04-25 05:26:04.000000 libmsiecf-20240425/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56797 2024-04-25 05:26:18.000000 libmsiecf-20240425/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7505 2024-04-25 04:44:23.000000 libmsiecf-20240425/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      417 2024-04-25 05:44:30.297971 libmsiecf-20240425/PKG-INFO
```

### Comparing `libmsiecf-20240209/libfole/libfole_value_type.h` & `libmsiecf-20240425/libfole/libfole_value_type.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfole/libfole_error.c` & `libmsiecf-20240425/libfole/libfole_error.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfole/Makefile.am` & `libmsiecf-20240425/libfole/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFOLE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfole.la
 
 libfole_la_SOURCES = \
 	libfole_definitions.h \
 	libfole_extern.h \
@@ -13,19 +13,17 @@
 	libfole_libcerror.h \
 	libfole_support.c libfole_support.h \
 	libfole_types.h \
 	libfole_unused.h \
 	libfole_value_type.c libfole_value_type.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfole ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfole_la_SOURCES)
```

### Comparing `libmsiecf-20240209/libfole/libfole_definitions.h` & `libmsiecf-20240425/libfole/libfole_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfole/definitions.h> are copied here
  * for local use of libfole
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFOLE_VERSION					20240119
+#define LIBFOLE_VERSION					20240416
 
 /* The version string
  */
-#define LIBFOLE_VERSION_STRING				"20240119"
+#define LIBFOLE_VERSION_STRING				"20240416"
 
 /* The byte order definitions
  */
 #define LIBFOLE_ENDIAN_BIG				_BYTE_STREAM_ENDIAN_BIG
 #define LIBFOLE_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 #endif /* !defined( HAVE_LOCAL_LIBFOLE ) */
```

### Comparing `libmsiecf-20240209/libfole/libfole_error.h` & `libmsiecf-20240425/libfole/libfole_error.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfole/libfole_support.h` & `libmsiecf-20240425/libfole/libfole_support.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfole/libfole_types.h` & `libmsiecf-20240425/libfole/libfole_types.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfole/libfole_support.c` & `libmsiecf-20240425/libfole/libfole_support.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfole/libfole_value_type.c` & `libmsiecf-20240425/libfole/libfole_value_type.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfole/libfole_unused.h` & `libmsiecf-20240425/libfole/libfole_unused.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfole/libfole_libcerror.h` & `libmsiecf-20240425/libfole/libfole_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfole/Makefile.in` & `libmsiecf-20240425/libfole/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -500,30 +500,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFOLE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFOLE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFOLE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFOLE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFOLE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFOLE_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFOLE_TRUE@noinst_LTLIBRARIES = libfole.la
 @HAVE_LOCAL_LIBFOLE_TRUE@libfole_la_SOURCES = \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_definitions.h \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_extern.h \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_error.c libfole_error.h \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_libcerror.h \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_support.c libfole_support.h \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_types.h \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_unused.h \
 @HAVE_LOCAL_LIBFOLE_TRUE@	libfole_value_type.c libfole_value_type.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -725,24 +726,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfole_error.Plo
+	-rm -f ./$(DEPDIR)/libfole_support.Plo
+	-rm -f ./$(DEPDIR)/libfole_value_type.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -828,17 +834,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfole ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfole_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmsiecf-20240209/libfole/libfole_extern.h` & `libmsiecf-20240425/libfole/libfole_extern.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf.pc.in` & `libmsiecf-20240425/libmsiecf.pc.in`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/COPYING` & `libmsiecf-20240425/COPYING`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf.spec.in` & `libmsiecf-20240425/libmsiecf.spec.in`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/install-sh` & `libmsiecf-20240425/install-sh`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_leak_values.c` & `libmsiecf-20240425/libmsiecf/libmsiecf_leak_values.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_allocation_table.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_allocation_table.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_debug.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_debug.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_directory_descriptor.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_directory_descriptor.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_item.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_item.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_libfdatetime.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_support.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_support.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_property_type.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_property_type.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_io_handle.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_io_handle.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_error.c` & `libmsiecf-20240425/libmsiecf/libmsiecf_error.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_notify.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_notify.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_item_descriptor.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_item_descriptor.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_redirected_values.c` & `libmsiecf-20240425/libmsiecf/libmsiecf_redirected_values.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/msiecf_cache_directory_table.h` & `libmsiecf-20240425/libmsiecf/msiecf_cache_directory_table.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf.rc.in` & `libmsiecf-20240425/libmsiecf/libmsiecf.rc.in`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_cache_directory_table.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_cache_directory_table.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_notify.c` & `libmsiecf-20240425/libmsiecf/libmsiecf_notify.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_url.c` & `libmsiecf-20240425/libmsiecf/libmsiecf_url.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_libuna.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_libuna.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_cache_directory_table.c` & `libmsiecf-20240425/libmsiecf/libmsiecf_cache_directory_table.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf.rc` & `libmsiecf-20240425/libmsiecf/libmsiecf.rc`

 * *Files 12% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the MSIE Cache File (index.dat) format\0"
-      VALUE "FileVersion",		"20240209" "\0"
+      VALUE "FileVersion",		"20240425" "\0"
       VALUE "InternalName",		"libmsiecf.dll\0"
       VALUE "LegalCopyright",		"(C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libmsiecf.dll\0"
       VALUE "ProductName",		"libmsiecf\0"
-      VALUE "ProductVersion",		"20240209" "\0"
+      VALUE "ProductVersion",		"20240425" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libmsiecf/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_file_header.c` & `libmsiecf-20240425/libmsiecf/libmsiecf_file_header.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/msiecf_redr_record.h` & `libmsiecf-20240425/libmsiecf/msiecf_redr_record.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_hash.c` & `libmsiecf-20240425/libmsiecf/libmsiecf_hash.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_libfvalue.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_libfvalue.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_types.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_types.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/Makefile.am` & `libmsiecf-20240425/libmsiecf/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -86,21 +86,19 @@
 libmsiecf_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libmsiecf_definitions.h.in \
 	libmsiecf.rc \
 	libmsiecf.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libmsiecf_definitions.h \
+	libmsiecf.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libmsiecf_definitions.h
-	-rm -f libmsiecf.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libmsiecf ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libmsiecf_la_SOURCES)
```

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_url.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_url.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/msiecf_file_header.h` & `libmsiecf-20240425/libmsiecf/msiecf_file_header.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf.c` & `libmsiecf-20240425/libmsiecf/libmsiecf.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_io_handle.c` & `libmsiecf-20240425/libmsiecf/libmsiecf_io_handle.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_redirected_values.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_redirected_values.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_redirected.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_redirected.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/msiecf_hash_record.h` & `libmsiecf-20240425/libmsiecf/msiecf_hash_record.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_definitions.h.in` & `libmsiecf-20240425/libmsiecf/libmsiecf_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_file_header.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_file_header.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_support.c` & `libmsiecf-20240425/libmsiecf/libmsiecf_support.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_libcthreads.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/msiecf_url_record.h` & `libmsiecf-20240425/libmsiecf/msiecf_url_record.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_definitions.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -34,19 +34,19 @@
 #include <libmsiecf/definitions.h>
 
 /* The definitions in <libmsiecf/definitions.h> are copied here
  * for local use of libmsiecf
  */
 #else
 
-#define LIBMSIECF_VERSION				20240209
+#define LIBMSIECF_VERSION				20240425
 
 /* The version string
  */
-#define LIBMSIECF_VERSION_STRING			"20240209"
+#define LIBMSIECF_VERSION_STRING			"20240425"
 
 /* The file access flags
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBMSIECF_ACCESS_FLAGS
```

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_hash_table.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_hash_table.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_hash_table.c` & `libmsiecf-20240425/libmsiecf/libmsiecf_hash_table.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_directory_descriptor.c` & `libmsiecf-20240425/libmsiecf/libmsiecf_directory_descriptor.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_url_values.c` & `libmsiecf-20240425/libmsiecf/libmsiecf_url_values.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_extern.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_extern.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_libbfio.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_libbfio.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_file.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_file.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_libcdata.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_libcdata.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_leak.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_leak.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_hash.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_hash.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_unused.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_unused.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_codepage.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_codepage.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_file.c` & `libmsiecf-20240425/libmsiecf/libmsiecf_file.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_item_descriptor.c` & `libmsiecf-20240425/libmsiecf/libmsiecf_item_descriptor.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_leak_values.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_leak_values.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_libclocale.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_libclocale.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/msiecf_record.h` & `libmsiecf-20240425/libmsiecf/msiecf_record.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_libcerror.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_libcnotify.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_error.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_error.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_allocation_table.c` & `libmsiecf-20240425/libmsiecf/libmsiecf_allocation_table.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_property_type.c` & `libmsiecf-20240425/libmsiecf/libmsiecf_property_type.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/msiecf_leak_record.h` & `libmsiecf-20240425/libmsiecf/msiecf_leak_record.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_redirected.c` & `libmsiecf-20240425/libmsiecf/libmsiecf_redirected.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/Makefile.in` & `libmsiecf-20240425/libmsiecf/Makefile.in`

 * *Files 8% similar despite different names*

```diff
@@ -552,16 +552,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -641,15 +641,18 @@
 
 libmsiecf_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libmsiecf_definitions.h.in \
 	libmsiecf.rc \
 	libmsiecf.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libmsiecf_definitions.h \
+	libmsiecf.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -901,24 +904,48 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libLTLIBRARIES clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libmsiecf.Plo
+	-rm -f ./$(DEPDIR)/libmsiecf_allocation_table.Plo
+	-rm -f ./$(DEPDIR)/libmsiecf_cache_directory_table.Plo
+	-rm -f ./$(DEPDIR)/libmsiecf_debug.Plo
+	-rm -f ./$(DEPDIR)/libmsiecf_directory_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libmsiecf_error.Plo
+	-rm -f ./$(DEPDIR)/libmsiecf_file.Plo
+	-rm -f ./$(DEPDIR)/libmsiecf_file_header.Plo
+	-rm -f ./$(DEPDIR)/libmsiecf_hash.Plo
+	-rm -f ./$(DEPDIR)/libmsiecf_hash_table.Plo
+	-rm -f ./$(DEPDIR)/libmsiecf_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libmsiecf_item.Plo
+	-rm -f ./$(DEPDIR)/libmsiecf_item_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libmsiecf_leak.Plo
+	-rm -f ./$(DEPDIR)/libmsiecf_leak_values.Plo
+	-rm -f ./$(DEPDIR)/libmsiecf_notify.Plo
+	-rm -f ./$(DEPDIR)/libmsiecf_property_type.Plo
+	-rm -f ./$(DEPDIR)/libmsiecf_redirected.Plo
+	-rm -f ./$(DEPDIR)/libmsiecf_redirected_values.Plo
+	-rm -f ./$(DEPDIR)/libmsiecf_support.Plo
+	-rm -f ./$(DEPDIR)/libmsiecf_url.Plo
+	-rm -f ./$(DEPDIR)/libmsiecf_url_values.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1023,19 +1050,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libmsiecf_definitions.h
-	-rm -f libmsiecf.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libmsiecf ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libmsiecf_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_leak.c` & `libmsiecf-20240425/libmsiecf/libmsiecf_leak.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_item.c` & `libmsiecf-20240425/libmsiecf/libmsiecf_item.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_debug.c` & `libmsiecf-20240425/libmsiecf/libmsiecf_debug.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_url_values.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_url_values.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf/libmsiecf_libfole.h` & `libmsiecf-20240425/libmsiecf/libmsiecf_libfole.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_datetime.c` & `libmsiecf-20240425/pymsiecf/pymsiecf_datetime.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_libmsiecf.h` & `libmsiecf-20240425/pymsiecf/pymsiecf_libmsiecf.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_libcerror.h` & `libmsiecf-20240425/pymsiecf/pymsiecf_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_file_object_io_handle.h` & `libmsiecf-20240425/pymsiecf/pymsiecf_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_file_object_io_handle.c` & `libmsiecf-20240425/pymsiecf/pymsiecf_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_leak.c` & `libmsiecf-20240425/pymsiecf/pymsiecf_leak.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_item_types.h` & `libmsiecf-20240425/pymsiecf/pymsiecf_item_types.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_leak.h` & `libmsiecf-20240425/pymsiecf/pymsiecf_leak.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_items.c` & `libmsiecf-20240425/pymsiecf/pymsiecf_items.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_codepage.h` & `libmsiecf-20240425/pymsiecf/pymsiecf_codepage.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_datetime.h` & `libmsiecf-20240425/pymsiecf/pymsiecf_datetime.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_python.h` & `libmsiecf-20240425/pymsiecf/pymsiecf_python.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_libclocale.h` & `libmsiecf-20240425/pymsiecf/pymsiecf_libclocale.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_file.c` & `libmsiecf-20240425/pymsiecf/pymsiecf_file.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/Makefile.am` & `libmsiecf-20240425/pymsiecf/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_PYTHON
 AM_CFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -50,13 +50,11 @@
 	@LIBBFIO_LIBADD@
 
 pymsiecf_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pymsiecf_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_codepage.c` & `libmsiecf-20240425/pymsiecf/pymsiecf_codepage.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_cache_directories.c` & `libmsiecf-20240425/pymsiecf/pymsiecf_cache_directories.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_unused.h` & `libmsiecf-20240425/pymsiecf/pymsiecf_unused.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_item_types.c` & `libmsiecf-20240425/pymsiecf/pymsiecf_item_types.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_item.c` & `libmsiecf-20240425/pymsiecf/pymsiecf_item.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_error.c` & `libmsiecf-20240425/pymsiecf/pymsiecf_error.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_items.h` & `libmsiecf-20240425/pymsiecf/pymsiecf_items.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_integer.h` & `libmsiecf-20240425/pymsiecf/pymsiecf_integer.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf.c` & `libmsiecf-20240425/pymsiecf/pymsiecf.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_redirected.c` & `libmsiecf-20240425/pymsiecf/pymsiecf_redirected.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_item.h` & `libmsiecf-20240425/pymsiecf/pymsiecf_item.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_redirected.h` & `libmsiecf-20240425/pymsiecf/pymsiecf_redirected.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_url_types.c` & `libmsiecf-20240425/pymsiecf/pymsiecf_url_types.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_url.h` & `libmsiecf-20240425/pymsiecf/pymsiecf_url.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_url.c` & `libmsiecf-20240425/pymsiecf/pymsiecf_url.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_integer.c` & `libmsiecf-20240425/pymsiecf/pymsiecf_integer.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_libbfio.h` & `libmsiecf-20240425/pymsiecf/pymsiecf_libbfio.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_item_flags.c` & `libmsiecf-20240425/pymsiecf/pymsiecf_item_flags.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_error.h` & `libmsiecf-20240425/pymsiecf/pymsiecf_error.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf.h` & `libmsiecf-20240425/pymsiecf/pymsiecf.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_item_flags.h` & `libmsiecf-20240425/pymsiecf/pymsiecf_item_flags.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/Makefile.in` & `libmsiecf-20240425/pymsiecf/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -569,16 +569,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_PYTHON_TRUE@AM_CFLAGS = \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/include \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/common \
+@HAVE_PYTHON_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_PYTHON_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -619,15 +619,16 @@
 @HAVE_PYTHON_TRUE@	@LIBUNA_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBBFIO_LIBADD@
 
 @HAVE_PYTHON_TRUE@pymsiecf_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pymsiecf_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -981,24 +982,42 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-pyexecLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/pymsiecf_la-pymsiecf.Plo
+	-rm -f ./$(DEPDIR)/pymsiecf_la-pymsiecf_cache_directories.Plo
+	-rm -f ./$(DEPDIR)/pymsiecf_la-pymsiecf_codepage.Plo
+	-rm -f ./$(DEPDIR)/pymsiecf_la-pymsiecf_datetime.Plo
+	-rm -f ./$(DEPDIR)/pymsiecf_la-pymsiecf_error.Plo
+	-rm -f ./$(DEPDIR)/pymsiecf_la-pymsiecf_file.Plo
+	-rm -f ./$(DEPDIR)/pymsiecf_la-pymsiecf_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pymsiecf_la-pymsiecf_integer.Plo
+	-rm -f ./$(DEPDIR)/pymsiecf_la-pymsiecf_item.Plo
+	-rm -f ./$(DEPDIR)/pymsiecf_la-pymsiecf_item_flags.Plo
+	-rm -f ./$(DEPDIR)/pymsiecf_la-pymsiecf_item_types.Plo
+	-rm -f ./$(DEPDIR)/pymsiecf_la-pymsiecf_items.Plo
+	-rm -f ./$(DEPDIR)/pymsiecf_la-pymsiecf_leak.Plo
+	-rm -f ./$(DEPDIR)/pymsiecf_la-pymsiecf_redirected.Plo
+	-rm -f ./$(DEPDIR)/pymsiecf_la-pymsiecf_url.Plo
+	-rm -f ./$(DEPDIR)/pymsiecf_la-pymsiecf_url_types.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1098,13 +1117,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-pyexecLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_cache_directories.h` & `libmsiecf-20240425/pymsiecf/pymsiecf_cache_directories.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_url_types.h` & `libmsiecf-20240425/pymsiecf/pymsiecf_url_types.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/pymsiecf/pymsiecf_file.h` & `libmsiecf-20240425/pymsiecf/pymsiecf_file.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/depcomp` & `libmsiecf-20240425/depcomp`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfguid/libfguid_error.c` & `libmsiecf-20240425/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfguid/libfguid_support.h` & `libmsiecf-20240425/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfguid/libfguid_identifier.h` & `libmsiecf-20240425/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfguid/libfguid_libcerror.h` & `libmsiecf-20240425/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfguid/Makefile.am` & `libmsiecf-20240425/libfguid/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFGUID
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfguid.la
 
 libfguid_la_SOURCES = \
 	libfguid_definitions.h \
 	libfguid_extern.h \
@@ -13,19 +13,17 @@
 	libfguid_libcerror.h \
 	libfguid_identifier.c libfguid_identifier.h \
 	libfguid_support.c libfguid_support.h \
 	libfguid_types.h \
 	libfguid_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
```

### Comparing `libmsiecf-20240209/libfguid/libfguid_unused.h` & `libmsiecf-20240425/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfguid/libfguid_extern.h` & `libmsiecf-20240425/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfguid/libfguid_types.h` & `libmsiecf-20240425/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfguid/libfguid_identifier.c` & `libmsiecf-20240425/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfguid/libfguid_support.c` & `libmsiecf-20240425/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfguid/libfguid_definitions.h` & `libmsiecf-20240425/libfguid/libfguid_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfguid/definitions.h> are copied here
  * for local use of libfguid
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFGUID_VERSION					20240116
+#define LIBFGUID_VERSION					20240415
 
 /* The version string
  */
-#define LIBFGUID_VERSION_STRING					"20240116"
+#define LIBFGUID_VERSION_STRING					"20240415"
 
 /* The byte order definitions
  */
 #define LIBFGUID_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFGUID_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The GUID identifier version definitions
```

### Comparing `libmsiecf-20240209/libfguid/Makefile.in` & `libmsiecf-20240425/libfguid/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -501,30 +501,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFGUID_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFGUID_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFGUID_TRUE@noinst_LTLIBRARIES = libfguid.la
 @HAVE_LOCAL_LIBFGUID_TRUE@libfguid_la_SOURCES = \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_definitions.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_extern.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_error.c libfguid_error.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_libcerror.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_identifier.c libfguid_identifier.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_support.c libfguid_support.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_types.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -726,24 +727,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfguid_error.Plo
+	-rm -f ./$(DEPDIR)/libfguid_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfguid_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -829,17 +835,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmsiecf-20240209/libfguid/libfguid_error.h` & `libmsiecf-20240425/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/m4/libcfile.m4` & `libmsiecf-20240425/m4/libcfile.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcfile required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcfile is available
 dnl ac_libcfile_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCFILE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno],
     [ac_cv_libcfile=no],
     [ac_cv_libcfile=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcfile which returns "yes" and --with-libcfile= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect],
+      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcfile"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcfile],
           [1])
@@ -199,16 +201,17 @@
             libcfile_file_remove_wide,
             [ac_cv_libcfile_dummy=yes],
             [ac_cv_libcfile=no])
           ])
 
         ac_cv_libcfile_LIBADD="-lcfile"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes],
+      [test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcfile in directory: $ac_cv_with_libcfile],
         [1])
       ])
     ])
 
   AS_IF(
@@ -354,15 +357,15 @@
   AS_IF(
     [test "x$ac_cv_func_unlink" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: unlink],
       [1])
     ])
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
   ])
 
 dnl Function to detect how to enable libcfile
 AC_DEFUN([AX_LIBCFILE_CHECK_ENABLE],
```

### Comparing `libmsiecf-20240209/m4/libfdatetime.m4` & `libmsiecf-20240425/m4/libfdatetime.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfdatetime required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfdatetime is available
 dnl ac_libfdatetime_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATETIME_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdatetime" = xno],
     [ac_cv_libfdatetime=no],
     [ac_cv_libfdatetime=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfdatetime which returns "yes" and --with-libfdatetime= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect],
+      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfdatetime"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfdatetime}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdatetime}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfdatetime],
           [1])
@@ -455,16 +457,17 @@
           fdatetime,
           libfdatetime_systemetime_copy_to_utf32_string_with_index,
           [ac_cv_libfdatetime_dummy=yes],
           [ac_cv_libfdatetime=no])
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_libfdatetime" != xyes],
+      [test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime],
         [1])
       ])
     ])
 
   AS_IF(
@@ -486,15 +489,15 @@
     ])
   ])
 
 dnl Function to detect if libfdatetime dependencies are available
 AC_DEFUN([AX_LIBFDATETIME_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
   ])
 
 dnl Function to detect how to enable libfdatetime
 AC_DEFUN([AX_LIBFDATETIME_CHECK_ENABLE],
```

### Comparing `libmsiecf-20240209/m4/tests.m4` & `libmsiecf-20240425/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/m4/libcpath.m4` & `libmsiecf-20240425/m4/libcpath.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcpath required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcpath is available
 dnl ac_libcpath_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCPATH_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno],
     [ac_cv_libcpath=no],
     [ac_cv_libcpath=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcpath which returns "yes" and --with-libcpath= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect],
+      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcpath"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcpath],
           [1])
@@ -148,16 +150,17 @@
             libcpath_path_make_directory_wide,
             [ac_cv_libcpath_dummy=yes],
             [ac_cv_libcpath=no])
           ])
 
         ac_cv_libcpath_LIBADD="-lcpath"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes],
+      [test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcpath in directory: $ac_cv_with_libcpath],
         [1])
       ])
     ])
 
   AS_IF(
@@ -269,15 +272,15 @@
     [AC_MSG_FAILURE(
       [Missing functions: getcwd],
       [1])
     ])
 
   AX_LIBCPATH_CHECK_FUNC_MKDIR
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
   ])
 
 dnl Function to detect how to enable libcpath
 AC_DEFUN([AX_LIBCPATH_CHECK_ENABLE],
```

### Comparing `libmsiecf-20240209/m4/lib-prefix.m4` & `libmsiecf-20240425/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/m4/progtest.m4` & `libmsiecf-20240425/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/m4/libuna.m4` & `libmsiecf-20240425/m4/libuna.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libuna or required headers and functions
 dnl
-dnl Version: 20230702
+dnl Version: 20240413
 
 dnl Function to detect if a specific libuna definition is available.
 AC_DEFUN([AX_LIBUNA_CHECK_DEFINITION],
   [AC_CACHE_CHECK(
     [if `$1' is defined],
     [$2],
     [AC_LANG_PUSH(C)
@@ -23,16 +23,18 @@
 dnl ac_libuna_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBUNA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno],
     [ac_cv_libuna=no],
     [ac_cv_libuna=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libuna which returns "yes" and --with-libuna= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect],
+      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libuna"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libuna],
           [1])
@@ -938,16 +940,17 @@
           [ac_cv_libuna_defines_compare_greater])
         AS_IF(
           [test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes],
           [ac_cv_libuna=no])
 
         ac_cv_libuna_LIBADD="-luna"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes],
+      [test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libuna in directory: $ac_cv_with_libuna],
         [1])
       ])
     ])
 
   AS_IF(
@@ -969,15 +972,15 @@
     ])
   ])
 
 dnl Function to detect if libuna dependencies are available
 AC_DEFUN([AX_LIBUNA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
   ])
 
 dnl Function to detect how to enable libuna
 AC_DEFUN([AX_LIBUNA_CHECK_ENABLE],
```

### Comparing `libmsiecf-20240209/m4/gettext.m4` & `libmsiecf-20240425/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/m4/lib-ld.m4` & `libmsiecf-20240425/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/m4/libfole.m4` & `libmsiecf-20240425/m4/libfole.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfole required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfole is available
 dnl ac_libfole_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFOLE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfole" = xno],
     [ac_cv_libfole=no],
     [ac_cv_libfole=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfole which returns "yes" and --with-libfole= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect],
+      [test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect && test "x$ac_cv_with_libfole" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfole"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfole}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfole}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfole],
           [1])
@@ -53,16 +55,17 @@
           [ac_cv_libfole_dummy=yes],
           [ac_cv_libfole=no])
 
         dnl TODO add functions
 
         ac_cv_libfole_LIBADD="-lfole"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect && test "x$ac_cv_libfole" != xyes],
+      [test "x$ac_cv_libfole" != xyes && test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect && test "x$ac_cv_with_libfole" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfole in directory: $ac_cv_with_libfole],
         [1])
       ])
     ])
 
   AS_IF(
@@ -84,15 +87,15 @@
     ])
   ])
 
 dnl Function to detect if libfole dependencies are available
 AC_DEFUN([AX_LIBFOLE_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfole_CPPFLAGS="-I../libfole";
+  ac_cv_libfole_CPPFLAGS="-I../libfole -I\$(top_srcdir)/libfole";
   ac_cv_libfole_LIBADD="../libfole/libfole.la";
 
   ac_cv_libfole=local
   ])
 
 dnl Function to detect how to enable libfole
 AC_DEFUN([AX_LIBFOLE_CHECK_ENABLE],
```

### Comparing `libmsiecf-20240209/m4/libclocale.m4` & `libmsiecf-20240425/m4/libclocale.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libclocale required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libclocale is available
 dnl ac_libclocale_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCLOCALE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno],
     [ac_cv_libclocale=no],
     [ac_cv_libclocale=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libclocale which returns "yes" and --with-libclocale= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect],
+      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libclocale"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libclocale],
           [1])
@@ -122,16 +124,17 @@
           clocale,
           libclocale_initialize,
           [ac_cv_libclocale_dummy=yes],
           [ac_cv_libclocale=no])
 
         ac_cv_libclocale_LIBADD="-lclocale"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes],
+      [test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libclocale in directory: $ac_cv_with_libclocale],
         [1])
       ])
     ])
 
   AS_IF(
@@ -216,15 +219,15 @@
     [AC_MSG_FAILURE(
       [Missing function: setlocale],
       [1])
     ])
 
   AX_LIBCLOCALE_CHECK_FUNC_LANGINFO_CODESET
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
   ])
 
 dnl Function to detect how to enable libclocale
 AC_DEFUN([AX_LIBCLOCALE_CHECK_ENABLE],
```

### Comparing `libmsiecf-20240209/m4/libcdata.m4` & `libmsiecf-20240425/m4/libcdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcdata required headers and functions
 dnl
-dnl Version: 20230108
+dnl Version: 20240413
 
 dnl Function to detect if libcdata is available
 dnl ac_libcdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno],
     [ac_cv_libcdata=no],
     [ac_cv_libcdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcdata which returns "yes" and --with-libcdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect],
+      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcdata],
           [1])
@@ -493,16 +495,17 @@
           cdata,
           libcdata_tree_node_get_leaf_node_list,
           [ac_cv_libcdata_dummy=yes],
           [ac_cv_libcdata=no])
 
         ac_cv_libcdata_LIBADD="-lcdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes],
+      [test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcdata in directory: $ac_cv_with_libcdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -524,15 +527,15 @@
     ])
   ])
 
 dnl Function to detect if libcdata dependencies are available
 AC_DEFUN([AX_LIBCDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
   ])
 
 dnl Function to detect how to enable libcdata
 AC_DEFUN([AX_LIBCDATA_CHECK_ENABLE],
```

### Comparing `libmsiecf-20240209/m4/libcsplit.m4` & `libmsiecf-20240425/m4/libcsplit.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcsplit required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcsplit is available
 dnl ac_libcsplit_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno],
     [ac_cv_libcsplit=no],
     [ac_cv_libcsplit=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcsplit which returns "yes" and --with-libcsplit= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect],
+      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcsplit"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcsplit],
           [1])
@@ -143,16 +145,17 @@
             libcsplit_wide_split_string_set_segment_by_index,
             [ac_cv_libcsplit_dummy=yes],
             [ac_cv_libcsplit=no])
           ])
 
         ac_cv_libcsplit_LIBADD="-lcsplit"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes],
+      [test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcsplit in directory: $ac_cv_with_libcsplit],
         [1])
       ])
     ])
 
   AS_IF(
@@ -174,15 +177,15 @@
     ])
   ])
 
 dnl Function to detect if libcsplit dependencies are available
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
   ])
 
 dnl Function to detect how to enable libcsplit
 AC_DEFUN([AX_LIBCSPLIT_CHECK_ENABLE],
```

### Comparing `libmsiecf-20240209/m4/common.m4` & `libmsiecf-20240425/m4/common.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for common headers and functions
 dnl
-dnl Version: 20181117
+dnl Version: 20240308
 
 dnl Function to test if a certain feature was disabled
 AC_DEFUN([AX_COMMON_ARG_DISABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
@@ -22,15 +22,15 @@
 dnl Function to test if a certain feature was enabled
 AC_DEFUN([AX_COMMON_ARG_ENABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
       [--enable-$1],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_enable_$2=$enableval],
     [ac_cv_enable_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to enable $3],
       [ac_cv_enable_$2],
       [ac_cv_enable_$2=$4])dnl
@@ -39,15 +39,15 @@
 dnl Function to test if the location of a certain feature was provided
 AC_DEFUN([AX_COMMON_ARG_WITH],
 [
   AC_ARG_WITH(
     [$1],
     [AS_HELP_STRING(
       [--with-$1[[=$5]]],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_with_$2=$withval],
     [ac_cv_with_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to use $3],
       [ac_cv_with_$2],
       [ac_cv_with_$2=$4])dnl
```

### Comparing `libmsiecf-20240209/m4/libcthreads.m4` & `libmsiecf-20240425/m4/libcthreads.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcthreads required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcthreads is available
 dnl ac_libcthreads_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCTHREADS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno],
     [ac_cv_libcthreads=no],
     [ac_cv_libcthreads=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcthreads which returns "yes" and --with-libcthreads= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect],
+      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcthreads"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcthreads],
           [1])
@@ -244,15 +246,15 @@
           [ac_cv_libcthreads_dummy=yes],
           [ac_cv_libcthreads=no])
 
         ac_cv_libcthreads_LIBADD="-lcthreads"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes],
+      [test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcthreads in directory: $ac_cv_with_libcthreads],
         [1])
       ])
     ])
 
   AS_IF(
@@ -286,15 +288,15 @@
     [dnl Check for enabling pthread support
     AX_PTHREAD_CHECK_ENABLE
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread],
     [ac_cv_libcthreads_multi_threading="winapi"])
 
   AS_IF(
     [test "x$ac_cv_libcthreads_multi_threading" != xno],
-    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local],
     [ac_cv_libcthreads=no])
   ])
 
 dnl Function to detect how to enable libcthreads
```

### Comparing `libmsiecf-20240209/m4/ltversion.m4` & `libmsiecf-20240425/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/m4/ltsugar.m4` & `libmsiecf-20240425/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/m4/host-cpu-c-abi.m4` & `libmsiecf-20240425/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/m4/libtool.m4` & `libmsiecf-20240425/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/m4/po.m4` & `libmsiecf-20240425/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/m4/libcerror.m4` & `libmsiecf-20240425/m4/libcerror.m4`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcerror required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcerror is available
 dnl ac_libcerror_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCERROR_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno],
     [ac_cv_libcerror=no],
     [ac_cv_libcerror=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcerror which returns "yes" and --with-libcerror= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect],
+      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcerror"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcerror],
           [1])
@@ -95,16 +97,17 @@
           cerror,
           libcerror_system_set_error,
           [ac_cv_libcerror_dummy=yes],
           [ac_cv_libcerror=no])
 
         ac_cv_libcerror_LIBADD="-lcerror"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes],
+      [test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcerror in directory: $ac_cv_with_libcerror],
         [1])
       ])
     ])
 
   AS_IF(
@@ -162,15 +165,15 @@
       [test "x$ac_cv_func_strerror" != xyes],
       [AC_MSG_FAILURE(
         [Missing functions: strerror_r and strerror],
         [1])
       ])
     ])
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
   ])
 
 dnl Function to detect how to enable libcerror
 AC_DEFUN([AX_LIBCERROR_CHECK_ENABLE],
```

### Comparing `libmsiecf-20240209/m4/libcnotify.m4` & `libmsiecf-20240425/m4/libcnotify.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcnotify required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcnotify is available
 dnl ac_libcnotify_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno],
     [ac_cv_libcnotify=no],
     [ac_cv_libcnotify=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcnotify which returns "yes" and --with-libcnotify= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect],
+      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcnotify"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcnotify],
           [1])
@@ -92,16 +94,17 @@
           cnotify,
           libcnotify_verbose_set,
           [ac_cv_libcnotify_dummy=yes],
           [ac_cv_libcnotify=no])
 
         ac_cv_libcnotify_LIBADD="-lcnotify"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes],
+      [test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcnotify in directory: $ac_cv_with_libcnotify],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
       [Missing headers: stdarg.h and varargs.h],
       [1])
     ])
 
   dnl Headers included in libcnotify/libcnotify_stream.c
   AC_CHECK_HEADERS([errno.h])
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
   ])
 
 dnl Function to detect how to enable libcnotify
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_ENABLE],
```

### Comparing `libmsiecf-20240209/m4/libfguid.m4` & `libmsiecf-20240425/m4/libfguid.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfguid required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfguid is available
 dnl ac_libfguid_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFGUID_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno],
     [ac_cv_libfguid=no],
     [ac_cv_libfguid=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfguid which returns "yes" and --with-libfguid= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect],
+      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfguid"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfguid],
           [1])
@@ -103,16 +105,17 @@
           fguid,
           libfguid_identifier_copy_to_utf32_string_with_index,
           [ac_cv_libfguid_dummy=yes],
           [ac_cv_libfguid=no])
 
         ac_cv_libfguid_LIBADD="-lfguid"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes],
+      [test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfguid in directory: $ac_cv_with_libfguid],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
     ])
   ])
 
 dnl Function to detect if libfguid dependencies are available
 AC_DEFUN([AX_LIBFGUID_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
   ])
 
 
 dnl Function to detect how to enable libfguid
```

### Comparing `libmsiecf-20240209/m4/libbfio.m4` & `libmsiecf-20240425/m4/libbfio.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libbfio required headers and functions
 dnl
-dnl Version: 20201125
+dnl Version: 20240413
 
 dnl Function to detect if libbfio is available
 dnl ac_libbfio_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBBFIO_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno],
     [ac_cv_libbfio=no],
     [ac_cv_libbfio=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libbfio which returns "yes" and --with-libbfio= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect],
+      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libbfio"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libbfio],
           [1])
@@ -316,16 +318,17 @@
             libbfio_file_pool_open_wide,
             [ac_cv_libbfio_dummy=yes],
             [ac_cv_libbfio=no])
           ])
 
         ac_cv_libbfio_LIBADD="-lbfio"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes],
+      [test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libbfio in directory: $ac_cv_with_libbfio],
         [1])
       ])
     ])
 
   AS_IF(
@@ -347,15 +350,15 @@
     ])
   ])
 
 dnl Function to detect if libbfio dependencies are available
 AC_DEFUN([AX_LIBBFIO_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
   ])
 
 dnl Function to detect how to enable libbfio
 AC_DEFUN([AX_LIBBFIO_CHECK_ENABLE],
```

### Comparing `libmsiecf-20240209/m4/intlmacosx.m4` & `libmsiecf-20240425/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/m4/lt~obsolete.m4` & `libmsiecf-20240425/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/m4/lib-link.m4` & `libmsiecf-20240425/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/m4/iconv.m4` & `libmsiecf-20240425/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/m4/ltoptions.m4` & `libmsiecf-20240425/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/m4/nls.m4` & `libmsiecf-20240425/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/m4/python.m4` & `libmsiecf-20240425/m4/python.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Functions for Python bindings
 dnl
-dnl Version: 20231119
+dnl Version: 20240418
 
 dnl Function to check if the python binary is available
 dnl "python${PYTHON_VERSION} python python# python#.#"
 AC_DEFUN([AX_PROG_PYTHON],
   [AS_IF(
     [test "x${PYTHON_VERSION}" != x],
     [ax_python_progs="python${PYTHON_VERSION}"],
@@ -72,18 +72,20 @@
     PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     AC_MSG_CHECKING(
       [for Python libraries])
     AC_MSG_RESULT(
       [$PYTHON_LDFLAGS])
 
-    dnl For CygWin add the -no-undefined linker flag
+    dnl For CygWin and MinGW add the -no-undefined linker flag
     AS_CASE(
-      [$host_os],
-      [cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [$build],
+      [*-*-cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-mingw*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-msys*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
       [*],[])
 
     dnl Check for the existence of Python.h
     BACKUP_CPPFLAGS="${CPPFLAGS}"
     CPPFLAGS="${CPPFLAGS} ${PYTHON_INCLUDES}"
 
     AC_CHECK_HEADERS(
```

### Comparing `libmsiecf-20240209/m4/libfvalue.m4` & `libmsiecf-20240425/m4/libfvalue.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfvalue required headers and functions
 dnl
-dnl Version: 20200711
+dnl Version: 20240413
 
 dnl Function to detect if libfvalue is available
 dnl ac_libfvalue_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFVALUE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfvalue" = xno],
     [ac_cv_libfvalue=no],
     [ac_cv_libfvalue=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfvalue which returns "yes" and --with-libfvalue= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect],
+      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfvalue"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfvalue}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfvalue}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfvalue],
           [1])
@@ -585,16 +587,17 @@
           fvalue,
           libfvalue_value_type_set_data_strings_array,
           [ac_cv_libfvalue_dummy=yes],
           [ac_cv_libfvalue=no])
 
         ac_cv_libfvalue_LIBADD="-lfvalue"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_libfvalue" != xyes],
+      [test "x$ac_cv_libfvalue" != xyes && test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfvalue in directory: $ac_cv_with_libfvalue],
         [1])
       ])
     ])
 
   AS_IF(
@@ -616,15 +619,15 @@
     ])
   ])
 
 dnl Function to detect if libfvalue dependencies are available
 AC_DEFUN([AX_LIBFVALUE_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue";
+  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue -I\$(top_srcdir)/libfvalue";
   ac_cv_libfvalue_LIBADD="../libfvalue/libfvalue.la";
 
   ac_cv_libfvalue=local
   ])
 
 dnl Function to detect how to enable libfvalue
 AC_DEFUN([AX_LIBFVALUE_CHECK_ENABLE],
```

### Comparing `libmsiecf-20240209/m4/types.m4` & `libmsiecf-20240425/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/m4/pthread.m4` & `libmsiecf-20240425/m4/pthread.m4`

 * *Files 18% similar despite different names*

```diff
@@ -1,183 +1,196 @@
 dnl Functions for pthread
 dnl
-dnl Version: 20130509
+dnl Version: 20240308
 
 dnl Function to detect if pthread is available
 AC_DEFUN([AX_PTHREAD_CHECK_LIB],
- [dnl Check if parameters were provided
- AS_IF(
-  [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect],
   [AS_IF(
-   [test -d "$ac_cv_with_pthread"],
-   [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
-   [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
-   ])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_with_pthread" = xno],
-  [ac_cv_pthread=no],
-  [dnl Check for headers
-  AC_CHECK_HEADERS([pthread.h])
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno],
+    [ac_cv_pthread=no],
+    [ac_cv_pthread=check
+    dnl Check if parameters were provided
+    dnl For both --with-pthread which returns "yes" and --with-pthread= which returns ""
+    dnl treat them as auto-detection.
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_pthread"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
+        [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
+        ])
+      ])
+    ])
+
+    AS_IF(
+      [test "x$ac_cv_pthread" = xcheck],
+      [dnl Check for headers
+      AC_CHECK_HEADERS([pthread.h])
+
+      AS_IF(
+        [test "x$ac_cv_header_pthread_h" = xno],
+        [ac_cv_pthread=no],
+        [dnl Check for the individual functions
+        ac_cv_pthread=pthread
+
+        dnl Thread functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_create,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_exit,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_join,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Condition functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_broadcast,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_signal,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_wait,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Mutex functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_lock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_trylock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Read/Write lock functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_rdlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_wrlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        ac_cv_pthread_LIBADD="-lpthread";
+      ])
+
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported pthread in directory: $ac_cv_with_pthread],
+        [1])
+      ])
+    ])
 
   AS_IF(
-   [test "x$ac_cv_header_pthread_h" = xno],
-   [ac_cv_pthread=no],
-   [dnl Check for the individual functions
-   ac_cv_pthread=pthread
-
-   dnl Thread functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_create,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_exit,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_join,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Condition functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_broadcast,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_signal,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_wait,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Mutex functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_lock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_trylock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Read/Write lock functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_rdlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_wrlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   ac_cv_pthread_LIBADD="-lpthread";
-   ])
-  ])
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_DEFINE(
+      [HAVE_PTHREAD],
+      [1],
+      [Define to 1 if you have the 'pthread' library (-lpthread).])
+    ])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_DEFINE(
-   [HAVE_PTHREAD],
-   [1],
-   [Define to 1 if you have the 'pthread' library (-lpthread).])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_pthread" != xno],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [1]) ],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [0])
+  AS_IF(
+    [test "x$ac_cv_pthread" != xno],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [1]) ],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [0])
+    ])
   ])
- ])
 
 dnl Function to detect how to enable pthread
 AC_DEFUN([AX_PTHREAD_CHECK_ENABLE],
- [AX_COMMON_ARG_WITH(
-  [pthread],
-  [pthread],
-  [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
-  [auto-detect],
-  [DIR])
-
- dnl Check for a shared library version
- AX_PTHREAD_CHECK_LIB
-
- AS_IF(
-  [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
-  [AC_SUBST(
-   [PTHREAD_CPPFLAGS],
-   [$ac_cv_pthread_CPPFLAGS])
-  ])
- AS_IF(
-  [test "x$ac_cv_pthread_LIBADD" != "x"],
-  [AC_SUBST(
-   [PTHREAD_LIBADD],
-   [$ac_cv_pthread_LIBADD])
-  ])
+  [AX_COMMON_ARG_WITH(
+    [pthread],
+    [pthread],
+    [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
+    [auto-detect],
+    [DIR])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_SUBST(
-   [ax_pthread_pc_libs_private],
-   [-lpthread])
+  dnl Check for a shared library version
+  AX_PTHREAD_CHECK_LIB
+
+  AS_IF(
+    [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
+    [AC_SUBST(
+      [PTHREAD_CPPFLAGS],
+      [$ac_cv_pthread_CPPFLAGS])
+    ])
+  AS_IF(
+    [test "x$ac_cv_pthread_LIBADD" != "x"],
+    [AC_SUBST(
+      [PTHREAD_LIBADD],
+      [$ac_cv_pthread_LIBADD])
+    ])
+
+  AS_IF(
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_SUBST(
+      [ax_pthread_pc_libs_private],
+      [-lpthread])
+    ])
   ])
- ])
```

### Comparing `libmsiecf-20240209/include/libmsiecf/definitions.h.in` & `libmsiecf-20240425/include/libmsiecf/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/include/libmsiecf/definitions.h` & `libmsiecf-20240425/include/libmsiecf/definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBMSIECF_DEFINITIONS_H )
 #define _LIBMSIECF_DEFINITIONS_H
 
 #include <libmsiecf/types.h>
 
-#define LIBMSIECF_VERSION		20240209
+#define LIBMSIECF_VERSION		20240425
 
 /* The version string
  */
-#define LIBMSIECF_VERSION_STRING	"20240209"
+#define LIBMSIECF_VERSION_STRING	"20240425"
 
 /* The file access flags
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBMSIECF_ACCESS_FLAGS
```

### Comparing `libmsiecf-20240209/include/libmsiecf/types.h.in` & `libmsiecf-20240425/include/libmsiecf/types.h.in`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/include/libmsiecf/types.h` & `libmsiecf-20240425/include/libmsiecf/types.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/include/libmsiecf/features.h.in` & `libmsiecf-20240425/include/libmsiecf/features.h.in`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/include/libmsiecf/error.h` & `libmsiecf-20240425/include/libmsiecf/error.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/include/libmsiecf/extern.h` & `libmsiecf-20240425/include/libmsiecf/extern.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/include/libmsiecf/features.h` & `libmsiecf-20240425/include/libmsiecf/features.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/include/libmsiecf/codepage.h` & `libmsiecf-20240425/include/libmsiecf/codepage.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/include/libmsiecf.h` & `libmsiecf-20240425/include/libmsiecf.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/include/libmsiecf.h.in` & `libmsiecf-20240425/include/libmsiecf.h.in`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/include/Makefile.in` & `libmsiecf-20240425/include/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -507,15 +507,20 @@
 
 EXTRA_DIST = \
 	libmsiecf.h.in \
 	libmsiecf/definitions.h.in \
 	libmsiecf/features.h.in \
 	libmsiecf/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libmsiecf.h \
+	libmsiecf/definitions.h \
+	libmsiecf/features.h \
+	libmsiecf/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -712,23 +717,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -810,17 +817,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libmsiecf.h
-	-rm -f libmsiecf/definitions.h
-	-rm -f libmsiecf/features.h
-	-rm -f libmsiecf/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libmsiecf-20240209/common/config_borlandc.h` & `libmsiecf-20240425/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/common/file_stream.h` & `libmsiecf-20240425/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/common/memory.h` & `libmsiecf-20240425/common/memory.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/common/byte_stream.h` & `libmsiecf-20240425/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/common/common.h` & `libmsiecf-20240425/common/common.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/common/config_winapi.h` & `libmsiecf-20240425/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/common/system_string.h` & `libmsiecf-20240425/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/common/types.h.in` & `libmsiecf-20240425/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/common/types.h` & `libmsiecf-20240425/common/types.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/common/config.h.in` & `libmsiecf-20240425/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/common/config.h` & `libmsiecf-20240425/common/config.h`

 * *Files 0% similar despite different names*

```diff
@@ -514,24 +514,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libmsiecf"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libmsiecf 20240209"
+#define PACKAGE_STRING "libmsiecf 20240425"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libmsiecf"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240209"
+#define PACKAGE_VERSION "20240425"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -549,15 +549,15 @@
    backward compatibility; new code need not use it. */
 #define STDC_HEADERS 1
 
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Version number of package */
-#define VERSION "20240209"
+#define VERSION "20240425"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libmsiecf-20240209/common/wide_string.h` & `libmsiecf-20240425/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/common/narrow_string.h` & `libmsiecf-20240425/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/common/config_msc.h` & `libmsiecf-20240425/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/common/Makefile.in` & `libmsiecf-20240425/common/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -460,15 +460,17 @@
 sharedstatedir = @sharedstatedir@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
-AM_CPPFLAGS = -I$(top_srcdir)/include
+AM_CPPFLAGS = \
+	-I../include -I$(top_srcdir)/include
+
 EXTRA_DIST = \
 	byte_stream.h \
 	common.h \
 	config.h \
 	config_borlandc.h \
 	config_msc.h \
 	config_winapi.h \
@@ -476,15 +478,18 @@
 	memory.h \
 	narrow_string.h \
 	system_string.h \
 	types.h \
 	types.h.in \
 	wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	config.h \
+	types.h \
+	Makefile \
 	Makefile.in
 
 all: config.h
 	$(MAKE) $(AM_MAKEFLAGS) all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -652,23 +657,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-hdr distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -748,15 +755,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f config.h
-	-rm -f types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libmsiecf-20240209/libclocale/libclocale_wide_string.c` & `libmsiecf-20240425/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libclocale/libclocale_support.h` & `libmsiecf-20240425/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libclocale/Makefile.am` & `libmsiecf-20240425/libclocale/Makefile.am`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 if HAVE_LOCAL_LIBCLOCALE
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libclocale.la
 
 libclocale_la_SOURCES = \
 	libclocale_codepage.c libclocale_codepage.h \
 	libclocale_definitions.h \
@@ -14,19 +14,17 @@
 	libclocale_libcerror.h \
 	libclocale_locale.c libclocale_locale.h \
 	libclocale_support.c libclocale_support.h \
 	libclocale_unused.h \
 	libclocale_wide_string.c libclocale_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
```

### Comparing `libmsiecf-20240209/libclocale/libclocale_definitions.h` & `libmsiecf-20240425/libclocale/libclocale_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #include <libclocale/definitions.h>
 
 /* The definitions in <libclocale/definitions.h> are copied here
  * for local use of libclocale
  */
 #else
 
-#define LIBCLOCALE_VERSION					20240107
+#define LIBCLOCALE_VERSION					20240414
 
 /* The libclocale version string
  */
-#define LIBCLOCALE_VERSION_STRING				"20240107"
+#define LIBCLOCALE_VERSION_STRING				"20240414"
 
 /* The codepage feature flag definitions
  */
 enum LIBCLOCALE_CODEPAGES_FEATURE_FLAGS
 {
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_ISO_8859		= 0x00000001UL,
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_KOI8		= 0x00000002UL,
```

### Comparing `libmsiecf-20240209/libclocale/libclocale_unused.h` & `libmsiecf-20240425/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libclocale/libclocale_libcerror.h` & `libmsiecf-20240425/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libclocale/libclocale_locale.h` & `libmsiecf-20240425/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libclocale/libclocale_support.c` & `libmsiecf-20240425/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libclocale/libclocale_codepage.c` & `libmsiecf-20240425/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libclocale/libclocale_locale.c` & `libmsiecf-20240425/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libclocale/Makefile.in` & `libmsiecf-20240425/libclocale/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -506,30 +506,31 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCLOCALE_TRUE@AM_CPPFLAGS = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	-DLOCALEDIR=\"$(datadir)/locale\" \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCLOCALE_TRUE@noinst_LTLIBRARIES = libclocale.la
 @HAVE_LOCAL_LIBCLOCALE_TRUE@libclocale_la_SOURCES = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_codepage.c libclocale_codepage.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_definitions.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_extern.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_libcerror.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_locale.c libclocale_locale.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_support.c libclocale_support.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_unused.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_wide_string.c libclocale_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -732,24 +733,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libclocale_codepage.Plo
+	-rm -f ./$(DEPDIR)/libclocale_locale.Plo
+	-rm -f ./$(DEPDIR)/libclocale_support.Plo
+	-rm -f ./$(DEPDIR)/libclocale_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -836,17 +843,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmsiecf-20240209/libclocale/libclocale_extern.h` & `libmsiecf-20240425/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libclocale/libclocale_wide_string.h` & `libmsiecf-20240425/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libclocale/libclocale_codepage.h` & `libmsiecf-20240425/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/Makefile.am` & `libmsiecf-20240425/Makefile.am`

 * *Files 12% similar despite different names*

```diff
@@ -59,16 +59,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libmsiecf.pc \
+	libmsiecf.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libmsiecf.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -91,19 +98,7 @@
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfole && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfvalue && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libmsiecf && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libmsiecf.pc
-	-rm -f libmsiecf.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_file_range.h` & `libmsiecf-20240425/libbfio/libbfio_file_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_file_range_io_handle.c` & `libmsiecf-20240425/libbfio/libbfio_file_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_support.c` & `libmsiecf-20240425/libbfio/libbfio_support.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_libcpath.h` & `libmsiecf-20240425/libbfio/libbfio_libcpath.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcpath header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_error.h` & `libmsiecf-20240425/libbfio/libbfio_error.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_libclocale.h` & `libmsiecf-20240425/libbfio/libbfio_libclocale.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libclocale header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_error.c` & `libmsiecf-20240425/libbfio/libbfio_error.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_libuna.h` & `libmsiecf-20240425/libbfio/libbfio_libuna.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_file_io_handle.h` & `libmsiecf-20240425/libbfio/libbfio_file_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_file_pool.h` & `libmsiecf-20240425/libbfio/libbfio_file_pool.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_file_range.c` & `libmsiecf-20240425/libbfio/libbfio_file_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_types.h` & `libmsiecf-20240425/libbfio/libbfio_types.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_unused.h` & `libmsiecf-20240425/libbfio/libbfio_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_libcdata.h` & `libmsiecf-20240425/libbfio/libbfio_libcdata.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_file.h` & `libmsiecf-20240425/libbfio/libbfio_file.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/Makefile.am` & `libmsiecf-20240425/libbfio/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBBFIO
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -38,17 +38,17 @@
 	libbfio_pool.c libbfio_pool.h \
 	libbfio_support.c libbfio_support.h \
 	libbfio_system_string.c libbfio_system_string.h \
 	libbfio_types.h \
 	libbfio_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_libcfile.h` & `libmsiecf-20240425/libbfio/libbfio_libcfile.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcfile header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_definitions.h` & `libmsiecf-20240425/libbfio/libbfio_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBBFIO )
 #include <libbfio/definitions.h>
 
 /* The definitions in <libbfio/definitions.h> are copied here
  * for local use of libbfio
  */
 #else
-#define LIBBFIO_VERSION					20221025
+#define LIBBFIO_VERSION					20240414
 
 /* The libbfio version string
  */
-#define LIBBFIO_VERSION_STRING				"20221025"
+#define LIBBFIO_VERSION_STRING				"20240414"
 
 /* The library flags definitions
  */
 enum LIBBFIO_FLAGS
 {
 	/* The IO handle is not managed by the library
 	 */
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_codepage.h` & `libmsiecf-20240425/libbfio/libbfio_codepage.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Codepage functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_file_io_handle.c` & `libmsiecf-20240425/libbfio/libbfio_file_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_support.h` & `libmsiecf-20240425/libbfio/libbfio_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_memory_range.h` & `libmsiecf-20240425/libbfio/libbfio_memory_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_file_pool.c` & `libmsiecf-20240425/libbfio/libbfio_file_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_file_range_io_handle.h` & `libmsiecf-20240425/libbfio/libbfio_file_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_libcthreads.h` & `libmsiecf-20240425/libbfio/libbfio_libcthreads.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcthreads header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_system_string.h` & `libmsiecf-20240425/libbfio/libbfio_system_string.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_memory_range_io_handle.c` & `libmsiecf-20240425/libbfio/libbfio_memory_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_handle.c` & `libmsiecf-20240425/libbfio/libbfio_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_file.c` & `libmsiecf-20240425/libbfio/libbfio_file.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_handle.h` & `libmsiecf-20240425/libbfio/libbfio_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_memory_range.c` & `libmsiecf-20240425/libbfio/libbfio_memory_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_pool.c` & `libmsiecf-20240425/libbfio/libbfio_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_libcerror.h` & `libmsiecf-20240425/libbfio/libbfio_libcerror.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/Makefile.in` & `libmsiecf-20240425/libbfio/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -526,16 +526,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBBFIO_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCFILE_CPPFLAGS@ \
@@ -566,15 +566,16 @@
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_memory_range_io_handle.c libbfio_memory_range_io_handle.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_pool.c libbfio_pool.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_support.c libbfio_support.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_system_string.c libbfio_system_string.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_types.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -785,24 +786,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libbfio_error.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_support.Plo
+	-rm -f ./$(DEPDIR)/libbfio_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -871,14 +886,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -889,23 +906,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_system_string.c` & `libmsiecf-20240425/libbfio/libbfio_system_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_memory_range_io_handle.h` & `libmsiecf-20240425/libbfio/libbfio_memory_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_extern.h` & `libmsiecf-20240425/libbfio/libbfio_extern.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/libbfio/libbfio_pool.h` & `libmsiecf-20240425/libbfio/libbfio_pool.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libmsiecf-20240209/config.guess` & `libmsiecf-20240425/config.guess`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/dpkg/copyright` & `libmsiecf-20240425/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/dpkg/control` & `libmsiecf-20240425/dpkg/control`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/dpkg/rules` & `libmsiecf-20240425/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/COPYING.LESSER` & `libmsiecf-20240425/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/configure` & `libmsiecf-20240425/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libmsiecf 20240209.
+# Generated by GNU Autoconf 2.71 for libmsiecf 20240425.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libmsiecf'
 PACKAGE_TARNAME='libmsiecf'
-PACKAGE_VERSION='20240209'
-PACKAGE_STRING='libmsiecf 20240209'
+PACKAGE_VERSION='20240425'
+PACKAGE_STRING='libmsiecf 20240425'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libmsiecf.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1639,15 +1639,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libmsiecf 20240209 to adapt to many kinds of systems.
+\`configure' configures libmsiecf 20240425 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1710,15 +1710,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libmsiecf 20240209:";;
+     short | recursive ) echo "Configuration of libmsiecf 20240425:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1955,15 +1955,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libmsiecf configure 20240209
+libmsiecf configure 20240425
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2676,15 +2676,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libmsiecf $as_me 20240209, which was
+It was created by libmsiecf $as_me 20240425, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4165,15 +4165,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libmsiecf'
- VERSION='20240209'
+ VERSION='20240425'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23760,15 +23760,15 @@
 printf "%s\n" "$ac_cv_with_libcerror" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno
 then :
   ac_cv_libcerror=no
 else $as_nop
   ac_cv_libcerror=check
-        if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect
+                if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   if test -d "$ac_cv_with_libcerror"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -24259,15 +24259,16 @@
 fi
 
 
         ac_cv_libcerror_LIBADD="-lcerror"
 fi
 
 fi
-    if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes
+
+    if test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcerror in directory: $ac_cv_with_libcerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -24409,15 +24410,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24511,15 +24512,15 @@
     ac_cv_libcthreads_multi_threading="no"
 else $as_nop
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno
 then :
   ac_cv_libcthreads=no
 else $as_nop
   ac_cv_libcthreads=check
-        if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect
+                if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   if test -d "$ac_cv_with_libcthreads"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -26151,15 +26152,15 @@
 
 
         ac_cv_libcthreads_LIBADD="-lcthreads"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes
+    if test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcthreads in directory: $ac_cv_with_libcthreads
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -26213,47 +26214,52 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_pthread=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_pthread" >&5
 printf "%s\n" "$ac_cv_with_pthread" >&6; }
 
-   if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno
+then :
+  ac_cv_pthread=no
+else $as_nop
+  ac_cv_pthread=check
+                if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
 then :
   if test -d "$ac_cv_with_pthread"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
 else $as_nop
   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_pthread" >&5
 printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_pthread" >&2;}
 
 fi
 
 fi
 
- if test "x$ac_cv_with_pthread" = xno
+fi
+
+    if test "x$ac_cv_pthread" = xcheck
 then :
-  ac_cv_pthread=no
-else $as_nop
-    ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
+        ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
 if test "x$ac_cv_header_pthread_h" = xyes
 then :
   printf "%s\n" "#define HAVE_PTHREAD_H 1" >>confdefs.h
 
 fi
 
 
-  if test "x$ac_cv_header_pthread_h" = xno
+      if test "x$ac_cv_header_pthread_h" = xno
 then :
   ac_cv_pthread=no
 else $as_nop
-     ac_cv_pthread=pthread
+          ac_cv_pthread=pthread
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
 printf %s "checking for pthread_create in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_create+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26287,15 +26293,15 @@
 if test "x$ac_cv_lib_pthread_pthread_create" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
 printf %s "checking for pthread_exit in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_exit+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26329,15 +26335,15 @@
 if test "x$ac_cv_lib_pthread_pthread_exit" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
 printf %s "checking for pthread_join in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_join+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26372,15 +26378,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
 printf %s "checking for pthread_cond_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26414,15 +26420,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
 printf %s "checking for pthread_cond_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26456,15 +26462,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
 printf %s "checking for pthread_cond_broadcast in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_broadcast+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26498,15 +26504,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_broadcast" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
 printf %s "checking for pthread_cond_signal in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_signal+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26540,15 +26546,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_signal" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
 printf %s "checking for pthread_cond_wait in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_wait+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26583,15 +26589,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
 printf %s "checking for pthread_mutex_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26625,15 +26631,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
 printf %s "checking for pthread_mutex_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26667,15 +26673,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
 printf %s "checking for pthread_mutex_lock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_lock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26709,15 +26715,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_lock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
 printf %s "checking for pthread_mutex_trylock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_trylock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26751,15 +26757,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_trylock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
 printf %s "checking for pthread_mutex_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26794,15 +26800,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
 printf %s "checking for pthread_rwlock_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26836,15 +26842,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
 printf %s "checking for pthread_rwlock_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26878,15 +26884,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_rdlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_rdlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26920,15 +26926,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_rdlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_wrlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_wrlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26962,15 +26968,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_wrlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27005,67 +27011,76 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-   ac_cv_pthread_LIBADD="-lpthread";
+        ac_cv_pthread_LIBADD="-lpthread";
+
+fi
+
+    if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported pthread in directory: $ac_cv_with_pthread
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
 
 printf "%s\n" "#define HAVE_PTHREAD 1" >>confdefs.h
 
 
 fi
 
- if test "x$ac_cv_pthread" != xno
+  if test "x$ac_cv_pthread" != xno
 then :
   HAVE_PTHREAD=1
 
 else $as_nop
   HAVE_PTHREAD=0
 
 
 fi
 
 
- if test "x$ac_cv_pthread_CPPFLAGS" != "x"
+  if test "x$ac_cv_pthread_CPPFLAGS" != "x"
 then :
   PTHREAD_CPPFLAGS=$ac_cv_pthread_CPPFLAGS
 
 
 fi
- if test "x$ac_cv_pthread_LIBADD" != "x"
+  if test "x$ac_cv_pthread_LIBADD" != "x"
 then :
   PTHREAD_LIBADD=$ac_cv_pthread_LIBADD
 
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
   ax_pthread_pc_libs_private=-lpthread
 
 
 fi
 
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread
 else $as_nop
   ac_cv_libcthreads_multi_threading="winapi"
 fi
 
   if test "x$ac_cv_libcthreads_multi_threading" != xno
 then :
-  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local
 else $as_nop
   ac_cv_libcthreads=no
 fi
 
@@ -27153,15 +27168,15 @@
 printf "%s\n" "$ac_cv_with_libcdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno
 then :
   ac_cv_libcdata=no
 else $as_nop
   ac_cv_libcdata=check
-        if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect
+                if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   if test -d "$ac_cv_with_libcdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -30932,15 +30947,16 @@
 fi
 
 
         ac_cv_libcdata_LIBADD="-lcdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes
+
+    if test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcdata in directory: $ac_cv_with_libcdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -30965,15 +30981,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -31043,15 +31059,15 @@
 printf "%s\n" "$ac_cv_with_libclocale" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno
 then :
   ac_cv_libclocale=no
 else $as_nop
   ac_cv_libclocale=check
-        if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect
+                if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   if test -d "$ac_cv_with_libclocale"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -31598,15 +31614,16 @@
 fi
 
 
         ac_cv_libclocale_LIBADD="-lclocale"
 fi
 
 fi
-    if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes
+
+    if test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libclocale in directory: $ac_cv_with_libclocale
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31762,15 +31779,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -31840,15 +31857,15 @@
 printf "%s\n" "$ac_cv_with_libcnotify" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno
 then :
   ac_cv_libcnotify=no
 else $as_nop
   ac_cv_libcnotify=check
-        if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect
+                if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   if test -d "$ac_cv_with_libcnotify"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -32298,15 +32315,16 @@
 fi
 
 
         ac_cv_libcnotify_LIBADD="-lcnotify"
 fi
 
 fi
-    if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes
+
+    if test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcnotify in directory: $ac_cv_with_libcnotify
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -32361,15 +32379,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32439,15 +32457,15 @@
 printf "%s\n" "$ac_cv_with_libcsplit" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno
 then :
   ac_cv_libcsplit=no
 else $as_nop
   ac_cv_libcsplit=check
-        if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect
+                if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   if test -d "$ac_cv_with_libcsplit"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -33162,15 +33180,16 @@
 
 fi
 
         ac_cv_libcsplit_LIBADD="-lcsplit"
 fi
 
 fi
-    if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes
+
+    if test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcsplit in directory: $ac_cv_with_libcsplit
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -33195,15 +33214,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -33273,15 +33292,15 @@
 printf "%s\n" "$ac_cv_with_libuna" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno
 then :
   ac_cv_libuna=no
 else $as_nop
   ac_cv_libuna=check
-        if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect
+                if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   if test -d "$ac_cv_with_libuna"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -40483,15 +40502,16 @@
   ac_cv_libuna=no
 fi
 
         ac_cv_libuna_LIBADD="-luna"
 fi
 
 fi
-    if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes
+
+    if test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libuna in directory: $ac_cv_with_libuna
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -40516,15 +40536,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -40594,15 +40614,15 @@
 printf "%s\n" "$ac_cv_with_libcfile" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno
 then :
   ac_cv_libcfile=no
 else $as_nop
   ac_cv_libcfile=check
-        if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect
+                if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   if test -d "$ac_cv_with_libcfile"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -41783,15 +41803,16 @@
 
 fi
 
         ac_cv_libcfile_LIBADD="-lcfile"
 fi
 
 fi
-    if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes
+
+    if test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcfile in directory: $ac_cv_with_libcfile
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -42105,15 +42126,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: unlink
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCFILE 1" >>confdefs.h
@@ -42183,15 +42204,15 @@
 printf "%s\n" "$ac_cv_with_libcpath" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno
 then :
   ac_cv_libcpath=no
 else $as_nop
   ac_cv_libcpath=check
-        if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect
+                if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   if test -d "$ac_cv_with_libcpath"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -42988,15 +43009,16 @@
 
 fi
 
         ac_cv_libcpath_LIBADD="-lcpath"
 fi
 
 fi
-    if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes
+
+    if test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcpath in directory: $ac_cv_with_libcpath
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -43186,15 +43208,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -43264,15 +43286,15 @@
 printf "%s\n" "$ac_cv_with_libbfio" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno
 then :
   ac_cv_libbfio=no
 else $as_nop
   ac_cv_libbfio=check
-        if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect
+                if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   if test -d "$ac_cv_with_libbfio"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -45382,15 +45404,16 @@
 
 fi
 
         ac_cv_libbfio_LIBADD="-lbfio"
 fi
 
 fi
-    if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes
+
+    if test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libbfio in directory: $ac_cv_with_libbfio
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -45415,15 +45438,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -45493,15 +45516,15 @@
 printf "%s\n" "$ac_cv_with_libfdatetime" >&6; }
 
   if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdatetime" = xno
 then :
   ac_cv_libfdatetime=no
 else $as_nop
   ac_cv_libfdatetime=check
-        if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect
+                if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
 then :
   if test -d "$ac_cv_with_libfdatetime"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfdatetime}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdatetime}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -48937,15 +48960,16 @@
 fi
 
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"
 fi
 
 fi
-    if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_libfdatetime" != xyes
+
+    if test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -48970,15 +48994,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdatetime" != xyes
 then :
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATETIME 1" >>confdefs.h
@@ -49048,15 +49072,15 @@
 printf "%s\n" "$ac_cv_with_libfguid" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno
 then :
   ac_cv_libfguid=no
 else $as_nop
   ac_cv_libfguid=check
-        if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect
+                if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   if test -d "$ac_cv_with_libfguid"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -49630,15 +49654,16 @@
 fi
 
 
         ac_cv_libfguid_LIBADD="-lfguid"
 fi
 
 fi
-    if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes
+
+    if test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfguid in directory: $ac_cv_with_libfguid
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -49663,15 +49688,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfguid" != xyes
 then :
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFGUID 1" >>confdefs.h
@@ -49741,15 +49766,15 @@
 printf "%s\n" "$ac_cv_with_libfole" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfole" = xno
 then :
   ac_cv_libfole=no
 else $as_nop
   ac_cv_libfole=check
-        if test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect
+                if test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect && test "x$ac_cv_with_libfole" != xyes
 then :
   if test -d "$ac_cv_with_libfole"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfole}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfole}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -49903,15 +49928,16 @@
 
 
 
         ac_cv_libfole_LIBADD="-lfole"
 fi
 
 fi
-    if test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect && test "x$ac_cv_libfole" != xyes
+
+    if test "x$ac_cv_libfole" != xyes && test "x$ac_cv_with_libfole" != x && test "x$ac_cv_with_libfole" != xauto-detect && test "x$ac_cv_with_libfole" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfole in directory: $ac_cv_with_libfole
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -49936,15 +49962,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfole" != xyes
 then :
 
-  ac_cv_libfole_CPPFLAGS="-I../libfole";
+  ac_cv_libfole_CPPFLAGS="-I../libfole -I\$(top_srcdir)/libfole";
   ac_cv_libfole_LIBADD="../libfole/libfole.la";
 
   ac_cv_libfole=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFOLE 1" >>confdefs.h
@@ -50014,15 +50040,15 @@
 printf "%s\n" "$ac_cv_with_libfvalue" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfvalue" = xno
 then :
   ac_cv_libfvalue=no
 else $as_nop
   ac_cv_libfvalue=check
-        if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect
+                if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes
 then :
   if test -d "$ac_cv_with_libfvalue"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfvalue}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfvalue}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -54328,15 +54354,16 @@
 fi
 
 
         ac_cv_libfvalue_LIBADD="-lfvalue"
 fi
 
 fi
-    if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_libfvalue" != xyes
+
+    if test "x$ac_cv_libfvalue" != xyes && test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfvalue in directory: $ac_cv_with_libfvalue
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -54361,15 +54388,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfvalue" != xyes
 then :
 
-  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue";
+  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue -I\$(top_srcdir)/libfvalue";
   ac_cv_libfvalue_LIBADD="../libfvalue/libfvalue.la";
 
   ac_cv_libfvalue=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFVALUE 1" >>confdefs.h
@@ -54680,16 +54707,20 @@
         PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for Python libraries" >&5
 printf %s "checking for Python libraries... " >&6; }
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $PYTHON_LDFLAGS" >&5
 printf "%s\n" "$PYTHON_LDFLAGS" >&6; }
 
-        case $host_os in #(
-  cygwin*) :
+        case $build in #(
+  *-*-cygwin*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-mingw*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-msys*) :
     PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
   *) :
      ;; #(
   *) :
      ;;
 esac
 
@@ -55723,15 +55754,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libmsiecf $as_me 20240209, which was
+This file was extended by libmsiecf $as_me 20240425, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -55791,15 +55822,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libmsiecf config.status 20240209
+libmsiecf config.status 20240425
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libmsiecf-20240209/compile` & `libmsiecf-20240425/compile`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/missing` & `libmsiecf-20240425/missing`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecf_test_error/msiecf_test_error.vcproj` & `libmsiecf-20240425/msvscpp/msiecf_test_error/msiecf_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/libfole/libfole.vcproj` & `libmsiecf-20240425/msvscpp/libfole/libfole.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/libmsiecf.sln` & `libmsiecf-20240425/msvscpp/libmsiecf.sln`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecf_test_property_type/msiecf_test_property_type.vcproj` & `libmsiecf-20240425/msvscpp/msiecf_test_property_type/msiecf_test_property_type.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecf_test_allocation_table/msiecf_test_allocation_table.vcproj` & `libmsiecf-20240425/msvscpp/msiecf_test_allocation_table/msiecf_test_allocation_table.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/libmsiecf/libmsiecf.vcproj` & `libmsiecf-20240425/msvscpp/libmsiecf/libmsiecf.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecf_test_cache_directory_table/msiecf_test_cache_directory_table.vcproj` & `libmsiecf-20240425/msvscpp/msiecf_test_cache_directory_table/msiecf_test_cache_directory_table.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/pymsiecf/pymsiecf.vcproj` & `libmsiecf-20240425/msvscpp/pymsiecf/pymsiecf.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/libfguid/libfguid.vcproj` & `libmsiecf-20240425/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecf_test_leak_values/msiecf_test_leak_values.vcproj` & `libmsiecf-20240425/msvscpp/msiecf_test_leak_values/msiecf_test_leak_values.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/libclocale/libclocale.vcproj` & `libmsiecf-20240425/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecf_test_file/msiecf_test_file.vcproj` & `libmsiecf-20240425/msvscpp/msiecf_test_file/msiecf_test_file.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/Makefile.am` & `libmsiecf-20240425/msvscpp/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -40,13 +40,11 @@
 	msiecfinfo/msiecfinfo.vcproj \
 	pymsiecf/pymsiecf.vcproj \
 	libmsiecf.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libmsiecf-20240209/msvscpp/libbfio/libbfio.vcproj` & `libmsiecf-20240425/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecfinfo/msiecfinfo.vcproj` & `libmsiecf-20240425/msvscpp/msiecfinfo/msiecfinfo.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecf_test_file_header/msiecf_test_file_header.vcproj` & `libmsiecf-20240425/msvscpp/msiecf_test_file_header/msiecf_test_file_header.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecf_test_hash_table/msiecf_test_hash_table.vcproj` & `libmsiecf-20240425/msvscpp/msiecf_test_hash_table/msiecf_test_hash_table.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/libcfile/libcfile.vcproj` & `libmsiecf-20240425/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecf_test_tools_signal/msiecf_test_tools_signal.vcproj` & `libmsiecf-20240425/msvscpp/msiecf_test_tools_signal/msiecf_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/libcdata/libcdata.vcproj` & `libmsiecf-20240425/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecf_test_support/msiecf_test_support.vcproj` & `libmsiecf-20240425/msvscpp/msiecf_test_support/msiecf_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecf_test_redirected_values/msiecf_test_redirected_values.vcproj` & `libmsiecf-20240425/msvscpp/msiecf_test_redirected_values/msiecf_test_redirected_values.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecf_test_notify/msiecf_test_notify.vcproj` & `libmsiecf-20240425/msvscpp/msiecf_test_notify/msiecf_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/libcthreads/libcthreads.vcproj` & `libmsiecf-20240425/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecf_test_item/msiecf_test_item.vcproj` & `libmsiecf-20240425/msvscpp/msiecf_test_item/msiecf_test_item.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecf_test_tools_info_handle/msiecf_test_tools_info_handle.vcproj` & `libmsiecf-20240425/msvscpp/msiecf_test_tools_info_handle/msiecf_test_tools_info_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/libcpath/libcpath.vcproj` & `libmsiecf-20240425/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecf_test_url/msiecf_test_url.vcproj` & `libmsiecf-20240425/msvscpp/msiecf_test_url/msiecf_test_url.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecf_test_tools_output/msiecf_test_tools_output.vcproj` & `libmsiecf-20240425/msvscpp/msiecf_test_tools_output/msiecf_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecf_test_leak/msiecf_test_leak.vcproj` & `libmsiecf-20240425/msvscpp/msiecf_test_leak/msiecf_test_leak.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecf_test_url_values/msiecf_test_url_values.vcproj` & `libmsiecf-20240425/msvscpp/msiecf_test_url_values/msiecf_test_url_values.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/libcsplit/libcsplit.vcproj` & `libmsiecf-20240425/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/libuna/libuna.vcproj` & `libmsiecf-20240425/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/Makefile.in` & `libmsiecf-20240425/msvscpp/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -488,15 +488,16 @@
 	msiecfinfo/msiecfinfo.vcproj \
 	pymsiecf/pymsiecf.vcproj \
 	libmsiecf.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -600,23 +601,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -695,13 +698,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libmsiecf-20240209/msvscpp/libfvalue/libfvalue.vcproj` & `libmsiecf-20240425/msvscpp/libfvalue/libfvalue.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecf_test_item_descriptor/msiecf_test_item_descriptor.vcproj` & `libmsiecf-20240425/msvscpp/msiecf_test_item_descriptor/msiecf_test_item_descriptor.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecf_test_io_handle/msiecf_test_io_handle.vcproj` & `libmsiecf-20240425/msvscpp/msiecf_test_io_handle/msiecf_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/libcnotify/libcnotify.vcproj` & `libmsiecf-20240425/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/libcerror/libcerror.vcproj` & `libmsiecf-20240425/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecfexport/msiecfexport.vcproj` & `libmsiecf-20240425/msvscpp/msiecfexport/msiecfexport.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/libfdatetime/libfdatetime.vcproj` & `libmsiecf-20240425/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecf_test_redirected/msiecf_test_redirected.vcproj` & `libmsiecf-20240425/msvscpp/msiecf_test_redirected/msiecf_test_redirected.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msvscpp/msiecf_test_directory_descriptor/msiecf_test_directory_descriptor.vcproj` & `libmsiecf-20240425/msvscpp/msiecf_test_directory_descriptor/msiecf_test_directory_descriptor.vcproj`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcfile/libcfile_extern.h` & `libmsiecf-20240425/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcfile/libcfile_support.h` & `libmsiecf-20240425/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcfile/libcfile_unused.h` & `libmsiecf-20240425/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcfile/libcfile_notify.h` & `libmsiecf-20240425/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcfile/libcfile_support.c` & `libmsiecf-20240425/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcfile/libcfile_types.h` & `libmsiecf-20240425/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcfile/Makefile.am` & `libmsiecf-20240425/libcfile/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCFILE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcfile.la
 
@@ -22,19 +22,17 @@
 	libcfile_support.c libcfile_support.h \
 	libcfile_system_string.c libcfile_system_string.h \
 	libcfile_types.h \
 	libcfile_unused.h \
 	libcfile_winapi.c libcfile_winapi.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
```

### Comparing `libmsiecf-20240209/libcfile/libcfile_notify.c` & `libmsiecf-20240425/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcfile/libcfile_system_string.h` & `libmsiecf-20240425/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcfile/libcfile_file.h` & `libmsiecf-20240425/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcfile/libcfile_libcnotify.h` & `libmsiecf-20240425/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcfile/libcfile_system_string.c` & `libmsiecf-20240425/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcfile/libcfile_error.h` & `libmsiecf-20240425/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcfile/libcfile_libcerror.h` & `libmsiecf-20240425/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcfile/libcfile_file.c` & `libmsiecf-20240425/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcfile/libcfile_libclocale.h` & `libmsiecf-20240425/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcfile/libcfile_winapi.h` & `libmsiecf-20240425/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcfile/Makefile.in` & `libmsiecf-20240425/libcfile/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -508,16 +508,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCFILE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCFILE_TRUE@noinst_LTLIBRARIES = libcfile.la
 @HAVE_LOCAL_LIBCFILE_TRUE@libcfile_la_SOURCES = \
@@ -532,15 +532,16 @@
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_notify.c libcfile_notify.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_support.c libcfile_support.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_system_string.c libcfile_system_string.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_types.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_unused.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_winapi.c libcfile_winapi.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -745,24 +746,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcfile_error.Plo
+	-rm -f ./$(DEPDIR)/libcfile_file.Plo
+	-rm -f ./$(DEPDIR)/libcfile_notify.Plo
+	-rm -f ./$(DEPDIR)/libcfile_support.Plo
+	-rm -f ./$(DEPDIR)/libcfile_system_string.Plo
+	-rm -f ./$(DEPDIR)/libcfile_winapi.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -851,17 +860,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmsiecf-20240209/libcfile/libcfile_error.c` & `libmsiecf-20240425/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcfile/libcfile_libuna.h` & `libmsiecf-20240425/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcfile/libcfile_winapi.c` & `libmsiecf-20240425/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcfile/libcfile_definitions.h` & `libmsiecf-20240425/libcfile/libcfile_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcfile/definitions.h>
 
 /* The definitions in <libcfile/definitions.h> are copied here
  * for local use of libcfile
  */
 #else
 
-#define LIBCFILE_VERSION				20240106
+#define LIBCFILE_VERSION				20240414
 
 /* The libcfile version string
  */
-#define LIBCFILE_VERSION_STRING				"20240106"
+#define LIBCFILE_VERSION_STRING				"20240414"
 
 /* The file access flags
  * bit 1	set to 1 for read access
  * bit 2	set to 1 for write access
  * bit 3	set to 1 to truncate an existing file on write
  * bit 4-8	not used
  */
```

### Comparing `libmsiecf-20240209/INSTALL` & `libmsiecf-20240425/INSTALL`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_list_element.h` & `libmsiecf-20240425/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_array.h` & `libmsiecf-20240425/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_definitions.h` & `libmsiecf-20240425/libcdata/libcdata_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcdata/definitions.h>
 
 /* The definitions in <libcdata/definitions.h> are copied here
  * for local use of libcdata
  */
 #else
 
-#define LIBCDATA_VERSION				20240103
+#define LIBCDATA_VERSION				20240414
 
 /* The libcdata version string
  */
-#define LIBCDATA_VERSION_STRING				"20240103"
+#define LIBCDATA_VERSION_STRING				"20240414"
 
 /* The comparison function definitions
  */
 enum LIBCDATA_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libmsiecf-20240209/libcdata/libcdata_libcerror.h` & `libmsiecf-20240425/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_unused.h` & `libmsiecf-20240425/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_btree.h` & `libmsiecf-20240425/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_btree.c` & `libmsiecf-20240425/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_support.c` & `libmsiecf-20240425/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_list.c` & `libmsiecf-20240425/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_extern.h` & `libmsiecf-20240425/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_list.h` & `libmsiecf-20240425/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_btree_values_list.h` & `libmsiecf-20240425/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/Makefile.am` & `libmsiecf-20240425/libcdata/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcdata.la
 
 libcdata_la_SOURCES = \
@@ -24,19 +24,17 @@
 	libcdata_range_list_value.c libcdata_range_list_value.h \
 	libcdata_support.c libcdata_support.h \
 	libcdata_tree_node.c libcdata_tree_node.h \
 	libcdata_types.h \
 	libcdata_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
```

### Comparing `libmsiecf-20240209/libcdata/libcdata_btree_node.h` & `libmsiecf-20240425/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_range_list_value.h` & `libmsiecf-20240425/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_range_list.h` & `libmsiecf-20240425/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_range_list.c` & `libmsiecf-20240425/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_array.c` & `libmsiecf-20240425/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_list_element.c` & `libmsiecf-20240425/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_libcthreads.h` & `libmsiecf-20240425/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_tree_node.h` & `libmsiecf-20240425/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_error.h` & `libmsiecf-20240425/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_types.h` & `libmsiecf-20240425/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_btree_node.c` & `libmsiecf-20240425/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_tree_node.c` & `libmsiecf-20240425/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_support.h` & `libmsiecf-20240425/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/Makefile.in` & `libmsiecf-20240425/libcdata/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -522,16 +522,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCDATA_TRUE@noinst_LTLIBRARIES = libcdata.la
 @HAVE_LOCAL_LIBCDATA_TRUE@libcdata_la_SOURCES = \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_array.c libcdata_array.h \
@@ -548,15 +548,16 @@
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list.c libcdata_range_list.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list_value.c libcdata_range_list_value.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_support.c libcdata_support.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_tree_node.c libcdata_tree_node.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_types.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -766,24 +767,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcdata_array.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_node.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_values_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_error.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list_value.Plo
+	-rm -f ./$(DEPDIR)/libcdata_support.Plo
+	-rm -f ./$(DEPDIR)/libcdata_tree_node.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -877,17 +891,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmsiecf-20240209/libcdata/libcdata_range_list_value.c` & `libmsiecf-20240425/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_btree_values_list.c` & `libmsiecf-20240425/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcdata/libcdata_error.c` & `libmsiecf-20240425/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/config.sub` & `libmsiecf-20240425/config.sub`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/setup.py` & `libmsiecf-20240425/setup.py`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/acinclude.m4` & `libmsiecf-20240425/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/config.rpath` & `libmsiecf-20240425/config.rpath`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_thread.h` & `libmsiecf-20240425/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_read_write_lock.h` & `libmsiecf-20240425/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_thread.c` & `libmsiecf-20240425/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_thread_pool.h` & `libmsiecf-20240425/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_support.h` & `libmsiecf-20240425/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_lock.h` & `libmsiecf-20240425/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_unused.h` & `libmsiecf-20240425/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_lock.c` & `libmsiecf-20240425/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_condition.h` & `libmsiecf-20240425/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_repeating_thread.h` & `libmsiecf-20240425/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/Makefile.am` & `libmsiecf-20240425/libcthreads/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCTHREADS
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcthreads.la
 
 libcthreads_la_SOURCES = \
 	libcthreads_condition.c libcthreads_condition.h \
@@ -22,19 +22,17 @@
 	libcthreads_thread.c libcthreads_thread.h \
 	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 	libcthreads_types.h \
 	libcthreads_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
```

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_support.c` & `libmsiecf-20240425/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_mutex.c` & `libmsiecf-20240425/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_queue.c` & `libmsiecf-20240425/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_mutex.h` & `libmsiecf-20240425/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_types.h` & `libmsiecf-20240425/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_thread_attributes.h` & `libmsiecf-20240425/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_condition.c` & `libmsiecf-20240425/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_error.c` & `libmsiecf-20240425/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_read_write_lock.c` & `libmsiecf-20240425/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_libcerror.h` & `libmsiecf-20240425/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_definitions.h` & `libmsiecf-20240425/libcthreads/libcthreads_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcthreads/definitions.h>
 
 /* The definitions in <libcthreads/definitions.h> are copied here
  * for local use of libcthreads
  */
 #else
 
-#define LIBCTHREADS_VERSION				20240102
+#define LIBCTHREADS_VERSION				20240413
 
 /* The libcthreads version string
  */
-#define LIBCTHREADS_VERSION_STRING			"20240102"
+#define LIBCTHREADS_VERSION_STRING			"20240413"
 
 /* The comparison function definitions
  */
 enum LIBCTHREADS_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_thread_pool.c` & `libmsiecf-20240425/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_error.h` & `libmsiecf-20240425/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_thread_attributes.c` & `libmsiecf-20240425/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_extern.h` & `libmsiecf-20240425/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_repeating_thread.c` & `libmsiecf-20240425/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcthreads/Makefile.in` & `libmsiecf-20240425/libcthreads/Makefile.in`

 * *Files 5% similar despite different names*

```diff
@@ -526,16 +526,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCTHREADS_TRUE@noinst_LTLIBRARIES = libcthreads.la
 @HAVE_LOCAL_LIBCTHREADS_TRUE@libcthreads_la_SOURCES = \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_condition.c libcthreads_condition.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_definitions.h \
@@ -550,15 +550,16 @@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_support.c libcthreads_support.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread.c libcthreads_thread.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_types.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -768,24 +769,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcthreads_condition.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_error.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_mutex.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_queue.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_read_write_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_repeating_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_support.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_attributes.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_pool.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -879,17 +893,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmsiecf-20240209/libcthreads/libcthreads_queue.h` & `libmsiecf-20240425/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libmsiecf.spec` & `libmsiecf-20240425/libmsiecf.spec`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libmsiecf
-Version: 20240209
+Version: 20240425
 Release: 1
 Summary: Library to access the MSIE Cache File (index.dat) format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libmsiecf
               
@@ -90,10 +90,10 @@
 %files -n libmsiecf-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Fri Feb  9 2024 Joachim Metz <joachim.metz@gmail.com> 20240209-1
+* Thu Apr 25 2024 Joachim Metz <joachim.metz@gmail.com> 20240425-1
 - Auto-generated
```

### Comparing `libmsiecf-20240209/test-driver` & `libmsiecf-20240425/test-driver`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcpath/libcpath_support.c` & `libmsiecf-20240425/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcpath/libcpath_libcerror.h` & `libmsiecf-20240425/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcpath/libcpath_definitions.h` & `libmsiecf-20240425/libcpath/libcpath_definitions.h`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcpath/definitions.h>
 
 /* The definitions in <libcpath/definitions.h> are copied here
  * for local use of libcpath
  */
 #else
 
-#define LIBCPATH_VERSION			20240109
+#define LIBCPATH_VERSION			20240414
 
 /* The libcpath version string
  */
-#define LIBCPATH_VERSION_STRING			"20240109"
+#define LIBCPATH_VERSION_STRING			"20240414"
 
 #if defined( WINAPI )
 #define LIBCPATH_SEPARATOR			'\\'
 
 #else
 #define LIBCPATH_SEPARATOR			'/'
```

### Comparing `libmsiecf-20240209/libcpath/Makefile.am` & `libmsiecf-20240425/libcpath/Makefile.am`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCPATH
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcpath.la
 
@@ -19,19 +19,17 @@
 	libcpath_libcsplit.h \
 	libcpath_libuna.h \
 	libcpath_support.c libcpath_support.h \
 	libcpath_system_string.c libcpath_system_string.h \
 	libcpath_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
```

### Comparing `libmsiecf-20240209/libcpath/libcpath_error.c` & `libmsiecf-20240425/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcpath/libcpath_extern.h` & `libmsiecf-20240425/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcpath/libcpath_system_string.h` & `libmsiecf-20240425/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcpath/libcpath_support.h` & `libmsiecf-20240425/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcpath/libcpath_libcsplit.h` & `libmsiecf-20240425/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcpath/libcpath_system_string.c` & `libmsiecf-20240425/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcpath/libcpath_libclocale.h` & `libmsiecf-20240425/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcpath/libcpath_error.h` & `libmsiecf-20240425/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcpath/Makefile.in` & `libmsiecf-20240425/libcpath/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -502,16 +502,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCPATH_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCPATH_TRUE@noinst_LTLIBRARIES = libcpath.la
 @HAVE_LOCAL_LIBCPATH_TRUE@libcpath_la_SOURCES = \
@@ -523,15 +523,16 @@
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libclocale.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libcsplit.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libuna.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_support.c libcpath_support.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_system_string.c libcpath_system_string.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -734,24 +735,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcpath_error.Plo
+	-rm -f ./$(DEPDIR)/libcpath_path.Plo
+	-rm -f ./$(DEPDIR)/libcpath_support.Plo
+	-rm -f ./$(DEPDIR)/libcpath_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -838,17 +845,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmsiecf-20240209/libcpath/libcpath_libuna.h` & `libmsiecf-20240425/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcpath/libcpath_unused.h` & `libmsiecf-20240425/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcpath/libcpath_path.c` & `libmsiecf-20240425/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcpath/libcpath_path.h` & `libmsiecf-20240425/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/ChangeLog` & `libmsiecf-20240425/ChangeLog`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/manuals/libmsiecf.3` & `libmsiecf-20240425/manuals/libmsiecf.3`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/manuals/msiecfexport.1` & `libmsiecf-20240425/manuals/msiecfexport.1`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/manuals/msiecfinfo.1` & `libmsiecf-20240425/manuals/msiecfinfo.1`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/manuals/Makefile.in` & `libmsiecf-20240425/manuals/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -484,15 +484,16 @@
 	msiecfinfo.1
 
 EXTRA_DIST = \
 	libmsiecf.3 \
 	msiecfexport.1 \
 	msiecfinfo.1
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -685,23 +686,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -783,13 +786,10 @@
 	mostlyclean-libtool pdf pdf-am ps ps-am sources-am \
 	sources-local splint-am splint-local tags-am uninstall \
 	uninstall-am uninstall-man uninstall-man1 uninstall-man3
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libmsiecf-20240209/tests/msiecf_test_redirected.c` & `libmsiecf-20240425/tests/msiecf_test_redirected.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_functions.h` & `libmsiecf-20240425/tests/msiecf_test_functions.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/pymsiecf_test_file.py` & `libmsiecf-20240425/tests/pymsiecf_test_file.py`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_redirected_values.c` & `libmsiecf-20240425/tests/msiecf_test_redirected_values.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_libcnotify.h` & `libmsiecf-20240425/tests/msiecf_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_file_header.c` & `libmsiecf-20240425/tests/msiecf_test_file_header.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_libclocale.h` & `libmsiecf-20240425/tests/msiecf_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_libcdata.h` & `libmsiecf-20240425/tests/msiecf_test_libcdata.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_io_handle.c` & `libmsiecf-20240425/tests/msiecf_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/test_tools.sh` & `libmsiecf-20240425/tests/test_library.sh`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env bash
-# Tests tools functions and types.
+# Tests library functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
-TOOLS_TESTS="info_handle output signal";
-TOOLS_TESTS_WITH_INPUT="";
+LIBRARY_TESTS="allocation_table cache_directory_table directory_descriptor error file_header hash_table io_handle item item_descriptor leak_values notify property_type redirected_values url_values";
+LIBRARY_TESTS_WITH_INPUT="file support";
 OPTION_SETS=();
 
 INPUT_GLOB="*";
 
 run_test()
 {
 	local TEST_NAME=$1;
 
 	local TEST_DESCRIPTION="Testing: ${TEST_NAME}";
-	local TEST_EXECUTABLE="./msiecf_test_tools_${TEST_NAME}";
+	local TEST_EXECUTABLE="./msiecf_test_${TEST_NAME}";
 
 	if ! test -x "${TEST_EXECUTABLE}";
 	then
 		TEST_EXECUTABLE="${TEST_EXECUTABLE}.exe";
 	fi
 
 	# TODO: add support for TEST_PROFILE and OPTION_SETS?
@@ -33,15 +33,15 @@
 }
 
 run_test_with_input()
 {
 	local TEST_NAME=$1;
 
 	local TEST_DESCRIPTION="Testing: ${TEST_NAME}";
-	local TEST_EXECUTABLE="./msiecf_test_tools_${TEST_NAME}";
+	local TEST_EXECUTABLE="./msiecf_test_${TEST_NAME}";
 
 	if ! test -x "${TEST_EXECUTABLE}";
 	then
 		TEST_EXECUTABLE="${TEST_EXECUTABLE}.exe";
 	fi
 
 	if ! test -d "input";
@@ -55,15 +55,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "msiecftools");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "libmsiecf");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -132,38 +132,35 @@
 			break;
 		fi
 	done
 
 	return ${RESULT};
 }
 
-if test -n "${SKIP_TOOLS_TESTS}";
+if test -n "${SKIP_LIBRARY_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
 RESULT=${EXIT_IGNORE};
 
-for TEST_NAME in ${TOOLS_TESTS};
+for TEST_NAME in ${LIBRARY_TESTS};
 do
 	run_test "${TEST_NAME}";
 	RESULT=$?;
 
 	if test ${RESULT} -ne ${EXIT_SUCCESS};
 	then
 		break;
@@ -171,15 +168,15 @@
 done
 
 if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 then
 	exit ${RESULT};
 fi
 
-for TEST_NAME in ${TOOLS_TESTS_WITH_INPUT};
+for TEST_NAME in ${LIBRARY_TESTS_WITH_INPUT};
 do
 	if test -d "input";
 	then
 		run_test_with_input "${TEST_NAME}";
 		RESULT=$?;
 	else
 		run_test "${TEST_NAME}";
```

### Comparing `libmsiecf-20240209/tests/msiecf_test_item_descriptor.c` & `libmsiecf-20240425/tests/msiecf_test_item_descriptor.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_support.c` & `libmsiecf-20240425/tests/msiecf_test_support.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_tools_signal.c` & `libmsiecf-20240425/tests/msiecf_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_property_type.c` & `libmsiecf-20240425/tests/msiecf_test_property_type.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_error.c` & `libmsiecf-20240425/tests/msiecf_test_error.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/test_msiecfinfo.sh` & `libmsiecf-20240425/tests/test_msiecfinfo.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Info tool testing script
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("msiecfinfo");
 OPTIONS_PER_PROFILE=("");
@@ -28,20 +28,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libmsiecf-20240209/tests/test_msiecfexport.sh` & `libmsiecf-20240425/tests/test_msiecfexport.sh`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Export tool testing script
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("msiecfexport");
 OPTIONS_PER_PROFILE=("");
@@ -28,20 +28,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libmsiecf-20240209/tests/Makefile.am` & `libmsiecf-20240425/tests/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTOMAKE_OPTIONS = subdir-objects
 
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -422,13 +422,12 @@
 	@LIBCSPLIT_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libmsiecf/libmsiecf.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
-
-distclean: clean
-	-rm -f Makefile
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
```

### Comparing `libmsiecf-20240209/tests/msiecf_test_url.c` & `libmsiecf-20240425/tests/msiecf_test_url.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_file.c` & `libmsiecf-20240425/tests/msiecf_test_file.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_getopt.h` & `libmsiecf-20240425/tests/msiecf_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_directory_descriptor.c` & `libmsiecf-20240425/tests/msiecf_test_directory_descriptor.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_leak.c` & `libmsiecf-20240425/tests/msiecf_test_leak.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/pymsiecf_test_support.py` & `libmsiecf-20240425/tests/pymsiecf_test_support.py`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/test_python_module.sh` & `libmsiecf-20240425/tests/test_python_module.sh`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20240120
+# Version: 20240417
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="support";
 TEST_FUNCTIONS_WITH_INPUT="file item";
 OPTION_SETS=();
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libmsiecf";
+PYTHON_MODULE="pymsiecf";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pymsiecf_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pymsiecf_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	if ! test -d "input";
 	then
 		echo "Test input directory not found.";
 
 		return ${EXIT_IGNORE};
 	fi
@@ -46,15 +49,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pymsiecf");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "${PYTHON_MODULE}");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -121,30 +124,35 @@
 }
 
 if test -n "${SKIP_PYTHON_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
+PLATFORM=`uname -s | sed 's/-.*$//'`;
+
+if test "${PLATFORM}" = "MINGW64_NT" || test "${PLATFORM}" = "MSYS_NT";
+then
+	cp ../${LIBRARY_NAME}/.libs/*.dll ../${PYTHON_MODULE}/.libs/;
+	cp ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.dll ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.pyd;
+fi
+
 RESULT=${EXIT_IGNORE};
 
 for TEST_FUNCTION in ${TEST_FUNCTIONS};
 do
 	test_python_function "${TEST_FUNCTION}";
 	RESULT=$?;
```

### Comparing `libmsiecf-20240209/tests/msiecf_test_unused.h` & `libmsiecf-20240425/tests/msiecf_test_unused.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_hash_table.c` & `libmsiecf-20240425/tests/msiecf_test_hash_table.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_item.c` & `libmsiecf-20240425/tests/msiecf_test_item.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_libuna.h` & `libmsiecf-20240425/tests/msiecf_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_leak_values.c` & `libmsiecf-20240425/tests/msiecf_test_leak_values.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_memory.c` & `libmsiecf-20240425/tests/msiecf_test_memory.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/test_runner.sh` & `libmsiecf-20240425/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_cache_directory_table.c` & `libmsiecf-20240425/tests/msiecf_test_cache_directory_table.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_libcerror.h` & `libmsiecf-20240425/tests/msiecf_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_memory.h` & `libmsiecf-20240425/tests/msiecf_test_memory.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_tools_info_handle.c` & `libmsiecf-20240425/tests/msiecf_test_tools_info_handle.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_allocation_table.c` & `libmsiecf-20240425/tests/msiecf_test_allocation_table.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_tools_output.c` & `libmsiecf-20240425/tests/msiecf_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_url_values.c` & `libmsiecf-20240425/tests/msiecf_test_url_values.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_libmsiecf.h` & `libmsiecf-20240425/tests/msiecf_test_libmsiecf.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/Makefile.in` & `libmsiecf-20240425/tests/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -881,16 +881,16 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AUTOMAKE_OPTIONS = subdir-objects
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -1280,16 +1280,18 @@
 	@LIBCSPLIT_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libmsiecf/libmsiecf.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .log .o .obj .test .test$(EXEEXT) .trs
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -1814,24 +1816,54 @@
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
 	-rm -f ../msiecftools/$(DEPDIR)/$(am__dirstamp)
 	-rm -f ../msiecftools/$(am__dirstamp)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ../msiecftools/$(DEPDIR)/info_handle.Po
+	-rm -f ../msiecftools/$(DEPDIR)/msiecftools_output.Po
+	-rm -f ../msiecftools/$(DEPDIR)/msiecftools_signal.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_allocation_table.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_cache_directory_table.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_directory_descriptor.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_error.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_file.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_file_header.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_functions.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_getopt.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_hash_table.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_io_handle.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_item.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_item_descriptor.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_leak.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_leak_values.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_memory.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_notify.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_property_type.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_redirected.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_redirected_values.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_support.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_tools_info_handle.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_tools_output.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_tools_signal.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_url.Po
+	-rm -f ./$(DEPDIR)/msiecf_test_url_values.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1942,13 +1974,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	recheck sources-am sources-local splint-am splint-local tags \
 	tags-am uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libmsiecf-20240209/tests/msiecf_test_getopt.c` & `libmsiecf-20240425/tests/msiecf_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_notify.c` & `libmsiecf-20240425/tests/msiecf_test_notify.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_macros.h` & `libmsiecf-20240425/tests/msiecf_test_macros.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_libbfio.h` & `libmsiecf-20240425/tests/msiecf_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/msiecf_test_functions.c` & `libmsiecf-20240425/tests/msiecf_test_functions.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/tests/test_library.sh` & `libmsiecf-20240425/tests/test_tools.sh`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env bash
-# Tests library functions and types.
+# Tests tools functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
-LIBRARY_TESTS="allocation_table cache_directory_table directory_descriptor error file_header hash_table io_handle item item_descriptor leak_values notify property_type redirected_values url_values";
-LIBRARY_TESTS_WITH_INPUT="file support";
+TOOLS_TESTS="info_handle output signal";
+TOOLS_TESTS_WITH_INPUT="";
 OPTION_SETS=();
 
 INPUT_GLOB="*";
 
 run_test()
 {
 	local TEST_NAME=$1;
 
 	local TEST_DESCRIPTION="Testing: ${TEST_NAME}";
-	local TEST_EXECUTABLE="./msiecf_test_${TEST_NAME}";
+	local TEST_EXECUTABLE="./msiecf_test_tools_${TEST_NAME}";
 
 	if ! test -x "${TEST_EXECUTABLE}";
 	then
 		TEST_EXECUTABLE="${TEST_EXECUTABLE}.exe";
 	fi
 
 	# TODO: add support for TEST_PROFILE and OPTION_SETS?
@@ -33,15 +33,15 @@
 }
 
 run_test_with_input()
 {
 	local TEST_NAME=$1;
 
 	local TEST_DESCRIPTION="Testing: ${TEST_NAME}";
-	local TEST_EXECUTABLE="./msiecf_test_${TEST_NAME}";
+	local TEST_EXECUTABLE="./msiecf_test_tools_${TEST_NAME}";
 
 	if ! test -x "${TEST_EXECUTABLE}";
 	then
 		TEST_EXECUTABLE="${TEST_EXECUTABLE}.exe";
 	fi
 
 	if ! test -d "input";
@@ -55,15 +55,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "libmsiecf");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "msiecftools");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -132,38 +132,35 @@
 			break;
 		fi
 	done
 
 	return ${RESULT};
 }
 
-if test -n "${SKIP_LIBRARY_TESTS}";
+if test -n "${SKIP_TOOLS_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
 RESULT=${EXIT_IGNORE};
 
-for TEST_NAME in ${LIBRARY_TESTS};
+for TEST_NAME in ${TOOLS_TESTS};
 do
 	run_test "${TEST_NAME}";
 	RESULT=$?;
 
 	if test ${RESULT} -ne ${EXIT_SUCCESS};
 	then
 		break;
@@ -171,15 +168,15 @@
 done
 
 if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 then
 	exit ${RESULT};
 fi
 
-for TEST_NAME in ${LIBRARY_TESTS_WITH_INPUT};
+for TEST_NAME in ${TOOLS_TESTS_WITH_INPUT};
 do
 	if test -d "input";
 	then
 		run_test_with_input "${TEST_NAME}";
 		RESULT=$?;
 	else
 		run_test "${TEST_NAME}";
```

### Comparing `libmsiecf-20240209/ossfuzz/ossfuzz_libmsiecf.h` & `libmsiecf-20240425/ossfuzz/ossfuzz_libmsiecf.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/ossfuzz/Makefile.am` & `libmsiecf-20240425/ossfuzz/Makefile.am`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LIB_FUZZING_ENGINE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -48,19 +48,17 @@
 	../libmsiecf/libmsiecf.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on file_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(file_fuzzer_SOURCES)
 	@echo "Running splint on item_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(item_fuzzer_SOURCES)
```

### Comparing `libmsiecf-20240209/ossfuzz/ossfuzz_libbfio.h` & `libmsiecf-20240425/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/ossfuzz/item_fuzzer.cc` & `libmsiecf-20240425/ossfuzz/item_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/ossfuzz/file_fuzzer.cc` & `libmsiecf-20240425/ossfuzz/file_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/ossfuzz/Makefile.in` & `libmsiecf-20240425/ossfuzz/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -525,16 +525,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@AM_CPPFLAGS = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -572,15 +572,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libmsiecf/libmsiecf.la \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -827,23 +828,27 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/file_fuzzer.Po
+	-rm -f ./$(DEPDIR)/item_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -928,17 +933,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on file_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(file_fuzzer_SOURCES)
 	@echo "Running splint on item_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(item_fuzzer_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmsiecf-20240209/ltmain.sh` & `libmsiecf-20240425/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcsplit/libcsplit_narrow_string.c` & `libmsiecf-20240425/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcsplit/libcsplit_definitions.h` & `libmsiecf-20240425/libcsplit/libcsplit_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 #include <libcsplit/definitions.h>
 
 /* The definitions in <libcsplit/definitions.h> are copied here
  * for local use of libcsplit
  */
 #else
 
-#define LIBCSPLIT_VERSION			20240110
+#define LIBCSPLIT_VERSION			20240414
 
 /* The libcsplit version string
  */
-#define LIBCSPLIT_VERSION_STRING		"20240110"
+#define LIBCSPLIT_VERSION_STRING		"20240414"
 
 #endif /* !defined( HAVE_LOCAL_LIBCSPLIT ) */
 
 #endif
```

### Comparing `libmsiecf-20240209/libcsplit/libcsplit_types.h` & `libmsiecf-20240425/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcsplit/libcsplit_wide_split_string.c` & `libmsiecf-20240425/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcsplit/libcsplit_support.h` & `libmsiecf-20240425/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcsplit/Makefile.am` & `libmsiecf-20240425/libcsplit/Makefile.am`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCSPLIT
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcsplit.la
 
 libcsplit_la_SOURCES = \
 	libcsplit_definitions.h \
 	libcsplit_error.c libcsplit_error.h \
@@ -16,19 +16,17 @@
 	libcsplit_support.c libcsplit_support.h \
 	libcsplit_types.h \
 	libcsplit_unused.h \
 	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 	libcsplit_wide_string.c libcsplit_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
```

### Comparing `libmsiecf-20240209/libcsplit/libcsplit_libcerror.h` & `libmsiecf-20240425/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcsplit/libcsplit_wide_string.c` & `libmsiecf-20240425/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcsplit/libcsplit_unused.h` & `libmsiecf-20240425/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcsplit/libcsplit_wide_split_string.h` & `libmsiecf-20240425/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcsplit/libcsplit_error.c` & `libmsiecf-20240425/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcsplit/libcsplit_narrow_split_string.c` & `libmsiecf-20240425/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcsplit/libcsplit_extern.h` & `libmsiecf-20240425/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcsplit/libcsplit_error.h` & `libmsiecf-20240425/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcsplit/libcsplit_support.c` & `libmsiecf-20240425/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcsplit/libcsplit_wide_string.h` & `libmsiecf-20240425/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcsplit/Makefile.in` & `libmsiecf-20240425/libcsplit/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -512,16 +512,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCSPLIT_TRUE@noinst_LTLIBRARIES = libcsplit.la
 @HAVE_LOCAL_LIBCSPLIT_TRUE@libcsplit_la_SOURCES = \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_definitions.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_error.c libcsplit_error.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_extern.h \
@@ -530,15 +530,16 @@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_libcerror.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_support.c libcsplit_support.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_types.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_unused.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_string.c libcsplit_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -743,24 +744,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcsplit_error.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_support.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -849,17 +858,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmsiecf-20240209/libcsplit/libcsplit_narrow_split_string.h` & `libmsiecf-20240425/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcsplit/libcsplit_narrow_string.h` & `libmsiecf-20240425/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/po/remove-potcdate.sin` & `libmsiecf-20240425/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/po/Makefile.in.in` & `libmsiecf-20240425/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/po/en@quot.header` & `libmsiecf-20240425/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/po/en@boldquot.header` & `libmsiecf-20240425/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/po/insert-header.sin` & `libmsiecf-20240425/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/po/Makevars` & `libmsiecf-20240425/po/Makevars`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/po/Makevars.in` & `libmsiecf-20240425/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/po/Rules-quot` & `libmsiecf-20240425/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_1251.c` & `libmsiecf-20240425/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_utf16_string.c` & `libmsiecf-20240425/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_base16_stream.c` & `libmsiecf-20240425/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_utf8_stream.h` & `libmsiecf-20240425/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_2.h` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_932.c` & `libmsiecf-20240425/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_dingbats.h` & `libmsiecf-20240425/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_utf8_string.c` & `libmsiecf-20240425/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_base64_stream.c` & `libmsiecf-20240425/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_error.h` & `libmsiecf-20240425/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_turkish.h` & `libmsiecf-20240425/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_unicode_character.c` & `libmsiecf-20240425/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_gaelic.c` & `libmsiecf-20240425/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_arabic.h` & `libmsiecf-20240425/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_thai.c` & `libmsiecf-20240425/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_874.h` & `libmsiecf-20240425/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_15.h` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_utf8_string.h` & `libmsiecf-20240425/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_16.c` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_1255.c` & `libmsiecf-20240425/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_utf7_stream.c` & `libmsiecf-20240425/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_byte_stream.h` & `libmsiecf-20240425/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_koi8_u.c` & `libmsiecf-20240425/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_unused.h` & `libmsiecf-20240425/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_6.c` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_14.c` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_base64_stream.h` & `libmsiecf-20240425/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_error.c` & `libmsiecf-20240425/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_centraleurroman.h` & `libmsiecf-20240425/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_romanian.c` & `libmsiecf-20240425/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_6.h` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_9.c` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_russian.h` & `libmsiecf-20240425/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_dingbats.c` & `libmsiecf-20240425/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_15.c` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_936.c` & `libmsiecf-20240425/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_croatian.h` & `libmsiecf-20240425/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_scsu.h` & `libmsiecf-20240425/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/Makefile.am` & `libmsiecf-20240425/libuna/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBUNA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libuna.la
 
 libuna_la_SOURCES = \
 	libuna_base16_stream.c libuna_base16_stream.h \
 	libuna_base32_stream.c libuna_base32_stream.h \
@@ -73,19 +73,17 @@
 	libuna_utf32_stream.c libuna_utf32_stream.h \
 	libuna_utf32_string.c libuna_utf32_string.h \
 	libuna_utf7_stream.c libuna_utf7_stream.h \
 	libuna_utf8_stream.c libuna_utf8_stream.h \
 	libuna_utf8_string.c libuna_utf8_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
```

### Comparing `libmsiecf-20240209/libuna/libuna_utf32_stream.c` & `libmsiecf-20240425/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_936.h` & `libmsiecf-20240425/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_10.c` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_roman.c` & `libmsiecf-20240425/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_utf7_stream.h` & `libmsiecf-20240425/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_3.h` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_thai.h` & `libmsiecf-20240425/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_farsi.h` & `libmsiecf-20240425/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_ukrainian.c` & `libmsiecf-20240425/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_inuit.c` & `libmsiecf-20240425/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_932.h` & `libmsiecf-20240425/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_874.c` & `libmsiecf-20240425/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_5.c` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_10.h` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_definitions.h` & `libmsiecf-20240425/libuna/libuna_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 
 /* The definitions in <libuna/definitions.h> are copied here
  * for local use of libuna
  */
 #else
 #include <byte_stream.h>
 
-#define LIBUNA_VERSION						20240130
+#define LIBUNA_VERSION						20240414
 
 /* The libuna version string
  */
-#define LIBUNA_VERSION_STRING					"20240130"
+#define LIBUNA_VERSION_STRING					"20240414"
 
 /* The endian definitions
  */
 #define	LIBUNA_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define	LIBUNA_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The codepage definitions
```

### Comparing `libmsiecf-20240209/libuna/libuna_url_stream.h` & `libmsiecf-20240425/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_icelandic.h` & `libmsiecf-20240425/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_koi8_u.h` & `libmsiecf-20240425/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_utf16_stream.c` & `libmsiecf-20240425/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_1253.c` & `libmsiecf-20240425/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_4.h` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_greek.c` & `libmsiecf-20240425/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_libcerror.h` & `libmsiecf-20240425/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_centraleurroman.c` & `libmsiecf-20240425/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_1254.c` & `libmsiecf-20240425/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_13.h` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_7.h` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_1255.h` & `libmsiecf-20240425/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_unicode_character.h` & `libmsiecf-20240425/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_8.h` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_13.c` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_949.h` & `libmsiecf-20240425/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_cyrillic.c` & `libmsiecf-20240425/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_celtic.c` & `libmsiecf-20240425/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_support.h` & `libmsiecf-20240425/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_4.c` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_949.c` & `libmsiecf-20240425/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_utf16_stream.h` & `libmsiecf-20240425/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_symbol.c` & `libmsiecf-20240425/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_roman.h` & `libmsiecf-20240425/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_1257.c` & `libmsiecf-20240425/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_1254.h` & `libmsiecf-20240425/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_950.c` & `libmsiecf-20240425/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_extern.h` & `libmsiecf-20240425/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_1256.c` & `libmsiecf-20240425/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_types.h` & `libmsiecf-20240425/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_base32_stream.h` & `libmsiecf-20240425/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_1253.h` & `libmsiecf-20240425/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_16.h` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_utf8_stream.c` & `libmsiecf-20240425/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_1250.h` & `libmsiecf-20240425/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_2.c` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_support.c` & `libmsiecf-20240425/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_koi8_r.c` & `libmsiecf-20240425/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_5.h` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_utf16_string.h` & `libmsiecf-20240425/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_utf32_string.c` & `libmsiecf-20240425/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_icelandic.c` & `libmsiecf-20240425/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_1256.h` & `libmsiecf-20240425/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_utf32_string.h` & `libmsiecf-20240425/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_romanian.h` & `libmsiecf-20240425/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_8.c` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_koi8_r.h` & `libmsiecf-20240425/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_cyrillic.h` & `libmsiecf-20240425/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_arabic.c` & `libmsiecf-20240425/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_croatian.c` & `libmsiecf-20240425/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_9.h` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_greek.h` & `libmsiecf-20240425/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_1258.h` & `libmsiecf-20240425/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_7.c` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/Makefile.in` & `libmsiecf-20240425/libuna/Makefile.in`

 * *Files 11% similar despite different names*

```diff
@@ -680,16 +680,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBUNA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBUNA_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBUNA_TRUE@noinst_LTLIBRARIES = libuna.la
 @HAVE_LOCAL_LIBUNA_TRUE@libuna_la_SOURCES = \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base16_stream.c libuna_base16_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base32_stream.c libuna_base32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base64_stream.c libuna_base64_stream.h \
@@ -755,15 +755,16 @@
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf16_string.c libuna_utf16_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_stream.c libuna_utf32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_string.c libuna_utf32_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf7_stream.c libuna_utf7_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_stream.c libuna_utf8_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_string.c libuna_utf8_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1025,24 +1026,89 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libuna_base16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base64_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_byte_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_10.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_13.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_14.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_15.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_16.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_2.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_3.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_4.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_5.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_6.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_7.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_8.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_9.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_r.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_u.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_arabic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_celtic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_centraleurroman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_croatian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_cyrillic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_dingbats.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_farsi.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_gaelic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_greek.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_icelandic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_inuit.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_roman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_romanian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_russian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_symbol.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_thai.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_turkish.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_ukrainian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1250.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1251.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1252.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1253.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1254.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1255.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1256.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1257.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1258.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_874.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_932.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_936.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_949.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_950.Plo
+	-rm -f ./$(DEPDIR)/libuna_error.Plo
+	-rm -f ./$(DEPDIR)/libuna_scsu.Plo
+	-rm -f ./$(DEPDIR)/libuna_support.Plo
+	-rm -f ./$(DEPDIR)/libuna_unicode_character.Plo
+	-rm -f ./$(DEPDIR)/libuna_url_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf7_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1188,17 +1254,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_3.c` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_1250.c` & `libmsiecf-20240425/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_scsu.c` & `libmsiecf-20240425/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_1252.c` & `libmsiecf-20240425/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_turkish.c` & `libmsiecf-20240425/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_ukrainian.h` & `libmsiecf-20240425/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_russian.c` & `libmsiecf-20240425/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_1258.c` & `libmsiecf-20240425/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_celtic.h` & `libmsiecf-20240425/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_byte_stream.c` & `libmsiecf-20240425/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_gaelic.h` & `libmsiecf-20240425/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_utf32_stream.h` & `libmsiecf-20240425/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_symbol.h` & `libmsiecf-20240425/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_1257.h` & `libmsiecf-20240425/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_inuit.h` & `libmsiecf-20240425/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_mac_farsi.c` & `libmsiecf-20240425/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_950.h` & `libmsiecf-20240425/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_url_stream.c` & `libmsiecf-20240425/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_1251.h` & `libmsiecf-20240425/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_windows_1252.h` & `libmsiecf-20240425/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_codepage_iso_8859_14.h` & `libmsiecf-20240425/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_base16_stream.h` & `libmsiecf-20240425/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libuna/libuna_base32_stream.c` & `libmsiecf-20240425/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/Makefile.in` & `libmsiecf-20240425/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -625,16 +625,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libmsiecf.pc \
+	libmsiecf.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libmsiecf.pc
 
 all: all-recursive
 
@@ -1051,23 +1058,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-recursive
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-recursive
+	-rm -f $(am__CONFIG_DISTCLEAN_FILES)
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-libtool \
 	distclean-tags
 
 dvi: dvi-recursive
 
 dvi-am:
 
@@ -1178,22 +1188,10 @@
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfole && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfvalue && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libmsiecf && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libmsiecf.pc
-	-rm -f libmsiecf.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_filetime.c` & `libmsiecf-20240425/libfvalue/libfvalue_filetime.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_utf16_string.c` & `libmsiecf-20240425/libfvalue/libfvalue_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_libfwnt.h` & `libmsiecf-20240425/libfvalue/libfvalue_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_value.c` & `libmsiecf-20240425/libfvalue/libfvalue_value.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_value.h` & `libmsiecf-20240425/libfvalue/libfvalue_value.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_definitions.h` & `libmsiecf-20240425/libfvalue/libfvalue_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfvalue/definitions.h> are copied here
  * for local use of libfvalue
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFVALUE_VERSION						20240124
+#define LIBFVALUE_VERSION						20240415
 
 /* The libfvalue version string
  */
-#define LIBFVALUE_VERSION_STRING					"20240124"
+#define LIBFVALUE_VERSION_STRING					"20240415"
 
 /* The endian definitions
  */
 #define LIBFVALUE_ENDIAN_BIG						_BYTE_STREAM_ENDIAN_BIG
 #define LIBFVALUE_ENDIAN_LITTLE						_BYTE_STREAM_ENDIAN_LITTLE
 #define LIBFVALUE_ENDIAN_NATIVE						(uint8_t) 'n'
```

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_codepage.h` & `libmsiecf-20240425/libfvalue/libfvalue_codepage.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_split_utf16_string.c` & `libmsiecf-20240425/libfvalue/libfvalue_split_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_error.c` & `libmsiecf-20240425/libfvalue/libfvalue_error.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_utf8_string.c` & `libmsiecf-20240425/libfvalue/libfvalue_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_unused.h` & `libmsiecf-20240425/libfvalue/libfvalue_unused.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_split_utf16_string.h` & `libmsiecf-20240425/libfvalue/libfvalue_split_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_filetime.h` & `libmsiecf-20240425/libfvalue/libfvalue_filetime.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_support.c` & `libmsiecf-20240425/libfvalue/libfvalue_support.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_extern.h` & `libmsiecf-20240425/libfvalue/libfvalue_extern.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/Makefile.am` & `libmsiecf-20240425/libfvalue/Makefile.am`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFVALUE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFDATETIME_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
@@ -40,19 +40,17 @@
 	libfvalue_value_type.c libfvalue_value_type.h \
 	libfvalue_support.c libfvalue_support.h \
 	libfvalue_unused.h \
 	libfvalue_utf8_string.c libfvalue_utf8_string.h \
 	libfvalue_utf16_string.c libfvalue_utf16_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfvalue ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvalue_la_SOURCES)
```

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_value_type.h` & `libmsiecf-20240425/libfvalue/libfvalue_value_type.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_libcerror.h` & `libmsiecf-20240425/libfvalue/libfvalue_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_split_utf8_string.c` & `libmsiecf-20240425/libfvalue/libfvalue_split_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_data_handle.h` & `libmsiecf-20240425/libfvalue/libfvalue_data_handle.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_libcnotify.h` & `libmsiecf-20240425/libfvalue/libfvalue_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_data_handle.c` & `libmsiecf-20240425/libfvalue/libfvalue_data_handle.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_integer.c` & `libmsiecf-20240425/libfvalue/libfvalue_integer.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_value_type.c` & `libmsiecf-20240425/libfvalue/libfvalue_value_type.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_integer.h` & `libmsiecf-20240425/libfvalue/libfvalue_integer.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_binary_data.h` & `libmsiecf-20240425/libfvalue/libfvalue_binary_data.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_value_entry.h` & `libmsiecf-20240425/libfvalue/libfvalue_value_entry.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_utf16_string.h` & `libmsiecf-20240425/libfvalue/libfvalue_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_error.h` & `libmsiecf-20240425/libfvalue/libfvalue_error.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_table.h` & `libmsiecf-20240425/libfvalue/libfvalue_table.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_libfguid.h` & `libmsiecf-20240425/libfvalue/libfvalue_libfguid.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_split_utf8_string.h` & `libmsiecf-20240425/libfvalue/libfvalue_split_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_floating_point.h` & `libmsiecf-20240425/libfvalue/libfvalue_floating_point.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_libfdatetime.h` & `libmsiecf-20240425/libfvalue/libfvalue_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_string.h` & `libmsiecf-20240425/libfvalue/libfvalue_string.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_binary_data.c` & `libmsiecf-20240425/libfvalue/libfvalue_binary_data.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_value_entry.c` & `libmsiecf-20240425/libfvalue/libfvalue_value_entry.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_libcdata.h` & `libmsiecf-20240425/libfvalue/libfvalue_libcdata.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_support.h` & `libmsiecf-20240425/libfvalue/libfvalue_support.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_table.c` & `libmsiecf-20240425/libfvalue/libfvalue_table.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/Makefile.in` & `libmsiecf-20240425/libfvalue/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -543,16 +543,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFVALUE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBFDATETIME_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBFGUID_CPPFLAGS@ \
@@ -585,15 +585,16 @@
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_entry.c libfvalue_value_entry.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_type.c libfvalue_value_type.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_support.c libfvalue_support.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_unused.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf8_string.c libfvalue_utf8_string.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf16_string.c libfvalue_utf16_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -808,24 +809,42 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfvalue_binary_data.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_error.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_filetime.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_floating_point.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_integer.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_split_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_split_utf8_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_support.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_table.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_utf8_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value_entry.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value_type.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -924,17 +943,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfvalue ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvalue_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_utf8_string.h` & `libmsiecf-20240425/libfvalue/libfvalue_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_floating_point.c` & `libmsiecf-20240425/libfvalue/libfvalue_floating_point.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_types.h` & `libmsiecf-20240425/libfvalue/libfvalue_types.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_string.c` & `libmsiecf-20240425/libfvalue/libfvalue_string.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfvalue/libfvalue_libuna.h` & `libmsiecf-20240425/libfvalue/libfvalue_libuna.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcnotify/libcnotify_definitions.h` & `libmsiecf-20240425/libcnotify/libcnotify_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcnotify/definitions.h>
 
 /* The definitions in <libcnotify/definitions.h> are copied here
  * for local use of libcnotify
  */
 #else
 
-#define LIBCNOTIFY_VERSION				20240108
+#define LIBCNOTIFY_VERSION				20240414
 
 /* The libcnotify version string
  */
-#define LIBCNOTIFY_VERSION_STRING			"20240108"
+#define LIBCNOTIFY_VERSION_STRING			"20240414"
 
 /* The print data flags
  */
 enum LIBCNOTIFY_NOTIFY_PRINT_DATA_FLAGS
 {
 	LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA		= 0x01,
 };
```

### Comparing `libmsiecf-20240209/libcnotify/libcnotify_extern.h` & `libmsiecf-20240425/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcnotify/libcnotify_support.c` & `libmsiecf-20240425/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcnotify/libcnotify_stream.h` & `libmsiecf-20240425/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcnotify/Makefile.am` & `libmsiecf-20240425/libcnotify/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCNOTIFY
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcnotify.la
 
 libcnotify_la_SOURCES = \
 	libcnotify_definitions.h \
 	libcnotify_extern.h \
@@ -13,19 +13,17 @@
 	libcnotify_print.c libcnotify_print.h \
 	libcnotify_stream.c libcnotify_stream.h \
 	libcnotify_support.c libcnotify_support.h \
 	libcnotify_unused.h \
 	libcnotify_verbose.c libcnotify_verbose.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
```

### Comparing `libmsiecf-20240209/libcnotify/libcnotify_unused.h` & `libmsiecf-20240425/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcnotify/libcnotify_verbose.h` & `libmsiecf-20240425/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcnotify/libcnotify_print.h` & `libmsiecf-20240425/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcnotify/libcnotify_stream.c` & `libmsiecf-20240425/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcnotify/libcnotify_support.h` & `libmsiecf-20240425/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcnotify/libcnotify_verbose.c` & `libmsiecf-20240425/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcnotify/Makefile.in` & `libmsiecf-20240425/libcnotify/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -504,30 +504,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@noinst_LTLIBRARIES = libcnotify.la
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@libcnotify_la_SOURCES = \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_definitions.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_extern.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_libcerror.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_print.c libcnotify_print.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_stream.c libcnotify_stream.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_support.c libcnotify_support.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_unused.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_verbose.c libcnotify_verbose.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -730,24 +731,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcnotify_print.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_stream.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_support.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_verbose.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -834,17 +841,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmsiecf-20240209/libcnotify/libcnotify_libcerror.h` & `libmsiecf-20240425/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcnotify/libcnotify_print.c` & `libmsiecf-20240425/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msiecftools/msiecftools_signal.h` & `libmsiecf-20240425/msiecftools/msiecftools_signal.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msiecftools/msiecftools_i18n.h` & `libmsiecf-20240425/msiecftools/msiecftools_i18n.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msiecftools/msiecftools_getopt.c` & `libmsiecf-20240425/msiecftools/msiecftools_getopt.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msiecftools/info_handle.h` & `libmsiecf-20240425/msiecftools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msiecftools/msiecftools_libcerror.h` & `libmsiecf-20240425/msiecftools/msiecftools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msiecftools/msiecftools_unused.h` & `libmsiecf-20240425/msiecftools/msiecftools_unused.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msiecftools/msiecftools_libuna.h` & `libmsiecf-20240425/msiecftools/msiecftools_libuna.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msiecftools/Makefile.am` & `libmsiecf-20240425/msiecftools/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -64,19 +64,17 @@
 	@LIBUNA_LIBADD@ \
 	../libmsiecf/libmsiecf.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on msiecfexport ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(msiecfexport_SOURCES)
 	@echo "Running splint on msiecfinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(msiecfinfo_SOURCES)
```

### Comparing `libmsiecf-20240209/msiecftools/info_handle.c` & `libmsiecf-20240425/msiecftools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msiecftools/export_handle.c` & `libmsiecf-20240425/msiecftools/export_handle.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msiecftools/msiecftools_getopt.h` & `libmsiecf-20240425/msiecftools/msiecftools_getopt.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msiecftools/msiecfinfo.c` & `libmsiecf-20240425/msiecftools/msiecfinfo.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msiecftools/msiecftools_signal.c` & `libmsiecf-20240425/msiecftools/msiecftools_signal.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msiecftools/msiecftools_libbfio.h` & `libmsiecf-20240425/msiecftools/msiecftools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msiecftools/msiecfexport.c` & `libmsiecf-20240425/msiecftools/msiecfexport.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msiecftools/msiecftools_libclocale.h` & `libmsiecf-20240425/msiecftools/msiecftools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msiecftools/log_handle.c` & `libmsiecf-20240425/msiecftools/log_handle.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msiecftools/msiecftools_output.h` & `libmsiecf-20240425/msiecftools/msiecftools_output.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msiecftools/export_handle.h` & `libmsiecf-20240425/msiecftools/export_handle.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msiecftools/Makefile.in` & `libmsiecf-20240425/msiecftools/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -505,16 +505,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -569,15 +569,16 @@
 	@LIBUNA_LIBADD@ \
 	../libmsiecf/libmsiecf.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -830,23 +831,33 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/export_handle.Po
+	-rm -f ./$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/log_handle.Po
+	-rm -f ./$(DEPDIR)/msiecfexport.Po
+	-rm -f ./$(DEPDIR)/msiecfinfo.Po
+	-rm -f ./$(DEPDIR)/msiecftools_getopt.Po
+	-rm -f ./$(DEPDIR)/msiecftools_output.Po
+	-rm -f ./$(DEPDIR)/msiecftools_signal.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -937,17 +948,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on msiecfexport ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(msiecfexport_SOURCES)
 	@echo "Running splint on msiecfinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(msiecfinfo_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmsiecf-20240209/msiecftools/log_handle.h` & `libmsiecf-20240425/msiecftools/log_handle.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msiecftools/msiecftools_output.c` & `libmsiecf-20240425/msiecftools/msiecftools_output.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msiecftools/msiecftools_libmsiecf.h` & `libmsiecf-20240425/msiecftools/msiecftools_libmsiecf.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msiecftools/msiecftools_libfdatetime.h` & `libmsiecf-20240425/msiecftools/msiecftools_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/msiecftools/msiecftools_libcnotify.h` & `libmsiecf-20240425/msiecftools/msiecftools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcerror/libcerror_system.c` & `libmsiecf-20240425/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcerror/libcerror_error.c` & `libmsiecf-20240425/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcerror/libcerror_extern.h` & `libmsiecf-20240425/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcerror/Makefile.am` & `libmsiecf-20240425/libcerror/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 if HAVE_LOCAL_LIBCERROR
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common 
 
 noinst_LTLIBRARIES = libcerror.la
 
 libcerror_la_SOURCES = \
 	libcerror_definitions.h \
 	libcerror_extern.h \
 	libcerror_error.c libcerror_error.h \
 	libcerror_support.c libcerror_support.h \
 	libcerror_system.c libcerror_system.h \
 	libcerror_types.h \
 	libcerror_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
```

### Comparing `libmsiecf-20240209/libcerror/libcerror_types.h` & `libmsiecf-20240425/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcerror/libcerror_support.h` & `libmsiecf-20240425/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcerror/libcerror_error.h` & `libmsiecf-20240425/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcerror/libcerror_system.h` & `libmsiecf-20240425/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcerror/libcerror_definitions.h` & `libmsiecf-20240425/libcerror/libcerror_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcerror/definitions.h>
 
 /* The definitions in <libcerror/definitions.h> are copied here
  * for local use of libcerror
  */
 #else
 
-#define LIBCERROR_VERSION				20240101
+#define LIBCERROR_VERSION				20240413
 
 /* The libcerror version string
  */
-#define LIBCERROR_VERSION_STRING			"20240101"
+#define LIBCERROR_VERSION_STRING			"20240413"
 
 /* The error domains
  */
 enum LIBCERROR_ERROR_DOMAINS
 {
 	LIBCERROR_ERROR_DOMAIN_ARGUMENTS		= (int) 'a',
 	LIBCERROR_ERROR_DOMAIN_CONVERSION		= (int) 'c',
```

### Comparing `libmsiecf-20240209/libcerror/libcerror_support.c` & `libmsiecf-20240425/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcerror/libcerror_unused.h` & `libmsiecf-20240425/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libcerror/Makefile.in` & `libmsiecf-20240425/libcerror/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -501,28 +501,29 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCERROR_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/common 
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../common -I$(top_srcdir)/common 
 
 @HAVE_LOCAL_LIBCERROR_TRUE@noinst_LTLIBRARIES = libcerror.la
 @HAVE_LOCAL_LIBCERROR_TRUE@libcerror_la_SOURCES = \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_definitions.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_extern.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_error.c libcerror_error.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_support.c libcerror_support.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_system.c libcerror_system.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_types.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -724,24 +725,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcerror_error.Plo
+	-rm -f ./$(DEPDIR)/libcerror_support.Plo
+	-rm -f ./$(DEPDIR)/libcerror_system.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -827,17 +833,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_floatingtime.h` & `libmsiecf-20240425/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_nsf_timedate.c` & `libmsiecf-20240425/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_error.h` & `libmsiecf-20240425/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_floatingtime.c` & `libmsiecf-20240425/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_support.h` & `libmsiecf-20240425/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_hfs_time.h` & `libmsiecf-20240425/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_definitions.h` & `libmsiecf-20240425/libfdatetime/libfdatetime_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfdatetime/definitions.h> are copied here
  * for local use of libfdatetime
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFDATETIME_VERSION					20240115
+#define LIBFDATETIME_VERSION					20240415
 
 /* The version string
  */
-#define LIBFDATETIME_VERSION_STRING				"20240115"
+#define LIBFDATETIME_VERSION_STRING				"20240415"
 
 /* The byte order definitions
  */
 #define LIBFDATETIME_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFDATETIME_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The string format definition flags
```

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_hfs_time.c` & `libmsiecf-20240425/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfdatetime/Makefile.am` & `libmsiecf-20240425/libfdatetime/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFDATETIME
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfdatetime.la
 
 libfdatetime_la_SOURCES = \
 	libfdatetime_date_time_values.c libfdatetime_date_time_values.h \
 	libfdatetime_definitions.h \
@@ -20,19 +20,17 @@
 	libfdatetime_posix_time.c libfdatetime_posix_time.h \
 	libfdatetime_support.c libfdatetime_support.h \
 	libfdatetime_systemtime.c libfdatetime_systemtime.h \
 	libfdatetime_types.h \
 	libfdatetime_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdatetime ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdatetime_la_SOURCES)
```

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_filetime.c` & `libmsiecf-20240425/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_systemtime.h` & `libmsiecf-20240425/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_extern.h` & `libmsiecf-20240425/libfdatetime/libfdatetime_extern.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_posix_time.c` & `libmsiecf-20240425/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_unused.h` & `libmsiecf-20240425/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_fat_date_time.h` & `libmsiecf-20240425/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_systemtime.c` & `libmsiecf-20240425/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_nsf_timedate.h` & `libmsiecf-20240425/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_libcerror.h` & `libmsiecf-20240425/libfdatetime/libfdatetime_libcerror.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_support.c` & `libmsiecf-20240425/libfdatetime/libfdatetime_support.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_error.c` & `libmsiecf-20240425/libfdatetime/libfdatetime_error.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_posix_time.h` & `libmsiecf-20240425/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_date_time_values.h` & `libmsiecf-20240425/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_filetime.h` & `libmsiecf-20240425/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_date_time_values.c` & `libmsiecf-20240425/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_types.h` & `libmsiecf-20240425/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/libfdatetime/Makefile.in` & `libmsiecf-20240425/libfdatetime/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -523,16 +523,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFDATETIME_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFDATETIME_TRUE@noinst_LTLIBRARIES = libfdatetime.la
 @HAVE_LOCAL_LIBFDATETIME_TRUE@libfdatetime_la_SOURCES = \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_date_time_values.c libfdatetime_date_time_values.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_definitions.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_extern.h \
@@ -545,15 +545,16 @@
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_nsf_timedate.c libfdatetime_nsf_timedate.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_posix_time.c libfdatetime_posix_time.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_support.c libfdatetime_support.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_systemtime.c libfdatetime_systemtime.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_types.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -762,24 +763,36 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfdatetime_date_time_values.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_error.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_fat_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_filetime.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_floatingtime.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_hfs_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_nsf_timedate.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_posix_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_support.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_systemtime.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -872,17 +885,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdatetime ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdatetime_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libmsiecf-20240209/libfdatetime/libfdatetime_fat_date_time.c` & `libmsiecf-20240425/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/aclocal.m4` & `libmsiecf-20240425/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libmsiecf-20240209/configure.ac` & `libmsiecf-20240425/configure.ac`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libmsiecf],
- [20240209],
+ [20240425],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libmsiecf.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```


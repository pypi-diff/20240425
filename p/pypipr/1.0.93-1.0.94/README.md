# Comparing `tmp/pypipr-1.0.93.tar.gz` & `tmp/pypipr-1.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypipr-1.0.93.tar", max compression
+gzip compressed data, was "pypipr-1.0.94.tar", max compression
```

## Comparing `pypipr-1.0.93.tar` & `pypipr-1.0.94.tar`

### file list

```diff
@@ -1,75 +1,76 @@
--rw-r--r--   0        0        0     3347 2024-04-24 08:30:19.029048 pypipr-1.0.93/pypipr/__init__.py
--rw-r--r--   0        0        0     2229 2024-03-17 17:38:37.508083 pypipr-1.0.93/pypipr/ibuiltins/ComparePerformance.py
--rw-r--r--   0        0        0      100 2024-03-17 17:38:37.508083 pypipr-1.0.93/pypipr/ibuiltins/LINUX.py
--rw-r--r--   0        0        0     7358 2024-04-23 10:50:10.015024 pypipr-1.0.93/pypipr/ibuiltins/RunParallel.py
--rw-r--r--   0        0        0      105 2024-03-17 17:38:37.508083 pypipr-1.0.93/pypipr/ibuiltins/WINDOWS.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.508083 pypipr-1.0.93/pypipr/ibuiltins/__init__.py
--rw-r--r--   0        0        0      218 2024-03-17 17:38:37.508083 pypipr-1.0.93/pypipr/ibuiltins/avg.py
--rw-r--r--   0        0        0      194 2024-03-17 17:38:37.508083 pypipr-1.0.93/pypipr/ibuiltins/basename.py
--rw-r--r--   0        0        0      385 2024-04-22 13:19:16.948654 pypipr-1.0.93/pypipr/ibuiltins/chunk_array.py
--rw-r--r--   0        0        0      500 2024-03-17 17:38:37.508083 pypipr-1.0.93/pypipr/ibuiltins/create_folder.py
--rw-r--r--   0        0        0      466 2024-03-17 17:38:37.508083 pypipr-1.0.93/pypipr/ibuiltins/datetime_from_string.py
--rw-r--r--   0        0        0      476 2024-03-17 17:38:37.508083 pypipr-1.0.93/pypipr/ibuiltins/datetime_now.py
--rw-r--r--   0        0        0      377 2024-03-17 17:38:37.508083 pypipr-1.0.93/pypipr/ibuiltins/dict_first.py
--rw-r--r--   0        0        0      229 2024-03-17 17:38:37.508083 pypipr-1.0.93/pypipr/ibuiltins/dirname.py
--rw-r--r--   0        0        0      321 2024-04-20 11:53:09.914721 pypipr-1.0.93/pypipr/ibuiltins/exit_if_empty.py
--rw-r--r--   0        0        0      543 2024-03-17 17:38:37.508083 pypipr-1.0.93/pypipr/ibuiltins/filter_empty.py
--rw-r--r--   0        0        0      335 2024-04-23 12:23:59.246031 pypipr-1.0.93/pypipr/ibuiltins/get_by_index.py
--rw-r--r--   0        0        0      639 2024-04-22 21:58:29.290425 pypipr-1.0.93/pypipr/ibuiltins/get_class_method.py
--rw-r--r--   0        0        0      227 2024-03-17 17:38:37.508083 pypipr-1.0.93/pypipr/ibuiltins/get_filemtime.py
--rw-r--r--   0        0        0      196 2024-03-17 17:38:37.508083 pypipr-1.0.93/pypipr/ibuiltins/get_filesize.py
--rw-r--r--   0        0        0      683 2024-04-20 11:02:21.923096 pypipr-1.0.93/pypipr/ibuiltins/is_empty.py
--rw-r--r--   0        0        0      922 2024-03-17 17:38:37.508083 pypipr-1.0.93/pypipr/ibuiltins/is_iterable.py
--rw-r--r--   0        0        0     1008 2024-03-17 17:38:37.508083 pypipr-1.0.93/pypipr/ibuiltins/is_valid_url.py
--rw-r--r--   0        0        0      899 2024-04-23 09:16:42.841403 pypipr-1.0.93/pypipr/ibuiltins/ivars.py
--rw-r--r--   0        0        0      496 2024-03-17 17:38:37.508083 pypipr-1.0.93/pypipr/ibuiltins/password_generator.py
--rw-r--r--   0        0        0      405 2024-03-17 17:38:37.508083 pypipr-1.0.93/pypipr/ibuiltins/random_bool.py
--rw-r--r--   0        0        0      698 2024-03-17 17:38:37.512083 pypipr-1.0.93/pypipr/ibuiltins/set_timeout.py
--rw-r--r--   0        0        0      325 2024-03-17 17:38:37.512083 pypipr-1.0.93/pypipr/ibuiltins/sets_ordered.py
--rw-r--r--   0        0        0      377 2024-03-17 17:38:37.512083 pypipr-1.0.93/pypipr/ibuiltins/str_cmp.py
--rw-r--r--   0        0        0      597 2024-03-17 17:38:37.512083 pypipr-1.0.93/pypipr/ibuiltins/to_str.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.93/pypipr/iconsole/__init__.py
--rw-r--r--   0        0        0     1686 2024-03-17 17:38:37.512083 pypipr-1.0.93/pypipr/iconsole/choices.py
--rw-r--r--   0        0        0      525 2024-03-17 17:38:37.512083 pypipr-1.0.93/pypipr/iconsole/console_run.py
--rw-r--r--   0        0        0     1030 2024-04-23 12:02:12.950032 pypipr-1.0.93/pypipr/iconsole/input_char.py
--rw-r--r--   0        0        0     1041 2024-03-17 17:38:37.512083 pypipr-1.0.93/pypipr/iconsole/log.py
--rw-r--r--   0        0        0      474 2024-03-17 17:38:37.512083 pypipr-1.0.93/pypipr/iconsole/print_colorize.py
--rw-r--r--   0        0        0      930 2024-04-22 21:43:34.984645 pypipr-1.0.93/pypipr/iconsole/print_dir.py
--rw-r--r--   0        0        0      282 2024-04-22 21:44:47.788645 pypipr-1.0.93/pypipr/iconsole/print_log.py
--rw-r--r--   0        0        0      914 2024-04-24 02:48:07.180538 pypipr-1.0.93/pypipr/iconsole/print_to_last_line.py
--rw-r--r--   0        0        0      396 2024-03-17 17:38:37.512083 pypipr-1.0.93/pypipr/iconsole/text_colorize.py
--rw-r--r--   0        0        0     1093 2024-03-17 17:38:37.512083 pypipr-1.0.93/pypipr/idjango/APIMixinView.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.93/pypipr/idjango/__init__.py
--rw-r--r--   0        0        0      222 2024-03-17 17:38:37.512083 pypipr-1.0.93/pypipr/iengineering/PintUreg.py
--rw-r--r--   0        0        0      118 2024-03-17 17:38:37.512083 pypipr-1.0.93/pypipr/iengineering/PintUregQuantity.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.93/pypipr/iengineering/__init__.py
--rw-r--r--   0        0        0      695 2024-04-22 21:59:57.598425 pypipr-1.0.93/pypipr/iengineering/batch_calculate.py
--rw-r--r--   0        0        0     1277 2024-03-17 17:38:37.512083 pypipr-1.0.93/pypipr/iengineering/batchmaker.py
--rw-r--r--   0        0        0      805 2024-03-17 17:38:37.512083 pypipr-1.0.93/pypipr/iengineering/calculate.py
--rw-r--r--   0        0        0      966 2024-04-23 11:50:40.860964 pypipr-1.0.93/pypipr/iflow/auto_reload.py
--rw-r--r--   0        0        0      243 2024-03-17 17:38:37.516083 pypipr-1.0.93/pypipr/iflow/github_pull.py
--rw-r--r--   0        0        0      951 2024-03-17 17:38:37.516083 pypipr-1.0.93/pypipr/iflow/github_push.py
--rw-r--r--   0        0        0      600 2024-03-17 17:38:37.516083 pypipr-1.0.93/pypipr/iflow/github_user.py
--rw-r--r--   0        0        0      839 2024-04-20 02:24:51.624107 pypipr-1.0.93/pypipr/iflow/pip_freeze_without_version.py
--rw-r--r--   0        0        0      409 2024-03-17 17:38:37.516083 pypipr-1.0.93/pypipr/iflow/poetry_publish.py
--rw-r--r--   0        0        0      622 2024-03-17 17:38:37.516083 pypipr-1.0.93/pypipr/iflow/poetry_update_version.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.516083 pypipr-1.0.93/pypipr/ifunctions/__init__.py
--rw-r--r--   0        0        0      552 2024-04-24 08:03:08.734958 pypipr-1.0.93/pypipr/ifunctions/iargv.py
--rw-r--r--   0        0        0      748 2024-03-17 17:38:37.516083 pypipr-1.0.93/pypipr/ifunctions/idumps.py
--rw-r--r--   0        0        0     1423 2024-03-17 17:38:37.516083 pypipr-1.0.93/pypipr/ifunctions/idumps_html.py
--rw-r--r--   0        0        0      679 2024-04-23 11:41:52.328964 pypipr-1.0.93/pypipr/ifunctions/ienv.py
--rw-r--r--   0        0        0      465 2024-03-17 17:38:37.516083 pypipr-1.0.93/pypipr/ifunctions/iexec.py
--rw-r--r--   0        0        0     2069 2024-03-17 17:38:37.516083 pypipr-1.0.93/pypipr/ifunctions/ijoin.py
--rw-r--r--   0        0        0      638 2024-04-22 21:36:07.164645 pypipr-1.0.93/pypipr/ifunctions/iloads.py
--rw-r--r--   0        0        0     4146 2024-04-22 21:40:17.264645 pypipr-1.0.93/pypipr/ifunctions/iloads_html.py
--rw-r--r--   0        0        0     2808 2024-03-17 17:38:37.516083 pypipr-1.0.93/pypipr/ifunctions/iopen.py
--rw-r--r--   0        0        0      849 2024-04-22 21:41:31.764645 pypipr-1.0.93/pypipr/ifunctions/iprint.py
--rw-r--r--   0        0        0     2407 2024-03-17 17:38:37.516083 pypipr-1.0.93/pypipr/ifunctions/irange.py
--rw-r--r--   0        0        0      722 2024-03-17 17:38:37.516083 pypipr-1.0.93/pypipr/ifunctions/ireplace.py
--rw-r--r--   0        0        0      748 2024-04-23 09:11:14.125403 pypipr-1.0.93/pypipr/ifunctions/iscandir.py
--rw-r--r--   0        0        0      383 2024-03-17 17:38:37.520083 pypipr-1.0.93/pypipr/ifunctions/isplit.py
--rw-r--r--   0        0        0     1061 2024-04-20 02:38:18.131451 pypipr-1.0.93/pypipr/pypipr.py.bak
--rw-r--r--   0        0        0     1800 2024-04-24 08:29:46.253049 pypipr-1.0.93/pypipr/terminal.py
--rw-r--r--   0        0        0      544 2024-04-24 08:30:30.473048 pypipr-1.0.93/pyproject.toml
--rw-r--r--   0        0        0    49937 2024-04-24 08:30:22.297048 pypipr-1.0.93/readme.md
--rw-r--r--   0        0        0    50623 1970-01-01 00:00:00.000000 pypipr-1.0.93/PKG-INFO
+-rw-r--r--   0        0        0     3397 2024-04-25 13:41:49.827400 pypipr-1.0.94/pypipr/__init__.py
+-rw-r--r--   0        0        0     2229 2024-03-17 17:38:37.508083 pypipr-1.0.94/pypipr/ibuiltins/ComparePerformance.py
+-rw-r--r--   0        0        0      100 2024-03-17 17:38:37.508083 pypipr-1.0.94/pypipr/ibuiltins/LINUX.py
+-rw-r--r--   0        0        0     7358 2024-04-23 10:50:10.015024 pypipr-1.0.94/pypipr/ibuiltins/RunParallel.py
+-rw-r--r--   0        0        0      105 2024-03-17 17:38:37.508083 pypipr-1.0.94/pypipr/ibuiltins/WINDOWS.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.508083 pypipr-1.0.94/pypipr/ibuiltins/__init__.py
+-rw-r--r--   0        0        0      218 2024-03-17 17:38:37.508083 pypipr-1.0.94/pypipr/ibuiltins/avg.py
+-rw-r--r--   0        0        0      194 2024-03-17 17:38:37.508083 pypipr-1.0.94/pypipr/ibuiltins/basename.py
+-rw-r--r--   0        0        0      385 2024-04-22 13:19:16.948654 pypipr-1.0.94/pypipr/ibuiltins/chunk_array.py
+-rw-r--r--   0        0        0      500 2024-03-17 17:38:37.508083 pypipr-1.0.94/pypipr/ibuiltins/create_folder.py
+-rw-r--r--   0        0        0      466 2024-03-17 17:38:37.508083 pypipr-1.0.94/pypipr/ibuiltins/datetime_from_string.py
+-rw-r--r--   0        0        0      476 2024-03-17 17:38:37.508083 pypipr-1.0.94/pypipr/ibuiltins/datetime_now.py
+-rw-r--r--   0        0        0      377 2024-03-17 17:38:37.508083 pypipr-1.0.94/pypipr/ibuiltins/dict_first.py
+-rw-r--r--   0        0        0      229 2024-03-17 17:38:37.508083 pypipr-1.0.94/pypipr/ibuiltins/dirname.py
+-rw-r--r--   0        0        0      321 2024-04-20 11:53:09.914721 pypipr-1.0.94/pypipr/ibuiltins/exit_if_empty.py
+-rw-r--r--   0        0        0      543 2024-03-17 17:38:37.508083 pypipr-1.0.94/pypipr/ibuiltins/filter_empty.py
+-rw-r--r--   0        0        0      335 2024-04-23 12:23:59.246031 pypipr-1.0.94/pypipr/ibuiltins/get_by_index.py
+-rw-r--r--   0        0        0      639 2024-04-22 21:58:29.290425 pypipr-1.0.94/pypipr/ibuiltins/get_class_method.py
+-rw-r--r--   0        0        0      227 2024-03-17 17:38:37.508083 pypipr-1.0.94/pypipr/ibuiltins/get_filemtime.py
+-rw-r--r--   0        0        0      196 2024-03-17 17:38:37.508083 pypipr-1.0.94/pypipr/ibuiltins/get_filesize.py
+-rw-r--r--   0        0        0      683 2024-04-20 11:02:21.923096 pypipr-1.0.94/pypipr/ibuiltins/is_empty.py
+-rw-r--r--   0        0        0      922 2024-03-17 17:38:37.508083 pypipr-1.0.94/pypipr/ibuiltins/is_iterable.py
+-rw-r--r--   0        0        0     1008 2024-03-17 17:38:37.508083 pypipr-1.0.94/pypipr/ibuiltins/is_valid_url.py
+-rw-r--r--   0        0        0      899 2024-04-23 09:16:42.841403 pypipr-1.0.94/pypipr/ibuiltins/ivars.py
+-rw-r--r--   0        0        0      496 2024-03-17 17:38:37.508083 pypipr-1.0.94/pypipr/ibuiltins/password_generator.py
+-rw-r--r--   0        0        0      405 2024-03-17 17:38:37.508083 pypipr-1.0.94/pypipr/ibuiltins/random_bool.py
+-rw-r--r--   0        0        0      101 2024-04-25 13:41:39.719400 pypipr-1.0.94/pypipr/ibuiltins/restart.py
+-rw-r--r--   0        0        0      698 2024-03-17 17:38:37.512083 pypipr-1.0.94/pypipr/ibuiltins/set_timeout.py
+-rw-r--r--   0        0        0      325 2024-03-17 17:38:37.512083 pypipr-1.0.94/pypipr/ibuiltins/sets_ordered.py
+-rw-r--r--   0        0        0      377 2024-03-17 17:38:37.512083 pypipr-1.0.94/pypipr/ibuiltins/str_cmp.py
+-rw-r--r--   0        0        0      597 2024-03-17 17:38:37.512083 pypipr-1.0.94/pypipr/ibuiltins/to_str.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.94/pypipr/iconsole/__init__.py
+-rw-r--r--   0        0        0     1686 2024-03-17 17:38:37.512083 pypipr-1.0.94/pypipr/iconsole/choices.py
+-rw-r--r--   0        0        0      525 2024-03-17 17:38:37.512083 pypipr-1.0.94/pypipr/iconsole/console_run.py
+-rw-r--r--   0        0        0     1030 2024-04-23 12:02:12.950032 pypipr-1.0.94/pypipr/iconsole/input_char.py
+-rw-r--r--   0        0        0     1041 2024-03-17 17:38:37.512083 pypipr-1.0.94/pypipr/iconsole/log.py
+-rw-r--r--   0        0        0      474 2024-03-17 17:38:37.512083 pypipr-1.0.94/pypipr/iconsole/print_colorize.py
+-rw-r--r--   0        0        0      930 2024-04-22 21:43:34.984645 pypipr-1.0.94/pypipr/iconsole/print_dir.py
+-rw-r--r--   0        0        0      282 2024-04-22 21:44:47.788645 pypipr-1.0.94/pypipr/iconsole/print_log.py
+-rw-r--r--   0        0        0      914 2024-04-24 02:48:07.180538 pypipr-1.0.94/pypipr/iconsole/print_to_last_line.py
+-rw-r--r--   0        0        0      396 2024-03-17 17:38:37.512083 pypipr-1.0.94/pypipr/iconsole/text_colorize.py
+-rw-r--r--   0        0        0     1093 2024-03-17 17:38:37.512083 pypipr-1.0.94/pypipr/idjango/APIMixinView.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.94/pypipr/idjango/__init__.py
+-rw-r--r--   0        0        0      222 2024-03-17 17:38:37.512083 pypipr-1.0.94/pypipr/iengineering/PintUreg.py
+-rw-r--r--   0        0        0      118 2024-03-17 17:38:37.512083 pypipr-1.0.94/pypipr/iengineering/PintUregQuantity.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.94/pypipr/iengineering/__init__.py
+-rw-r--r--   0        0        0      695 2024-04-22 21:59:57.598425 pypipr-1.0.94/pypipr/iengineering/batch_calculate.py
+-rw-r--r--   0        0        0     1277 2024-03-17 17:38:37.512083 pypipr-1.0.94/pypipr/iengineering/batchmaker.py
+-rw-r--r--   0        0        0      805 2024-03-17 17:38:37.512083 pypipr-1.0.94/pypipr/iengineering/calculate.py
+-rw-r--r--   0        0        0      966 2024-04-23 11:50:40.860964 pypipr-1.0.94/pypipr/iflow/auto_reload.py
+-rw-r--r--   0        0        0      243 2024-03-17 17:38:37.516083 pypipr-1.0.94/pypipr/iflow/github_pull.py
+-rw-r--r--   0        0        0      951 2024-03-17 17:38:37.516083 pypipr-1.0.94/pypipr/iflow/github_push.py
+-rw-r--r--   0        0        0      600 2024-03-17 17:38:37.516083 pypipr-1.0.94/pypipr/iflow/github_user.py
+-rw-r--r--   0        0        0      839 2024-04-20 02:24:51.624107 pypipr-1.0.94/pypipr/iflow/pip_freeze_without_version.py
+-rw-r--r--   0        0        0      409 2024-03-17 17:38:37.516083 pypipr-1.0.94/pypipr/iflow/poetry_publish.py
+-rw-r--r--   0        0        0      622 2024-03-17 17:38:37.516083 pypipr-1.0.94/pypipr/iflow/poetry_update_version.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.516083 pypipr-1.0.94/pypipr/ifunctions/__init__.py
+-rw-r--r--   0        0        0      552 2024-04-24 08:03:08.734958 pypipr-1.0.94/pypipr/ifunctions/iargv.py
+-rw-r--r--   0        0        0      748 2024-03-17 17:38:37.516083 pypipr-1.0.94/pypipr/ifunctions/idumps.py
+-rw-r--r--   0        0        0     1423 2024-03-17 17:38:37.516083 pypipr-1.0.94/pypipr/ifunctions/idumps_html.py
+-rw-r--r--   0        0        0      679 2024-04-23 11:41:52.328964 pypipr-1.0.94/pypipr/ifunctions/ienv.py
+-rw-r--r--   0        0        0      465 2024-03-17 17:38:37.516083 pypipr-1.0.94/pypipr/ifunctions/iexec.py
+-rw-r--r--   0        0        0     2069 2024-03-17 17:38:37.516083 pypipr-1.0.94/pypipr/ifunctions/ijoin.py
+-rw-r--r--   0        0        0      638 2024-04-22 21:36:07.164645 pypipr-1.0.94/pypipr/ifunctions/iloads.py
+-rw-r--r--   0        0        0     4146 2024-04-22 21:40:17.264645 pypipr-1.0.94/pypipr/ifunctions/iloads_html.py
+-rw-r--r--   0        0        0     2808 2024-03-17 17:38:37.516083 pypipr-1.0.94/pypipr/ifunctions/iopen.py
+-rw-r--r--   0        0        0      849 2024-04-22 21:41:31.764645 pypipr-1.0.94/pypipr/ifunctions/iprint.py
+-rw-r--r--   0        0        0     2407 2024-03-17 17:38:37.516083 pypipr-1.0.94/pypipr/ifunctions/irange.py
+-rw-r--r--   0        0        0      722 2024-03-17 17:38:37.516083 pypipr-1.0.94/pypipr/ifunctions/ireplace.py
+-rw-r--r--   0        0        0      748 2024-04-23 09:11:14.125403 pypipr-1.0.94/pypipr/ifunctions/iscandir.py
+-rw-r--r--   0        0        0      383 2024-03-17 17:38:37.520083 pypipr-1.0.94/pypipr/ifunctions/isplit.py
+-rw-r--r--   0        0        0     1061 2024-04-20 02:38:18.131451 pypipr-1.0.94/pypipr/pypipr.py.bak
+-rw-r--r--   0        0        0     1800 2024-04-24 08:29:46.253049 pypipr-1.0.94/pypipr/terminal.py
+-rw-r--r--   0        0        0      544 2024-04-25 13:42:03.655400 pypipr-1.0.94/pyproject.toml
+-rw-r--r--   0        0        0    50004 2024-04-25 13:41:56.551400 pypipr-1.0.94/readme.md
+-rw-r--r--   0        0        0    50690 1970-01-01 00:00:00.000000 pypipr-1.0.94/PKG-INFO
```

### Comparing `pypipr-1.0.93/pypipr/__init__.py` & `pypipr-1.0.94/pypipr/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from .ibuiltins.get_filesize import get_filesize
 from .ibuiltins.is_empty import is_empty
 from .ibuiltins.is_iterable import is_iterable
 from .ibuiltins.is_valid_url import is_valid_url
 from .ibuiltins.ivars import ivars
 from .ibuiltins.password_generator import password_generator
 from .ibuiltins.random_bool import random_bool
+from .ibuiltins.restart import restart
 from .ibuiltins.set_timeout import set_timeout
 from .ibuiltins.sets_ordered import sets_ordered
 from .ibuiltins.str_cmp import str_cmp
 from .ibuiltins.to_str import to_str
 from .iconsole.choices import choices
 from .iconsole.console_run import console_run
 from .iconsole.input_char import input_char
@@ -60,14 +61,15 @@
 from .ifunctions.iprint import iprint
 from .ifunctions.irange import irange
 from .ifunctions.ireplace import ireplace
 from .ifunctions.iscandir import iscandir
 from .ifunctions.isplit import isplit
 import asyncio
 import colorama
+import csv
 import datetime
 import functools
 import inspect
 import io
 import json
 import lxml
 import math
```

### Comparing `pypipr-1.0.93/pypipr/ibuiltins/ComparePerformance.py` & `pypipr-1.0.94/pypipr/ibuiltins/ComparePerformance.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/ibuiltins/RunParallel.py` & `pypipr-1.0.94/pypipr/ibuiltins/RunParallel.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/ibuiltins/filter_empty.py` & `pypipr-1.0.94/pypipr/ibuiltins/filter_empty.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/ibuiltins/get_class_method.py` & `pypipr-1.0.94/pypipr/ibuiltins/get_class_method.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/ibuiltins/is_empty.py` & `pypipr-1.0.94/pypipr/ibuiltins/is_empty.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/ibuiltins/is_iterable.py` & `pypipr-1.0.94/pypipr/ibuiltins/is_iterable.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/ibuiltins/is_valid_url.py` & `pypipr-1.0.94/pypipr/ibuiltins/is_valid_url.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/ibuiltins/ivars.py` & `pypipr-1.0.94/pypipr/ibuiltins/ivars.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/ibuiltins/set_timeout.py` & `pypipr-1.0.94/pypipr/ibuiltins/set_timeout.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/ibuiltins/to_str.py` & `pypipr-1.0.94/pypipr/ibuiltins/to_str.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/iconsole/choices.py` & `pypipr-1.0.94/pypipr/iconsole/choices.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/iconsole/console_run.py` & `pypipr-1.0.94/pypipr/iconsole/console_run.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/iconsole/input_char.py` & `pypipr-1.0.94/pypipr/iconsole/input_char.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/iconsole/log.py` & `pypipr-1.0.94/pypipr/iconsole/log.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/iconsole/print_dir.py` & `pypipr-1.0.94/pypipr/iconsole/print_dir.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/iconsole/print_to_last_line.py` & `pypipr-1.0.94/pypipr/iconsole/print_to_last_line.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/idjango/APIMixinView.py` & `pypipr-1.0.94/pypipr/idjango/APIMixinView.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/iengineering/batch_calculate.py` & `pypipr-1.0.94/pypipr/iengineering/batch_calculate.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/iengineering/batchmaker.py` & `pypipr-1.0.94/pypipr/iengineering/batchmaker.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/iengineering/calculate.py` & `pypipr-1.0.94/pypipr/iengineering/calculate.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/iflow/auto_reload.py` & `pypipr-1.0.94/pypipr/iflow/auto_reload.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/iflow/github_push.py` & `pypipr-1.0.94/pypipr/iflow/github_push.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/iflow/github_user.py` & `pypipr-1.0.94/pypipr/iflow/github_user.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/iflow/pip_freeze_without_version.py` & `pypipr-1.0.94/pypipr/iflow/pip_freeze_without_version.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/iflow/poetry_update_version.py` & `pypipr-1.0.94/pypipr/iflow/poetry_update_version.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/ifunctions/iargv.py` & `pypipr-1.0.94/pypipr/ifunctions/iargv.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/ifunctions/idumps.py` & `pypipr-1.0.94/pypipr/ifunctions/idumps.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/ifunctions/idumps_html.py` & `pypipr-1.0.94/pypipr/ifunctions/idumps_html.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/ifunctions/ienv.py` & `pypipr-1.0.94/pypipr/ifunctions/ienv.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/ifunctions/ijoin.py` & `pypipr-1.0.94/pypipr/ifunctions/ijoin.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/ifunctions/iloads.py` & `pypipr-1.0.94/pypipr/ifunctions/iloads.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/ifunctions/iloads_html.py` & `pypipr-1.0.94/pypipr/ifunctions/iloads_html.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/ifunctions/iopen.py` & `pypipr-1.0.94/pypipr/ifunctions/iopen.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/ifunctions/iprint.py` & `pypipr-1.0.94/pypipr/ifunctions/iprint.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/ifunctions/irange.py` & `pypipr-1.0.94/pypipr/ifunctions/irange.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/ifunctions/ireplace.py` & `pypipr-1.0.94/pypipr/ifunctions/ireplace.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/ifunctions/iscandir.py` & `pypipr-1.0.94/pypipr/ifunctions/iscandir.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/pypipr.py.bak` & `pypipr-1.0.94/pypipr/pypipr.py.bak`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pypipr/terminal.py` & `pypipr-1.0.94/pypipr/terminal.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.93/pyproject.toml` & `pypipr-1.0.94/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypipr"
-version = "1.0.93"
+version = "1.0.94"
 description = "The Python Package Index Project"
 authors = ["ufiapjj <ufiapjj@gmail.com>"]
 readme = "readme.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 getch = { version = "*", markers = "platform_system == 'Linux'" }
```

### Comparing `pypipr-1.0.93/readme.md` & `pypipr-1.0.94/readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 arr = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(chunk_array(arr, 5))  
 print(list(chunk_array(arr, 5)))  
 ```
 
 Output:
 ```py
-<generator object chunk_array at 0x71ec8ac240>
+<generator object chunk_array at 0x7a72a00240>
 [[2, 3, 12, 3, 3], [42, 42, 1, 43, 2], [42, 41, 4, 24, 32], [42, 3, 12, 32, 42], [42]]
 ```
 
 ## create_folder
 
 `create_folder(folder_name)`
 
@@ -125,17 +125,17 @@
 print(datetime_now("Asia/Jakarta"))  
 print(datetime_now("GMT"))  
 print(datetime_now("Etc/GMT+7"))  
 ```
 
 Output:
 ```py
-2024-04-24 15:30:21.125582+07:00
-2024-04-24 08:30:21.126382+00:00
-2024-04-24 01:30:21.127761-07:00
+2024-04-25 20:41:51.650942+07:00
+2024-04-25 13:41:51.652297+00:00
+2024-04-25 06:41:51.655828-07:00
 ```
 
 ## dict_first
 
 `dict_first(d: dict, remove=False)`
 
 Mengambil nilai (key, value) pertama dari dictionary dalam bentuk tuple.  
@@ -194,15 +194,15 @@
 ```python  
 var = [1, None, False, 0, "0", True, {}, ['eee']]  
 print(filter_empty(var))  
 ```
 
 Output:
 ```py
-<generator object filter_empty at 0x71ec842d40>
+<generator object filter_empty at 0x7a72992d40>
 ```
 
 ## get_by_index
 
 `get_by_index(obj, index, on_error=None)`
 
 Mendapatkan value dari object berdasarkan indexnya.  
@@ -240,16 +240,16 @@
   
 print(get_class_method(ExampleGetClassMethod))  
 print(list(get_class_method(ExampleGetClassMethod)))  
 ```
 
 Output:
 ```py
-<generator object get_class_method at 0x71ec843010>
-[<function ExampleGetClassMethod.a at 0x720457e7a0>, <function ExampleGetClassMethod.b at 0x71ec8b5580>, <function ExampleGetClassMethod.c at 0x71ec8b5620>, <function ExampleGetClassMethod.d at 0x71ec8b56c0>]
+<generator object get_class_method at 0x7a72993010>
+[<function ExampleGetClassMethod.a at 0x7a869867a0>, <function ExampleGetClassMethod.b at 0x7a72a096c0>, <function ExampleGetClassMethod.c at 0x7a72a09620>, <function ExampleGetClassMethod.d at 0x7a72a09760>]
 ```
 
 ## get_filemtime
 
 `get_filemtime(filename)`
 
 Mengambil informasi last modification time file dalam nano seconds  
@@ -366,17 +366,18 @@
 Output:
 ```py
 {'module': {'ibuiltins': <module 'pypipr.ibuiltins' from '/data/data/com.termux/files/home/pypipr/pypipr/ibuiltins/__init__.py'>,
             'iconsole': <module 'pypipr.iconsole' from '/data/data/com.termux/files/home/pypipr/pypipr/iconsole/__init__.py'>,
             'idjango': <module 'pypipr.idjango' from '/data/data/com.termux/files/home/pypipr/pypipr/idjango/__init__.py'>,
             'iengineering': <module 'pypipr.iengineering' from '/data/data/com.termux/files/home/pypipr/pypipr/iengineering/__init__.py'>,
             'ifunctions': <module 'pypipr.ifunctions' from '/data/data/com.termux/files/home/pypipr/pypipr/ifunctions/__init__.py'>,
-            'iflow': <module 'pypipr.iflow' (<_frozen_importlib_external.NamespaceLoader object at 0x71f481bed0>)>,
+            'iflow': <module 'pypipr.iflow' (<_frozen_importlib_external.NamespaceLoader object at 0x7a7f2cf610>)>,
             'asyncio': <module 'asyncio' from '/data/data/com.termux/files/usr/lib/python3.11/asyncio/__init__.py'>,
             'colorama': <module 'colorama' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/colorama/__init__.py'>,
+            'csv': <module 'csv' from '/data/data/com.termux/files/usr/lib/python3.11/csv.py'>,
             'datetime': <module 'datetime' from '/data/data/com.termux/files/usr/lib/python3.11/datetime.py'>,
             'functools': <module 'functools' from '/data/data/com.termux/files/usr/lib/python3.11/functools.py'>,
             'inspect': <module 'inspect' from '/data/data/com.termux/files/usr/lib/python3.11/inspect.py'>,
             'io': <module 'io' (frozen)>,
             'json': <module 'json' from '/data/data/com.termux/files/usr/lib/python3.11/json/__init__.py'>,
             'lxml': <module 'lxml' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/lxml/__init__.py'>,
             'math': <module 'math' from '/data/data/com.termux/files/usr/lib/python3.11/lib-dynload/math.cpython-311.so'>,
@@ -403,87 +404,88 @@
             'zoneinfo': <module 'zoneinfo' from '/data/data/com.termux/files/usr/lib/python3.11/zoneinfo/__init__.py'>},
  'class': {'ComparePerformance': <class 'pypipr.ibuiltins.ComparePerformance.ComparePerformance'>,
            'RunParallel': <class 'pypipr.ibuiltins.RunParallel.RunParallel'>,
            'APIMixinView': <class 'pypipr.idjango.APIMixinView.APIMixinView'>,
            'PintUregQuantity': <class 'pint.Quantity'>},
  'variable': {'LINUX': True,
               'WINDOWS': False,
-              'PintUreg': <pint.registry.UnitRegistry object at 0x71fe1eb710>},
- 'function': {'avg': <function avg at 0x72045b6d40>,
-              'basename': <function basename at 0x720457e8e0>,
-              'chunk_array': <function chunk_array at 0x71fe125120>,
-              'create_folder': <function create_folder at 0x71fe125300>,
-              'datetime_from_string': <function datetime_from_string at 0x71fe1254e0>,
-              'datetime_now': <function datetime_now at 0x71fe1cd620>,
-              'dict_first': <function dict_first at 0x71fe1cd580>,
-              'dirname': <function dirname at 0x71fe1cd4e0>,
-              'exit_if_empty': <function exit_if_empty at 0x71fe1a74c0>,
-              'filter_empty': <function filter_empty at 0x71fe1cd1c0>,
-              'get_by_index': <function get_by_index at 0x71fe1ccea0>,
-              'get_class_method': <function get_class_method at 0x71fe1cccc0>,
-              'get_filemtime': <function get_filemtime at 0x71fe1ccb80>,
-              'get_filesize': <function get_filesize at 0x71fe1cc9a0>,
-              'is_empty': <function is_empty at 0x71fe1cd260>,
-              'is_iterable': <function is_iterable at 0x71fe1ccfe0>,
-              'is_valid_url': <function is_valid_url at 0x71fe1cc860>,
-              'ivars': <function ivars at 0x71fe1cc7c0>,
-              'password_generator': <function password_generator at 0x71fe1cc680>,
-              'random_bool': <function random_bool at 0x71fe1cc400>,
-              'set_timeout': <function set_timeout at 0x71fe1cf7e0>,
-              'sets_ordered': <function sets_ordered at 0x71fe1cf920>,
-              'str_cmp': <function str_cmp at 0x71fe1cf9c0>,
-              'to_str': <function to_str at 0x71fe1ccf40>,
-              'choices': <function choices at 0x71fe1cfa60>,
-              'console_run': <function console_run at 0x71fe1cfce0>,
-              'input_char': <function input_char at 0x71fe1cfe20>,
-              'log': <function log at 0x71fe1f0040>,
-              'print_colorize': <function print_colorize at 0x71fe1f00e0>,
-              'print_dir': <function print_dir at 0x71fe1f0220>,
-              'print_log': <function print_log at 0x71fe1cfec0>,
-              'print_to_last_line': <function print_to_last_line at 0x71fe1cfc40>,
-              'text_colorize': <function text_colorize at 0x71fe1cfd80>,
-              'batch_calculate': <function batch_calculate at 0x71f4995580>,
-              'batchmaker': <function batchmaker at 0x71f496e980>,
-              'calculate': <function calculate at 0x71f49962a0>,
-              'auto_reload': <function auto_reload at 0x71f4996480>,
-              'github_pull': <function github_pull at 0x71f4996020>,
-              'github_push': <function github_push at 0x71f4996700>,
-              'github_user': <function github_user at 0x71f4996a20>,
-              'pip_freeze_without_version': <function pip_freeze_without_version at 0x71f46b9f80>,
-              'poetry_publish': <function poetry_publish at 0x71f46ba160>,
-              'poetry_update_version': <function poetry_update_version at 0x71f46da980>,
-              'iargv': <function iargv at 0x71eca7c0e0>,
-              'idumps': <function idumps at 0x71eca7c220>,
-              'idumps_html': <function idumps_html at 0x71ecae0c20>,
-              'ienv': <function ienv at 0x71eca7c360>,
-              'iexec': <function iexec at 0x71ecae0ea0>,
-              'ijoin': <function ijoin at 0x71f46b9ee0>,
-              'iloads': <function iloads at 0x71ecae0f40>,
-              'iloads_html': <function iloads_html at 0x71ecae11c0>,
-              'iopen': <function iopen at 0x71f46ba200>,
-              'iprint': <function iprint at 0x71eca7c180>,
-              'irange': <function irange at 0x71f49963e0>,
-              'ireplace': <function ireplace at 0x71ecae1080>,
-              'iscandir': <function iscandir at 0x71ecae2e80>,
-              'isplit': <function isplit at 0x71ecae2f20>}}
+              'PintUreg': <pint.registry.UnitRegistry object at 0x7a78af4750>},
+ 'function': {'avg': <function avg at 0x7a869bed40>,
+              'basename': <function basename at 0x7a869868e0>,
+              'chunk_array': <function chunk_array at 0x7a83471120>,
+              'create_folder': <function create_folder at 0x7a83471300>,
+              'datetime_from_string': <function datetime_from_string at 0x7a834714e0>,
+              'datetime_now': <function datetime_now at 0x7a83519620>,
+              'dict_first': <function dict_first at 0x7a83519580>,
+              'dirname': <function dirname at 0x7a835194e0>,
+              'exit_if_empty': <function exit_if_empty at 0x7a834f34c0>,
+              'filter_empty': <function filter_empty at 0x7a835191c0>,
+              'get_by_index': <function get_by_index at 0x7a83518ea0>,
+              'get_class_method': <function get_class_method at 0x7a83518cc0>,
+              'get_filemtime': <function get_filemtime at 0x7a83518b80>,
+              'get_filesize': <function get_filesize at 0x7a835189a0>,
+              'is_empty': <function is_empty at 0x7a83519260>,
+              'is_iterable': <function is_iterable at 0x7a83518fe0>,
+              'is_valid_url': <function is_valid_url at 0x7a83518860>,
+              'ivars': <function ivars at 0x7a835187c0>,
+              'password_generator': <function password_generator at 0x7a83518680>,
+              'random_bool': <function random_bool at 0x7a83518400>,
+              'restart': <function restart at 0x7a8351b740>,
+              'set_timeout': <function set_timeout at 0x7a8351b880>,
+              'sets_ordered': <function sets_ordered at 0x7a8351b9c0>,
+              'str_cmp': <function str_cmp at 0x7a8351ba60>,
+              'to_str': <function to_str at 0x7a83518f40>,
+              'choices': <function choices at 0x7a8351bb00>,
+              'console_run': <function console_run at 0x7a8351bd80>,
+              'input_char': <function input_char at 0x7a8351bec0>,
+              'log': <function log at 0x7a8351bc40>,
+              'print_colorize': <function print_colorize at 0x7a83540180>,
+              'print_dir': <function print_dir at 0x7a835402c0>,
+              'print_log': <function print_log at 0x7a8351bf60>,
+              'print_to_last_line': <function print_to_last_line at 0x7a8351bce0>,
+              'text_colorize': <function text_colorize at 0x7a8351be20>,
+              'batch_calculate': <function batch_calculate at 0x7a780d9620>,
+              'batchmaker': <function batchmaker at 0x7a780da0c0>,
+              'calculate': <function calculate at 0x7a780da340>,
+              'auto_reload': <function auto_reload at 0x7a780da5c0>,
+              'github_pull': <function github_pull at 0x7a780da520>,
+              'github_push': <function github_push at 0x7a780da7a0>,
+              'github_user': <function github_user at 0x7a780daac0>,
+              'pip_freeze_without_version': <function pip_freeze_without_version at 0x7a77e1a0c0>,
+              'poetry_publish': <function poetry_publish at 0x7a77e1a200>,
+              'poetry_update_version': <function poetry_update_version at 0x7a77e3aa20>,
+              'iargv': <function iargv at 0x7a72bd0180>,
+              'idumps': <function idumps at 0x7a72bd02c0>,
+              'idumps_html': <function idumps_html at 0x7a72c38cc0>,
+              'ienv': <function ienv at 0x7a72bd0400>,
+              'iexec': <function iexec at 0x7a72c38f40>,
+              'ijoin': <function ijoin at 0x7a77e19f80>,
+              'iloads': <function iloads at 0x7a72c38fe0>,
+              'iloads_html': <function iloads_html at 0x7a72c39260>,
+              'iopen': <function iopen at 0x7a77e1a2a0>,
+              'iprint': <function iprint at 0x7a72c39120>,
+              'irange': <function irange at 0x7a780da480>,
+              'ireplace': <function ireplace at 0x7a72c39300>,
+              'iscandir': <function iscandir at 0x7a72c3af20>,
+              'isplit': <function isplit at 0x7a72c3afc0>}}
 ```
 
 ## password_generator
 
 `password_generator(length=8, characters='abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~')`
 
 Membuat pssword secara acak  
   
 ```python  
 print(password_generator())  
 ```
 
 Output:
 ```py
-;U&Ljx6Z
+n.,UG}_N
 ```
 
 ## random_bool
 
 `random_bool()`
 
 Menghasilkan nilai random True atau False.  
@@ -493,17 +495,21 @@
   
 ```python  
 print(random_bool())  
 ```
 
 Output:
 ```py
-True
+False
 ```
 
+## restart
+
+`restart()`
+
 ## set_timeout
 
 `set_timeout(interval, func, args=None, kwargs=None)`
 
 Menjalankan fungsi ketika sudah sekian detik.  
 Apabila timeout masih berjalan tapi kode sudah selesai dieksekusi semua, maka  
 program tidak akan berhenti sampai timeout selesai, kemudian fungsi dijalankan,  
@@ -515,15 +521,15 @@
 print(x)  
 print("menghentikan timeout 7")  
 x.cancel()  
 ```
 
 Output:
 ```py
-<Timer(Thread-2, started 489281289456)>
+<Timer(Thread-2, started 525885381872)>
 menghentikan timeout 7
 ```
 
 ## sets_ordered
 
 `sets_ordered(iterator)`
 
@@ -533,15 +539,15 @@
 array = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(sets_ordered(array))  
 print(list(sets_ordered(array)))  
 ```
 
 Output:
 ```py
-<generator object sets_ordered at 0x71ec8c01e0>
+<generator object sets_ordered at 0x7a72a141e0>
 [2, 3, 12, 42, 1, 43, 41, 4, 24, 32]
 ```
 
 ## str_cmp
 
 `str_cmp(t1, t2)`
 
@@ -687,29 +693,29 @@
              __doc__ : Path subclass for non-Windows systems.
 
     On a POSIX system, instantiating a Path should return this object.
     
            __enter__ : https:/www.google.com
           __fspath__ : https:/www.google.com
         __getstate__ : (None, {'_drv': '', '_root': '', '_parts': ['https:', 'www.google.com'], '_str': 'https:/www.google.com'})
-            __hash__ : -6619349520802782460
+            __hash__ : 355454826737572805
             __init__ : None
    __init_subclass__ : None
           __module__ : pathlib
           __reduce__ : (<class 'pathlib.PosixPath'>, ('https:', 'www.google.com'))
             __repr__ : PosixPath('https:/www.google.com')
           __sizeof__ : 72
            __slots__ : ()
              __str__ : https:/www.google.com
     __subclasshook__ : NotImplemented
       _cached_cparts : ['https:', 'www.google.com']
              _cparts : ['https:', 'www.google.com']
                 _drv : 
-            _flavour : <pathlib._PosixFlavour object at 0x71fe1a0790>
-               _hash : -6619349520802782460
+            _flavour : <pathlib._PosixFlavour object at 0x7a834ec650>
+               _hash : 355454826737572805
               _parts : ['https:', 'www.google.com']
                _root : 
                 _str : https:/www.google.com
             absolute : /data/data/com.termux/files/home/pypipr/https:/www.google.com
               anchor : 
             as_posix : https:/www.google.com
                  cwd : /data/data/com.termux/files/home/pypipr
@@ -723,15 +729,15 @@
               is_dir : False
              is_fifo : False
              is_file : False
             is_mount : False
          is_reserved : False
            is_socket : False
           is_symlink : False
-             iterdir : <generator object Path.iterdir at 0x71ec898c80>
+             iterdir : <generator object Path.iterdir at 0x7a729f0900>
             joinpath : https:/www.google.com
                 name : www.google.com
               parent : https:
              parents : <PosixPath.parents>
                parts : ('https:', 'www.google.com')
              resolve : /data/data/com.termux/files/home/pypipr/https:/www.google.com
                 root : 
@@ -790,15 +796,15 @@
 ```python  
 print(batch_calculate("{1 10} m ** {1 3}"))  
 print(list(batch_calculate("{1 10} m ** {1 3}")))  
 ```
 
 Output:
 ```py
-<generator object batch_calculate at 0x71ec843b50>
+<generator object batch_calculate at 0x7a72993970>
 [('1 m ** 1', <Quantity(1, 'meter')>), ('1 m ** 2', <Quantity(1, 'meter ** 2')>), ('1 m ** 3', <Quantity(1, 'meter ** 3')>), ('2 m ** 1', <Quantity(2, 'meter')>), ('2 m ** 2', <Quantity(2, 'meter ** 2')>), ('2 m ** 3', <Quantity(2, 'meter ** 3')>), ('3 m ** 1', <Quantity(3, 'meter')>), ('3 m ** 2', <Quantity(3, 'meter ** 2')>), ('3 m ** 3', <Quantity(3, 'meter ** 3')>), ('4 m ** 1', <Quantity(4, 'meter')>), ('4 m ** 2', <Quantity(4, 'meter ** 2')>), ('4 m ** 3', <Quantity(4, 'meter ** 3')>), ('5 m ** 1', <Quantity(5, 'meter')>), ('5 m ** 2', <Quantity(5, 'meter ** 2')>), ('5 m ** 3', <Quantity(5, 'meter ** 3')>), ('6 m ** 1', <Quantity(6, 'meter')>), ('6 m ** 2', <Quantity(6, 'meter ** 2')>), ('6 m ** 3', <Quantity(6, 'meter ** 3')>), ('7 m ** 1', <Quantity(7, 'meter')>), ('7 m ** 2', <Quantity(7, 'meter ** 2')>), ('7 m ** 3', <Quantity(7, 'meter ** 3')>), ('8 m ** 1', <Quantity(8, 'meter')>), ('8 m ** 2', <Quantity(8, 'meter ** 2')>), ('8 m ** 3', <Quantity(8, 'meter ** 3')>), ('9 m ** 1', <Quantity(9, 'meter')>), ('9 m ** 2', <Quantity(9, 'meter ** 2')>), ('9 m ** 3', <Quantity(9, 'meter ** 3')>), ('10 m ** 1', <Quantity(10, 'meter')>), ('10 m ** 2', <Quantity(10, 'meter ** 2')>), ('10 m ** 3', <Quantity(10, 'meter ** 3')>)]
 ```
 
 ## batchmaker
 
 `batchmaker(pattern: str)`
 
@@ -815,15 +821,15 @@
 s = "Urutan {1/6/3} dan {10:9} dan {j k} dan {Z - A - 15} saja."  
 print(batchmaker(s))  
 print(list(batchmaker(s)))  
 ```
 
 Output:
 ```py
-<generator object batchmaker at 0x71ec8b0040>
+<generator object batchmaker at 0x7a72a04160>
 ['Urutan 1 dan 10 dan j dan Z saja.', 'Urutan 1 dan 10 dan j dan K saja.', 'Urutan 1 dan 10 dan k dan Z saja.', 'Urutan 1 dan 10 dan k dan K saja.', 'Urutan 1 dan 9 dan j dan Z saja.', 'Urutan 1 dan 9 dan j dan K saja.', 'Urutan 1 dan 9 dan k dan Z saja.', 'Urutan 1 dan 9 dan k dan K saja.', 'Urutan 4 dan 10 dan j dan Z saja.', 'Urutan 4 dan 10 dan j dan K saja.', 'Urutan 4 dan 10 dan k dan Z saja.', 'Urutan 4 dan 10 dan k dan K saja.', 'Urutan 4 dan 9 dan j dan Z saja.', 'Urutan 4 dan 9 dan j dan K saja.', 'Urutan 4 dan 9 dan k dan Z saja.', 'Urutan 4 dan 9 dan k dan K saja.']
 ```
 
 ## calculate
 
 `calculate(teks)`
 
@@ -1179,15 +1185,15 @@
     recursive_flat=True))  
 print(ijoin(arr, separator='</div>\n<div>', start='<div>', end='</div>'))  
 print(ijoin(10, ' '))  
 ```
 
 Output:
 ```py
-dfs, qweqw, asd, weq
+weq, asd, dfs, qweqw
 ,ini,path,seperti,url,
 ini,path,seperti,url
 <li>satu</li>
 <li>12</li>
 <li>34</li>
 <li>56</li>
 <li>tiga</li>
@@ -1244,190 +1250,187 @@
 pprint.pprint(iloads_html(iopen("https://harga-emas.org/")), depth=10)  
 pprint.pprint(iloads_html(iopen("https://harga-emas.org/1-gram/")), depth=10)  
 ```
 
 Output:
 ```py
 (['Home', 'Emas 1 Gram', 'History', 'Trend', 'Perak 1 Gram', 'Pluang'],
- [['Harga Emas Hari Ini - Rabu, 24 April 2024'],
-  ['Spot Emas USD↓2.318,00 (-11,91) / oz',
-   'Kurs IDR↑16.244,00 (+20,00) / USD',
-   'Emas IDR↓1.210.591 (-4.722) / gr'],
-  ['LM Antam (Jual)↓1.320.000 (-5.000) / gr',
-   'LM Antam (Beli)↓1.218.000 (-5.000) / gr']],
+ [['Harga Emas Hari Ini - Kamis, 25 April 2024'],
+  ['Spot Emas USD↓2.316,87 (-8,41) / oz',
+   'Kurs IDR↓16.161,00 (-83,00) / USD',
+   'Emas IDR↓1.203.818 (-10.575) / gr'],
+  ['LM Antam (Jual)↓1.319.000 (-1.000) / gr',
+   'LM Antam (Beli)↓1.217.000 (-1.000) / gr']],
  [['Harga Emas Hari Ini'],
   ['Gram', 'Gedung Antam Jakarta', 'Pegadaian'],
   ['per Gram (Rp)', 'per Batangan (Rp)', 'per Gram (Rp)', 'per Batangan (Rp)'],
   ['1000',
-   '1.261 (-5)',
-   '1.260.600 (-5.000)',
+   '1.260 (-1)',
+   '1.259.600 (-1.000)',
    '1.043.040 (+8.200)',
    '1.043.040.000 (+8.200.000)'],
   ['500',
-   '2.521 (-10)',
-   '1.260.640 (-5.000)',
+   '2.519 (-2)',
+   '1.259.640 (-1.000)',
    '1.043.082 (+8.200)',
    '521.541.000 (+4.100.000)'],
   ['250',
-   '5.044 (-20)',
-   '1.261.060 (-5.000)',
+   '5.040 (-4)',
+   '1.260.060 (-1.000)',
    '1.043.512 (+8.200)',
    '260.878.000 (+2.050.000)'],
   ['100',
-   '12.621 (-50)',
-   '1.262.120 (-5.000)',
+   '12.611 (-10)',
+   '1.261.120 (-1.000)',
    '1.044.600 (+8.200)',
    '104.460.000 (+820.000)'],
   ['50',
-   '25.258 (-100)',
-   '1.262.900 (-5.000)',
+   '25.238 (-20)',
+   '1.261.900 (-1.000)',
    '1.045.400 (+8.200)',
    '52.270.000 (+410.000)'],
   ['25',
-   '50.579 (-200)',
-   '1.264.480 (-5.000)',
+   '50.539 (-40)',
+   '1.263.480 (-1.000)',
    '1.047.040 (+8.200)',
    '26.176.000 (+205.000)'],
   ['10',
-   '126.950 (-500)',
-   '1.269.500 (-5.000)',
+   '126.850 (-100)',
+   '1.268.500 (-1.000)',
    '1.052.200 (+8.200)',
    '10.522.000 (+82.000)'],
   ['5',
-   '255.000 (-1.000)',
-   '1.275.000 (-5.000)',
+   '254.800 (-200)',
+   '1.274.000 (-1.000)',
    '1.057.800 (+8.200)',
    '5.289.000 (+41.000)'],
   ['3',
-   '427.222 (-1.667)',
-   '1.281.667 (-5.000)',
+   '426.889 (-333)',
+   '1.280.667 (-1.000)',
    '1.064.667 (+8.000)',
    '3.194.000 (+24.000)'],
   ['2',
-   '645.000 (-2.500)',
-   '1.290.000 (-5.000)',
+   '644.500 (-500)',
+   '1.289.000 (-1.000)',
    '1.073.500 (+8.500)',
    '2.147.000 (+17.000)'],
   ['1',
-   '1.320.000 (-5.000)',
-   '1.320.000 (-5.000)',
+   '1.319.000 (-1.000)',
+   '1.319.000 (-1.000)',
    '1.104.000 (+8.000)',
    '1.104.000 (+8.000)'],
   ['0.5',
-   '2.840.000 (-10.000)',
-   '1.420.000 (-5.000)',
+   '2.838.000 (-2.000)',
+   '1.419.000 (-1.000)',
    '1.208.000 (+8.000)',
    '604.000 (+4.000)'],
-  ['Update harga LM Antam :24 April 2024, pukul 08:12Harga pembelian kembali '
-   ':Rp. 1.218.000/gram (-5.000)',
+  ['Update harga LM Antam :25 April 2024, pukul 08:05Harga pembelian kembali '
+   ':Rp. 1.217.000/gram (-1.000)',
    'Update harga LM Pegadaian :31 Agustus 2023']],
  [['Spot Harga Emas Hari Ini (Market Open)'],
   ['Satuan', 'USD', 'Kurs\xa0Dollar', 'IDR'],
-  ['Ounce\xa0(oz)', '2.318,00 (-11,91)', '16.244,00 (+20,00)', '37.653.592'],
-  ['Gram\xa0(gr)', '74,53', '16.244,00', '1.210.591 (-4.722)'],
-  ['Kilogram\xa0(kg)', '74.525,43', '16.244,00', '1.210.591.095'],
-  ['Update harga emas :24 April 2024, pukul 15:30Update kurs :24 April 2024, '
+  ['Ounce\xa0(oz)', '2.316,87 (-8,41)', '16.161,00 (-83,00)', '37.442.936'],
+  ['Gram\xa0(gr)', '74,49', '16.161,00', '1.203.818 (-10.575)'],
+  ['Kilogram\xa0(kg)', '74.489,10', '16.161,00', '1.203.818.350'],
+  ['Update harga emas :25 April 2024, pukul 20:41Update kurs :25 April 2024, '
    'pukul 13:10']],
  [['Gram', 'UBS Gold 99.99%'],
   ['Jual', 'Beli'],
   ['/ Batang', '/ Gram', '/ Batang', '/ Gram'],
   ['100',
-   '126.000.000 (-712.000)',
-   '1.260.000 (-7.120)',
-   '123.985.000 (+250.000)',
-   '1.239.850 (+2.500)'],
+   '126.000.000',
+   '1.260.000',
+   '124.385.000 (+400.000)',
+   '1.243.850 (+4.000)'],
   ['50',
-   '63.100.000 (-295.000)',
-   '1.262.000 (-5.900)',
-   '62.045.000 (+125.000)',
-   '1.240.900 (+2.500)'],
+   '63.100.000',
+   '1.262.000',
+   '62.245.000 (+200.000)',
+   '1.244.900 (+4.000)'],
   ['25',
-   '31.600.000 (-137.000)',
-   '1.264.000 (-5.480)',
-   '31.125.000 (+62.500)',
-   '1.245.000 (+2.500)'],
+   '31.600.000',
+   '1.264.000',
+   '31.225.000 (+100.000)',
+   '1.249.000 (+4.000)'],
   ['10',
-   '12.680.000 (-65.000)',
-   '1.268.000 (-6.500)',
-   '12.500.000 (+25.000)',
-   '1.250.000 (+2.500)'],
-  ['5',
-   '6.365.000 (-35.000)',
-   '1.273.000 (-7.000)',
-   '6.302.000 (+12.500)',
-   '1.260.400 (+2.500)'],
+   '12.680.000',
+   '1.268.000',
+   '12.540.000 (+40.000)',
+   '1.254.000 (+4.000)'],
+  ['5', '6.365.000', '1.273.000', '6.322.000 (+20.000)', '1.264.400 (+4.000)'],
   ['1',
-   '1.320.000 (-5.000)',
-   '1.320.000 (-5.000)',
-   '1.293.000 (+2.500)',
-   '1.293.000 (+2.500)'],
-  ['', 'Update :24 April 2024, pukul 13:02']],
+   '1.315.000 (-5.000)',
+   '1.315.000 (-5.000)',
+   '1.297.000 (+4.000)',
+   '1.297.000 (+4.000)'],
+  ['', 'Update :25 April 2024, pukul 14:44']],
  [['Konversi Satuan'],
   ['Satuan', 'Ounce (oz)', 'Gram (gr)', 'Kilogram (kg)'],
   ['Ounce\xa0(oz)', '1', '31,1034767696', '0,0311034768'],
   ['Gram\xa0(gr)', '0,0321507466', '1', '0.001'],
   ['Kilogram\xa0(kg)', '32,1507466000', '1.000', '1']],
  [['Pergerakan Harga Emas Dunia'],
   ['Waktu', 'Emas'],
   ['Unit', 'USD', 'IDR'],
   ['Angka', '+/-', 'Angka', '+/-'],
-  ['Hari Ini', 'Kurs', '', '', '16.224', '+20+0,12%'],
-  ['oz', '2.329,91', '-11,91-0,51%', '37.800.460', '-146.868-0,39%'],
-  ['gr', '74,91', '-0,38-0,51%', '1.215.313', '-4.722-0,39%'],
-  ['30 Hari', 'Kurs', '', '', '15.773', '+471+2,99%'],
-  ['oz', '2.175,55', '+142,45+6,55%', '34.314.950', '+3.338.642+9,73%'],
-  ['gr', '69,95', '+4,58+6,55%', '1.103.251', '+107.340+9,73%'],
-  ['2 Bulan', 'Kurs', '', '', '15.630', '+614+3,93%'],
-  ['oz', '2.035,57', '+282,43+13,87%', '31.815.959', '+5.837.633+18,35%'],
-  ['gr', '65,45', '+9,08+13,87', '1.022.907', '+187.684+18,35%'],
-  ['6 Bulan', 'Kurs', '', '', '15.933', '+311+1,95%'],
-  ['oz', '1.983,13', '+334,87+16,89%', '31.597.210', '+6.056.382+19,17%'],
-  ['gr', '63,76', '+10,77+16,89%', '1.015.874', '+194.717+19,17%'],
-  ['1 Tahun', 'Kurs', '', '', '15.731', '+513+3,26%'],
-  ['oz', '1.823,86', '+494,14+27,09%', '28.691.142', '+8.962.450+31,24%'],
-  ['gr', '58,64', '+15,89+27,09%', '922.442', '+288.149+31,24%'],
-  ['2 Tahun', 'Kurs', '', '', '14.361', '+1.883+13,11%'],
-  ['oz', '1.896,13', '+421,87+22,25%', '27.230.342', '+10.423.250+38,28%'],
-  ['gr', '60,96', '+13,56+22,25%', '875.476', '+335.115+38,28%'],
-  ['3 Tahun', 'Kurs', '', '', '14.530', '+1.714+11,80%'],
-  ['oz', '1.777,11', '+540,89+30,44%', '25.821.408', '+11.832.184+45,82%'],
-  ['gr', '57,14', '+17,39+30,44%', '830.178', '+380.414+45,82%'],
-  ['5 Tahun', 'Kurs', '', '', '14.188', '+2.056+14,49%'],
-  ['oz', '1.288,10', '+1.029,90+79,95%', '18.275.563', '+19.378.029+106,03%'],
-  ['gr', '41,41', '+33,11+79,95%', '587.573', '+623.018+106,03%']])
+  ['Hari Ini', 'Kurs', '', '', '16.244', '-83-0,51%'],
+  ['oz', '2.325,28', '-8,41-0,36%', '37.771.848', '-328.912-0,87%'],
+  ['gr', '74,76', '-0,27-0,36%', '1.214.393', '-10.575-0,87%'],
+  ['30 Hari', 'Kurs', '', '', '15.795', '+366+2,32%'],
+  ['oz', '2.177,78', '+139,09+6,39%', '34.398.035', '+3.044.901+8,85%'],
+  ['gr', '70,02', '+4,47+6,39%', '1.105.923', '+97.896+8,85%'],
+  ['2 Bulan', 'Kurs', '', '', '15.630', '+531+3,40%'],
+  ['oz', '2.035,57', '+281,30+13,82%', '31.815.959', '+5.626.977+17,69%'],
+  ['gr', '65,45', '+9,04+13,82', '1.022.907', '+180.912+17,69%'],
+  ['6 Bulan', 'Kurs', '', '', '15.933', '+228+1,43%'],
+  ['oz', '2.006,33', '+310,54+15,48%', '31.966.856', '+5.476.080+17,13%'],
+  ['gr', '64,51', '+9,98+15,48%', '1.027.758', '+176.060+17,13%'],
+  ['1 Tahun', 'Kurs', '', '', '15.731', '+430+2,73%'],
+  ['oz', '1.823,86', '+493,01+27,03%', '28.691.142', '+8.751.794+30,50%'],
+  ['gr', '58,64', '+15,85+27,03%', '922.442', '+281.377+30,50%'],
+  ['2 Tahun', 'Kurs', '', '', '14.452', '+1.709+11,83%'],
+  ['oz', '1.901,97', '+414,90+21,81%', '27.487.270', '+9.955.666+36,22%'],
+  ['gr', '61,15', '+13,34+21,81%', '883.736', '+320.082+36,22%'],
+  ['3 Tahun', 'Kurs', '', '', '14.548', '+1.613+11,09%'],
+  ['oz', '1.779,86', '+537,01+30,17%', '25.893.403', '+11.549.533+44,60%'],
+  ['gr', '57,22', '+17,27+30,17%', '832.492', '+371.326+44,60%'],
+  ['5 Tahun', 'Kurs', '', '', '14.188', '+1.973+13,91%'],
+  ['oz', '1.286,10', '+1.030,77+80,15%', '18.247.187', '+19.195.749+105,20%'],
+  ['gr', '41,35', '+33,14+80,15%', '586.661', '+617.158+105,20%']])
+Timeout 3
 (['Home', 'Emas 1 Gram', 'History', 'Trend', 'Perak 1 Gram', 'Pluang'],
  [[''],
   ['Emas 24 KaratHarga Emas 1 Gram', ''],
-  ['USD', '74,53↓', '-0,38-0,51%'],
-  ['KURS', '16.169,15↑', '+22,25+0,14%'],
-  ['IDR', '1.205.012,87↓', '-4.524,70-0,37%'],
-  ['Rabu, 24 April 2024 15:30']],
+  ['USD', '74,49↓', '-0,27-0,36%'],
+  ['KURS', '16.227,80↓', '-4,55-0,03%'],
+  ['IDR', '1.208.794,22↓', '-4.727,96-0,39%'],
+  ['Kamis, 25 April 2024 20:41']],
  [[''],
   ['Emas 1 Gram (IDR)Emas 1 Gram (USD)Kurs USD-IDR',
    'Hari Ini',
    '1 Bulan',
    '1 Tahun',
    '5 Tahun',
    'Max',
    '']],
  [['Pergerakkan Harga Emas 1 Gram'],
   ['', 'Penutupan Kemarin', 'Pergerakkan Hari Ini', 'Rata-rata'],
-  ['USD', '74,91', '74,53 - 74,91', '74,72'],
-  ['KURS', '16.146,90', '16.146,90 - 16.169,15', '16.158,03'],
-  ['IDR', '1.209.537,57', '1.205.012,87 - 1.209.537,57', '1.207.275,22'],
+  ['USD', '74,76', '74,49 - 74,76', '74,63'],
+  ['KURS', '16.232,35', '16.227,80 - 16.232,35', '16.230,08'],
+  ['IDR', '1.213.522,18', '1.208.794,22 - 1.213.522,18', '1.211.158,20'],
   [''],
   ['', 'Awal Tahun', 'Pergerakkan YTD', '+/- YTD'],
-  ['USD', '66,32', '64,07 - 77,14', '+8,21 (12,38%)'],
-  ['KURS', '15.390,10', '15.390,00 - 16.307,80', '+779,05 (5,06%)'],
-  ['IDR', '1.020.729,53', '997.660,12 - 1.256.829,06', '+184.283,34 (18,05%)'],
+  ['USD', '66,32', '64,07 - 77,14', '+8,17 (12,32%)'],
+  ['KURS', '15.390,10', '15.390,00 - 16.307,80', '+837,70 (5,44%)'],
+  ['IDR', '1.020.729,53', '997.660,12 - 1.256.829,06', '+188.064,69 (18,42%)'],
   [''],
   ['', 'Tahun Lalu / 52 Minggu', 'Pergerakkan 52 Minggu', '+/- 52 Minggu'],
-  ['USD', '63,76', '58,43 - 77,14', '+10,77 (16,89%)'],
-  ['KURS', '14.936,00', '14.669,40 - 16.307,80', '+1.233,15 (8,26%)'],
-  ['IDR', '952.339,68', '912.925,68 - 1.256.829,06', '+252.673,19 (26,53%)']])
+  ['USD', '63,84', '58,43 - 77,14', '+10,65 (16,68%)'],
+  ['KURS', '14.930,10', '14.669,40 - 16.307,80', '+1.297,70 (8,69%)'],
+  ['IDR', '953.091,52', '912.925,68 - 1.256.829,06', '+255.702,70 (26,83%)']])
 ```
 
 ## iopen
 
 `iopen(path, data=None, regex=None, css_select=None, xpath=None, file_append=False)`
 
 Membaca atau Tulis pada path yang bisa merupakan FILE maupun URL.  
@@ -1461,15 +1464,15 @@
 print(iopen("https://www.google.com/", dict(coba="dulu"), xpath="//a"))  
 ```
 
 Output:
 ```py
 8
 ['mana', 'aja']
-[<Element a at 0x71ec8a2fd0>, <Element a at 0x71ec8ee7b0>, <Element a at 0x71ec8ee850>, <Element a at 0x71ec8ee8a0>, <Element a at 0x71ec8ee8f0>, <Element a at 0x71ec8ee940>, <Element a at 0x71ec8ee990>, <Element a at 0x71ec8ee9e0>, <Element a at 0x71ec8eea30>, <Element a at 0x71ec8eea80>, <Element a at 0x71ec8eead0>, <Element a at 0x71ec8eeb20>, <Element a at 0x71ec8eeb70>, <Element a at 0x71ec8eebc0>, <Element a at 0x71ec8eec10>, <Element a at 0x71ec8eec60>, <Element a at 0x71ec8eecb0>, <Element a at 0x71ec8eed00>]
+[<Element a at 0x7a729faee0>, <Element a at 0x7a72a42580>, <Element a at 0x7a72a42620>, <Element a at 0x7a72a42670>, <Element a at 0x7a72a426c0>, <Element a at 0x7a72a42710>, <Element a at 0x7a72a42760>, <Element a at 0x7a72a427b0>, <Element a at 0x7a72a42800>, <Element a at 0x7a72a42850>, <Element a at 0x7a72a428a0>, <Element a at 0x7a72a428f0>, <Element a at 0x7a72a42940>, <Element a at 0x7a72a42990>, <Element a at 0x7a72a429e0>, <Element a at 0x7a72a42a30>, <Element a at 0x7a72a42a80>, <Element a at 0x7a72a42ad0>]
 False
 ```
 
 ## iprint
 
 `iprint(*args, color=None, sort_dicts=False, **kwargs)`
 
@@ -1502,16 +1505,16 @@
 print(list(irange('a', 'z', 10)))  
 print(list(irange(1, '7')))  
 print(list(irange(10, 5)))  
 ```
 
 Output:
 ```py
-<generator object irange at 0x71ec876ac0>
-<generator object irange at 0x71ec876ac0>
+<generator object irange at 0x7a729ca9b0>
+<generator object irange at 0x7a729ca9b0>
 ['a', 'k', 'u']
 [1, 2, 3, 4, 5, 6, 7]
 [10, 9, 8, 7, 6, 5]
 ```
 
 ## ireplace
 
@@ -1546,15 +1549,15 @@
 ```python  
 print(iscandir())  
 print(list(iscandir("./", recursive=False, scan_file=False)))  
 ```
 
 Output:
 ```py
-<generator object iscandir at 0x71ec8ac840>
+<generator object iscandir at 0x7a72a00840>
 [PosixPath('.git'), PosixPath('.vscode'), PosixPath('pypipr'), PosixPath('__pycache__'), PosixPath('dist')]
 ```
 
 ## isplit
 
 `isplit(text, separator='', include_separator=False)`
 
@@ -1603,15 +1606,15 @@
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 ```
 
 Output:
 ```py
-{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x71ec8c4520>,
+{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x7a72a14520>,
  'b': (0, 1, 2, 3, 4, 5, 6, 7, 8, 9),
  'c': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
  'd': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
```

### Comparing `pypipr-1.0.93/PKG-INFO` & `pypipr-1.0.94/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypipr
-Version: 1.0.93
+Version: 1.0.94
 Summary: The Python Package Index Project
 Author: ufiapjj
 Author-email: ufiapjj@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -97,15 +97,15 @@
 arr = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(chunk_array(arr, 5))  
 print(list(chunk_array(arr, 5)))  
 ```
 
 Output:
 ```py
-<generator object chunk_array at 0x71ec8ac240>
+<generator object chunk_array at 0x7a72a00240>
 [[2, 3, 12, 3, 3], [42, 42, 1, 43, 2], [42, 41, 4, 24, 32], [42, 3, 12, 32, 42], [42]]
 ```
 
 ## create_folder
 
 `create_folder(folder_name)`
 
@@ -148,17 +148,17 @@
 print(datetime_now("Asia/Jakarta"))  
 print(datetime_now("GMT"))  
 print(datetime_now("Etc/GMT+7"))  
 ```
 
 Output:
 ```py
-2024-04-24 15:30:21.125582+07:00
-2024-04-24 08:30:21.126382+00:00
-2024-04-24 01:30:21.127761-07:00
+2024-04-25 20:41:51.650942+07:00
+2024-04-25 13:41:51.652297+00:00
+2024-04-25 06:41:51.655828-07:00
 ```
 
 ## dict_first
 
 `dict_first(d: dict, remove=False)`
 
 Mengambil nilai (key, value) pertama dari dictionary dalam bentuk tuple.  
@@ -217,15 +217,15 @@
 ```python  
 var = [1, None, False, 0, "0", True, {}, ['eee']]  
 print(filter_empty(var))  
 ```
 
 Output:
 ```py
-<generator object filter_empty at 0x71ec842d40>
+<generator object filter_empty at 0x7a72992d40>
 ```
 
 ## get_by_index
 
 `get_by_index(obj, index, on_error=None)`
 
 Mendapatkan value dari object berdasarkan indexnya.  
@@ -263,16 +263,16 @@
   
 print(get_class_method(ExampleGetClassMethod))  
 print(list(get_class_method(ExampleGetClassMethod)))  
 ```
 
 Output:
 ```py
-<generator object get_class_method at 0x71ec843010>
-[<function ExampleGetClassMethod.a at 0x720457e7a0>, <function ExampleGetClassMethod.b at 0x71ec8b5580>, <function ExampleGetClassMethod.c at 0x71ec8b5620>, <function ExampleGetClassMethod.d at 0x71ec8b56c0>]
+<generator object get_class_method at 0x7a72993010>
+[<function ExampleGetClassMethod.a at 0x7a869867a0>, <function ExampleGetClassMethod.b at 0x7a72a096c0>, <function ExampleGetClassMethod.c at 0x7a72a09620>, <function ExampleGetClassMethod.d at 0x7a72a09760>]
 ```
 
 ## get_filemtime
 
 `get_filemtime(filename)`
 
 Mengambil informasi last modification time file dalam nano seconds  
@@ -389,17 +389,18 @@
 Output:
 ```py
 {'module': {'ibuiltins': <module 'pypipr.ibuiltins' from '/data/data/com.termux/files/home/pypipr/pypipr/ibuiltins/__init__.py'>,
             'iconsole': <module 'pypipr.iconsole' from '/data/data/com.termux/files/home/pypipr/pypipr/iconsole/__init__.py'>,
             'idjango': <module 'pypipr.idjango' from '/data/data/com.termux/files/home/pypipr/pypipr/idjango/__init__.py'>,
             'iengineering': <module 'pypipr.iengineering' from '/data/data/com.termux/files/home/pypipr/pypipr/iengineering/__init__.py'>,
             'ifunctions': <module 'pypipr.ifunctions' from '/data/data/com.termux/files/home/pypipr/pypipr/ifunctions/__init__.py'>,
-            'iflow': <module 'pypipr.iflow' (<_frozen_importlib_external.NamespaceLoader object at 0x71f481bed0>)>,
+            'iflow': <module 'pypipr.iflow' (<_frozen_importlib_external.NamespaceLoader object at 0x7a7f2cf610>)>,
             'asyncio': <module 'asyncio' from '/data/data/com.termux/files/usr/lib/python3.11/asyncio/__init__.py'>,
             'colorama': <module 'colorama' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/colorama/__init__.py'>,
+            'csv': <module 'csv' from '/data/data/com.termux/files/usr/lib/python3.11/csv.py'>,
             'datetime': <module 'datetime' from '/data/data/com.termux/files/usr/lib/python3.11/datetime.py'>,
             'functools': <module 'functools' from '/data/data/com.termux/files/usr/lib/python3.11/functools.py'>,
             'inspect': <module 'inspect' from '/data/data/com.termux/files/usr/lib/python3.11/inspect.py'>,
             'io': <module 'io' (frozen)>,
             'json': <module 'json' from '/data/data/com.termux/files/usr/lib/python3.11/json/__init__.py'>,
             'lxml': <module 'lxml' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/lxml/__init__.py'>,
             'math': <module 'math' from '/data/data/com.termux/files/usr/lib/python3.11/lib-dynload/math.cpython-311.so'>,
@@ -426,87 +427,88 @@
             'zoneinfo': <module 'zoneinfo' from '/data/data/com.termux/files/usr/lib/python3.11/zoneinfo/__init__.py'>},
  'class': {'ComparePerformance': <class 'pypipr.ibuiltins.ComparePerformance.ComparePerformance'>,
            'RunParallel': <class 'pypipr.ibuiltins.RunParallel.RunParallel'>,
            'APIMixinView': <class 'pypipr.idjango.APIMixinView.APIMixinView'>,
            'PintUregQuantity': <class 'pint.Quantity'>},
  'variable': {'LINUX': True,
               'WINDOWS': False,
-              'PintUreg': <pint.registry.UnitRegistry object at 0x71fe1eb710>},
- 'function': {'avg': <function avg at 0x72045b6d40>,
-              'basename': <function basename at 0x720457e8e0>,
-              'chunk_array': <function chunk_array at 0x71fe125120>,
-              'create_folder': <function create_folder at 0x71fe125300>,
-              'datetime_from_string': <function datetime_from_string at 0x71fe1254e0>,
-              'datetime_now': <function datetime_now at 0x71fe1cd620>,
-              'dict_first': <function dict_first at 0x71fe1cd580>,
-              'dirname': <function dirname at 0x71fe1cd4e0>,
-              'exit_if_empty': <function exit_if_empty at 0x71fe1a74c0>,
-              'filter_empty': <function filter_empty at 0x71fe1cd1c0>,
-              'get_by_index': <function get_by_index at 0x71fe1ccea0>,
-              'get_class_method': <function get_class_method at 0x71fe1cccc0>,
-              'get_filemtime': <function get_filemtime at 0x71fe1ccb80>,
-              'get_filesize': <function get_filesize at 0x71fe1cc9a0>,
-              'is_empty': <function is_empty at 0x71fe1cd260>,
-              'is_iterable': <function is_iterable at 0x71fe1ccfe0>,
-              'is_valid_url': <function is_valid_url at 0x71fe1cc860>,
-              'ivars': <function ivars at 0x71fe1cc7c0>,
-              'password_generator': <function password_generator at 0x71fe1cc680>,
-              'random_bool': <function random_bool at 0x71fe1cc400>,
-              'set_timeout': <function set_timeout at 0x71fe1cf7e0>,
-              'sets_ordered': <function sets_ordered at 0x71fe1cf920>,
-              'str_cmp': <function str_cmp at 0x71fe1cf9c0>,
-              'to_str': <function to_str at 0x71fe1ccf40>,
-              'choices': <function choices at 0x71fe1cfa60>,
-              'console_run': <function console_run at 0x71fe1cfce0>,
-              'input_char': <function input_char at 0x71fe1cfe20>,
-              'log': <function log at 0x71fe1f0040>,
-              'print_colorize': <function print_colorize at 0x71fe1f00e0>,
-              'print_dir': <function print_dir at 0x71fe1f0220>,
-              'print_log': <function print_log at 0x71fe1cfec0>,
-              'print_to_last_line': <function print_to_last_line at 0x71fe1cfc40>,
-              'text_colorize': <function text_colorize at 0x71fe1cfd80>,
-              'batch_calculate': <function batch_calculate at 0x71f4995580>,
-              'batchmaker': <function batchmaker at 0x71f496e980>,
-              'calculate': <function calculate at 0x71f49962a0>,
-              'auto_reload': <function auto_reload at 0x71f4996480>,
-              'github_pull': <function github_pull at 0x71f4996020>,
-              'github_push': <function github_push at 0x71f4996700>,
-              'github_user': <function github_user at 0x71f4996a20>,
-              'pip_freeze_without_version': <function pip_freeze_without_version at 0x71f46b9f80>,
-              'poetry_publish': <function poetry_publish at 0x71f46ba160>,
-              'poetry_update_version': <function poetry_update_version at 0x71f46da980>,
-              'iargv': <function iargv at 0x71eca7c0e0>,
-              'idumps': <function idumps at 0x71eca7c220>,
-              'idumps_html': <function idumps_html at 0x71ecae0c20>,
-              'ienv': <function ienv at 0x71eca7c360>,
-              'iexec': <function iexec at 0x71ecae0ea0>,
-              'ijoin': <function ijoin at 0x71f46b9ee0>,
-              'iloads': <function iloads at 0x71ecae0f40>,
-              'iloads_html': <function iloads_html at 0x71ecae11c0>,
-              'iopen': <function iopen at 0x71f46ba200>,
-              'iprint': <function iprint at 0x71eca7c180>,
-              'irange': <function irange at 0x71f49963e0>,
-              'ireplace': <function ireplace at 0x71ecae1080>,
-              'iscandir': <function iscandir at 0x71ecae2e80>,
-              'isplit': <function isplit at 0x71ecae2f20>}}
+              'PintUreg': <pint.registry.UnitRegistry object at 0x7a78af4750>},
+ 'function': {'avg': <function avg at 0x7a869bed40>,
+              'basename': <function basename at 0x7a869868e0>,
+              'chunk_array': <function chunk_array at 0x7a83471120>,
+              'create_folder': <function create_folder at 0x7a83471300>,
+              'datetime_from_string': <function datetime_from_string at 0x7a834714e0>,
+              'datetime_now': <function datetime_now at 0x7a83519620>,
+              'dict_first': <function dict_first at 0x7a83519580>,
+              'dirname': <function dirname at 0x7a835194e0>,
+              'exit_if_empty': <function exit_if_empty at 0x7a834f34c0>,
+              'filter_empty': <function filter_empty at 0x7a835191c0>,
+              'get_by_index': <function get_by_index at 0x7a83518ea0>,
+              'get_class_method': <function get_class_method at 0x7a83518cc0>,
+              'get_filemtime': <function get_filemtime at 0x7a83518b80>,
+              'get_filesize': <function get_filesize at 0x7a835189a0>,
+              'is_empty': <function is_empty at 0x7a83519260>,
+              'is_iterable': <function is_iterable at 0x7a83518fe0>,
+              'is_valid_url': <function is_valid_url at 0x7a83518860>,
+              'ivars': <function ivars at 0x7a835187c0>,
+              'password_generator': <function password_generator at 0x7a83518680>,
+              'random_bool': <function random_bool at 0x7a83518400>,
+              'restart': <function restart at 0x7a8351b740>,
+              'set_timeout': <function set_timeout at 0x7a8351b880>,
+              'sets_ordered': <function sets_ordered at 0x7a8351b9c0>,
+              'str_cmp': <function str_cmp at 0x7a8351ba60>,
+              'to_str': <function to_str at 0x7a83518f40>,
+              'choices': <function choices at 0x7a8351bb00>,
+              'console_run': <function console_run at 0x7a8351bd80>,
+              'input_char': <function input_char at 0x7a8351bec0>,
+              'log': <function log at 0x7a8351bc40>,
+              'print_colorize': <function print_colorize at 0x7a83540180>,
+              'print_dir': <function print_dir at 0x7a835402c0>,
+              'print_log': <function print_log at 0x7a8351bf60>,
+              'print_to_last_line': <function print_to_last_line at 0x7a8351bce0>,
+              'text_colorize': <function text_colorize at 0x7a8351be20>,
+              'batch_calculate': <function batch_calculate at 0x7a780d9620>,
+              'batchmaker': <function batchmaker at 0x7a780da0c0>,
+              'calculate': <function calculate at 0x7a780da340>,
+              'auto_reload': <function auto_reload at 0x7a780da5c0>,
+              'github_pull': <function github_pull at 0x7a780da520>,
+              'github_push': <function github_push at 0x7a780da7a0>,
+              'github_user': <function github_user at 0x7a780daac0>,
+              'pip_freeze_without_version': <function pip_freeze_without_version at 0x7a77e1a0c0>,
+              'poetry_publish': <function poetry_publish at 0x7a77e1a200>,
+              'poetry_update_version': <function poetry_update_version at 0x7a77e3aa20>,
+              'iargv': <function iargv at 0x7a72bd0180>,
+              'idumps': <function idumps at 0x7a72bd02c0>,
+              'idumps_html': <function idumps_html at 0x7a72c38cc0>,
+              'ienv': <function ienv at 0x7a72bd0400>,
+              'iexec': <function iexec at 0x7a72c38f40>,
+              'ijoin': <function ijoin at 0x7a77e19f80>,
+              'iloads': <function iloads at 0x7a72c38fe0>,
+              'iloads_html': <function iloads_html at 0x7a72c39260>,
+              'iopen': <function iopen at 0x7a77e1a2a0>,
+              'iprint': <function iprint at 0x7a72c39120>,
+              'irange': <function irange at 0x7a780da480>,
+              'ireplace': <function ireplace at 0x7a72c39300>,
+              'iscandir': <function iscandir at 0x7a72c3af20>,
+              'isplit': <function isplit at 0x7a72c3afc0>}}
 ```
 
 ## password_generator
 
 `password_generator(length=8, characters='abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~')`
 
 Membuat pssword secara acak  
   
 ```python  
 print(password_generator())  
 ```
 
 Output:
 ```py
-;U&Ljx6Z
+n.,UG}_N
 ```
 
 ## random_bool
 
 `random_bool()`
 
 Menghasilkan nilai random True atau False.  
@@ -516,17 +518,21 @@
   
 ```python  
 print(random_bool())  
 ```
 
 Output:
 ```py
-True
+False
 ```
 
+## restart
+
+`restart()`
+
 ## set_timeout
 
 `set_timeout(interval, func, args=None, kwargs=None)`
 
 Menjalankan fungsi ketika sudah sekian detik.  
 Apabila timeout masih berjalan tapi kode sudah selesai dieksekusi semua, maka  
 program tidak akan berhenti sampai timeout selesai, kemudian fungsi dijalankan,  
@@ -538,15 +544,15 @@
 print(x)  
 print("menghentikan timeout 7")  
 x.cancel()  
 ```
 
 Output:
 ```py
-<Timer(Thread-2, started 489281289456)>
+<Timer(Thread-2, started 525885381872)>
 menghentikan timeout 7
 ```
 
 ## sets_ordered
 
 `sets_ordered(iterator)`
 
@@ -556,15 +562,15 @@
 array = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(sets_ordered(array))  
 print(list(sets_ordered(array)))  
 ```
 
 Output:
 ```py
-<generator object sets_ordered at 0x71ec8c01e0>
+<generator object sets_ordered at 0x7a72a141e0>
 [2, 3, 12, 42, 1, 43, 41, 4, 24, 32]
 ```
 
 ## str_cmp
 
 `str_cmp(t1, t2)`
 
@@ -710,29 +716,29 @@
              __doc__ : Path subclass for non-Windows systems.
 
     On a POSIX system, instantiating a Path should return this object.
     
            __enter__ : https:/www.google.com
           __fspath__ : https:/www.google.com
         __getstate__ : (None, {'_drv': '', '_root': '', '_parts': ['https:', 'www.google.com'], '_str': 'https:/www.google.com'})
-            __hash__ : -6619349520802782460
+            __hash__ : 355454826737572805
             __init__ : None
    __init_subclass__ : None
           __module__ : pathlib
           __reduce__ : (<class 'pathlib.PosixPath'>, ('https:', 'www.google.com'))
             __repr__ : PosixPath('https:/www.google.com')
           __sizeof__ : 72
            __slots__ : ()
              __str__ : https:/www.google.com
     __subclasshook__ : NotImplemented
       _cached_cparts : ['https:', 'www.google.com']
              _cparts : ['https:', 'www.google.com']
                 _drv : 
-            _flavour : <pathlib._PosixFlavour object at 0x71fe1a0790>
-               _hash : -6619349520802782460
+            _flavour : <pathlib._PosixFlavour object at 0x7a834ec650>
+               _hash : 355454826737572805
               _parts : ['https:', 'www.google.com']
                _root : 
                 _str : https:/www.google.com
             absolute : /data/data/com.termux/files/home/pypipr/https:/www.google.com
               anchor : 
             as_posix : https:/www.google.com
                  cwd : /data/data/com.termux/files/home/pypipr
@@ -746,15 +752,15 @@
               is_dir : False
              is_fifo : False
              is_file : False
             is_mount : False
          is_reserved : False
            is_socket : False
           is_symlink : False
-             iterdir : <generator object Path.iterdir at 0x71ec898c80>
+             iterdir : <generator object Path.iterdir at 0x7a729f0900>
             joinpath : https:/www.google.com
                 name : www.google.com
               parent : https:
              parents : <PosixPath.parents>
                parts : ('https:', 'www.google.com')
              resolve : /data/data/com.termux/files/home/pypipr/https:/www.google.com
                 root : 
@@ -813,15 +819,15 @@
 ```python  
 print(batch_calculate("{1 10} m ** {1 3}"))  
 print(list(batch_calculate("{1 10} m ** {1 3}")))  
 ```
 
 Output:
 ```py
-<generator object batch_calculate at 0x71ec843b50>
+<generator object batch_calculate at 0x7a72993970>
 [('1 m ** 1', <Quantity(1, 'meter')>), ('1 m ** 2', <Quantity(1, 'meter ** 2')>), ('1 m ** 3', <Quantity(1, 'meter ** 3')>), ('2 m ** 1', <Quantity(2, 'meter')>), ('2 m ** 2', <Quantity(2, 'meter ** 2')>), ('2 m ** 3', <Quantity(2, 'meter ** 3')>), ('3 m ** 1', <Quantity(3, 'meter')>), ('3 m ** 2', <Quantity(3, 'meter ** 2')>), ('3 m ** 3', <Quantity(3, 'meter ** 3')>), ('4 m ** 1', <Quantity(4, 'meter')>), ('4 m ** 2', <Quantity(4, 'meter ** 2')>), ('4 m ** 3', <Quantity(4, 'meter ** 3')>), ('5 m ** 1', <Quantity(5, 'meter')>), ('5 m ** 2', <Quantity(5, 'meter ** 2')>), ('5 m ** 3', <Quantity(5, 'meter ** 3')>), ('6 m ** 1', <Quantity(6, 'meter')>), ('6 m ** 2', <Quantity(6, 'meter ** 2')>), ('6 m ** 3', <Quantity(6, 'meter ** 3')>), ('7 m ** 1', <Quantity(7, 'meter')>), ('7 m ** 2', <Quantity(7, 'meter ** 2')>), ('7 m ** 3', <Quantity(7, 'meter ** 3')>), ('8 m ** 1', <Quantity(8, 'meter')>), ('8 m ** 2', <Quantity(8, 'meter ** 2')>), ('8 m ** 3', <Quantity(8, 'meter ** 3')>), ('9 m ** 1', <Quantity(9, 'meter')>), ('9 m ** 2', <Quantity(9, 'meter ** 2')>), ('9 m ** 3', <Quantity(9, 'meter ** 3')>), ('10 m ** 1', <Quantity(10, 'meter')>), ('10 m ** 2', <Quantity(10, 'meter ** 2')>), ('10 m ** 3', <Quantity(10, 'meter ** 3')>)]
 ```
 
 ## batchmaker
 
 `batchmaker(pattern: str)`
 
@@ -838,15 +844,15 @@
 s = "Urutan {1/6/3} dan {10:9} dan {j k} dan {Z - A - 15} saja."  
 print(batchmaker(s))  
 print(list(batchmaker(s)))  
 ```
 
 Output:
 ```py
-<generator object batchmaker at 0x71ec8b0040>
+<generator object batchmaker at 0x7a72a04160>
 ['Urutan 1 dan 10 dan j dan Z saja.', 'Urutan 1 dan 10 dan j dan K saja.', 'Urutan 1 dan 10 dan k dan Z saja.', 'Urutan 1 dan 10 dan k dan K saja.', 'Urutan 1 dan 9 dan j dan Z saja.', 'Urutan 1 dan 9 dan j dan K saja.', 'Urutan 1 dan 9 dan k dan Z saja.', 'Urutan 1 dan 9 dan k dan K saja.', 'Urutan 4 dan 10 dan j dan Z saja.', 'Urutan 4 dan 10 dan j dan K saja.', 'Urutan 4 dan 10 dan k dan Z saja.', 'Urutan 4 dan 10 dan k dan K saja.', 'Urutan 4 dan 9 dan j dan Z saja.', 'Urutan 4 dan 9 dan j dan K saja.', 'Urutan 4 dan 9 dan k dan Z saja.', 'Urutan 4 dan 9 dan k dan K saja.']
 ```
 
 ## calculate
 
 `calculate(teks)`
 
@@ -1202,15 +1208,15 @@
     recursive_flat=True))  
 print(ijoin(arr, separator='</div>\n<div>', start='<div>', end='</div>'))  
 print(ijoin(10, ' '))  
 ```
 
 Output:
 ```py
-dfs, qweqw, asd, weq
+weq, asd, dfs, qweqw
 ,ini,path,seperti,url,
 ini,path,seperti,url
 <li>satu</li>
 <li>12</li>
 <li>34</li>
 <li>56</li>
 <li>tiga</li>
@@ -1267,190 +1273,187 @@
 pprint.pprint(iloads_html(iopen("https://harga-emas.org/")), depth=10)  
 pprint.pprint(iloads_html(iopen("https://harga-emas.org/1-gram/")), depth=10)  
 ```
 
 Output:
 ```py
 (['Home', 'Emas 1 Gram', 'History', 'Trend', 'Perak 1 Gram', 'Pluang'],
- [['Harga Emas Hari Ini - Rabu, 24 April 2024'],
-  ['Spot Emas USD↓2.318,00 (-11,91) / oz',
-   'Kurs IDR↑16.244,00 (+20,00) / USD',
-   'Emas IDR↓1.210.591 (-4.722) / gr'],
-  ['LM Antam (Jual)↓1.320.000 (-5.000) / gr',
-   'LM Antam (Beli)↓1.218.000 (-5.000) / gr']],
+ [['Harga Emas Hari Ini - Kamis, 25 April 2024'],
+  ['Spot Emas USD↓2.316,87 (-8,41) / oz',
+   'Kurs IDR↓16.161,00 (-83,00) / USD',
+   'Emas IDR↓1.203.818 (-10.575) / gr'],
+  ['LM Antam (Jual)↓1.319.000 (-1.000) / gr',
+   'LM Antam (Beli)↓1.217.000 (-1.000) / gr']],
  [['Harga Emas Hari Ini'],
   ['Gram', 'Gedung Antam Jakarta', 'Pegadaian'],
   ['per Gram (Rp)', 'per Batangan (Rp)', 'per Gram (Rp)', 'per Batangan (Rp)'],
   ['1000',
-   '1.261 (-5)',
-   '1.260.600 (-5.000)',
+   '1.260 (-1)',
+   '1.259.600 (-1.000)',
    '1.043.040 (+8.200)',
    '1.043.040.000 (+8.200.000)'],
   ['500',
-   '2.521 (-10)',
-   '1.260.640 (-5.000)',
+   '2.519 (-2)',
+   '1.259.640 (-1.000)',
    '1.043.082 (+8.200)',
    '521.541.000 (+4.100.000)'],
   ['250',
-   '5.044 (-20)',
-   '1.261.060 (-5.000)',
+   '5.040 (-4)',
+   '1.260.060 (-1.000)',
    '1.043.512 (+8.200)',
    '260.878.000 (+2.050.000)'],
   ['100',
-   '12.621 (-50)',
-   '1.262.120 (-5.000)',
+   '12.611 (-10)',
+   '1.261.120 (-1.000)',
    '1.044.600 (+8.200)',
    '104.460.000 (+820.000)'],
   ['50',
-   '25.258 (-100)',
-   '1.262.900 (-5.000)',
+   '25.238 (-20)',
+   '1.261.900 (-1.000)',
    '1.045.400 (+8.200)',
    '52.270.000 (+410.000)'],
   ['25',
-   '50.579 (-200)',
-   '1.264.480 (-5.000)',
+   '50.539 (-40)',
+   '1.263.480 (-1.000)',
    '1.047.040 (+8.200)',
    '26.176.000 (+205.000)'],
   ['10',
-   '126.950 (-500)',
-   '1.269.500 (-5.000)',
+   '126.850 (-100)',
+   '1.268.500 (-1.000)',
    '1.052.200 (+8.200)',
    '10.522.000 (+82.000)'],
   ['5',
-   '255.000 (-1.000)',
-   '1.275.000 (-5.000)',
+   '254.800 (-200)',
+   '1.274.000 (-1.000)',
    '1.057.800 (+8.200)',
    '5.289.000 (+41.000)'],
   ['3',
-   '427.222 (-1.667)',
-   '1.281.667 (-5.000)',
+   '426.889 (-333)',
+   '1.280.667 (-1.000)',
    '1.064.667 (+8.000)',
    '3.194.000 (+24.000)'],
   ['2',
-   '645.000 (-2.500)',
-   '1.290.000 (-5.000)',
+   '644.500 (-500)',
+   '1.289.000 (-1.000)',
    '1.073.500 (+8.500)',
    '2.147.000 (+17.000)'],
   ['1',
-   '1.320.000 (-5.000)',
-   '1.320.000 (-5.000)',
+   '1.319.000 (-1.000)',
+   '1.319.000 (-1.000)',
    '1.104.000 (+8.000)',
    '1.104.000 (+8.000)'],
   ['0.5',
-   '2.840.000 (-10.000)',
-   '1.420.000 (-5.000)',
+   '2.838.000 (-2.000)',
+   '1.419.000 (-1.000)',
    '1.208.000 (+8.000)',
    '604.000 (+4.000)'],
-  ['Update harga LM Antam :24 April 2024, pukul 08:12Harga pembelian kembali '
-   ':Rp. 1.218.000/gram (-5.000)',
+  ['Update harga LM Antam :25 April 2024, pukul 08:05Harga pembelian kembali '
+   ':Rp. 1.217.000/gram (-1.000)',
    'Update harga LM Pegadaian :31 Agustus 2023']],
  [['Spot Harga Emas Hari Ini (Market Open)'],
   ['Satuan', 'USD', 'Kurs\xa0Dollar', 'IDR'],
-  ['Ounce\xa0(oz)', '2.318,00 (-11,91)', '16.244,00 (+20,00)', '37.653.592'],
-  ['Gram\xa0(gr)', '74,53', '16.244,00', '1.210.591 (-4.722)'],
-  ['Kilogram\xa0(kg)', '74.525,43', '16.244,00', '1.210.591.095'],
-  ['Update harga emas :24 April 2024, pukul 15:30Update kurs :24 April 2024, '
+  ['Ounce\xa0(oz)', '2.316,87 (-8,41)', '16.161,00 (-83,00)', '37.442.936'],
+  ['Gram\xa0(gr)', '74,49', '16.161,00', '1.203.818 (-10.575)'],
+  ['Kilogram\xa0(kg)', '74.489,10', '16.161,00', '1.203.818.350'],
+  ['Update harga emas :25 April 2024, pukul 20:41Update kurs :25 April 2024, '
    'pukul 13:10']],
  [['Gram', 'UBS Gold 99.99%'],
   ['Jual', 'Beli'],
   ['/ Batang', '/ Gram', '/ Batang', '/ Gram'],
   ['100',
-   '126.000.000 (-712.000)',
-   '1.260.000 (-7.120)',
-   '123.985.000 (+250.000)',
-   '1.239.850 (+2.500)'],
+   '126.000.000',
+   '1.260.000',
+   '124.385.000 (+400.000)',
+   '1.243.850 (+4.000)'],
   ['50',
-   '63.100.000 (-295.000)',
-   '1.262.000 (-5.900)',
-   '62.045.000 (+125.000)',
-   '1.240.900 (+2.500)'],
+   '63.100.000',
+   '1.262.000',
+   '62.245.000 (+200.000)',
+   '1.244.900 (+4.000)'],
   ['25',
-   '31.600.000 (-137.000)',
-   '1.264.000 (-5.480)',
-   '31.125.000 (+62.500)',
-   '1.245.000 (+2.500)'],
+   '31.600.000',
+   '1.264.000',
+   '31.225.000 (+100.000)',
+   '1.249.000 (+4.000)'],
   ['10',
-   '12.680.000 (-65.000)',
-   '1.268.000 (-6.500)',
-   '12.500.000 (+25.000)',
-   '1.250.000 (+2.500)'],
-  ['5',
-   '6.365.000 (-35.000)',
-   '1.273.000 (-7.000)',
-   '6.302.000 (+12.500)',
-   '1.260.400 (+2.500)'],
+   '12.680.000',
+   '1.268.000',
+   '12.540.000 (+40.000)',
+   '1.254.000 (+4.000)'],
+  ['5', '6.365.000', '1.273.000', '6.322.000 (+20.000)', '1.264.400 (+4.000)'],
   ['1',
-   '1.320.000 (-5.000)',
-   '1.320.000 (-5.000)',
-   '1.293.000 (+2.500)',
-   '1.293.000 (+2.500)'],
-  ['', 'Update :24 April 2024, pukul 13:02']],
+   '1.315.000 (-5.000)',
+   '1.315.000 (-5.000)',
+   '1.297.000 (+4.000)',
+   '1.297.000 (+4.000)'],
+  ['', 'Update :25 April 2024, pukul 14:44']],
  [['Konversi Satuan'],
   ['Satuan', 'Ounce (oz)', 'Gram (gr)', 'Kilogram (kg)'],
   ['Ounce\xa0(oz)', '1', '31,1034767696', '0,0311034768'],
   ['Gram\xa0(gr)', '0,0321507466', '1', '0.001'],
   ['Kilogram\xa0(kg)', '32,1507466000', '1.000', '1']],
  [['Pergerakan Harga Emas Dunia'],
   ['Waktu', 'Emas'],
   ['Unit', 'USD', 'IDR'],
   ['Angka', '+/-', 'Angka', '+/-'],
-  ['Hari Ini', 'Kurs', '', '', '16.224', '+20+0,12%'],
-  ['oz', '2.329,91', '-11,91-0,51%', '37.800.460', '-146.868-0,39%'],
-  ['gr', '74,91', '-0,38-0,51%', '1.215.313', '-4.722-0,39%'],
-  ['30 Hari', 'Kurs', '', '', '15.773', '+471+2,99%'],
-  ['oz', '2.175,55', '+142,45+6,55%', '34.314.950', '+3.338.642+9,73%'],
-  ['gr', '69,95', '+4,58+6,55%', '1.103.251', '+107.340+9,73%'],
-  ['2 Bulan', 'Kurs', '', '', '15.630', '+614+3,93%'],
-  ['oz', '2.035,57', '+282,43+13,87%', '31.815.959', '+5.837.633+18,35%'],
-  ['gr', '65,45', '+9,08+13,87', '1.022.907', '+187.684+18,35%'],
-  ['6 Bulan', 'Kurs', '', '', '15.933', '+311+1,95%'],
-  ['oz', '1.983,13', '+334,87+16,89%', '31.597.210', '+6.056.382+19,17%'],
-  ['gr', '63,76', '+10,77+16,89%', '1.015.874', '+194.717+19,17%'],
-  ['1 Tahun', 'Kurs', '', '', '15.731', '+513+3,26%'],
-  ['oz', '1.823,86', '+494,14+27,09%', '28.691.142', '+8.962.450+31,24%'],
-  ['gr', '58,64', '+15,89+27,09%', '922.442', '+288.149+31,24%'],
-  ['2 Tahun', 'Kurs', '', '', '14.361', '+1.883+13,11%'],
-  ['oz', '1.896,13', '+421,87+22,25%', '27.230.342', '+10.423.250+38,28%'],
-  ['gr', '60,96', '+13,56+22,25%', '875.476', '+335.115+38,28%'],
-  ['3 Tahun', 'Kurs', '', '', '14.530', '+1.714+11,80%'],
-  ['oz', '1.777,11', '+540,89+30,44%', '25.821.408', '+11.832.184+45,82%'],
-  ['gr', '57,14', '+17,39+30,44%', '830.178', '+380.414+45,82%'],
-  ['5 Tahun', 'Kurs', '', '', '14.188', '+2.056+14,49%'],
-  ['oz', '1.288,10', '+1.029,90+79,95%', '18.275.563', '+19.378.029+106,03%'],
-  ['gr', '41,41', '+33,11+79,95%', '587.573', '+623.018+106,03%']])
+  ['Hari Ini', 'Kurs', '', '', '16.244', '-83-0,51%'],
+  ['oz', '2.325,28', '-8,41-0,36%', '37.771.848', '-328.912-0,87%'],
+  ['gr', '74,76', '-0,27-0,36%', '1.214.393', '-10.575-0,87%'],
+  ['30 Hari', 'Kurs', '', '', '15.795', '+366+2,32%'],
+  ['oz', '2.177,78', '+139,09+6,39%', '34.398.035', '+3.044.901+8,85%'],
+  ['gr', '70,02', '+4,47+6,39%', '1.105.923', '+97.896+8,85%'],
+  ['2 Bulan', 'Kurs', '', '', '15.630', '+531+3,40%'],
+  ['oz', '2.035,57', '+281,30+13,82%', '31.815.959', '+5.626.977+17,69%'],
+  ['gr', '65,45', '+9,04+13,82', '1.022.907', '+180.912+17,69%'],
+  ['6 Bulan', 'Kurs', '', '', '15.933', '+228+1,43%'],
+  ['oz', '2.006,33', '+310,54+15,48%', '31.966.856', '+5.476.080+17,13%'],
+  ['gr', '64,51', '+9,98+15,48%', '1.027.758', '+176.060+17,13%'],
+  ['1 Tahun', 'Kurs', '', '', '15.731', '+430+2,73%'],
+  ['oz', '1.823,86', '+493,01+27,03%', '28.691.142', '+8.751.794+30,50%'],
+  ['gr', '58,64', '+15,85+27,03%', '922.442', '+281.377+30,50%'],
+  ['2 Tahun', 'Kurs', '', '', '14.452', '+1.709+11,83%'],
+  ['oz', '1.901,97', '+414,90+21,81%', '27.487.270', '+9.955.666+36,22%'],
+  ['gr', '61,15', '+13,34+21,81%', '883.736', '+320.082+36,22%'],
+  ['3 Tahun', 'Kurs', '', '', '14.548', '+1.613+11,09%'],
+  ['oz', '1.779,86', '+537,01+30,17%', '25.893.403', '+11.549.533+44,60%'],
+  ['gr', '57,22', '+17,27+30,17%', '832.492', '+371.326+44,60%'],
+  ['5 Tahun', 'Kurs', '', '', '14.188', '+1.973+13,91%'],
+  ['oz', '1.286,10', '+1.030,77+80,15%', '18.247.187', '+19.195.749+105,20%'],
+  ['gr', '41,35', '+33,14+80,15%', '586.661', '+617.158+105,20%']])
+Timeout 3
 (['Home', 'Emas 1 Gram', 'History', 'Trend', 'Perak 1 Gram', 'Pluang'],
  [[''],
   ['Emas 24 KaratHarga Emas 1 Gram', ''],
-  ['USD', '74,53↓', '-0,38-0,51%'],
-  ['KURS', '16.169,15↑', '+22,25+0,14%'],
-  ['IDR', '1.205.012,87↓', '-4.524,70-0,37%'],
-  ['Rabu, 24 April 2024 15:30']],
+  ['USD', '74,49↓', '-0,27-0,36%'],
+  ['KURS', '16.227,80↓', '-4,55-0,03%'],
+  ['IDR', '1.208.794,22↓', '-4.727,96-0,39%'],
+  ['Kamis, 25 April 2024 20:41']],
  [[''],
   ['Emas 1 Gram (IDR)Emas 1 Gram (USD)Kurs USD-IDR',
    'Hari Ini',
    '1 Bulan',
    '1 Tahun',
    '5 Tahun',
    'Max',
    '']],
  [['Pergerakkan Harga Emas 1 Gram'],
   ['', 'Penutupan Kemarin', 'Pergerakkan Hari Ini', 'Rata-rata'],
-  ['USD', '74,91', '74,53 - 74,91', '74,72'],
-  ['KURS', '16.146,90', '16.146,90 - 16.169,15', '16.158,03'],
-  ['IDR', '1.209.537,57', '1.205.012,87 - 1.209.537,57', '1.207.275,22'],
+  ['USD', '74,76', '74,49 - 74,76', '74,63'],
+  ['KURS', '16.232,35', '16.227,80 - 16.232,35', '16.230,08'],
+  ['IDR', '1.213.522,18', '1.208.794,22 - 1.213.522,18', '1.211.158,20'],
   [''],
   ['', 'Awal Tahun', 'Pergerakkan YTD', '+/- YTD'],
-  ['USD', '66,32', '64,07 - 77,14', '+8,21 (12,38%)'],
-  ['KURS', '15.390,10', '15.390,00 - 16.307,80', '+779,05 (5,06%)'],
-  ['IDR', '1.020.729,53', '997.660,12 - 1.256.829,06', '+184.283,34 (18,05%)'],
+  ['USD', '66,32', '64,07 - 77,14', '+8,17 (12,32%)'],
+  ['KURS', '15.390,10', '15.390,00 - 16.307,80', '+837,70 (5,44%)'],
+  ['IDR', '1.020.729,53', '997.660,12 - 1.256.829,06', '+188.064,69 (18,42%)'],
   [''],
   ['', 'Tahun Lalu / 52 Minggu', 'Pergerakkan 52 Minggu', '+/- 52 Minggu'],
-  ['USD', '63,76', '58,43 - 77,14', '+10,77 (16,89%)'],
-  ['KURS', '14.936,00', '14.669,40 - 16.307,80', '+1.233,15 (8,26%)'],
-  ['IDR', '952.339,68', '912.925,68 - 1.256.829,06', '+252.673,19 (26,53%)']])
+  ['USD', '63,84', '58,43 - 77,14', '+10,65 (16,68%)'],
+  ['KURS', '14.930,10', '14.669,40 - 16.307,80', '+1.297,70 (8,69%)'],
+  ['IDR', '953.091,52', '912.925,68 - 1.256.829,06', '+255.702,70 (26,83%)']])
 ```
 
 ## iopen
 
 `iopen(path, data=None, regex=None, css_select=None, xpath=None, file_append=False)`
 
 Membaca atau Tulis pada path yang bisa merupakan FILE maupun URL.  
@@ -1484,15 +1487,15 @@
 print(iopen("https://www.google.com/", dict(coba="dulu"), xpath="//a"))  
 ```
 
 Output:
 ```py
 8
 ['mana', 'aja']
-[<Element a at 0x71ec8a2fd0>, <Element a at 0x71ec8ee7b0>, <Element a at 0x71ec8ee850>, <Element a at 0x71ec8ee8a0>, <Element a at 0x71ec8ee8f0>, <Element a at 0x71ec8ee940>, <Element a at 0x71ec8ee990>, <Element a at 0x71ec8ee9e0>, <Element a at 0x71ec8eea30>, <Element a at 0x71ec8eea80>, <Element a at 0x71ec8eead0>, <Element a at 0x71ec8eeb20>, <Element a at 0x71ec8eeb70>, <Element a at 0x71ec8eebc0>, <Element a at 0x71ec8eec10>, <Element a at 0x71ec8eec60>, <Element a at 0x71ec8eecb0>, <Element a at 0x71ec8eed00>]
+[<Element a at 0x7a729faee0>, <Element a at 0x7a72a42580>, <Element a at 0x7a72a42620>, <Element a at 0x7a72a42670>, <Element a at 0x7a72a426c0>, <Element a at 0x7a72a42710>, <Element a at 0x7a72a42760>, <Element a at 0x7a72a427b0>, <Element a at 0x7a72a42800>, <Element a at 0x7a72a42850>, <Element a at 0x7a72a428a0>, <Element a at 0x7a72a428f0>, <Element a at 0x7a72a42940>, <Element a at 0x7a72a42990>, <Element a at 0x7a72a429e0>, <Element a at 0x7a72a42a30>, <Element a at 0x7a72a42a80>, <Element a at 0x7a72a42ad0>]
 False
 ```
 
 ## iprint
 
 `iprint(*args, color=None, sort_dicts=False, **kwargs)`
 
@@ -1525,16 +1528,16 @@
 print(list(irange('a', 'z', 10)))  
 print(list(irange(1, '7')))  
 print(list(irange(10, 5)))  
 ```
 
 Output:
 ```py
-<generator object irange at 0x71ec876ac0>
-<generator object irange at 0x71ec876ac0>
+<generator object irange at 0x7a729ca9b0>
+<generator object irange at 0x7a729ca9b0>
 ['a', 'k', 'u']
 [1, 2, 3, 4, 5, 6, 7]
 [10, 9, 8, 7, 6, 5]
 ```
 
 ## ireplace
 
@@ -1569,15 +1572,15 @@
 ```python  
 print(iscandir())  
 print(list(iscandir("./", recursive=False, scan_file=False)))  
 ```
 
 Output:
 ```py
-<generator object iscandir at 0x71ec8ac840>
+<generator object iscandir at 0x7a72a00840>
 [PosixPath('.git'), PosixPath('.vscode'), PosixPath('pypipr'), PosixPath('__pycache__'), PosixPath('dist')]
 ```
 
 ## isplit
 
 `isplit(text, separator='', include_separator=False)`
 
@@ -1626,15 +1629,15 @@
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 ```
 
 Output:
 ```py
-{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x71ec8c4520>,
+{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x7a72a14520>,
  'b': (0, 1, 2, 3, 4, 5, 6, 7, 8, 9),
  'c': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
  'd': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
```


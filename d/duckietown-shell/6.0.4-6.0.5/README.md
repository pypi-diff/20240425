# Comparing `tmp/duckietown-shell-6.0.4.tar.gz` & `tmp/duckietown-shell-6.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckietown-shell-6.0.4.tar", last modified: Fri Apr 19 21:18:25 2024, max compression
+gzip compressed data, was "duckietown-shell-6.0.5.tar", last modified: Thu Apr 25 05:41:59 2024, max compression
```

## Comparing `duckietown-shell-6.0.4.tar` & `duckietown-shell-6.0.5.tar`

### file list

```diff
@@ -1,168 +1,117 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.498242 duckietown-shell-6.0.4/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    75933 2023-04-19 20:12:13.000000 duckietown-shell-6.0.4/LICENSE.pdf
--rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      599 2024-04-19 21:18:25.498242 duckietown-shell-6.0.4/PKG-INFO
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.498242 duckietown-shell-6.0.4/duckietown_shell.egg-info/
--rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      599 2024-04-19 21:18:25.000000 duckietown-shell-6.0.4/duckietown_shell.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5787 2024-04-19 21:18:25.000000 duckietown-shell-6.0.4/duckietown_shell.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2024-04-19 21:18:25.000000 duckietown-shell-6.0.4/duckietown_shell.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       45 2024-04-19 21:18:25.000000 duckietown-shell-6.0.4/duckietown_shell.egg-info/entry_points.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-09-27 20:34:45.000000 duckietown-shell-6.0.4/duckietown_shell.egg-info/not-zip-safe
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      259 2024-04-19 21:18:25.000000 duckietown-shell-6.0.4/duckietown_shell.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2024-04-19 21:18:25.000000 duckietown-shell-6.0.4/duckietown_shell.egg-info/top_level.txt
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.482242 duckietown-shell-6.0.4/lib/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.486242 duckietown-shell-6.0.4/lib/dt_shell/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1143 2024-04-19 21:18:21.000000 duckietown-shell-6.0.4/lib/dt_shell/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.486242 duckietown-shell-6.0.4/lib/dt_shell/assets/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      145 2023-11-09 03:05:44.000000 duckietown-shell-6.0.4/lib/dt_shell/assets/dts-completion.bash
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)  2605506 2023-09-27 20:00:04.000000 duckietown-shell-6.0.4/lib/dt_shell/assets/get-pip.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      241 2024-04-19 21:18:25.000000 duckietown-shell-6.0.4/lib/dt_shell/assets/requirements.txt
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.486242 duckietown-shell-6.0.4/lib/dt_shell/checks/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-08-30 15:12:15.000000 duckietown-shell-6.0.4/lib/dt_shell/checks/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2731 2023-11-09 04:14:27.000000 duckietown-shell-6.0.4/lib/dt_shell/checks/environment.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2431 2023-08-30 15:22:10.000000 duckietown-shell-6.0.4/lib/dt_shell/checks/packages.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4081 2023-10-06 06:56:43.000000 duckietown-shell-6.0.4/lib/dt_shell/checks/version.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.490242 duckietown-shell-6.0.4/lib/dt_shell/commands/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      314 2023-09-28 15:48:57.000000 duckietown-shell-6.0.4/lib/dt_shell/commands/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1744 2023-11-09 03:07:56.000000 duckietown-shell-6.0.4/lib/dt_shell/commands/autocomplete.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    22097 2024-01-12 06:05:30.000000 duckietown-shell-6.0.4/lib/dt_shell/commands/commands.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6891 2024-01-12 06:09:42.000000 duckietown-shell-6.0.4/lib/dt_shell/commands/importer.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3832 2023-11-19 07:06:12.000000 duckietown-shell-6.0.4/lib/dt_shell/commands/repository.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.490242 duckietown-shell-6.0.4/lib/dt_shell/compatibility/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1703 2024-01-07 23:52:54.000000 duckietown-shell-6.0.4/lib/dt_shell/compatibility/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      253 2023-09-30 02:55:23.000000 duckietown-shell-6.0.4/lib/dt_shell/compatibility/commands_.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1394 2024-02-25 15:04:23.000000 duckietown-shell-6.0.4/lib/dt_shell/compatibility/config.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      120 2023-08-30 20:27:08.000000 duckietown-shell-6.0.4/lib/dt_shell/compatibility/duckietown_tokens.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      753 2023-10-14 03:04:10.000000 duckietown-shell-6.0.4/lib/dt_shell/compatibility/env_checks.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.490242 duckietown-shell-6.0.4/lib/dt_shell/compatibility/migrations/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       26 2023-10-05 05:02:57.000000 duckietown-shell-6.0.4/lib/dt_shell/compatibility/migrations/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4545 2023-11-02 04:51:34.000000 duckietown-shell-6.0.4/lib/dt_shell/compatibility/migrations/migrations.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      820 2023-10-06 06:20:59.000000 duckietown-shell-6.0.4/lib/dt_shell/compatibility/tokens_cli.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      179 2023-08-30 15:56:05.000000 duckietown-shell-6.0.4/lib/dt_shell/compatibility/version_check.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3559 2024-03-19 04:43:27.000000 duckietown-shell-6.0.4/lib/dt_shell/constants.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.490242 duckietown-shell-6.0.4/lib/dt_shell/database/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-09-28 15:30:42.000000 duckietown-shell-6.0.4/lib/dt_shell/database/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7316 2024-02-22 22:50:09.000000 duckietown-shell-6.0.4/lib/dt_shell/database/database.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2046 2023-12-17 15:44:08.000000 duckietown-shell-6.0.4/lib/dt_shell/database/utils.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.482242 duckietown-shell-6.0.4/lib/dt_shell/embedded/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.490242 duckietown-shell-6.0.4/lib/dt_shell/embedded/__command_set__/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.490242 duckietown-shell-6.0.4/lib/dt_shell/embedded/__command_set__/__pycache__/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1833 2023-10-14 02:59:39.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/__command_set__/__pycache__/configuration.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      209 2023-10-14 02:59:43.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/__command_set__/__pycache__/init.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1241 2023-10-14 00:54:41.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/__command_set__/configuration.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       21 2023-10-14 00:54:41.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/__command_set__/init.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2023-10-14 02:59:36.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/__command_set__/requirements.txt
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.490242 duckietown-shell-6.0.4/lib/dt_shell/embedded/commands/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      519 2023-04-19 19:49:53.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/commands/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.490242 duckietown-shell-6.0.4/lib/dt_shell/embedded/commands/__pycache__/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      642 2023-09-29 23:50:53.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/commands/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1205 2023-11-19 06:38:19.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/commands/__pycache__/command.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      875 2023-11-19 06:26:16.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/commands/command.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.490242 duckietown-shell-6.0.4/lib/dt_shell/embedded/exit/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-08-31 04:56:47.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/exit/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.490242 duckietown-shell-6.0.4/lib/dt_shell/embedded/exit/__pycache__/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      202 2023-09-29 23:50:53.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/exit/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      678 2023-11-19 06:38:19.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/exit/__pycache__/command.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1149 2023-10-06 05:21:17.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/exit/__pycache__/configuration.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      211 2023-11-19 06:26:16.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/exit/command.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      553 2023-10-06 05:20:21.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/exit/configuration.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.490242 duckietown-shell-6.0.4/lib/dt_shell/embedded/install/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-09-30 02:45:11.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/install/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.490242 duckietown-shell-6.0.4/lib/dt_shell/embedded/install/__pycache__/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      205 2023-09-30 03:34:33.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/install/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      865 2023-11-19 06:38:19.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/install/__pycache__/command.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      387 2023-11-19 06:26:16.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/install/command.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.494242 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-10-21 21:19:31.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.494242 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/__pycache__/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      205 2023-10-21 21:19:34.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      812 2023-10-13 15:25:39.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/__pycache__/configuration.cpython-310.pyc
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.494242 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/dependencies/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-10-10 18:22:39.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/dependencies/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.494242 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/dependencies/__pycache__/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      218 2023-10-13 15:25:39.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/dependencies/__pycache__/__init__.cpython-310.pyc
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.494242 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/dependencies/reinstall/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-10-10 18:22:39.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/dependencies/reinstall/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1027 2023-11-19 06:26:16.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/dependencies/reinstall/command.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      336 2023-10-10 18:22:39.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/dependencies/reinstall/configuration.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.494242 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/list/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-10-14 02:59:36.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/list/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.494242 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/list/__pycache__/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      210 2023-10-14 02:59:39.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/list/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1562 2023-11-19 06:38:19.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/list/__pycache__/command.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      914 2023-10-14 02:59:39.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/list/__pycache__/configuration.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1492 2023-11-19 06:33:54.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/list/command.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      431 2023-10-14 02:59:36.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/list/configuration.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.494242 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/new/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-10-14 02:59:36.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/new/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.494242 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/new/__pycache__/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      209 2023-10-14 02:59:39.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/new/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2656 2024-04-19 21:15:25.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/new/__pycache__/command.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1064 2024-03-19 17:30:11.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/new/__pycache__/configuration.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3341 2024-04-19 21:16:24.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/new/command.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      639 2024-03-19 04:43:27.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/new/configuration.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.494242 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/switch/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-10-14 02:59:36.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/switch/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.494242 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/switch/__pycache__/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      212 2023-10-14 02:59:39.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/switch/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1866 2023-11-19 06:38:19.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/switch/__pycache__/command.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1014 2023-10-14 02:59:39.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/switch/__pycache__/configuration.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2207 2023-11-19 06:26:16.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/switch/command.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      532 2023-10-14 02:59:36.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/switch/configuration.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.494242 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-11-05 21:59:38.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.494242 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/__pycache__/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      201 2023-11-09 03:51:02.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      666 2023-11-09 03:51:41.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/__pycache__/configuration.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      218 2023-11-09 03:51:38.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/configuration.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.494242 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/set/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-11-05 21:59:38.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/set/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.494242 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/set/__pycache__/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      205 2023-11-09 04:56:06.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/set/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2199 2023-11-19 06:38:19.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/set/__pycache__/command.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2006 2023-11-19 06:26:16.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/set/command.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.494242 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/status/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-11-05 21:59:38.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/status/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.494242 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/status/__pycache__/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      208 2023-11-09 04:56:06.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/status/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      847 2023-11-19 06:38:19.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/status/__pycache__/command.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      409 2023-11-19 06:26:16.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/status/command.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.494242 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/verify/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-11-05 21:59:38.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/verify/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.494242 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/verify/__pycache__/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      208 2023-11-09 04:56:06.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/verify/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1326 2023-11-19 06:38:19.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/verify/__pycache__/command.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1028 2023-11-19 06:26:16.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/verify/command.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.498242 duckietown-shell-6.0.4/lib/dt_shell/embedded/uninstall/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-09-30 02:45:13.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/uninstall/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.498242 duckietown-shell-6.0.4/lib/dt_shell/embedded/uninstall/__pycache__/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      207 2023-09-30 03:34:33.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/uninstall/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      865 2023-11-19 06:38:19.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/uninstall/__pycache__/command.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      383 2023-11-19 06:26:16.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/uninstall/command.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.498242 duckietown-shell-6.0.4/lib/dt_shell/embedded/update/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-10-14 00:54:41.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/update/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.498242 duckietown-shell-6.0.4/lib/dt_shell/embedded/update/__pycache__/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      204 2023-10-14 02:59:43.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/update/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      770 2023-12-18 21:39:22.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/update/__pycache__/command.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      393 2023-12-18 21:39:12.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/update/command.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.498242 duckietown-shell-6.0.4/lib/dt_shell/embedded/version/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       69 2023-04-19 19:49:53.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/version/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.498242 duckietown-shell-6.0.4/lib/dt_shell/embedded/version/__pycache__/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      246 2023-09-29 23:50:53.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/version/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1127 2023-11-19 06:38:19.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/version/__pycache__/command.cpython-310.pyc
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1174 2023-11-19 06:26:16.000000 duckietown-shell-6.0.4/lib/dt_shell/embedded/version/command.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7557 2023-11-20 17:33:23.000000 duckietown-shell-6.0.4/lib/dt_shell/environments.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2662 2023-10-14 02:59:36.000000 duckietown-shell-6.0.4/lib/dt_shell/exceptions.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2487 2024-02-05 05:10:23.000000 duckietown-shell-6.0.4/lib/dt_shell/hub.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1756 2024-03-12 20:20:31.000000 duckietown-shell-6.0.4/lib/dt_shell/logging.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    17337 2024-03-19 04:43:27.000000 duckietown-shell-6.0.4/lib/dt_shell/profile.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    34688 2024-04-19 00:44:32.000000 duckietown-shell-6.0.4/lib/dt_shell/shell.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1976 2024-02-21 21:27:34.000000 duckietown-shell-6.0.4/lib/dt_shell/statistics.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6765 2023-11-19 07:00:22.000000 duckietown-shell-6.0.4/lib/dt_shell/tasks.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      194 2023-11-19 06:28:00.000000 duckietown-shell-6.0.4/lib/dt_shell/typing.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    10749 2024-04-15 05:35:34.000000 duckietown-shell-6.0.4/lib/dt_shell/utils.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-19 21:18:25.498242 duckietown-shell-6.0.4/lib/dt_shell_cli/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      218 2024-02-25 15:04:23.000000 duckietown-shell-6.0.4/lib/dt_shell_cli/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     8501 2024-01-27 02:23:56.000000 duckietown-shell-6.0.4/lib/dt_shell_cli/dts.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1971 2024-01-19 21:30:29.000000 duckietown-shell-6.0.4/lib/dt_shell_cli/main.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2024-04-19 21:18:25.498242 duckietown-shell-6.0.4/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3017 2024-03-19 04:24:17.000000 duckietown-shell-6.0.4/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.916978 duckietown-shell-6.0.5/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    75933 2023-03-22 21:05:31.000000 duckietown-shell-6.0.5/LICENSE.pdf
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      599 2024-04-25 05:41:59.916978 duckietown-shell-6.0.5/PKG-INFO
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.916978 duckietown-shell-6.0.5/duckietown_shell.egg-info/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      599 2024-04-25 05:41:59.000000 duckietown-shell-6.0.5/duckietown_shell.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3347 2024-04-25 05:41:59.000000 duckietown-shell-6.0.5/duckietown_shell.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2024-04-25 05:41:59.000000 duckietown-shell-6.0.5/duckietown_shell.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       45 2024-04-25 05:41:59.000000 duckietown-shell-6.0.5/duckietown_shell.egg-info/entry_points.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2024-03-20 14:56:50.000000 duckietown-shell-6.0.5/duckietown_shell.egg-info/not-zip-safe
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      259 2024-04-25 05:41:59.000000 duckietown-shell-6.0.5/duckietown_shell.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2024-04-25 05:41:59.000000 duckietown-shell-6.0.5/duckietown_shell.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.904977 duckietown-shell-6.0.5/lib/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.908978 duckietown-shell-6.0.5/lib/dt_shell/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1143 2024-04-25 05:41:57.000000 duckietown-shell-6.0.5/lib/dt_shell/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.908978 duckietown-shell-6.0.5/lib/dt_shell/assets/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      145 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/assets/dts-completion.bash
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)  2605506 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/assets/get-pip.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      241 2024-04-25 05:41:59.000000 duckietown-shell-6.0.5/lib/dt_shell/assets/requirements.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.908978 duckietown-shell-6.0.5/lib/dt_shell/checks/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/checks/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2731 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/checks/environment.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2431 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/checks/packages.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4081 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/checks/version.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.908978 duckietown-shell-6.0.5/lib/dt_shell/commands/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      314 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/commands/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1744 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/commands/autocomplete.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    22097 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/commands/commands.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6891 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/commands/importer.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3832 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/commands/repository.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.912978 duckietown-shell-6.0.5/lib/dt_shell/compatibility/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1703 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/compatibility/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      253 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/compatibility/commands_.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1394 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/compatibility/config.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      120 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/compatibility/duckietown_tokens.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      753 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/compatibility/env_checks.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.912978 duckietown-shell-6.0.5/lib/dt_shell/compatibility/migrations/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       26 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/compatibility/migrations/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4545 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/compatibility/migrations/migrations.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      820 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/compatibility/tokens_cli.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      186 2024-04-25 05:40:03.000000 duckietown-shell-6.0.5/lib/dt_shell/compatibility/version_check.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3559 2024-03-20 14:43:29.000000 duckietown-shell-6.0.5/lib/dt_shell/constants.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.912978 duckietown-shell-6.0.5/lib/dt_shell/database/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/database/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7316 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/database/database.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2046 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/database/utils.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.904977 duckietown-shell-6.0.5/lib/dt_shell/embedded/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.912978 duckietown-shell-6.0.5/lib/dt_shell/embedded/__command_set__/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1241 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/__command_set__/configuration.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       21 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/__command_set__/init.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/__command_set__/requirements.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.912978 duckietown-shell-6.0.5/lib/dt_shell/embedded/commands/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      519 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/commands/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      875 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/commands/command.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.912978 duckietown-shell-6.0.5/lib/dt_shell/embedded/exit/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/exit/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      211 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/exit/command.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      553 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/exit/configuration.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.912978 duckietown-shell-6.0.5/lib/dt_shell/embedded/install/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/install/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      387 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/install/command.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.912978 duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.912978 duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/dependencies/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/dependencies/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.912978 duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/dependencies/reinstall/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/dependencies/reinstall/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1027 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/dependencies/reinstall/command.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      336 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/dependencies/reinstall/configuration.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.912978 duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/list/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/list/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1492 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/list/command.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      431 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/list/configuration.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.912978 duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/new/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/new/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3341 2024-04-25 05:40:49.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/new/command.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      639 2024-03-20 14:43:29.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/new/configuration.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.912978 duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/switch/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/switch/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2207 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/switch/command.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      532 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/switch/configuration.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.912978 duckietown-shell-6.0.5/lib/dt_shell/embedded/tok/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/tok/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      218 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/tok/configuration.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.912978 duckietown-shell-6.0.5/lib/dt_shell/embedded/tok/set/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/tok/set/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2006 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/tok/set/command.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.912978 duckietown-shell-6.0.5/lib/dt_shell/embedded/tok/status/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/tok/status/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      409 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/tok/status/command.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.912978 duckietown-shell-6.0.5/lib/dt_shell/embedded/tok/verify/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/tok/verify/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1028 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/tok/verify/command.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.912978 duckietown-shell-6.0.5/lib/dt_shell/embedded/uninstall/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/uninstall/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      383 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/uninstall/command.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.912978 duckietown-shell-6.0.5/lib/dt_shell/embedded/update/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/update/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      393 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/update/command.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.912978 duckietown-shell-6.0.5/lib/dt_shell/embedded/version/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       69 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/version/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1174 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/embedded/version/command.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7557 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/environments.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2662 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/exceptions.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2487 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/hub.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1756 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/logging.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    17337 2024-03-20 14:43:29.000000 duckietown-shell-6.0.5/lib/dt_shell/profile.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    34688 2024-04-17 19:24:14.000000 duckietown-shell-6.0.5/lib/dt_shell/shell.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1976 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/statistics.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6765 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/tasks.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      194 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell/typing.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    10749 2024-03-20 14:56:28.000000 duckietown-shell-6.0.5/lib/dt_shell/utils.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-25 05:41:59.916978 duckietown-shell-6.0.5/lib/dt_shell_cli/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      218 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell_cli/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     8501 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell_cli/dts.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1971 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/lib/dt_shell_cli/main.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2024-04-25 05:41:59.916978 duckietown-shell-6.0.5/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3017 2024-03-13 05:31:54.000000 duckietown-shell-6.0.5/setup.py
```

### Comparing `duckietown-shell-6.0.4/LICENSE.pdf` & `duckietown-shell-6.0.5/LICENSE.pdf`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/PKG-INFO` & `duckietown-shell-6.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: duckietown-shell
-Version: 6.0.4
-Download-URL: http://github.com/duckietown/duckietown-shell/tarball/6.0.4
+Version: 6.0.5
+Download-URL: http://github.com/duckietown/duckietown-shell/tarball/6.0.5
 License-File: LICENSE.pdf
 Requires-Dist: termcolor<3,>=2.3.0
 Requires-Dist: requests<3,>=2.31.0
 Requires-Dist: pyyaml!=5.4.0,!=5.4.1,!=6.0.0,<7
 Requires-Dist: pyfiglet<1,>=0.8.0
 Requires-Dist: questionary<3,>=2.0.1
 Requires-Dist: argcomplete<4,>=3.1.4
```

### Comparing `duckietown-shell-6.0.4/duckietown_shell.egg-info/PKG-INFO` & `duckietown-shell-6.0.5/duckietown_shell.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: duckietown-shell
-Version: 6.0.4
-Download-URL: http://github.com/duckietown/duckietown-shell/tarball/6.0.4
+Version: 6.0.5
+Download-URL: http://github.com/duckietown/duckietown-shell/tarball/6.0.5
 License-File: LICENSE.pdf
 Requires-Dist: termcolor<3,>=2.3.0
 Requires-Dist: requests<3,>=2.31.0
 Requires-Dist: pyyaml!=5.4.0,!=5.4.1,!=6.0.0,<7
 Requires-Dist: pyfiglet<1,>=0.8.0
 Requires-Dist: questionary<3,>=2.0.1
 Requires-Dist: argcomplete<4,>=3.1.4
```

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/__init__.py` & `duckietown-shell-6.0.5/lib/dt_shell/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from dt_shell_cli import logger
 
 # logger dedicated to the commands
 dtslogger = logging.getLogger("dts")
 dtslogger.setLevel(logging.INFO)
 
-__version__ = "6.0.4"
+__version__ = "6.0.5"
 
 import sys
 
 if sys.version_info < (3, 6):
     msg = f"! duckietown-shell works with Python 3.6 and later !.\nDetected {sys.version}."
     logger.error(msg)
     sys.exit(2)
```

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/assets/get-pip.py` & `duckietown-shell-6.0.5/lib/dt_shell/assets/get-pip.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/checks/environment.py` & `duckietown-shell-6.0.5/lib/dt_shell/checks/environment.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/checks/packages.py` & `duckietown-shell-6.0.5/lib/dt_shell/checks/packages.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/checks/version.py` & `duckietown-shell-6.0.5/lib/dt_shell/checks/version.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/commands/autocomplete.py` & `duckietown-shell-6.0.5/lib/dt_shell/commands/autocomplete.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/commands/commands.py` & `duckietown-shell-6.0.5/lib/dt_shell/commands/commands.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/commands/importer.py` & `duckietown-shell-6.0.5/lib/dt_shell/commands/importer.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/commands/repository.py` & `duckietown-shell-6.0.5/lib/dt_shell/commands/repository.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/compatibility/__init__.py` & `duckietown-shell-6.0.5/lib/dt_shell/compatibility/__init__.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/compatibility/config.py` & `duckietown-shell-6.0.5/lib/dt_shell/compatibility/config.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/compatibility/env_checks.py` & `duckietown-shell-6.0.5/lib/dt_shell/compatibility/env_checks.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/compatibility/migrations/migrations.py` & `duckietown-shell-6.0.5/lib/dt_shell/compatibility/migrations/migrations.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/compatibility/tokens_cli.py` & `duckietown-shell-6.0.5/lib/dt_shell/compatibility/tokens_cli.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/constants.py` & `duckietown-shell-6.0.5/lib/dt_shell/constants.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/database/database.py` & `duckietown-shell-6.0.5/lib/dt_shell/database/database.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/database/utils.py` & `duckietown-shell-6.0.5/lib/dt_shell/database/utils.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/embedded/__command_set__/configuration.py` & `duckietown-shell-6.0.5/lib/dt_shell/embedded/__command_set__/configuration.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/embedded/commands/__init__.py` & `duckietown-shell-6.0.5/lib/dt_shell/embedded/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/embedded/commands/command.py` & `duckietown-shell-6.0.5/lib/dt_shell/embedded/commands/command.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/embedded/exit/configuration.py` & `duckietown-shell-6.0.5/lib/dt_shell/embedded/exit/configuration.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/dependencies/reinstall/command.py` & `duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/dependencies/reinstall/command.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/list/command.py` & `duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/list/command.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/new/command.py` & `duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/new/command.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/new/configuration.py` & `duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/new/configuration.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/switch/command.py` & `duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/switch/command.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/embedded/profile/switch/configuration.py` & `duckietown-shell-6.0.5/lib/dt_shell/embedded/profile/switch/configuration.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/set/command.py` & `duckietown-shell-6.0.5/lib/dt_shell/embedded/tok/set/command.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/embedded/tok/verify/command.py` & `duckietown-shell-6.0.5/lib/dt_shell/embedded/tok/verify/command.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/embedded/version/command.py` & `duckietown-shell-6.0.5/lib/dt_shell/embedded/version/command.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/environments.py` & `duckietown-shell-6.0.5/lib/dt_shell/environments.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/exceptions.py` & `duckietown-shell-6.0.5/lib/dt_shell/exceptions.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/hub.py` & `duckietown-shell-6.0.5/lib/dt_shell/hub.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/logging.py` & `duckietown-shell-6.0.5/lib/dt_shell/logging.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/profile.py` & `duckietown-shell-6.0.5/lib/dt_shell/profile.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/shell.py` & `duckietown-shell-6.0.5/lib/dt_shell/shell.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/statistics.py` & `duckietown-shell-6.0.5/lib/dt_shell/statistics.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/tasks.py` & `duckietown-shell-6.0.5/lib/dt_shell/tasks.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell/utils.py` & `duckietown-shell-6.0.5/lib/dt_shell/utils.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell_cli/dts.py` & `duckietown-shell-6.0.5/lib/dt_shell_cli/dts.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/lib/dt_shell_cli/main.py` & `duckietown-shell-6.0.5/lib/dt_shell_cli/main.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-6.0.4/setup.py` & `duckietown-shell-6.0.5/setup.py`

 * *Files identical despite different names*


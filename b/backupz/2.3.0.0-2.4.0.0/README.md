# Comparing `tmp/backupz-2.3.0.0.tar.gz` & `tmp/backupz-2.4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backupz-2.3.0.0.tar", last modified: Sun Mar 24 11:33:45 2024, max compression
+gzip compressed data, was "backupz-2.4.0.0.tar", last modified: Thu Apr 25 16:48:51 2024, max compression
```

## Comparing `backupz-2.3.0.0.tar` & `backupz-2.4.0.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-24 11:33:45.905895 backupz-2.3.0.0/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)    11358 2024-03-16 15:01:43.000000 backupz-2.3.0.0/LICENSE
--rw-r--r--   0 keygenqt  (1000) keygenqt  (1000)     1404 2024-03-24 11:33:45.905895 backupz-2.3.0.0/PKG-INFO
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1140 2024-03-16 15:01:43.000000 backupz-2.3.0.0/README.md
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-24 11:33:45.901895 backupz-2.3.0.0/backupz/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:01:43.000000 backupz-2.3.0.0/backupz/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1681 2024-03-24 11:25:34.000000 backupz-2.3.0.0/backupz/__main__.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-24 11:33:45.901895 backupz-2.3.0.0/backupz/src/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:01:43.000000 backupz-2.3.0.0/backupz/src/__init__.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-24 11:33:45.901895 backupz-2.3.0.0/backupz/src/features/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:01:43.000000 backupz-2.3.0.0/backupz/src/features/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     5298 2024-03-24 11:29:47.000000 backupz-2.3.0.0/backupz/src/features/group_make.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-24 11:33:45.901895 backupz-2.3.0.0/backupz/src/features/impl/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-22 20:45:22.000000 backupz-2.3.0.0/backupz/src/features/impl/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4660 2024-03-24 11:25:34.000000 backupz-2.3.0.0/backupz/src/features/impl/utils.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-24 11:33:45.905895 backupz-2.3.0.0/backupz/src/support/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:01:43.000000 backupz-2.3.0.0/backupz/src/support/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     9279 2024-03-24 11:26:14.000000 backupz-2.3.0.0/backupz/src/support/conf.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-24 11:33:45.905895 backupz-2.3.0.0/backupz/src/support/data/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-21 17:21:31.000000 backupz-2.3.0.0/backupz/src/support/data/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2542 2024-03-21 17:21:31.000000 backupz-2.3.0.0/backupz/src/support/data/data_ftp.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2816 2024-03-21 17:21:31.000000 backupz-2.3.0.0/backupz/src/support/data/data_ssh.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1969 2024-03-24 11:29:13.000000 backupz-2.3.0.0/backupz/src/support/dependency.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3421 2024-03-22 20:45:22.000000 backupz-2.3.0.0/backupz/src/support/download.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2777 2024-03-22 20:45:22.000000 backupz-2.3.0.0/backupz/src/support/helper.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1784 2024-03-16 15:01:43.000000 backupz-2.3.0.0/backupz/src/support/output.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2441 2024-03-24 11:25:34.000000 backupz-2.3.0.0/backupz/src/support/progress_alive_bar.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2659 2024-03-22 20:45:22.000000 backupz-2.3.0.0/backupz/src/support/progress_alive_bar_git.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3929 2024-03-24 11:28:41.000000 backupz-2.3.0.0/backupz/src/support/texts.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-24 11:33:45.905895 backupz-2.3.0.0/backupz.egg-info/
--rw-r--r--   0 keygenqt  (1000) keygenqt  (1000)     1404 2024-03-24 11:33:45.000000 backupz-2.3.0.0/backupz.egg-info/PKG-INFO
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)      833 2024-03-24 11:33:45.000000 backupz-2.3.0.0/backupz.egg-info/SOURCES.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        1 2024-03-24 11:33:45.000000 backupz-2.3.0.0/backupz.egg-info/dependency_links.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       50 2024-03-24 11:33:45.000000 backupz-2.3.0.0/backupz.egg-info/entry_points.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)      151 2024-03-24 11:33:45.000000 backupz-2.3.0.0/backupz.egg-info/requires.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       15 2024-03-24 11:33:45.000000 backupz-2.3.0.0/backupz.egg-info/top_level.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       38 2024-03-24 11:33:45.905895 backupz-2.3.0.0/setup.cfg
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1733 2024-03-24 11:26:02.000000 backupz-2.3.0.0/setup.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-25 16:48:51.729232 backupz-2.4.0.0/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)    11358 2024-03-16 15:01:43.000000 backupz-2.4.0.0/LICENSE
+-rw-r--r--   0 keygenqt  (1000) keygenqt  (1000)     1549 2024-04-25 16:48:51.729232 backupz-2.4.0.0/PKG-INFO
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1253 2024-04-25 16:43:04.000000 backupz-2.4.0.0/README.md
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-25 16:48:51.725232 backupz-2.4.0.0/backupz/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:01:43.000000 backupz-2.4.0.0/backupz/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1681 2024-03-24 11:25:34.000000 backupz-2.4.0.0/backupz/__main__.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-25 16:48:51.725232 backupz-2.4.0.0/backupz/src/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:01:43.000000 backupz-2.4.0.0/backupz/src/__init__.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-25 16:48:51.725232 backupz-2.4.0.0/backupz/src/features/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:01:43.000000 backupz-2.4.0.0/backupz/src/features/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     5967 2024-04-25 16:43:04.000000 backupz-2.4.0.0/backupz/src/features/group_make.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-25 16:48:51.725232 backupz-2.4.0.0/backupz/src/features/impl/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-22 20:45:22.000000 backupz-2.4.0.0/backupz/src/features/impl/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4621 2024-04-25 16:43:04.000000 backupz-2.4.0.0/backupz/src/features/impl/utils.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-25 16:48:51.729232 backupz-2.4.0.0/backupz/src/support/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:01:43.000000 backupz-2.4.0.0/backupz/src/support/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)    10872 2024-04-25 16:43:04.000000 backupz-2.4.0.0/backupz/src/support/conf.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-25 16:48:51.729232 backupz-2.4.0.0/backupz/src/support/data/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-21 17:21:31.000000 backupz-2.4.0.0/backupz/src/support/data/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2542 2024-03-21 17:21:31.000000 backupz-2.4.0.0/backupz/src/support/data/data_ftp.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2816 2024-03-21 17:21:31.000000 backupz-2.4.0.0/backupz/src/support/data/data_ssh.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3738 2024-04-25 16:43:04.000000 backupz-2.4.0.0/backupz/src/support/data/data_telegram.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1969 2024-03-26 15:26:00.000000 backupz-2.4.0.0/backupz/src/support/dependency.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3421 2024-03-22 20:45:22.000000 backupz-2.4.0.0/backupz/src/support/download.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2307 2024-04-25 16:43:04.000000 backupz-2.4.0.0/backupz/src/support/helper.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1784 2024-03-16 15:01:43.000000 backupz-2.4.0.0/backupz/src/support/output.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2441 2024-03-24 11:25:34.000000 backupz-2.4.0.0/backupz/src/support/progress_alive_bar.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2659 2024-03-22 20:45:22.000000 backupz-2.4.0.0/backupz/src/support/progress_alive_bar_git.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4357 2024-04-25 16:43:04.000000 backupz-2.4.0.0/backupz/src/support/texts.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-25 16:48:51.729232 backupz-2.4.0.0/backupz.egg-info/
+-rw-r--r--   0 keygenqt  (1000) keygenqt  (1000)     1549 2024-04-25 16:48:51.000000 backupz-2.4.0.0/backupz.egg-info/PKG-INFO
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)      875 2024-04-25 16:48:51.000000 backupz-2.4.0.0/backupz.egg-info/SOURCES.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        1 2024-04-25 16:48:51.000000 backupz-2.4.0.0/backupz.egg-info/dependency_links.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       50 2024-04-25 16:48:51.000000 backupz-2.4.0.0/backupz.egg-info/entry_points.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)      168 2024-04-25 16:48:51.000000 backupz-2.4.0.0/backupz.egg-info/requires.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       15 2024-04-25 16:48:51.000000 backupz-2.4.0.0/backupz.egg-info/top_level.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       38 2024-04-25 16:48:51.729232 backupz-2.4.0.0/setup.cfg
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1874 2024-04-25 16:43:04.000000 backupz-2.4.0.0/setup.py
```

### Comparing `backupz-2.3.0.0/LICENSE` & `backupz-2.4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `backupz-2.3.0.0/PKG-INFO` & `backupz-2.4.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backupz
-Version: 2.3.0.0
+Version: 2.4.0.0
 Summary: The application allows you to generate CHANGELOG files based on Git tags.
 Home-page: https://github.com/keygenqt/backupz
 Author: Vitaliy Zarubin
 Author-email: keygenqt@gmail.com
 Requires-Python: >=3.8.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,20 +13,30 @@
 Requires-Dist: cffi>=1.16.0
 Requires-Dist: beautifulsoup4>=4.12.3
 Requires-Dist: alive-progress>=3.1.5
 Requires-Dist: paramiko>=3.4.0
 Requires-Dist: GitPython>=3.1.41
 Requires-Dist: requests>=2.31.0
 Requires-Dist: pytube>=15.0.0
+Requires-Dist: Telethon>=1.34.0
 
 
 ![picture](https://github.com/keygenqt/backupz/blob/main/data/banners/banner_round_grey.png?raw=true)
 
 Create and save a backup archive in multiple processes.
 
+#### Can make backups from:
+
+- GitHub
+- YouTube
+- Telegram
+- Database
+- Folders/Files
+- Files from direct links
+
 [More...](https://keygenqt.github.io/backupz)
 
 ### License
 
 ```
 Copyright 2021-2024 Vitaliy Zarubin
```

### Comparing `backupz-2.3.0.0/README.md` & `backupz-2.4.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,23 @@
 
 [![PyPI version](https://badge.fury.io/py/backupz.svg?v=1)](https://badge.fury.io/py/backupz)
 
 ![picture](https://github.com/keygenqt/backupz/blob/main/data/banners/banner_round_grey.png?raw=true)
 
 Create and save a backup archive in multiple processes.
 
+#### Can make backups from:
+
+- GitHub
+- YouTube
+- Telegram
+- Database
+- Folders/Files
+- Files from direct links
+
 #### Documentation:
 <p>
     <a href="https://keygenqt.github.io/backupz">
         <img src="data/other/see_more.gif" width="136px"/>
     </a>
 </p>
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 Backupz =================== ### Subscribe and like! [https://github.com/
 keygenqt/backupz/blob/main/data/other/star.gif?raw=true][![PyPI version](https:
 //badge.fury.io/py/backupz.svg?v=1)](https://badge.fury.io/py/backupz) !
 [picture](https://github.com/keygenqt/backupz/blob/main/data/banners/
 banner_round_grey.png?raw=true) Create and save a backup archive in multiple
-processes. #### Documentation:
+processes. #### Can make backups from: - GitHub - YouTube - Telegram - Database
+- Folders/Files - Files from direct links #### Documentation:
 _[_d_a_t_a_/_o_t_h_e_r_/_s_e_e___m_o_r_e_._g_i_f_]
 ### License ``` Copyright 2021-2024 Vitaliy Zarubin Licensed under the Apache
 License, Version 2.0 (the "License"); you may not use this file except in
 compliance with the License. You may obtain a copy of the License at http://
 www.apache.org/licenses/LICENSE-2.0 Unless required by applicable law or agreed
 to in writing, software distributed under the License is distributed on an "AS
 IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
```

### Comparing `backupz-2.3.0.0/backupz/__main__.py` & `backupz-2.4.0.0/backupz/__main__.py`

 * *Files identical despite different names*

### Comparing `backupz-2.3.0.0/backupz/src/features/group_make.py` & `backupz-2.4.0.0/backupz/src/features/group_make.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 import multiprocessing
 import shutil
 
 from backupz.src.features.impl.utils import git_clone, get_size_blocks, downloads, youtube_download
 from backupz.src.support.conf import Conf
 from backupz.src.support.dependency import check_dependency_git, check_dependency_ffmpeg
-from backupz.src.support.helper import get_path_folder, get_path_file, pc_command, get_download_folder
+from backupz.src.support.helper import get_path_folder, get_path_file, pc_command
 from backupz.src.support.output import echo_stderr, echo_stdout
 from backupz.src.support.progress_alive_bar import ProgressAliveBar
 from backupz.src.support.texts import AppTexts
 
 
 # Create archive with backup
 def group_make(config: Conf, is_delete_temp: bool):
@@ -34,25 +34,33 @@
         import subprocess
         try:
             subprocess.run(command, check=True, shell=True, capture_output=True)
         except subprocess.CalledProcessError as e:
             echo_stderr(AppTexts.error_exception(str(e)))
             exit(1)
 
+    # Download folder
+    download_folder = config.get_download_folder()
+
     # Exclude files by regex
     excludes = ['--exclude={}'.format(exclude) for exclude in config.get_exclude()]
 
     gits = []
     urls = []
+    telegram_urls = []
     youtube = []
     files = []
     folders = []
 
     # Parse backup file and folder from config
     for item in config.get_backup_paths():
+        # Check is link Telegram
+        if 't.me' in item:
+            telegram_urls.append(item)
+            continue
         # Check is link YouTube
         if 'youtu.be' in item or 'youtube.com' in item:
             check_dependency_ffmpeg()
             youtube.append(item)
             continue
         # Check is git repos
         if '.git' in item and ('git@' in item or 'https' in item):
@@ -72,34 +80,47 @@
         path = get_path_folder(item)
         if path:
             folders.append(str(path))
             continue
         echo_stderr(AppTexts.error_found_path(item))
         exit(1)
 
+    # Run save posts
+    if telegram_urls and not config.get_telegram():
+        echo_stderr(AppTexts.error_telegram_configuration())
+        exit(1)
+
+    for url in telegram_urls:
+        for path in config.get_telegram().get_posts(url, download_folder):
+            if not path:
+                echo_stderr(AppTexts.error_telegram_get_posts(url))
+                exit(1)
+            else:
+                folders.append(str(path))
+
     # Run clone repos
     for item in gits:
-        path = git_clone(item)
+        path = git_clone(download_folder, item)
         if not path:
             echo_stderr(AppTexts.error_clone_project(item))
             exit(1)
         else:
             folders.append(str(path))
 
     # Run download video youtube
     for item in youtube:
-        path = youtube_download(item)
+        path = youtube_download(download_folder, item)
         if not path:
             echo_stderr(AppTexts.error_download(item))
             exit(1)
         else:
             files.append(str(path))
 
     # Run multi downloads
-    files = files + downloads(urls)
+    files = files + downloads(download_folder, urls)
 
     if not files and not folders:
         echo_stderr(AppTexts.error_empty_data())
         exit(1)
 
     echo_stdout(AppTexts.info_counting())
 
@@ -150,12 +171,12 @@
 
     # Upload to ftp
     for ftp in config.get_data_ftp():
         ftp.upload(config.get_path_to_save())
 
     # Info abot cache
     if not is_delete_temp and (gits or urls):
-        echo_stdout(AppTexts.info_after_clone(str(get_download_folder())))
+        echo_stdout(AppTexts.info_after_clone(str(download_folder)))
 
     # Delete files if need
     if is_delete_temp:
-        shutil.rmtree(get_download_folder(), ignore_errors=True)
+        shutil.rmtree(download_folder, ignore_errors=True)
```

### Comparing `backupz-2.3.0.0/backupz/src/features/impl/utils.py` & `backupz-2.4.0.0/backupz/src/features/impl/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,43 +17,43 @@
 from pathlib import Path
 
 import requests
 from git import Repo
 from pytube import YouTube, extract
 
 from backupz.src.support.download import multi_download
-from backupz.src.support.helper import get_download_folder, pc_command
+from backupz.src.support.helper import pc_command
 from backupz.src.support.output import echo_stderr, echo_stdout
 from backupz.src.support.progress_alive_bar import ProgressAliveBar
 from backupz.src.support.progress_alive_bar_git import ProgressAliveBarGit
 from backupz.src.support.texts import AppTexts
 
 
 # Download video from youtube
-def youtube_download(url: str) -> Path | None:
+def youtube_download(folder: Path, url: str) -> Path | None:
     try:
         bar = ProgressAliveBar(AppTexts.success_downloads())
 
         def on_complete_callback(stream, event):
             # Download image preview max size
             try:
-                image_path = get_download_folder() / stream.default_filename.replace('.mp4', '') / 'maxresdefault.jpg'
+                image_path = folder / stream.default_filename.replace('.mp4', '') / 'maxresdefault.jpg'
                 image_url = 'https://i.ytimg.com/vi/{}/maxresdefault.jpg'.format(extract.video_id(url))
                 r = requests.get(image_url, allow_redirects=True)
                 open(image_path, 'wb').write(r.content)
             except (Exception,):
                 pass
             # End progress
             bar.spinner_end()
 
         # Get YouTube video
         echo_stdout(AppTexts.info_get_info_video())
         yt = YouTube(url, on_complete_callback=on_complete_callback)
         # Get path to file
-        download_path = get_download_folder() / yt.streams.first().default_filename.replace('.mp4', '')
+        download_path = folder / yt.streams.first().default_filename.replace('.mp4', '')
         # Check if exist file
         if download_path.is_dir():
             echo_stderr(AppTexts.info_download(str(download_path.absolute())))
             return download_path
         else:
             echo_stdout(AppTexts.info_download_start(url))
             bar.spinner_start()
@@ -67,20 +67,20 @@
             return download_path
     except (Exception,):
         pass
     return None
 
 
 # Download file
-def downloads(urls: [str]) -> [Path]:
+def downloads(folder: Path, urls: [str]) -> [Path]:
     download_files = []
     exist_files = []
     for url in urls:
         # Get path to file
-        download_path = get_download_folder() / os.path.basename(url)
+        download_path = folder / os.path.basename(url)
         # Check if exist file
         if download_path.is_file():
             echo_stderr(AppTexts.info_download(str(download_path.absolute())))
             exist_files.append(str(download_path))
         else:
             echo_stdout(AppTexts.info_download_start(url))
             download_files.append({'url': url, 'path': download_path})
@@ -92,17 +92,17 @@
     download_files = multi_download(download_files, catch_error)
     if download_files:
         echo_stdout(AppTexts.success_downloads())
     return download_files + exist_files
 
 
 # Clone git project
-def git_clone(url: str) -> Path | None:
+def git_clone(folder: Path, url: str) -> Path | None:
     # Get path
-    clone_path = get_download_folder() / os.path.basename(url).replace('.git', '')
+    clone_path = folder / os.path.basename(url).replace('.git', '')
 
     # Check if path file
     if clone_path.is_file():
         return None
 
     # Check if exist project
     if clone_path.is_dir():
```

### Comparing `backupz-2.3.0.0/backupz/src/support/conf.py` & `backupz-2.4.0.0/backupz/src/support/conf.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,43 +19,52 @@
 
 import click.exceptions
 from yaml import Loader
 from yaml import load
 
 from backupz.src.support.data.data_ftp import DataFTP
 from backupz.src.support.data.data_ssh import DataSSH
+from backupz.src.support.data.data_telegram import DataTelegram
 from backupz.src.support.helper import get_path_file, get_path_folder
 from backupz.src.support.output import echo_stdout, echo_stderr
 from backupz.src.support.texts import AppTexts
 
 # Data versions
 APP_NAME = 'backupz'
-APP_VERSION = '2.3.0'
+APP_VERSION = '2.4.0'
 
 # Default path config
 PATH_CONF = '~/.backupz/configuration.yaml'
 
 CHANGELOG_CONF = r'''## Application configuration file Backupz
-## Version config: 0.0.5
+## Version config: 0.0.6
 
 # Path to file
 # - /path/to/you.file
 # Path to folder
 # - /path/to/folder
 # SSH git repo
 # - git@github.com:git/ssh.git
 # HTTP git repo
 # - https://github.com/git/https.git
 # Download file by url
-# - https://github.com/keygenqt/backupz/raw/main/builds/backupz-2.3.0.pyz
-# Download youtube video, pytube seems to be playing cat and mouse with 1080p resolution
+# - https://github.com/keygenqt/backupz/raw/main/builds/backupz-2.4.0.pyz
+# Download YouTube video (720p)
 # - https://www.youtube.com/watch?v=N2_7kqSmTZU
+# Backup posts Telegram
+# - https://t.me/channel_name
 backup:
   - ~/.backupz
 
+# For backup telegram post channel
+# Use your own values from my.telegram.org
+# telegram:
+#   api_id: 0000000
+#   api_hash: 00000000000000000000000000000000
+
 # Execute command before dump
 # Example: mysqldump -u root -p00000 my_db > ~/my_db.sql
 execute: []
 
 # https://linux.die.net/man/1/tar
 # Exclude by regex (tar --exclude)
 exclude: []
@@ -69,15 +78,15 @@
 compression: best
 
 # Name folder for save backup in format 'datetime.strftime'
 # https://docs.python.org/3/library/datetime.html#strftime-and-strptime-behavior
 name: 'backupz_%d_%m_%Y'
 
 # Folder for save
-folder: ~/backupz
+folder: ~/
 
 # Array folders SSH for save
 # {
 #   hostname: 192.168.2.15
 #   username: defaultuser
 #   port: 22
 #   path: /path/to/folder
@@ -106,50 +115,69 @@
 
     @staticmethod
     def get_app_version() -> str:
         return APP_VERSION
 
     @staticmethod
     def _get_path_conf(path, default):
+        # Get file --conf
         path = get_path_file(path)
 
-        default = get_path_file(default, none=False)
+        # Create dir if not exist
+        path_dir = os.path.dirname(default)
+        if not os.path.isdir(path_dir):
+            Path(path_dir).mkdir()
 
         if path and str(path).lower().endswith('.yaml'):
             return path
         else:
             if not default.is_file():
                 Conf._create_default_config(default)
             return Path(default)
 
     @staticmethod
     def _create_default_config(path: Path):
         if not click.confirm(AppTexts.confirm_init()):
             exit(0)
 
-        path_dir = os.path.dirname(path)
-
-        # Create dir if not exist
-        if not os.path.isdir(path_dir):
-            Path(path_dir).mkdir()
-
         # Write default configuration file
         with open(path, 'w') as file:
             print(CHANGELOG_CONF, file=file)
 
         echo_stdout(AppTexts.success_init(str(path)), 2)
 
     def __init__(self, path):
+        # Save start time
+        self.start_time = datetime.now()
+        # Default config path
+        default = get_path_file(PATH_CONF, none=False)
         # Get path config
-        self.conf_path = Conf._get_path_conf(path, default=PATH_CONF)
+        self.conf_path = Conf._get_path_conf(path, default=default)
+        # Temp folder
+        self.temp_path = Path(os.path.dirname(default))
 
         # Load config
         with open(self.conf_path, 'rb') as file:
             self.conf = load(file.read(), Loader=Loader)
 
+    # Get download folder
+    def get_download_folder(self) -> Path:
+        # Select download dir
+        download_dir = Path.home() / "Загрузки"
+        if not download_dir.is_dir():
+            download_dir = Path.home() / "Downloads"
+            if not download_dir.is_dir():
+                download_dir.mkdir(parents=True, exist_ok=True)
+        # Create temp folder
+        path = download_dir / 'backupz_{}'.format(self.start_time.strftime('%f'))
+        if not path.is_dir():
+            path.mkdir(parents=True, exist_ok=True)
+
+        return path
+
     # Get path for save tar.gz archive
     def get_path_to_save(self) -> Path:
         return self.get_folder_for_save() / '{name}.tar.gz'.format(
             name=datetime.now().strftime(self.get_name())
         )
 
     # Get paths folder and files for backup
@@ -263,14 +291,30 @@
                     username=ftp['username'],
                     password=ftp['password'],
                     port=ftp['port'],
                     path=ftp['path'],
                 ))
             return datas_ftp
 
+    # Get ftp from config
+    def get_telegram(self) -> DataTelegram | None:
+        if 'telegram' not in self.conf.keys():
+            return None
+        else:
+            if not isinstance(self.conf['telegram'], dict):
+                echo_stderr(AppTexts.error_load_key('telegram'))
+                exit(1)
+            if not DataTelegram.validate(self.conf['telegram']):
+                return None
+            return DataTelegram(
+                api_id=self.conf['telegram']['api_id'],
+                api_hash=self.conf['telegram']['api_hash'],
+                path_session=self.temp_path
+            )
+
     # Get commands execute before dump from config
     def get_execute_commands(self) -> [str]:
         if 'execute' not in self.conf.keys():
             echo_stderr(AppTexts.error_load_key('execute'))
             exit(1)
         else:
             commands: [] = []
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `backupz-2.3.0.0/backupz/src/support/data/data_ftp.py` & `backupz-2.4.0.0/backupz/src/support/data/data_ftp.py`

 * *Files identical despite different names*

### Comparing `backupz-2.3.0.0/backupz/src/support/data/data_ssh.py` & `backupz-2.4.0.0/backupz/src/support/data/data_ssh.py`

 * *Files identical despite different names*

### Comparing `backupz-2.3.0.0/backupz/src/support/dependency.py` & `backupz-2.4.0.0/backupz/src/support/dependency.py`

 * *Files identical despite different names*

### Comparing `backupz-2.3.0.0/backupz/src/support/download.py` & `backupz-2.4.0.0/backupz/src/support/download.py`

 * *Files identical despite different names*

### Comparing `backupz-2.3.0.0/backupz/src/support/helper.py` & `backupz-2.4.0.0/backupz/src/support/helper.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,30 +17,14 @@
 import subprocess
 from pathlib import Path
 from typing import Callable
 
 from cffi.backend_ctypes import unicode
 
 
-# Get download folder
-def get_download_folder() -> Path:
-    # Select download dir
-    download_dir = Path.home() / "Загрузки"
-    if not download_dir.is_dir():
-        download_dir = Path.home() / "Downloads"
-        if not download_dir.is_dir():
-            download_dir.mkdir(parents=True, exist_ok=True)
-    # Create temp folder
-    path = download_dir / 'backupz'
-    if not path.is_dir():
-        path.mkdir(parents=True, exist_ok=True)
-
-    return path
-
-
 # Get full path folder
 def get_path_folder(
         path: str
 ) -> Path | None:
     path = get_path_file(path, False)
     if path.is_dir():
         return path
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `backupz-2.3.0.0/backupz/src/support/output.py` & `backupz-2.4.0.0/backupz/src/support/output.py`

 * *Files identical despite different names*

### Comparing `backupz-2.3.0.0/backupz/src/support/progress_alive_bar.py` & `backupz-2.4.0.0/backupz/src/support/progress_alive_bar.py`

 * *Files identical despite different names*

### Comparing `backupz-2.3.0.0/backupz/src/support/progress_alive_bar_git.py` & `backupz-2.4.0.0/backupz/src/support/progress_alive_bar_git.py`

 * *Files identical despite different names*

### Comparing `backupz-2.3.0.0/backupz/src/support/texts.py` & `backupz-2.4.0.0/backupz/src/support/texts.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,21 +47,32 @@
         return '<red>Error connect {} to</red> "{}" <red>host.</red>'.format(method, hostname)
 
     @staticmethod
     def error_exception(message: str):
         return '<red>Catch exception: {}</red>'.format(message.strip())
 
     @staticmethod
+    def error_telegram_get_posts(url: str):
+        return '<red>Telegram error get posts:</red> {}'.format(url)
+
+    @staticmethod
     def error_clone_project(url: str):
         return '<red>Git project error clone:</red> {}'.format(url)
 
     @staticmethod
     def error_download(url: str):
         return '<red>Error download:</red> {}'.format(url)
 
+    @staticmethod
+    def error_telegram_configuration():
+        return ('<red>Check your configuration file.</red>\n'
+                '<yellow>To use a telegram bot you need to specify</yellow> '
+                '"api_id" <yellow>and</yellow> '
+                '"api_hash"<yellow>.</yellow>')
+
     ##########
     # Confirms
     @staticmethod
     def confirm_init():
         return 'Add default backupz configuration file?'
 
     #########
```

### Comparing `backupz-2.3.0.0/backupz.egg-info/PKG-INFO` & `backupz-2.4.0.0/backupz.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backupz
-Version: 2.3.0.0
+Version: 2.4.0.0
 Summary: The application allows you to generate CHANGELOG files based on Git tags.
 Home-page: https://github.com/keygenqt/backupz
 Author: Vitaliy Zarubin
 Author-email: keygenqt@gmail.com
 Requires-Python: >=3.8.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,20 +13,30 @@
 Requires-Dist: cffi>=1.16.0
 Requires-Dist: beautifulsoup4>=4.12.3
 Requires-Dist: alive-progress>=3.1.5
 Requires-Dist: paramiko>=3.4.0
 Requires-Dist: GitPython>=3.1.41
 Requires-Dist: requests>=2.31.0
 Requires-Dist: pytube>=15.0.0
+Requires-Dist: Telethon>=1.34.0
 
 
 ![picture](https://github.com/keygenqt/backupz/blob/main/data/banners/banner_round_grey.png?raw=true)
 
 Create and save a backup archive in multiple processes.
 
+#### Can make backups from:
+
+- GitHub
+- YouTube
+- Telegram
+- Database
+- Folders/Files
+- Files from direct links
+
 [More...](https://keygenqt.github.io/backupz)
 
 ### License
 
 ```
 Copyright 2021-2024 Vitaliy Zarubin
```

### Comparing `backupz-2.3.0.0/backupz.egg-info/SOURCES.txt` & `backupz-2.4.0.0/backupz.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -21,8 +21,9 @@
 backupz/src/support/helper.py
 backupz/src/support/output.py
 backupz/src/support/progress_alive_bar.py
 backupz/src/support/progress_alive_bar_git.py
 backupz/src/support/texts.py
 backupz/src/support/data/__init__.py
 backupz/src/support/data/data_ftp.py
-backupz/src/support/data/data_ssh.py
+backupz/src/support/data/data_ssh.py
+backupz/src/support/data/data_telegram.py
```

### Comparing `backupz-2.3.0.0/setup.py` & `backupz-2.4.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 import setuptools
 
 long_description = """
 ![picture](https://github.com/keygenqt/backupz/blob/main/data/banners/banner_round_grey.png?raw=true)
 
 Create and save a backup archive in multiple processes.
 
+#### Can make backups from:
+
+- GitHub
+- YouTube
+- Telegram
+- Database
+- Folders/Files
+- Files from direct links
+
 [More...](https://keygenqt.github.io/backupz)
 
 ### License
 
 ```
 Copyright 2021-2024 Vitaliy Zarubin
 
@@ -24,15 +33,15 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 ```
 """
 
 setuptools.setup(
     name='backupz',
-    version='2.3.0.0',
+    version='2.4.0.0',
     author='Vitaliy Zarubin',
     author_email='keygenqt@gmail.com',
     description='The application allows you to generate CHANGELOG files based on Git tags.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/keygenqt/backupz",
     packages=setuptools.find_packages(exclude=['*tests.*', '*tests']),
@@ -44,14 +53,15 @@
         'cffi>=1.16.0',
         'beautifulsoup4>=4.12.3',
         'alive-progress>=3.1.5',
         'paramiko>=3.4.0',
         'GitPython>=3.1.41',
         'requests>=2.31.0',
         'pytube>=15.0.0',
+        'Telethon>=1.34.0',
     ],
     python_requires='>=3.8.2',
     entry_points="""
         [console_scripts]
         backupz = backupz.__main__:main
     """
 )
```


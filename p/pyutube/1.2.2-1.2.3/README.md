# Comparing `tmp/pyutube-1.2.2.tar.gz` & `tmp/pyutube-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutube-1.2.2.tar", last modified: Sun Apr 21 06:44:52 2024, max compression
+gzip compressed data, was "pyutube-1.2.3.tar", last modified: Thu Apr 25 10:05:13 2024, max compression
```

## Comparing `pyutube-1.2.2.tar` & `pyutube-1.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-21 06:44:52.494001 pyutube-1.2.2/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1078 2024-03-05 00:46:11.000000 pyutube-1.2.2/LICENSE.md
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     8633 2024-04-21 06:44:52.492424 pyutube-1.2.2/PKG-INFO
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     7812 2024-04-21 06:44:29.000000 pyutube-1.2.2/README.md
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-21 06:44:52.477846 pyutube-1.2.2/pyutube/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      399 2024-04-07 04:16:19.000000 pyutube-1.2.2/pyutube/__init__.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      184 2024-03-31 03:14:16.000000 pyutube-1.2.2/pyutube/__main__.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     6749 2024-04-20 09:57:31.000000 pyutube-1.2.2/pyutube/cli.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)    14032 2024-04-21 06:30:38.000000 pyutube-1.2.2/pyutube/downloader.py
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-21 06:44:52.488476 pyutube-1.2.2/pyutube/tests/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       30 2024-02-14 23:03:00.000000 pyutube-1.2.2/pyutube/tests/__init__.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     4676 2024-04-12 09:09:48.000000 pyutube-1.2.2/pyutube/tests/test_utils.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)    12375 2024-04-21 06:31:17.000000 pyutube-1.2.2/pyutube/utils.py
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-21 06:44:52.490517 pyutube-1.2.2/pyutube.egg-info/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     8633 2024-04-21 06:44:52.000000 pyutube-1.2.2/pyutube.egg-info/PKG-INFO
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      365 2024-04-21 06:44:52.000000 pyutube-1.2.2/pyutube.egg-info/SOURCES.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        1 2024-04-21 06:44:52.000000 pyutube-1.2.2/pyutube.egg-info/dependency_links.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       44 2024-04-21 06:44:52.000000 pyutube-1.2.2/pyutube.egg-info/entry_points.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       70 2024-04-21 06:44:52.000000 pyutube-1.2.2/pyutube.egg-info/requires.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        8 2024-04-21 06:44:52.000000 pyutube-1.2.2/pyutube.egg-info/top_level.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       38 2024-04-21 06:44:52.494253 pyutube-1.2.2/setup.cfg
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1436 2024-04-07 04:18:59.000000 pyutube-1.2.2/setup.py
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-25 10:05:13.821809 pyutube-1.2.3/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1078 2024-03-05 00:46:11.000000 pyutube-1.2.3/LICENSE.md
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     8616 2024-04-25 10:05:13.820541 pyutube-1.2.3/PKG-INFO
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     7795 2024-04-25 10:05:06.000000 pyutube-1.2.3/README.md
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-25 10:05:13.792628 pyutube-1.2.3/pyutube/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      399 2024-04-07 04:16:19.000000 pyutube-1.2.3/pyutube/__init__.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      184 2024-03-31 03:14:16.000000 pyutube-1.2.3/pyutube/__main__.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     6728 2024-04-25 10:00:48.000000 pyutube-1.2.3/pyutube/cli.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)    14053 2024-04-25 09:45:49.000000 pyutube-1.2.3/pyutube/downloader.py
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-25 10:05:13.816728 pyutube-1.2.3/pyutube/tests/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       30 2024-02-14 23:03:00.000000 pyutube-1.2.3/pyutube/tests/__init__.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     4676 2024-04-12 09:09:48.000000 pyutube-1.2.3/pyutube/tests/test_utils.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)    11318 2024-04-25 10:04:41.000000 pyutube-1.2.3/pyutube/utils.py
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-25 10:05:13.818966 pyutube-1.2.3/pyutube.egg-info/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     8616 2024-04-25 10:05:13.000000 pyutube-1.2.3/pyutube.egg-info/PKG-INFO
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      365 2024-04-25 10:05:13.000000 pyutube-1.2.3/pyutube.egg-info/SOURCES.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        1 2024-04-25 10:05:13.000000 pyutube-1.2.3/pyutube.egg-info/dependency_links.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       44 2024-04-25 10:05:13.000000 pyutube-1.2.3/pyutube.egg-info/entry_points.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       70 2024-04-25 10:05:13.000000 pyutube-1.2.3/pyutube.egg-info/requires.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        8 2024-04-25 10:05:13.000000 pyutube-1.2.3/pyutube.egg-info/top_level.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       38 2024-04-25 10:05:13.821973 pyutube-1.2.3/setup.cfg
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1436 2024-04-07 04:18:59.000000 pyutube-1.2.3/setup.py
```

### Comparing `pyutube-1.2.2/LICENSE.md` & `pyutube-1.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyutube-1.2.2/PKG-INFO` & `pyutube-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutube
-Version: 1.2.2
+Version: 1.2.3
 Summary: Awesome CLI to download YouTube videos (as video or audio)/shorts/playlists from the terminal
 Author: Ebraheem Alhetari
 Author-email: hetari4all@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/Hetari/pyutube
 Keywords: youtube,download,cli,pyutube,pytube
 Platform: Windows
@@ -110,31 +110,32 @@
 pyutube -v
 ```
 
 ### **- Download playlists:**
 
 1. `pyutube <YOUTUBE_PLAYLIST_LINK | PLAYLIST_ID> [the_download_path*]`
 
-   > [!NOTE]
-   > Don't forget, the path is optional.
+> [!NOTE]
+> Don't forget, the path is optional.
+
+1. Then choose the format of the download, video or audio.
+2. Choose the resolution if it is a video you want to download, otherwise, choose audio and it will download it all immediately 🔥.
 
-2. Then choose the format of the download, video or audio.
-3. Choose the resolution if it is a video you want to download, otherwise, choose audio and it will download it all immediately 🔥.
-   > [!NOTE]
-   > It will check all resolutions available in the first video in the playlist, then it will download all of them in the same resolution 👍.
+> [!NOTE]
+> It will check all resolutions available in the first video in the playlist, then it will download all of them in the same resolution 👍.
 
 ### **- Download shorts, videos, or audio:**
 
 1. `pyutube <YOUTUBE_LINK | VIDEO_ID | SHORT_LINK> [the_download_path*]`
 
-   > [!NOTE]
-   > Don't forget, the path is optional.
+> [!NOTE]
+> Don't forget, the path is optional.
 
-2. Then choose the format of the download, video or audio.
-3. Choose the resolution if it is a video you want to download, otherwise, choose audio and it will download it immediately 🔥.
+1. Then choose the format of the download, video or audio.
+2. Choose the resolution if it is a video you want to download, otherwise, choose audio and it will download it immediately 🔥.
 
 ```bash
 pyutube cMPnY7EuZvo
 pyutube youtu.be/cMPnY7EuZvo
 pyutube https://youtube.com/watch?v=cMPnY7EuZvo
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyutube Version: 1.2.2 Summary: Awesome CLI to
+Metadata-Version: 2.1 Name: pyutube Version: 1.2.3 Summary: Awesome CLI to
 download YouTube videos (as video or audio)/shorts/playlists from the terminal
 Author: Ebraheem Alhetari Author-email: hetari4all@gmail.com License: MIT
 Project-URL: Homepage, https://github.com/Hetari/pyutube Keywords:
 youtube,download,cli,pyutube,pytube Platform: Windows Platform: MacOS Platform:
 Linux Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
@@ -45,22 +45,22 @@
 ------------------------------------------------------- | | `-v` or `--version`
 | Show the version number. | | `-a` or `--audio` | Download only audio
 immediately without asking (video or audio). | | `-f` or `--footage` | Download
 only video immediately without asking (video or audio). | ## ðµï¸ââï¸
 Examples ### **- Show version:** ```bash pyutube -v ``` ### **- Download
 playlists:** 1. `pyutube
 PLAYLIST_ID> [the_download_path*]` > [!NOTE] > Don't forget, the path is
-optional. 2. Then choose the format of the download, video or audio. 3. Choose
+optional. 1. Then choose the format of the download, video or audio. 2. Choose
 the resolution if it is a video you want to download, otherwise, choose audio
 and it will download it all immediately ð¥. > [!NOTE] > It will check all
 resolutions available in the first video in the playlist, then it will download
 all of them in the same resolution ð. ### **- Download shorts, videos, or
 audio:** 1. `pyutube
 VIDEO_ID | SHORT_LINK> [the_download_path*]` > [!NOTE] > Don't forget, the path
-is optional. 2. Then choose the format of the download, video or audio. 3.
+is optional. 1. Then choose the format of the download, video or audio. 2.
 Choose the resolution if it is a video you want to download, otherwise, choose
 audio and it will download it immediately ð¥. ```bash pyutube cMPnY7EuZvo
 pyutube youtu.be/cMPnY7EuZvo pyutube https://youtube.com/watch?v=cMPnY7EuZvo
 ``` ### **- Download audio immediately:** 1. `pyutube
 VIDEO_ID | SHORT_LINK> [the_download_path*] -a` ```bash pyutube cMPnY7EuZvo -
 a ``` or ```bash pyutube -a youtu.be/cMPnY7EuZvo ``` and that's it ð. ###
 **- Download videos immediately:** 1. `pyutube
```

### Comparing `pyutube-1.2.2/README.md` & `pyutube-1.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -82,31 +82,32 @@
 pyutube -v
 ```
 
 ### **- Download playlists:**
 
 1. `pyutube <YOUTUBE_PLAYLIST_LINK | PLAYLIST_ID> [the_download_path*]`
 
-   > [!NOTE]
-   > Don't forget, the path is optional.
+> [!NOTE]
+> Don't forget, the path is optional.
 
-2. Then choose the format of the download, video or audio.
-3. Choose the resolution if it is a video you want to download, otherwise, choose audio and it will download it all immediately 🔥.
-   > [!NOTE]
-   > It will check all resolutions available in the first video in the playlist, then it will download all of them in the same resolution 👍.
+1. Then choose the format of the download, video or audio.
+2. Choose the resolution if it is a video you want to download, otherwise, choose audio and it will download it all immediately 🔥.
+
+> [!NOTE]
+> It will check all resolutions available in the first video in the playlist, then it will download all of them in the same resolution 👍.
 
 ### **- Download shorts, videos, or audio:**
 
 1. `pyutube <YOUTUBE_LINK | VIDEO_ID | SHORT_LINK> [the_download_path*]`
 
-   > [!NOTE]
-   > Don't forget, the path is optional.
+> [!NOTE]
+> Don't forget, the path is optional.
 
-2. Then choose the format of the download, video or audio.
-3. Choose the resolution if it is a video you want to download, otherwise, choose audio and it will download it immediately 🔥.
+1. Then choose the format of the download, video or audio.
+2. Choose the resolution if it is a video you want to download, otherwise, choose audio and it will download it immediately 🔥.
 
 ```bash
 pyutube cMPnY7EuZvo
 pyutube youtu.be/cMPnY7EuZvo
 pyutube https://youtube.com/watch?v=cMPnY7EuZvo
 ```
```

#### html2text {}

```diff
@@ -34,22 +34,22 @@
 ------------------------------------------------------- | | `-v` or `--version`
 | Show the version number. | | `-a` or `--audio` | Download only audio
 immediately without asking (video or audio). | | `-f` or `--footage` | Download
 only video immediately without asking (video or audio). | ## ðµï¸ââï¸
 Examples ### **- Show version:** ```bash pyutube -v ``` ### **- Download
 playlists:** 1. `pyutube
 PLAYLIST_ID> [the_download_path*]` > [!NOTE] > Don't forget, the path is
-optional. 2. Then choose the format of the download, video or audio. 3. Choose
+optional. 1. Then choose the format of the download, video or audio. 2. Choose
 the resolution if it is a video you want to download, otherwise, choose audio
 and it will download it all immediately ð¥. > [!NOTE] > It will check all
 resolutions available in the first video in the playlist, then it will download
 all of them in the same resolution ð. ### **- Download shorts, videos, or
 audio:** 1. `pyutube
 VIDEO_ID | SHORT_LINK> [the_download_path*]` > [!NOTE] > Don't forget, the path
-is optional. 2. Then choose the format of the download, video or audio. 3.
+is optional. 1. Then choose the format of the download, video or audio. 2.
 Choose the resolution if it is a video you want to download, otherwise, choose
 audio and it will download it immediately ð¥. ```bash pyutube cMPnY7EuZvo
 pyutube youtu.be/cMPnY7EuZvo pyutube https://youtube.com/watch?v=cMPnY7EuZvo
 ``` ### **- Download audio immediately:** 1. `pyutube
 VIDEO_ID | SHORT_LINK> [the_download_path*] -a` ```bash pyutube cMPnY7EuZvo -
 a ``` or ```bash pyutube -a youtu.be/cMPnY7EuZvo ``` and that's it ð. ###
 **- Download videos immediately:** 1. `pyutube
```

### Comparing `pyutube-1.2.2/pyutube/cli.py` & `pyutube-1.2.3/pyutube/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
     Args:
         url (str): The URL of the YouTube video.
         path (str): The path to save the video. Defaults to the current working directory.
 
     """
     if version:
         console.print(f"Pyutube {__version__}")
+        check_for_updates()
         sys.exit()
 
     if url is None:
         error_console.print("❗ Missing argument 'URL'.")
         sys.exit()
 
     clear()
@@ -185,26 +186,26 @@
     Args:
         url (str): The URL of the playlist.
         path (str): The path to save the downloaded videos.
 
     Returns:
         None
     """
-    # TODO: Make subfunction to download playlist
     def get_title(video):
         """Function to get the title of a YouTube video."""
         return video.title
 
     def fetch_title_thread(video):
         """Fetch the title of a YouTube video in a separate thread."""
         video_title = video.title
         video_id = video.video_id
         playlist_videos.append((video_title, video_id))
 
     global playlist_videos
+
     try:
         is_audio = handle_video_link()
     except TypeError:
         return
     playlist = download(url, path, is_audio, is_playlist=True)
 
     # links = playlist.video_urls
```

### Comparing `pyutube-1.2.2/pyutube/downloader.py` & `pyutube-1.2.3/pyutube/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     console,
     error_console,
     sanitize_filename,
     ask_rename_file,
     ask_resolution,
     rename_file,
     is_file_exists,
-    has_audio
 )
 
 import os
 import sys
 
 
 from yaspin import yaspin
@@ -206,29 +205,31 @@
         """
         Generate a filename for the downloaded video.
 
         Returns:
             str: The generated filename.
         """
         quality = 'audio' if self.is_audio else video.resolution
-        title = sanitize_filename(video.title)
+        title = video.default_filename
         extension = 'mp3' if self.is_audio else video.mime_type.split('/')[1]
 
         return f"{title} - {quality}_-_{video_id}.{extension}"
 
     def handle_existing_file(self, filename):
         """
         Handle the case where a file with the same name already exists.
 
         Returns:
             str: The user's choice.
         """
         choice = ask_rename_file(filename).lower()
         if choice.startswith('rename'):
-            filename = self.prompt_new_filename(filename)
+            filename = sanitize_filename(
+                self.prompt_new_filename(filename)
+            )
             if not filename:
                 error_console.print("Invalid filename")
                 return False
             return filename
         elif choice.startswith('cancel'):
             console.print("Download canceled", style="info")
             return False
@@ -388,16 +389,18 @@
 
         # If file with the same name already exists in the path
         if is_file_exists(self.path, video_filename):
             video_filename = self.handle_existing_file(video_filename)
             if not video_filename:
                 sys.exit()
         try:
+            console.print("⏳ Downloading video...", style="info")
             self.save_file(footage, self.path, video_filename)
-            if not self.is_audio and not has_audio(video_filename, os.path.join(self.path, audio_filename)):
+
+            if not self.is_audio:
                 self.save_file(video_audio, self.path, audio_filename)
                 self.merging(video_filename, audio_filename)
 
         except Exception as error:
             error_console.print(f"Error: {error}")
             sys.exit()
```

### Comparing `pyutube-1.2.2/pyutube/tests/test_utils.py` & `pyutube-1.2.3/pyutube/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyutube-1.2.2/pyutube/utils.py` & `pyutube-1.2.3/pyutube/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """
 This module contains the utils functions for the pyutube package.
 """
 
 import sys
 import re
 import os
+from datetime import timedelta
 
 import inquirer
 import requests
+import requests_cache
 from yaspin import yaspin
 from yaspin.spinners import Spinners
 from rich.console import Console
 from rich.theme import Theme
 from termcolor import colored
-from moviepy.tools import subprocess_call
-from moviepy.config import get_setting
 
 
-__version__ = "1.2.2"
+__version__ = "1.2.3"
 __app__ = "pyutube"
 ABORTED_PREFIX = "aborted"
 CANCEL_PREFIX = "cancel"
 
+requests_cache.install_cache('update_cache', expire_after=timedelta(days=2))
+
+
 # Set up the console
 custom_theme = Theme({
     "info": "#64b0f2",
     "warning": "color(3)",
     "danger": "red",
     "success": "green",
 })
@@ -194,28 +197,15 @@
     Args:
         resolutions (set): The set of available resolutions.
 
     Returns:
         str: The chosen resolution as a string.
     """
     # Create a dictionary to relate each size with its resolution
-    size_resolution_mapping = {}
-
-    for resolution, size in zip(resolutions, sizes):
-        # Check if the resolution already exists in the dictionary
-        if resolution not in size_resolution_mapping:
-            # If it doesn't exist, add it to the dictionary
-            size_resolution_mapping[resolution] = size
-        else:
-            # If it does exist, compare the sizes and keep the highest one
-            current_size = float(
-                size_resolution_mapping[resolution].replace(" MB", ""))
-            new_size = float(size.replace(" MB", ""))
-            if new_size > current_size:
-                size_resolution_mapping[resolution] = size
+    size_resolution_mapping = dict(zip(sizes, resolutions))
 
     # Generate the choices for the user prompt
     resolution_choices = [
         f"{size} ~= {resolution}" for size, resolution in size_resolution_mapping.items()
     ] + ["Cancel the download"]
 
     questions = [
@@ -252,15 +242,15 @@
     """
     console.print(
         f"'{filename}' is already exists, do you want to:", style="info")
     questions = [
         inquirer.List(
             "rename",
             message="Do you want to",
-            choices=['Rename it', 'Overwrite it', "Cancel"],
+            choices=['Rename it', 'Overwrite it', CANCEL_PREFIX.capitalize()],
         ),
     ]
     return inquirer.prompt(questions)["rename"]
 
 
 def ask_playlist_video_names(videos):
     note = colored("NOTE:", "cyan")
@@ -339,15 +329,43 @@
 
     Returns:
         bool: True if the file exists, False otherwise.
     """
     return os.path.isfile(os.path.join(path, filename))
 
 
+def check_for_updates() -> None:
+    """
+    A function to check for updates of a given package.
+
+    Returns:
+        None
+    """
+    try:
+        r = requests.get(
+            f'https://pypi.org/pypi/{__app__}/json', headers={'Accept': 'application/json'})
+    except Exception as error:
+        error_console.print(f"❗ Error checking for updates: {error}")
+    else:
+        if r.status_code == 200:
+            latest_version = r.json()['info']['version']
+
+            if latest_version != __version__:
+                console.print(
+                    f"👉 A new version of {__app__} is available: {latest_version}. Update it by running [bold red link=https://github.com/Hetari/pyutube]pip install --upgrade {__app__}[/bold red link]",
+                    style="warning"
+                )
+        else:
+            error_console.print(
+                f"❗ Error checking for updates: {r.status_code}")
+            sys.exit()
+
 # main utils
+
+
 def check_internet_connection() -> bool:
     """
     Checks if an internet connection is available.
 
     Returns:
         bool: True if internet connection is available, False otherwise.
     """
@@ -394,56 +412,7 @@
     if file_type_choice.startswith(CANCEL_PREFIX):
         error_console.print("❗ Cancel the download...")
         sys.exit()
     elif file_type_choice.startswith(ABORTED_PREFIX):
         sys.exit()
 
     return is_audio
-
-
-def has_audio(input_file, output, bitrate=3000, fps=44100):
-    """ extract the sound from a video file and save it in ``output`` """
-
-    try:
-        cmd = [
-            get_setting("FFMPEG_BINARY"),
-            "-y",
-            "-i",
-            input_file,
-            "-ab",
-            "%dk" % bitrate,
-            "-ar",
-            "%d" % fps,
-            output
-        ]
-        subprocess_call(cmd, logger=None)
-    except Exception as error:
-        return False
-
-    os.remove(output)
-    return True
-
-
-def check_for_updates() -> None:
-    """
-    A function to check for updates of a given package.
-
-    Returns:
-        None
-    """
-    try:
-        r = requests.get(
-            f'https://pypi.org/pypi/{__app__}/json', headers={'Accept': 'application/json'})
-    except Exception as error:
-        error_console.print(f"❗ Error checking for updates: {error}")
-    else:
-        if r.status_code == 200:
-            latest_version = r.json()['info']['version']
-            if latest_version != __version__:
-                console.print(
-                    f"👉 A new version of {__app__} is available: {latest_version}. Update it by running [bold red link=https://github.com/Hetari/pyutube]pip install --upgrade {__app__}[/bold red link]",
-                    style="warning"
-                )
-        else:
-            error_console.print(
-                f"❗ Error checking for updates: {r.status_code}")
-            sys.exit()
```

### Comparing `pyutube-1.2.2/pyutube.egg-info/PKG-INFO` & `pyutube-1.2.3/pyutube.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutube
-Version: 1.2.2
+Version: 1.2.3
 Summary: Awesome CLI to download YouTube videos (as video or audio)/shorts/playlists from the terminal
 Author: Ebraheem Alhetari
 Author-email: hetari4all@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/Hetari/pyutube
 Keywords: youtube,download,cli,pyutube,pytube
 Platform: Windows
@@ -110,31 +110,32 @@
 pyutube -v
 ```
 
 ### **- Download playlists:**
 
 1. `pyutube <YOUTUBE_PLAYLIST_LINK | PLAYLIST_ID> [the_download_path*]`
 
-   > [!NOTE]
-   > Don't forget, the path is optional.
+> [!NOTE]
+> Don't forget, the path is optional.
+
+1. Then choose the format of the download, video or audio.
+2. Choose the resolution if it is a video you want to download, otherwise, choose audio and it will download it all immediately 🔥.
 
-2. Then choose the format of the download, video or audio.
-3. Choose the resolution if it is a video you want to download, otherwise, choose audio and it will download it all immediately 🔥.
-   > [!NOTE]
-   > It will check all resolutions available in the first video in the playlist, then it will download all of them in the same resolution 👍.
+> [!NOTE]
+> It will check all resolutions available in the first video in the playlist, then it will download all of them in the same resolution 👍.
 
 ### **- Download shorts, videos, or audio:**
 
 1. `pyutube <YOUTUBE_LINK | VIDEO_ID | SHORT_LINK> [the_download_path*]`
 
-   > [!NOTE]
-   > Don't forget, the path is optional.
+> [!NOTE]
+> Don't forget, the path is optional.
 
-2. Then choose the format of the download, video or audio.
-3. Choose the resolution if it is a video you want to download, otherwise, choose audio and it will download it immediately 🔥.
+1. Then choose the format of the download, video or audio.
+2. Choose the resolution if it is a video you want to download, otherwise, choose audio and it will download it immediately 🔥.
 
 ```bash
 pyutube cMPnY7EuZvo
 pyutube youtu.be/cMPnY7EuZvo
 pyutube https://youtube.com/watch?v=cMPnY7EuZvo
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyutube Version: 1.2.2 Summary: Awesome CLI to
+Metadata-Version: 2.1 Name: pyutube Version: 1.2.3 Summary: Awesome CLI to
 download YouTube videos (as video or audio)/shorts/playlists from the terminal
 Author: Ebraheem Alhetari Author-email: hetari4all@gmail.com License: MIT
 Project-URL: Homepage, https://github.com/Hetari/pyutube Keywords:
 youtube,download,cli,pyutube,pytube Platform: Windows Platform: MacOS Platform:
 Linux Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
@@ -45,22 +45,22 @@
 ------------------------------------------------------- | | `-v` or `--version`
 | Show the version number. | | `-a` or `--audio` | Download only audio
 immediately without asking (video or audio). | | `-f` or `--footage` | Download
 only video immediately without asking (video or audio). | ## ðµï¸ââï¸
 Examples ### **- Show version:** ```bash pyutube -v ``` ### **- Download
 playlists:** 1. `pyutube
 PLAYLIST_ID> [the_download_path*]` > [!NOTE] > Don't forget, the path is
-optional. 2. Then choose the format of the download, video or audio. 3. Choose
+optional. 1. Then choose the format of the download, video or audio. 2. Choose
 the resolution if it is a video you want to download, otherwise, choose audio
 and it will download it all immediately ð¥. > [!NOTE] > It will check all
 resolutions available in the first video in the playlist, then it will download
 all of them in the same resolution ð. ### **- Download shorts, videos, or
 audio:** 1. `pyutube
 VIDEO_ID | SHORT_LINK> [the_download_path*]` > [!NOTE] > Don't forget, the path
-is optional. 2. Then choose the format of the download, video or audio. 3.
+is optional. 1. Then choose the format of the download, video or audio. 2.
 Choose the resolution if it is a video you want to download, otherwise, choose
 audio and it will download it immediately ð¥. ```bash pyutube cMPnY7EuZvo
 pyutube youtu.be/cMPnY7EuZvo pyutube https://youtube.com/watch?v=cMPnY7EuZvo
 ``` ### **- Download audio immediately:** 1. `pyutube
 VIDEO_ID | SHORT_LINK> [the_download_path*] -a` ```bash pyutube cMPnY7EuZvo -
 a ``` or ```bash pyutube -a youtu.be/cMPnY7EuZvo ``` and that's it ð. ###
 **- Download videos immediately:** 1. `pyutube
```

### Comparing `pyutube-1.2.2/setup.py` & `pyutube-1.2.3/setup.py`

 * *Files identical despite different names*


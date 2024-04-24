# Comparing `tmp/vidcrawler-1.0.8.tar.gz` & `tmp/vidcrawler-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vidcrawler-1.0.8.tar", last modified: Thu Jun 30 19:38:07 2022, max compression
+gzip compressed data, was "vidcrawler-1.0.9.tar", last modified: Sun Oct  9 03:08:19 2022, max compression
```

## Comparing `vidcrawler-1.0.8.tar` & `vidcrawler-1.0.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2022-06-30 19:38:07.712464 vidcrawler-1.0.8/
--rw-rw-rw-   0        0        0     1085 2022-05-16 02:03:37.000000 vidcrawler-1.0.8/LICENSE
--rw-rw-rw-   0        0        0       58 2022-05-11 03:18:30.000000 vidcrawler-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3487 2022-06-30 19:38:07.712464 vidcrawler-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2843 2022-06-30 19:37:28.000000 vidcrawler-1.0.8/README.md
--rw-rw-rw-   0        0        0       52 2022-05-16 02:06:18.000000 vidcrawler-1.0.8/requirements.testing.txt
--rw-rw-rw-   0        0        0      117 2022-05-16 08:06:27.000000 vidcrawler-1.0.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-06-30 19:38:07.713463 vidcrawler-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     3980 2022-05-16 06:59:07.000000 vidcrawler-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-30 19:38:07.690464 vidcrawler-1.0.8/vidcrawler/
--rw-rw-rw-   0        0        0       76 2022-05-16 07:04:00.000000 vidcrawler-1.0.8/vidcrawler/__init__.py
--rw-rw-rw-   0        0        0     5474 2022-05-16 08:06:27.000000 vidcrawler-1.0.8/vidcrawler/bitchute.py
--rw-rw-rw-   0        0        0     1966 2022-05-16 07:03:09.000000 vidcrawler-1.0.8/vidcrawler/brighteon.py
--rw-rw-rw-   0        0        0     1580 2022-05-16 05:42:38.000000 vidcrawler-1.0.8/vidcrawler/cmd.py
--rw-rw-rw-   0        0        0     2731 2022-05-26 04:49:33.000000 vidcrawler-1.0.8/vidcrawler/date.py
--rw-rw-rw-   0        0        0      176 2022-05-16 04:15:19.000000 vidcrawler-1.0.8/vidcrawler/error.py
--rw-rw-rw-   0        0        0     1440 2022-05-17 05:37:15.000000 vidcrawler-1.0.8/vidcrawler/fetch_html.py
--rw-rw-rw-   0        0        0     4187 2022-05-16 05:01:49.000000 vidcrawler-1.0.8/vidcrawler/gabtv.py
--rw-rw-rw-   0        0        0     2516 2022-05-16 04:34:08.000000 vidcrawler-1.0.8/vidcrawler/io.py
--rw-rw-rw-   0        0        0     1844 2022-06-30 19:33:08.000000 vidcrawler-1.0.8/vidcrawler/odysee.py
--rw-rw-rw-   0        0        0     3965 2022-05-16 07:03:09.000000 vidcrawler-1.0.8/vidcrawler/rumble.py
--rw-rw-rw-   0        0        0      360 2022-05-16 07:04:39.000000 vidcrawler-1.0.8/vidcrawler/run_tests.py
--rw-rw-rw-   0        0        0     6552 2022-05-16 07:03:25.000000 vidcrawler-1.0.8/vidcrawler/spider.py
--rw-rw-rw-   0        0        0     3243 2022-05-16 07:03:09.000000 vidcrawler-1.0.8/vidcrawler/spotify.py
--rw-rw-rw-   0        0        0     2260 2022-05-16 07:03:09.000000 vidcrawler-1.0.8/vidcrawler/spreaker.py
-drwxrwxrwx   0        0        0        0 2022-06-30 19:38:07.711463 vidcrawler-1.0.8/vidcrawler/testing/
--rw-rw-rw-   0        0        0        0 2022-05-11 00:37:25.000000 vidcrawler-1.0.8/vidcrawler/testing/__init__.py
--rw-rw-rw-   0        0        0     2665 2022-05-16 05:01:51.000000 vidcrawler-1.0.8/vidcrawler/testing/simple_http_server.py
--rw-rw-rw-   0        0        0     1071 2022-06-10 07:11:23.000000 vidcrawler-1.0.8/vidcrawler/testing/test_cmd.py
--rw-rw-rw-   0        0        0     1652 2022-05-16 05:08:52.000000 vidcrawler-1.0.8/vidcrawler/testing/test_io.py
--rw-rw-rw-   0        0        0     1856 2022-05-17 01:18:36.000000 vidcrawler-1.0.8/vidcrawler/testing/test_scraper_bitchute.py
--rw-rw-rw-   0        0        0      454 2022-05-16 05:04:57.000000 vidcrawler-1.0.8/vidcrawler/testing/test_scraper_brighteon.py
--rw-rw-rw-   0        0        0      737 2022-05-16 05:05:35.000000 vidcrawler-1.0.8/vidcrawler/testing/test_scraper_gabtv.py
--rw-rw-rw-   0        0        0     1436 2022-05-16 05:06:02.000000 vidcrawler-1.0.8/vidcrawler/testing/test_scraper_odysee.py
--rw-rw-rw-   0        0        0     1791 2022-05-26 03:40:39.000000 vidcrawler-1.0.8/vidcrawler/testing/test_scraper_rumble.py
--rw-rw-rw-   0        0        0      461 2022-05-16 05:06:15.000000 vidcrawler-1.0.8/vidcrawler/testing/test_scraper_spotify.py
--rw-rw-rw-   0        0        0      412 2022-05-16 05:06:20.000000 vidcrawler-1.0.8/vidcrawler/testing/test_scraper_spreaker.py
--rw-rw-rw-   0        0        0     3091 2022-06-10 07:11:23.000000 vidcrawler-1.0.8/vidcrawler/testing/test_scraper_youtube.py
--rw-rw-rw-   0        0        0     1176 2022-06-10 07:11:23.000000 vidcrawler-1.0.8/vidcrawler/testing/test_videoinfo.py
--rw-rw-rw-   0        0        0       41 2022-06-30 19:37:22.000000 vidcrawler-1.0.8/vidcrawler/version.py
--rw-rw-rw-   0        0        0     7986 2022-05-16 04:34:28.000000 vidcrawler-1.0.8/vidcrawler/video_info.py
--rw-rw-rw-   0        0        0    13611 2022-05-16 07:03:09.000000 vidcrawler-1.0.8/vidcrawler/youtube.py
-drwxrwxrwx   0        0        0        0 2022-06-30 19:38:07.699463 vidcrawler-1.0.8/vidcrawler.egg-info/
--rw-rw-rw-   0        0        0     3487 2022-06-30 19:38:07.000000 vidcrawler-1.0.8/vidcrawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1190 2022-06-30 19:38:07.000000 vidcrawler-1.0.8/vidcrawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-30 19:38:07.000000 vidcrawler-1.0.8/vidcrawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2022-06-30 19:38:07.000000 vidcrawler-1.0.8/vidcrawler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      111 2022-06-30 19:38:07.000000 vidcrawler-1.0.8/vidcrawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-06-30 19:38:07.000000 vidcrawler-1.0.8/vidcrawler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-10-09 03:08:19.174621 vidcrawler-1.0.9/
+-rw-rw-rw-   0        0        0     1064 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0       57 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3532 2022-10-09 03:08:19.173625 vidcrawler-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2804 2022-10-09 03:08:07.000000 vidcrawler-1.0.9/README.md
+-rw-rw-rw-   0        0        0       45 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/requirements.testing.txt
+-rw-rw-rw-   0        0        0      119 2022-10-09 01:10:57.000000 vidcrawler-1.0.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2022-10-09 03:08:19.174621 vidcrawler-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     3841 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-09 03:08:19.142625 vidcrawler-1.0.9/vidcrawler/
+-rw-rw-rw-   0        0        0       76 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/__init__.py
+-rw-rw-rw-   0        0        0     5323 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/bitchute.py
+-rw-rw-rw-   0        0        0     1910 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/brighteon.py
+-rw-rw-rw-   0        0        0     1580 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/cmd.py
+-rw-rw-rw-   0        0        0     2644 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/date.py
+-rw-rw-rw-   0        0        0      176 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/error.py
+-rw-rw-rw-   0        0        0     1391 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/fetch_html.py
+-rw-rw-rw-   0        0        0     4068 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/gabtv.py
+-rw-rw-rw-   0        0        0     2438 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/io.py
+-rw-rw-rw-   0        0        0     1814 2022-10-09 00:33:34.000000 vidcrawler-1.0.9/vidcrawler/odysee.py
+-rw-rw-rw-   0        0        0     4207 2022-10-09 01:12:01.000000 vidcrawler-1.0.9/vidcrawler/rumble.py
+-rw-rw-rw-   0        0        0      360 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/run_tests.py
+-rw-rw-rw-   0        0        0     6357 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/spider.py
+-rw-rw-rw-   0        0        0     3144 2022-10-09 03:07:17.000000 vidcrawler-1.0.9/vidcrawler/spotify.py
+-rw-rw-rw-   0        0        0     2145 2022-10-09 00:48:48.000000 vidcrawler-1.0.9/vidcrawler/spreaker.py
+drwxrwxrwx   0        0        0        0 2022-10-09 03:08:19.172622 vidcrawler-1.0.9/vidcrawler/testing/
+-rw-rw-rw-   0        0        0        0 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/testing/__init__.py
+-rw-rw-rw-   0        0        0     2698 2022-10-09 00:33:53.000000 vidcrawler-1.0.9/vidcrawler/testing/simple_http_server.py
+-rw-rw-rw-   0        0        0     1031 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/testing/test_cmd.py
+-rw-rw-rw-   0        0        0     1652 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/testing/test_io.py
+-rw-rw-rw-   0        0        0     1856 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/testing/test_scraper_bitchute.py
+-rw-rw-rw-   0        0        0      454 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/testing/test_scraper_brighteon.py
+-rw-rw-rw-   0        0        0      713 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/testing/test_scraper_gabtv.py
+-rw-rw-rw-   0        0        0     1600 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/testing/test_scraper_odysee.py
+-rw-rw-rw-   0        0        0     1742 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/testing/test_scraper_rumble.py
+-rw-rw-rw-   0        0        0      444 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/testing/test_scraper_spotify.py
+-rw-rw-rw-   0        0        0      397 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/testing/test_scraper_spreaker.py
+-rw-rw-rw-   0        0        0     3000 2022-10-09 00:36:01.000000 vidcrawler-1.0.9/vidcrawler/testing/test_scraper_youtube.py
+-rw-rw-rw-   0        0        0     1141 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/testing/test_videoinfo.py
+-rw-rw-rw-   0        0        0       38 2022-10-09 03:07:30.000000 vidcrawler-1.0.9/vidcrawler/version.py
+-rw-rw-rw-   0        0        0     7763 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/video_info.py
+-rw-rw-rw-   0        0        0    13255 2022-10-09 00:32:27.000000 vidcrawler-1.0.9/vidcrawler/youtube.py
+drwxrwxrwx   0        0        0        0 2022-10-09 03:08:19.158622 vidcrawler-1.0.9/vidcrawler.egg-info/
+-rw-rw-rw-   0        0        0     3532 2022-10-09 03:08:19.000000 vidcrawler-1.0.9/vidcrawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1190 2022-10-09 03:08:19.000000 vidcrawler-1.0.9/vidcrawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-09 03:08:19.000000 vidcrawler-1.0.9/vidcrawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2022-10-09 03:08:19.000000 vidcrawler-1.0.9/vidcrawler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      119 2022-10-09 03:08:19.000000 vidcrawler-1.0.9/vidcrawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2022-10-09 03:08:19.000000 vidcrawler-1.0.9/vidcrawler.egg-info/top_level.txt
```

### Comparing `vidcrawler-1.0.8/PKG-INFO` & `vidcrawler-1.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: vidcrawler
-Version: 1.0.8
+Version: 1.0.9
 Summary: Video Crawler
 Home-page: https://github.com/zackees/vidcrawler
 Author: Zach Vorhies
 Author-email: dont@email.me
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Environment :: Console
@@ -113,17 +112,15 @@
   {
       ...
   }
 ]
 ```
 
 # Releases
-
+  * 1.0.9: Fixes crawler for rumble and minor fixes + linting fixes.
   * 1.0.8: Readme correction.
   * 1.0.7: Fixes Odysee scraper by including image/webp thumbnail format.
   * 1.0.4: Fixes local_now() to be local timezone aware.
   * 1.0.3: Bump
   * 1.0.2: Updates testing
   * 1.0.1: improves command line
   * 1.0.0: Initial release
-
-
```

### Comparing `vidcrawler-1.0.8/README.md` & `vidcrawler-1.0.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-# vidcrawler
-
-Crawls major videos sites like YouTube/Rumble/Bitchute/Brighteon for video content and outputs a json feed of all the videos that were found.
-
-## Platform Unit Tests
-
-[![Actions Status](https://github.com/zackees/vidcrawler/workflows/MacOS_Tests/badge.svg)](https://github.com/zackees/vidcrawler/actions/workflows/test_macos.yml)
-[![Actions Status](https://github.com/zackees/vidcrawler/workflows/Win_Tests/badge.svg)](https://github.com/zackees/vidcrawler/actions/workflows/test_win.yml)
-[![Actions Status](https://github.com/zackees/vidcrawler/workflows/Ubuntu_Tests/badge.svg)](https://github.com/zackees/vidcrawler/actions/workflows/test_ubuntu.yml)
-
-## API
-
-#### Command line
-
-`vidcrawler --input_crawl_json "fetch_list.json" --output_json "out_list.json"`
-
-#### Python
-
-```
-import json
-from vidcrawler import crawl_video_sites
-
-crawl_list = [
-    ["channel name", "source", "channel_id"]
-]
-output = crawl_video_sites(crawl_list)
-print(json.dumps(output))
-```
-
-"source" and "channel_id" are used to generate the video-platform-specific urls to fetch data. The "channel name"
-is echo'd back in the generated json feeds, but doesn't not affect the fetching process in any way.
-
-## Testing
-
-Install vidcrawler and then the command `vidcralwer_test` will become available.
-
-```
-$ pip install vidcrawler
-$ vidcrawler_test
-```
-
-
-#### Example input `fetch_list.json`
-
-```
-[
-    [
-        "Health Ranger Report",
-        "brighteon",
-        "hrreport"
-    ],
-    [
-        "Sydney Watson",
-        "youtube",
-        "UCSFy-1JrpZf0tFlRZfo-Rvw"
-    ],
-    [
-        "Computing Forever",
-        "bitchute",
-        "hybm74uihjkf"
-    ],
-    [
-        "ThePeteSantilliShow",
-        "rumble",
-        "ThePeteSantilliShow"
-    ],
-    [
-        "Macroaggressions",
-        "odysee",
-        "Macroaggressions"
-    ]
-]
-```
-
-#### Example Output:
-
-```
-[
-  {
-    "channel_name": "ThePeteSantilliShow",
-    "title": "The damage this caused is now being totaled up",
-    "date_published": "2022-05-17T05:00:11+00:00",
-    "date_lastupdated": "2022-05-17T05:17:18.540084",
-    "channel_url": "https://www.youtube.com/channel/UCXIJgqnII2ZOINSWNOGFThA",
-    "source": "youtube.com",
-    "url": "https://www.youtube.com/watch?v=bwqBudCzDrQ",
-    "duration": 254,
-    "description": "",
-    "img_src": "https://i3.ytimg.com/vi/bwqBudCzDrQ/hqdefault.jpg",
-    "iframe_src": "https://youtube.com/embed/bwqBudCzDrQ",
-    "views": 1429
-  },
-  {
-      ...
-  }
-]
-```
-
-# Releases
-
-  * 1.0.8: Readme correction.
-  * 1.0.7: Fixes Odysee scraper by including image/webp thumbnail format.
-  * 1.0.4: Fixes local_now() to be local timezone aware.
-  * 1.0.3: Bump
-  * 1.0.2: Updates testing
-  * 1.0.1: improves command line
-  * 1.0.0: Initial release
+# vidcrawler
+
+Crawls major videos sites like YouTube/Rumble/Bitchute/Brighteon for video content and outputs a json feed of all the videos that were found.
+
+## Platform Unit Tests
+
+[![Actions Status](https://github.com/zackees/vidcrawler/workflows/MacOS_Tests/badge.svg)](https://github.com/zackees/vidcrawler/actions/workflows/test_macos.yml)
+[![Actions Status](https://github.com/zackees/vidcrawler/workflows/Win_Tests/badge.svg)](https://github.com/zackees/vidcrawler/actions/workflows/test_win.yml)
+[![Actions Status](https://github.com/zackees/vidcrawler/workflows/Ubuntu_Tests/badge.svg)](https://github.com/zackees/vidcrawler/actions/workflows/test_ubuntu.yml)
+
+## API
+
+#### Command line
+
+`vidcrawler --input_crawl_json "fetch_list.json" --output_json "out_list.json"`
+
+#### Python
+
+```
+import json
+from vidcrawler import crawl_video_sites
+
+crawl_list = [
+    ["channel name", "source", "channel_id"]
+]
+output = crawl_video_sites(crawl_list)
+print(json.dumps(output))
+```
+
+"source" and "channel_id" are used to generate the video-platform-specific urls to fetch data. The "channel name"
+is echo'd back in the generated json feeds, but doesn't not affect the fetching process in any way.
+
+## Testing
+
+Install vidcrawler and then the command `vidcralwer_test` will become available.
+
+```
+$ pip install vidcrawler
+$ vidcrawler_test
+```
+
+
+#### Example input `fetch_list.json`
+
+```
+[
+    [
+        "Health Ranger Report",
+        "brighteon",
+        "hrreport"
+    ],
+    [
+        "Sydney Watson",
+        "youtube",
+        "UCSFy-1JrpZf0tFlRZfo-Rvw"
+    ],
+    [
+        "Computing Forever",
+        "bitchute",
+        "hybm74uihjkf"
+    ],
+    [
+        "ThePeteSantilliShow",
+        "rumble",
+        "ThePeteSantilliShow"
+    ],
+    [
+        "Macroaggressions",
+        "odysee",
+        "Macroaggressions"
+    ]
+]
+```
+
+#### Example Output:
+
+```
+[
+  {
+    "channel_name": "ThePeteSantilliShow",
+    "title": "The damage this caused is now being totaled up",
+    "date_published": "2022-05-17T05:00:11+00:00",
+    "date_lastupdated": "2022-05-17T05:17:18.540084",
+    "channel_url": "https://www.youtube.com/channel/UCXIJgqnII2ZOINSWNOGFThA",
+    "source": "youtube.com",
+    "url": "https://www.youtube.com/watch?v=bwqBudCzDrQ",
+    "duration": 254,
+    "description": "",
+    "img_src": "https://i3.ytimg.com/vi/bwqBudCzDrQ/hqdefault.jpg",
+    "iframe_src": "https://youtube.com/embed/bwqBudCzDrQ",
+    "views": 1429
+  },
+  {
+      ...
+  }
+]
+```
+
+# Releases
+  * 1.0.9: Fixes crawler for rumble and minor fixes + linting fixes.
+  * 1.0.8: Readme correction.
+  * 1.0.7: Fixes Odysee scraper by including image/webp thumbnail format.
+  * 1.0.4: Fixes local_now() to be local timezone aware.
+  * 1.0.3: Bump
+  * 1.0.2: Updates testing
+  * 1.0.1: improves command line
+  * 1.0.0: Initial release
```

### Comparing `vidcrawler-1.0.8/setup.py` & `vidcrawler-1.0.9/setup.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-# pylint: disable=missing-function-docstring
-# pylint: disable=consider-using-f-string
-# pylint: disable=missing-module-docstring
-
-import os
-import sys
-from shutil import rmtree
-
-from setuptools import Command, find_packages, setup
-
-# The directory containing this file
-HERE = os.path.dirname(__file__)
-
-NAME = "vidcrawler"
-DESCRIPTION = "Video Crawler"
-URL = "https://github.com/zackees/vidcrawler"
-EMAIL = "dont@email.me"
-AUTHOR = "Zach Vorhies"
-REQUIRES_PYTHON = ">=3.6.0"
-VERSION = None
-
-# The text of the README file
-with open(os.path.join(HERE, "README.md"), encoding="utf-8", mode="rt") as fd:
-    LONG_DESCRIPTION = fd.read()
-
-with open(
-    os.path.join(HERE, "requirements.txt"), encoding="utf-8", mode="rt"
-) as fd:
-    REQUIREMENTS = [line.strip() for line in fd.readlines() if line.strip()]
-
-
-def get_requirements():
-    with open(
-        os.path.join(HERE, "requirements.txt"), encoding="utf-8", mode="rt"
-    ) as f:
-        packages = []
-        for line in f:
-            line = line.strip()
-            # let's also ignore empty lines and comments
-            if not line or line.startswith("#"):
-                continue
-            if "https://" in line:
-                tail = line.rsplit("/", 1)[1]
-                tail = tail.split("#")[0]
-                line = tail.replace("@", "==").replace(".git", "")
-            packages.append(line)
-    return packages
-
-
-def get_version() -> str:
-    version_file = os.path.join(HERE, NAME, "version.py")
-    with open(version_file, encoding="utf-8", mode="rt") as fd:
-        for line in fd.readlines():
-            if line.startswith("VERSION"):
-                VERSION = line.split("=")[1].strip().strip('"')
-                return VERSION
-    raise RuntimeError("Could not find version")
-
-
-VERSION = get_version()
-
-
-class UploadCommand(Command):
-    """Support setup.py upload."""
-
-    description = "Build and publish the package."
-    user_options = []
-
-    @staticmethod
-    def status(s):
-        pass
-
-    def initialize_options(self):
-        pass
-
-    def finalize_options(self):
-        pass
-
-    def run(self):
-        try:
-            self.status("Removing previous builds…")
-            rmtree(os.path.join(HERE, "dist"))
-        except OSError:
-            pass
-
-        self.status("Building Source and Wheel (universal) distribution…")
-
-        def exe(cmd: str) -> None:
-            print(f"Executing:\n  {cmd}\n")
-            return os.system(cmd)
-
-        exe(f'"{sys.executable}" setup.py sdist bdist_wheel --universal')
-
-        self.status("Uploading the package to PyPI via Twine…")
-        if 0 != exe("twine upload dist/*"):
-            raise RuntimeError("Upload failed")
-
-        self.status("Pushing git tags…")
-        exe(f"git tag v{VERSION} && git push --tags")
-
-        sys.exit()
-
-
-setup(
-    name=NAME,
-    python_requires=REQUIRES_PYTHON,
-    version=VERSION,
-    description=DESCRIPTION,
-    long_description=LONG_DESCRIPTION,
-    long_description_content_type="text/markdown",
-    url=URL,
-    author="Zach Vorhies",
-    author_email="dont@email.me",
-    license="MIT",
-    classifiers=[
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.9",
-        "Operating System :: Microsoft :: Windows",
-        "Operating System :: POSIX",
-        "Operating System :: MacOS :: MacOS X",
-        "Environment :: Console",
-    ],
-    install_requires=REQUIREMENTS,
-    packages=find_packages(
-        exclude=["tests", "*.tests", "*.tests.*", "tests.*"]
-    ),
-    package_data={},
-    include_package_data=True,
-    entry_points={
-        "console_scripts": [
-            "vidcrawler = vidcrawler.cmd:main",
-            "vidcrawler_test = vidcrawler.run_tests:main",
-        ],
-    },
-    cmdclass={
-        "upload": UploadCommand,
-    },
-)
+# pylint: disable=missing-function-docstring
+# pylint: disable=consider-using-f-string
+# pylint: disable=missing-module-docstring
+
+import os
+import sys
+from shutil import rmtree
+
+from setuptools import Command, find_packages, setup
+
+# The directory containing this file
+HERE = os.path.dirname(__file__)
+
+NAME = "vidcrawler"
+DESCRIPTION = "Video Crawler"
+URL = "https://github.com/zackees/vidcrawler"
+EMAIL = "dont@email.me"
+AUTHOR = "Zach Vorhies"
+REQUIRES_PYTHON = ">=3.6.0"
+VERSION = None
+
+# The text of the README file
+with open(os.path.join(HERE, "README.md"), encoding="utf-8", mode="rt") as fd:
+    LONG_DESCRIPTION = fd.read()
+
+with open(
+    os.path.join(HERE, "requirements.txt"), encoding="utf-8", mode="rt"
+) as fd:
+    REQUIREMENTS = [line.strip() for line in fd.readlines() if line.strip()]
+
+
+def get_requirements():
+    with open(
+        os.path.join(HERE, "requirements.txt"), encoding="utf-8", mode="rt"
+    ) as f:
+        packages = []
+        for line in f:
+            line = line.strip()
+            # let's also ignore empty lines and comments
+            if not line or line.startswith("#"):
+                continue
+            if "https://" in line:
+                tail = line.rsplit("/", 1)[1]
+                tail = tail.split("#")[0]
+                line = tail.replace("@", "==").replace(".git", "")
+            packages.append(line)
+    return packages
+
+
+def get_version() -> str:
+    version_file = os.path.join(HERE, NAME, "version.py")
+    with open(version_file, encoding="utf-8", mode="rt") as fd:
+        for line in fd.readlines():
+            if line.startswith("VERSION"):
+                VERSION = line.split("=")[1].strip().strip('"')
+                return VERSION
+    raise RuntimeError("Could not find version")
+
+
+VERSION = get_version()
+
+
+class UploadCommand(Command):
+    """Support setup.py upload."""
+
+    description = "Build and publish the package."
+    user_options = []
+
+    @staticmethod
+    def status(s):
+        pass
+
+    def initialize_options(self):
+        pass
+
+    def finalize_options(self):
+        pass
+
+    def run(self):
+        try:
+            self.status("Removing previous builds…")
+            rmtree(os.path.join(HERE, "dist"))
+        except OSError:
+            pass
+
+        self.status("Building Source and Wheel (universal) distribution…")
+
+        def exe(cmd: str) -> None:
+            print(f"Executing:\n  {cmd}\n")
+            return os.system(cmd)
+
+        exe(f'"{sys.executable}" setup.py sdist bdist_wheel --universal')
+
+        self.status("Uploading the package to PyPI via Twine…")
+        if 0 != exe("twine upload dist/*"):
+            raise RuntimeError("Upload failed")
+
+        self.status("Pushing git tags…")
+        exe(f"git tag v{VERSION} && git push --tags")
+
+        sys.exit()
+
+
+setup(
+    name=NAME,
+    python_requires=REQUIRES_PYTHON,
+    version=VERSION,
+    description=DESCRIPTION,
+    long_description=LONG_DESCRIPTION,
+    long_description_content_type="text/markdown",
+    url=URL,
+    author="Zach Vorhies",
+    author_email="dont@email.me",
+    license="MIT",
+    classifiers=[
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.9",
+        "Operating System :: Microsoft :: Windows",
+        "Operating System :: POSIX",
+        "Operating System :: MacOS :: MacOS X",
+        "Environment :: Console",
+    ],
+    install_requires=REQUIREMENTS,
+    packages=find_packages(
+        exclude=["tests", "*.tests", "*.tests.*", "tests.*"]
+    ),
+    package_data={},
+    include_package_data=True,
+    entry_points={
+        "console_scripts": [
+            "vidcrawler = vidcrawler.cmd:main",
+            "vidcrawler_test = vidcrawler.run_tests:main",
+        ],
+    },
+    cmdclass={
+        "upload": UploadCommand,
+    },
+)
```

### Comparing `vidcrawler-1.0.8/vidcrawler/bitchute.py` & `vidcrawler-1.0.9/vidcrawler/bitchute.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-"""
-    Scraper for bitchute
-"""
-
-# pylint: disable=line-too-long,missing-function-docstring,consider-using-f-string,too-many-locals,invalid-name
-
-import html
-import re
-import sys
-from typing import List, Optional
-
-import feedparser  # type: ignore
-from bs4 import BeautifulSoup  # type: ignore
-
-from .date import iso_fmt, now_local
-from .error import log_error
-
-# bitchute is bombing out on CURL so switch to the request-lib get version.
-from .fetch_html import fetch_html_using_request_lib
-from .video_info import VideoInfo
-
-_EMBED_BITCHUTE_PATT = r"/video/(.+)/"
-USER_AGENT = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/50.0.2661.102 Safari/537.36"
-
-
-def fetch_html(url: str) -> str:
-    return fetch_html_using_request_lib(url, user_agent=USER_AGENT)
-
-
-def parse_rss_url(html_doc: str) -> Optional[str]:
-    top_dom = BeautifulSoup(html_doc, "html.parser")
-    details_dom = top_dom.find("div", class_="details")
-    if not details_dom:
-        return None
-    inner_dom = details_dom.find("p", class_="name")
-    if not inner_dom:
-        return None
-    attrs = inner_dom.find("a")
-    suffix = attrs["href"]
-    rss_url: str = "https://www.bitchute.com/feeds/rss" + suffix
-    return rss_url
-
-
-def fetch_rss_url(
-    channel_name: str, channel_id: str  # pylint: disable=unused-argument
-) -> Optional[str]:
-    channel_url = "https://www.bitchute.com/channel/%s/" % channel_id
-    html_doc = fetch_html(channel_url)
-    return parse_rss_url(html_doc)
-
-
-def parse_rss_feed(content: str) -> List[dict]:
-    feed = feedparser.parse(content)
-    channel_url = feed["feed"]["link"]
-    # from pprint import pprint
-    output: List[dict] = []
-    for entry in feed.entries:
-        date_published = entry["published"]
-        summary = entry["summary"]
-        title = entry["title"]
-        id = entry["id"]  # pylint: disable=redefined-builtin
-        try:
-            type_ = entry["title_detail"]["type"]
-            if type_ == "text/html":
-                title = html.unescape(title)
-        except BaseException as err:  # pylint: disable=broad-except
-            log_error(f"Error while parsing because of {str(err)}")
-        links = entry["links"]
-        embed_link = links[0]["href"]
-        img_link = links[1]["href"]
-        id = re.findall(r".*/embed/([^\/]+)/", entry["link"])[0]
-        obj = dict(
-            title=title,
-            date_published=date_published,
-            alt_channel_url=channel_url,
-            description=summary,
-            img_src=img_link,
-            iframe_src=embed_link,
-            url="https://www.bitchute.com/video/%s" % id,
-        )
-        output.append(obj)
-    return output
-
-
-# type: ignore
-
-
-def fetch_bitchute_today(channel_name: str, channel_id: str) -> List[VideoInfo]:
-    output: List[VideoInfo] = []
-    channel_url = "https://www.bitchute.com/channel/%s/" % channel_id
-    sys.stdout.write(
-        "Bitchute visiting %s (%s)\n" % (channel_name, channel_url)
-    )
-    html_doc = fetch_html(channel_url)
-    rss_url = parse_rss_url(html_doc)
-    date_published_map = {}
-    if rss_url is None:
-        sys.stderr.write(
-            "---- ERROR ---- Failed to parse rss_channel for %s\n" % channel_url
-        )
-    else:
-        rss_content = fetch_html(rss_url)
-        # These objects contain the video publishing date.
-        rss_objects: List[dict] = parse_rss_feed(rss_content)
-        rss_obj: dict
-        for rss_obj in rss_objects:
-            key = rss_obj["url"]
-            date_published_map[key] = iso_fmt(rss_obj["date_published"])
-    soup = BeautifulSoup(html_doc, "html.parser")
-    vid_divs = soup.find_all(class_="channel-videos-container")
-    skipped_vid_urls: List[str] = []
-    for vd in vid_divs:
-        title_dom = vd.find(class_="channel-videos-title")
-        spa_dom = title_dom.find(class_="spa")
-        title_text = spa_dom.text
-        views_text = vd.find(class_="video-views").text.strip()
-        video_src = spa_dom["href"]
-        vid_id = re.findall(_EMBED_BITCHUTE_PATT, video_src)[0]
-        iframe_src = "https://www.bitchute.com/embed/%s" % vid_id
-        url = "https://www.bitchute.com/video/%s" % vid_id
-        duration = vd.find(class_="video-duration").text  # type: ignore
-        # poster_dom = plyr__poster
-        poster_dom = vd.find(class_="channel-videos-image")
-        img_src = poster_dom.find("img")["data-src"]
-        now_datestr = now_local().isoformat()
-        date_published = date_published_map.get(url)
-        if date_published is None:
-            skipped_vid_urls.append(url)
-            continue
-        o = VideoInfo(
-            channel_name=channel_name,
-            source="bitchute.com",
-            date_published=date_published,
-            date_discovered=now_datestr,
-            date_lastupdated=now_datestr,
-            url=url,
-            channel_url=channel_url,
-            title=title_text,
-            duration=duration,
-            description="TODO",
-            img_src=img_src,
-            iframe_src=iframe_src,
-            views=views_text,
-            profile_img_src="",
-        )
-        output.append(o)
-    if skipped_vid_urls:
-        sys.stdout.write(
-            f"{__file__}: Skipping {len(skipped_vid_urls)} videos from {channel_name} because no data from rss.\n"
-        )
-    return output
+"""
+    Scraper for bitchute
+"""
+
+# pylint: disable=line-too-long,missing-function-docstring,consider-using-f-string,too-many-locals,invalid-name
+
+import html
+import re
+import sys
+from typing import List, Optional
+
+import feedparser  # type: ignore
+from bs4 import BeautifulSoup  # type: ignore
+
+from .date import iso_fmt, now_local
+from .error import log_error
+
+# bitchute is bombing out on CURL so switch to the request-lib get version.
+from .fetch_html import fetch_html_using_request_lib
+from .video_info import VideoInfo
+
+_EMBED_BITCHUTE_PATT = r"/video/(.+)/"
+USER_AGENT = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/50.0.2661.102 Safari/537.36"
+
+
+def fetch_html(url: str) -> str:
+    return fetch_html_using_request_lib(url, user_agent=USER_AGENT)
+
+
+def parse_rss_url(html_doc: str) -> Optional[str]:
+    top_dom = BeautifulSoup(html_doc, "html.parser")
+    details_dom = top_dom.find("div", class_="details")
+    if not details_dom:
+        return None
+    inner_dom = details_dom.find("p", class_="name")
+    if not inner_dom:
+        return None
+    attrs = inner_dom.find("a")
+    suffix = attrs["href"]
+    rss_url: str = "https://www.bitchute.com/feeds/rss" + suffix
+    return rss_url
+
+
+def fetch_rss_url(
+    channel_name: str, channel_id: str  # pylint: disable=unused-argument
+) -> Optional[str]:
+    channel_url = "https://www.bitchute.com/channel/%s/" % channel_id
+    html_doc = fetch_html(channel_url)
+    return parse_rss_url(html_doc)
+
+
+def parse_rss_feed(content: str) -> List[dict]:
+    feed = feedparser.parse(content)
+    channel_url = feed["feed"]["link"]
+    # from pprint import pprint
+    output: List[dict] = []
+    for entry in feed.entries:
+        date_published = entry["published"]
+        summary = entry["summary"]
+        title = entry["title"]
+        id = entry["id"]  # pylint: disable=redefined-builtin
+        try:
+            type_ = entry["title_detail"]["type"]
+            if type_ == "text/html":
+                title = html.unescape(title)
+        except BaseException as err:  # pylint: disable=broad-except
+            log_error(f"Error while parsing because of {str(err)}")
+        links = entry["links"]
+        embed_link = links[0]["href"]
+        img_link = links[1]["href"]
+        id = re.findall(r".*/embed/([^\/]+)/", entry["link"])[0]
+        obj = dict(
+            title=title,
+            date_published=date_published,
+            alt_channel_url=channel_url,
+            description=summary,
+            img_src=img_link,
+            iframe_src=embed_link,
+            url="https://www.bitchute.com/video/%s" % id,
+        )
+        output.append(obj)
+    return output
+
+
+# type: ignore
+
+
+def fetch_bitchute_today(channel_name: str, channel_id: str) -> List[VideoInfo]:
+    output: List[VideoInfo] = []
+    channel_url = "https://www.bitchute.com/channel/%s/" % channel_id
+    sys.stdout.write(
+        "Bitchute visiting %s (%s)\n" % (channel_name, channel_url)
+    )
+    html_doc = fetch_html(channel_url)
+    rss_url = parse_rss_url(html_doc)
+    date_published_map = {}
+    if rss_url is None:
+        sys.stderr.write(
+            "---- ERROR ---- Failed to parse rss_channel for %s\n" % channel_url
+        )
+    else:
+        rss_content = fetch_html(rss_url)
+        # These objects contain the video publishing date.
+        rss_objects: List[dict] = parse_rss_feed(rss_content)
+        rss_obj: dict
+        for rss_obj in rss_objects:
+            key = rss_obj["url"]
+            date_published_map[key] = iso_fmt(rss_obj["date_published"])
+    soup = BeautifulSoup(html_doc, "html.parser")
+    vid_divs = soup.find_all(class_="channel-videos-container")
+    skipped_vid_urls: List[str] = []
+    for vd in vid_divs:
+        title_dom = vd.find(class_="channel-videos-title")
+        spa_dom = title_dom.find(class_="spa")
+        title_text = spa_dom.text
+        views_text = vd.find(class_="video-views").text.strip()
+        video_src = spa_dom["href"]
+        vid_id = re.findall(_EMBED_BITCHUTE_PATT, video_src)[0]
+        iframe_src = "https://www.bitchute.com/embed/%s" % vid_id
+        url = "https://www.bitchute.com/video/%s" % vid_id
+        duration = vd.find(class_="video-duration").text  # type: ignore
+        # poster_dom = plyr__poster
+        poster_dom = vd.find(class_="channel-videos-image")
+        img_src = poster_dom.find("img")["data-src"]
+        now_datestr = now_local().isoformat()
+        date_published = date_published_map.get(url)
+        if date_published is None:
+            skipped_vid_urls.append(url)
+            continue
+        o = VideoInfo(
+            channel_name=channel_name,
+            source="bitchute.com",
+            date_published=date_published,
+            date_discovered=now_datestr,
+            date_lastupdated=now_datestr,
+            url=url,
+            channel_url=channel_url,
+            title=title_text,
+            duration=duration,
+            description="TODO",
+            img_src=img_src,
+            iframe_src=iframe_src,
+            views=views_text,
+            profile_img_src="",
+        )
+        output.append(o)
+    if skipped_vid_urls:
+        sys.stdout.write(
+            f"{__file__}: Skipping {len(skipped_vid_urls)} videos from {channel_name} because no data from rss.\n"
+        )
+    return output
```

### Comparing `vidcrawler-1.0.8/vidcrawler/brighteon.py` & `vidcrawler-1.0.9/vidcrawler/brighteon.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-"""
-    Scraper for Brighteon.com
-"""
-
-# pylint: disable=line-too-long,missing-function-docstring,consider-using-f-string,too-many-locals,invalid-name,no-else-return
-
-
-import json
-import sys
-from typing import List
-
-from bs4 import BeautifulSoup  # type: ignore
-
-from .date import iso_fmt, now_local
-from .fetch_html import fetch_html_using_request_lib as fetch_html
-from .video_info import VideoInfo
-
-
-def fetch_brighteon_today(channel_name: str, channel: str) -> List[VideoInfo]:
-    output: List[VideoInfo] = []
-    url = "https://www.brighteon.com/channels/%s" % channel
-    sys.stdout.write("Brighteon visiting %s (%s)\n" % (channel, url))
-    html_doc = fetch_html(url)
-    soup = BeautifulSoup(html_doc, "html.parser")
-    json_data = soup.find("script", id="__NEXT_DATA__").string
-    data = json.loads(json_data)
-    channel_data = data["props"]["initialProps"]["pageProps"]["data"]
-    videos = channel_data["videos"]
-    for vid in videos:
-        created_time = vid["createdAt"]
-        id = vid["id"]  # pylint: disable=redefined-builtin
-        iframe_url = "https://www.brighteon.com/embed%s" % id
-        video_url = "https://www.brighteon.com/%s" % id
-        title = vid["name"]
-        image_src = vid["thumbnail"]
-        view_count = vid["analytics"]["videoView"]
-        duration = vid["duration"]
-        now_datestr = iso_fmt(now_local())
-        o = VideoInfo(
-            channel_name=channel_name,
-            source="brighteon.com",
-            date_published=created_time,
-            date_discovered=now_datestr,
-            date_lastupdated=now_datestr,
-            url=video_url,
-            channel_url=url,
-            title=title,
-            duration=duration,
-            description="TODO",
-            img_src=image_src,
-            iframe_src=iframe_url,
-            views=view_count,
-            profile_img_src="",
-        )
-        output.append(o)
-    return output
+"""
+    Scraper for Brighteon.com
+"""
+
+# pylint: disable=line-too-long,missing-function-docstring,consider-using-f-string,too-many-locals,invalid-name,no-else-return
+
+
+import json
+import sys
+from typing import List
+
+from bs4 import BeautifulSoup  # type: ignore
+
+from .date import iso_fmt, now_local
+from .fetch_html import fetch_html_using_request_lib as fetch_html
+from .video_info import VideoInfo
+
+
+def fetch_brighteon_today(channel_name: str, channel: str) -> List[VideoInfo]:
+    output: List[VideoInfo] = []
+    url = "https://www.brighteon.com/channels/%s" % channel
+    sys.stdout.write("Brighteon visiting %s (%s)\n" % (channel, url))
+    html_doc = fetch_html(url)
+    soup = BeautifulSoup(html_doc, "html.parser")
+    json_data = soup.find("script", id="__NEXT_DATA__").string
+    data = json.loads(json_data)
+    channel_data = data["props"]["initialProps"]["pageProps"]["data"]
+    videos = channel_data["videos"]
+    for vid in videos:
+        created_time = vid["createdAt"]
+        id = vid["id"]  # pylint: disable=redefined-builtin
+        iframe_url = "https://www.brighteon.com/embed%s" % id
+        video_url = "https://www.brighteon.com/%s" % id
+        title = vid["name"]
+        image_src = vid["thumbnail"]
+        view_count = vid["analytics"]["videoView"]
+        duration = vid["duration"]
+        now_datestr = iso_fmt(now_local())
+        o = VideoInfo(
+            channel_name=channel_name,
+            source="brighteon.com",
+            date_published=created_time,
+            date_discovered=now_datestr,
+            date_lastupdated=now_datestr,
+            url=video_url,
+            channel_url=url,
+            title=title,
+            duration=duration,
+            description="TODO",
+            img_src=image_src,
+            iframe_src=iframe_url,
+            views=view_count,
+            profile_img_src="",
+        )
+        output.append(o)
+    return output
```

### Comparing `vidcrawler-1.0.8/vidcrawler/cmd.py` & `vidcrawler-1.0.9/vidcrawler/cmd.py`

 * *Files identical despite different names*

### Comparing `vidcrawler-1.0.8/vidcrawler/fetch_html.py` & `vidcrawler-1.0.9/vidcrawler/fetch_html.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-"""
-Fetcher for html
-"""
-
-import subprocess
-
-# pylint: disable=line-too-long,missing-function-docstring,consider-using-f-string,too-many-locals,invalid-name,no-else-return
-from typing import Optional
-
-import requests
-
-try:
-    subprocess.check_output("curl --version", shell=True)
-    USE_CURL = True
-except BaseException:  # pylint: disable=broad-except
-    USE_CURL = False
-
-
-def fetch_html_using_request_lib(
-    url: str,
-    timeout: Optional[int] = None,
-    user_agent: Optional[str] = None,
-) -> str:
-    timeout = timeout or 10
-    # Workaround for long request time on windows
-    # see https://github.com/psf/requests/issues/4023
-    headers = {"Connection": "close"}
-    # headers = {"Connection": "close"}
-    if user_agent:
-        headers["User-Agent"] = user_agent
-    resp = requests.get(url, timeout=timeout, params={}, headers=headers)
-    resp.raise_for_status()
-    return resp.content.decode(resp.apparent_encoding)
-
-
-def fetch_html_using_curl(url: str, timeout: Optional[int] = None) -> str:
-    """Uses the curl library to do a fetch"""
-    timeout = int(timeout or 10)
-    out: bytes = subprocess.check_output(
-        f"curl --max-time {timeout} -s -X GET {url}", shell=True
-    )
-    return out.decode("utf-8")
-
-
-def fetch_html(url: str) -> str:
-    if USE_CURL:
-        return fetch_html_using_curl(url)
-    else:
-        return fetch_html_using_request_lib(url)
+"""
+Fetcher for html
+"""
+
+import subprocess
+
+# pylint: disable=line-too-long,missing-function-docstring,consider-using-f-string,too-many-locals,invalid-name,no-else-return
+from typing import Optional
+
+import requests
+
+try:
+    subprocess.check_output("curl --version", shell=True)
+    USE_CURL = True
+except BaseException:  # pylint: disable=broad-except
+    USE_CURL = False
+
+
+def fetch_html_using_request_lib(
+    url: str,
+    timeout: Optional[int] = None,
+    user_agent: Optional[str] = None,
+) -> str:
+    timeout = timeout or 10
+    # Workaround for long request time on windows
+    # see https://github.com/psf/requests/issues/4023
+    headers = {"Connection": "close"}
+    # headers = {"Connection": "close"}
+    if user_agent:
+        headers["User-Agent"] = user_agent
+    resp = requests.get(url, timeout=timeout, params={}, headers=headers)
+    resp.raise_for_status()
+    return resp.content.decode(resp.apparent_encoding)
+
+
+def fetch_html_using_curl(url: str, timeout: Optional[int] = None) -> str:
+    """Uses the curl library to do a fetch"""
+    timeout = int(timeout or 10)
+    out: bytes = subprocess.check_output(
+        f"curl --max-time {timeout} -s -X GET {url}", shell=True
+    )
+    return out.decode("utf-8")
+
+
+def fetch_html(url: str) -> str:
+    if USE_CURL:
+        return fetch_html_using_curl(url)
+    else:
+        return fetch_html_using_request_lib(url)
```

### Comparing `vidcrawler-1.0.8/vidcrawler/gabtv.py` & `vidcrawler-1.0.9/vidcrawler/gabtv.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-"""
-    Scraper for gabtv.com
-"""
-
-# pylint: disable=line-too-long,missing-function-docstring,consider-using-f-string,too-many-locals,invalid-name,no-else-return,redefined-builtin,W0511
-
-import json
-import re
-import subprocess
-import sys
-from typing import Dict, List
-
-from bs4 import BeautifulSoup  # type: ignore
-
-from .date import iso_fmt, now_local
-from .error import log_error
-from .video_info import VideoInfo
-
-_PATTERN_DATA_EPISODE_ID = re.compile('data-episode-id="([^"]*)"')
-
-
-def _fetch_html_using_curl(url: str) -> str:
-    out: bytes = subprocess.check_output(
-        "curl --max-time 10 -s -X GET " + url, shell=True
-    )
-    return out.decode("utf-8")
-
-
-def fetch_views(channel: str) -> Dict[str, str]:
-    out: Dict[str, str] = {}
-    html_url: str = f"https://tv.gab.com/channel/{channel}"
-    html_doc: str = _fetch_html_using_curl(html_url)
-    soup = BeautifulSoup(html_doc, "html.parser")
-    top_dom = soup.find("div", {"class": "tv-channel-episode-list"})
-    dom_episodes = top_dom.findAll("div")
-    for i, dom_episode in enumerate(dom_episodes):
-        str_episode = str(dom_episode)
-        if "data-episode-id" not in str_episode:
-            continue
-        try:
-            id = _PATTERN_DATA_EPISODE_ID.findall(str_episode)[0]
-        except IndexError as e:
-            raise IndexError(f"idx: {i}, url: {html_url}") from e
-        dom_published = dom_episode.find("div", {"class": "studio-episode-published"})
-        dom_spans = dom_published.findAll("span")
-        views = dom_spans[0].text
-        out[id] = views
-    return out
-
-
-def fetch_gabtv_today(channel_name: str, channel_id: str) -> List[VideoInfo]:
-    now_datestr = iso_fmt(now_local())
-    # GabTV does not PUBLISH VIEWS IN IT'S FEED, so scrape them from the html
-    # here.
-    out: List[VideoInfo] = []
-    view_data = fetch_views(channel_id)
-    channel_url = f"https://tv.gab.com/channel/{channel_id}"
-    json_feed_url: str = f"https://tv.gab.com/channel/{channel_id}/feed/json"
-    # Note: Gab.TV currently returns 403 when using the request lib. The
-    # work-around (for now) is to use the curl alternative. Gab should be
-    # notified of this limitation and if possible, we should go back to using
-    # the request lib to fetch this data.
-    json_str = _fetch_html_using_curl(json_feed_url)
-    data = json.loads(json_str)
-    for item in data["items"]:
-        try:
-            url: str = item["url"]
-            id: str = item["id"]
-            title: str = item["title"]
-            # Summary is sometimes empty.
-            summary: str = item.get("summary", "")
-            image: str = item["image"]
-            published_date: str = item["date_modified"]
-        except KeyError as ke:
-            log_error(err_str=f"Error while parsing {channel_id} because of {ke}\n")
-            continue
-
-        # GabTV does not PUBLISH VIEWS IN IT'S FEED.
-        # print(url)
-        views = view_data.get(id)
-        if views is None:
-            sys.stderr.write(f"{__file__}: Warning, views for {url} is None\n")
-            views = "?"
-        vi = VideoInfo(
-            channel_name=channel_name,
-            title=title,
-            date_published=published_date,
-            date_discovered=now_datestr,
-            date_lastupdated=now_datestr,
-            channel_url=channel_url,
-            source="tv.gab.com",
-            url=url,
-            duration="?",  # TODO: get this
-            description=summary,
-            img_src=image,
-            iframe_src="",  # No iframe source yet
-            views=views,
-            profile_img_src="",
-        )
-        out.append(vi)
-    return out
-
-
-def test() -> None:
-    from pprint import pprint  # pylint: disable=import-outside-toplevel
-
-    channel_id: str = input("Enter Channel ID: ")
-    channel_name: str = input("Enter Channel Name: ")
-    vids: List[VideoInfo] = fetch_gabtv_today(
-        channel_name=channel_name, channel_id=channel_id
-    )
-    print("First two videos:")
-    vids = vids[0:2]
-    for v in vids:
-        pprint(v.to_dict())
-
-
-if __name__ == "__main__":
-    test()
+"""
+    Scraper for gabtv.com
+"""
+
+# pylint: disable=line-too-long,missing-function-docstring,consider-using-f-string,too-many-locals,invalid-name,no-else-return,redefined-builtin,W0511
+
+import json
+import re
+import subprocess
+import sys
+from typing import Dict, List
+
+from bs4 import BeautifulSoup  # type: ignore
+
+from .date import iso_fmt, now_local
+from .error import log_error
+from .video_info import VideoInfo
+
+_PATTERN_DATA_EPISODE_ID = re.compile('data-episode-id="([^"]*)"')
+
+
+def _fetch_html_using_curl(url: str) -> str:
+    out: bytes = subprocess.check_output(
+        "curl --max-time 10 -s -X GET " + url, shell=True
+    )
+    return out.decode("utf-8")
+
+
+def fetch_views(channel: str) -> Dict[str, str]:
+    out: Dict[str, str] = {}
+    html_url: str = f"https://tv.gab.com/channel/{channel}"
+    html_doc: str = _fetch_html_using_curl(html_url)
+    soup = BeautifulSoup(html_doc, "html.parser")
+    top_dom = soup.find("div", {"class": "tv-channel-episode-list"})
+    dom_episodes = top_dom.findAll("div")
+    for i, dom_episode in enumerate(dom_episodes):
+        str_episode = str(dom_episode)
+        if "data-episode-id" not in str_episode:
+            continue
+        try:
+            id = _PATTERN_DATA_EPISODE_ID.findall(str_episode)[0]
+        except IndexError as e:
+            raise IndexError(f"idx: {i}, url: {html_url}") from e
+        dom_published = dom_episode.find("div", {"class": "studio-episode-published"})
+        dom_spans = dom_published.findAll("span")
+        views = dom_spans[0].text
+        out[id] = views
+    return out
+
+
+def fetch_gabtv_today(channel_name: str, channel_id: str) -> List[VideoInfo]:
+    now_datestr = iso_fmt(now_local())
+    # GabTV does not PUBLISH VIEWS IN IT'S FEED, so scrape them from the html
+    # here.
+    out: List[VideoInfo] = []
+    view_data = fetch_views(channel_id)
+    channel_url = f"https://tv.gab.com/channel/{channel_id}"
+    json_feed_url: str = f"https://tv.gab.com/channel/{channel_id}/feed/json"
+    # Note: Gab.TV currently returns 403 when using the request lib. The
+    # work-around (for now) is to use the curl alternative. Gab should be
+    # notified of this limitation and if possible, we should go back to using
+    # the request lib to fetch this data.
+    json_str = _fetch_html_using_curl(json_feed_url)
+    data = json.loads(json_str)
+    for item in data["items"]:
+        try:
+            url: str = item["url"]
+            id: str = item["id"]
+            title: str = item["title"]
+            # Summary is sometimes empty.
+            summary: str = item.get("summary", "")
+            image: str = item["image"]
+            published_date: str = item["date_modified"]
+        except KeyError as ke:
+            log_error(err_str=f"Error while parsing {channel_id} because of {ke}\n")
+            continue
+
+        # GabTV does not PUBLISH VIEWS IN IT'S FEED.
+        # print(url)
+        views = view_data.get(id)
+        if views is None:
+            sys.stderr.write(f"{__file__}: Warning, views for {url} is None\n")
+            views = "?"
+        vi = VideoInfo(
+            channel_name=channel_name,
+            title=title,
+            date_published=published_date,
+            date_discovered=now_datestr,
+            date_lastupdated=now_datestr,
+            channel_url=channel_url,
+            source="tv.gab.com",
+            url=url,
+            duration="?",  # TODO: get this
+            description=summary,
+            img_src=image,
+            iframe_src="",  # No iframe source yet
+            views=views,
+            profile_img_src="",
+        )
+        out.append(vi)
+    return out
+
+
+def test() -> None:
+    from pprint import pprint  # pylint: disable=import-outside-toplevel
+
+    channel_id: str = input("Enter Channel ID: ")
+    channel_name: str = input("Enter Channel Name: ")
+    vids: List[VideoInfo] = fetch_gabtv_today(
+        channel_name=channel_name, channel_id=channel_id
+    )
+    print("First two videos:")
+    vids = vids[0:2]
+    for v in vids:
+        pprint(v.to_dict())
+
+
+if __name__ == "__main__":
+    test()
```

### Comparing `vidcrawler-1.0.8/vidcrawler/io.py` & `vidcrawler-1.0.9/vidcrawler/io.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-"""
-Utilities for reading and writing files.
-"""
-
-# pylint: disable=missing-function-docstring,too-many-arguments,too-many-locals,too-many-statements,line-too-long,invalid-name
-
-import gzip
-import json
-import os
-import sys
-from datetime import datetime
-from typing import Any, Dict, List
-
-from .date import iso_fmt
-from .video_info import VideoInfo
-
-
-def write_gzip(out_path: str, content: bytes) -> None:
-    assert out_path.endswith(".gz")
-    with gzip.open(out_path, "wb") as f:
-        f.write(content)
-
-
-def write_utf8(out_path: str, content: str) -> None:
-    out_path = os.path.normpath(out_path)
-    dir_path: str = os.path.dirname(out_path)
-    os.makedirs(dir_path, exist_ok=True)
-    with open(out_path, "w", encoding="utf-8") as fd:
-        fd.write(content)
-
-
-def make_export_json(
-    now: datetime, content: List[Any], network_name: str, telegram: str
-) -> Dict[str, Any]:
-    # Type check, do we have a list of VideoInfo objects? If so convert to a list of dicts.
-    if len(content) > 0:
-        first = content[0]
-        if isinstance(first, VideoInfo):
-            content = VideoInfo.to_plain_list(content)
-    return {
-        "network_name": network_name,
-        "__update_time": iso_fmt(now),
-        "telegram": telegram,
-        "content": content,
-    }
-
-
-def write_json(out_path: str, content: Any, also_gzip: bool = False, minify: bool = False, **kwargs) -> None:  # type: ignore
-    """
-    If zip is True, then the same json file will ALSO be written out
-    with the extension *.zip and a single file inside labeled data.json.
-    """
-    assert "gzip" not in kwargs
-    if not minify:
-        kwargs["indent"] = 2
-    out_utf8 = json.dumps(content, ensure_ascii=False, **kwargs)
-    write_utf8(out_path, out_utf8)
-    if also_gzip:
-        if "indent" in kwargs:
-            del kwargs["indent"]
-        out_utf8 = json.dumps(content, ensure_ascii=False, **kwargs)
-        write_gzip(out_path + ".gz", out_utf8.encode("utf-8"))
-
-
-def read_utf8(in_path: str) -> str:
-    in_path = os.path.normpath(in_path)
-    with open(in_path, "r", encoding="utf-8") as fd:
-        return fd.read()
-
-
-def trap_win32_keyboard_interrupt_here() -> None:
-    if sys.platform == "win32":  # Play better with ctrl-c
-        import signal  # pylint: disable=import-outside-toplevel
-
-        def raise_exc(a: Any, b: Any) -> None:
-            raise KeyboardInterrupt("ctrl-c")
-
-        signal.signal(signal.SIGINT, raise_exc)
+"""
+Utilities for reading and writing files.
+"""
+
+# pylint: disable=missing-function-docstring,too-many-arguments,too-many-locals,too-many-statements,line-too-long,invalid-name
+
+import gzip
+import json
+import os
+import sys
+from datetime import datetime
+from typing import Any, Dict, List
+
+from .date import iso_fmt
+from .video_info import VideoInfo
+
+
+def write_gzip(out_path: str, content: bytes) -> None:
+    assert out_path.endswith(".gz")
+    with gzip.open(out_path, "wb") as f:
+        f.write(content)
+
+
+def write_utf8(out_path: str, content: str) -> None:
+    out_path = os.path.normpath(out_path)
+    dir_path: str = os.path.dirname(out_path)
+    os.makedirs(dir_path, exist_ok=True)
+    with open(out_path, "w", encoding="utf-8") as fd:
+        fd.write(content)
+
+
+def make_export_json(
+    now: datetime, content: List[Any], network_name: str, telegram: str
+) -> Dict[str, Any]:
+    # Type check, do we have a list of VideoInfo objects? If so convert to a list of dicts.
+    if len(content) > 0:
+        first = content[0]
+        if isinstance(first, VideoInfo):
+            content = VideoInfo.to_plain_list(content)
+    return {
+        "network_name": network_name,
+        "__update_time": iso_fmt(now),
+        "telegram": telegram,
+        "content": content,
+    }
+
+
+def write_json(out_path: str, content: Any, also_gzip: bool = False, minify: bool = False, **kwargs) -> None:  # type: ignore
+    """
+    If zip is True, then the same json file will ALSO be written out
+    with the extension *.zip and a single file inside labeled data.json.
+    """
+    assert "gzip" not in kwargs
+    if not minify:
+        kwargs["indent"] = 2
+    out_utf8 = json.dumps(content, ensure_ascii=False, **kwargs)
+    write_utf8(out_path, out_utf8)
+    if also_gzip:
+        if "indent" in kwargs:
+            del kwargs["indent"]
+        out_utf8 = json.dumps(content, ensure_ascii=False, **kwargs)
+        write_gzip(out_path + ".gz", out_utf8.encode("utf-8"))
+
+
+def read_utf8(in_path: str) -> str:
+    in_path = os.path.normpath(in_path)
+    with open(in_path, "r", encoding="utf-8") as fd:
+        return fd.read()
+
+
+def trap_win32_keyboard_interrupt_here() -> None:
+    if sys.platform == "win32":  # Play better with ctrl-c
+        import signal  # pylint: disable=import-outside-toplevel
+
+        def raise_exc(a: Any, b: Any) -> None:
+            raise KeyboardInterrupt("ctrl-c")
+
+        signal.signal(signal.SIGINT, raise_exc)
```

### Comparing `vidcrawler-1.0.8/vidcrawler/odysee.py` & `vidcrawler-1.0.9/vidcrawler/odysee.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,65 @@
-"""
-Odysee scrapper.
-"""
-
-# pylint: disable=invalid-name
-
-from typing import List
-
-import feedparser  # type: ignore
-import requests  # type: ignore
-
-from .date import iso_fmt, now_local
-from .video_info import VideoInfo
-
-
-def _parse_rss_entry(entry: feedparser.util.FeedParserDict) -> VideoInfo:
-    """Parses an rss entry and outputs a VideoInfo object."""
-    title = entry.title
-    link = entry.link
-    links = entry.links
-    published = entry.published
-    thumbnail_img = ""
-    for lnk in links:
-        if lnk.type.lower().startswith("image/"):
-            thumbnail_img = lnk.href
-            break
-    description = getattr(entry, "description", "")
-    o = VideoInfo(
-        channel_name="",
-        title=title,
-        date_published=published,
-        date_discovered="",
-        date_lastupdated="",
-        source="odysee.com",
-        url=link,
-        duration="?",  # No duration, suprisingly.
-        description=description,
-        img_src=thumbnail_img,
-        iframe_src="",
-        views="?",
-        profile_img_src=thumbnail_img,
-    )
-    return o
-
-
-def fetch_odysee_today(channel_name: str, channel: str) -> List[VideoInfo]:
-    """Fetches the latest videos from odysee.com."""
-    url: str = f"https://lbryfeed.melroy.org/channel/odysee/{channel}"
-    channel_url: str = f"https://odysee.com/@{channel}"
-    resp = requests.get(url)
-    now_str: str = iso_fmt(now_local())
-    resp.raise_for_status()
-    feed = feedparser.parse(resp.text)
-    out: List[VideoInfo] = []
-    for entry in feed.entries:
-        vo = _parse_rss_entry(entry)
-        vo.channel_name = channel_name
-        vo.channel_url = channel_url
-        vo.date_discovered = now_str
-        vo.date_lastupdated = now_str
-        if vo:
-            out.append(vo)
-    return out
+"""
+Odysee scrapper.
+"""
+
+# pylint: disable=invalid-name
+
+from typing import List
+
+import feedparser  # type: ignore
+import requests  # type: ignore
+
+from .date import iso_fmt, now_local
+from .video_info import VideoInfo
+
+_TIMEOUT = 10
+
+
+def _parse_rss_entry(entry: feedparser.util.FeedParserDict) -> VideoInfo:
+    """Parses an rss entry and outputs a VideoInfo object."""
+    title = entry.title
+    link = entry.link
+    links = entry.links
+    published = entry.published
+    thumbnail_img = ""
+    for lnk in links:
+        if lnk.type.lower().startswith("image/"):
+            thumbnail_img = lnk.href
+            break
+    description = getattr(entry, "description", "")
+    o = VideoInfo(
+        channel_name="",
+        title=title,
+        date_published=published,
+        date_discovered="",
+        date_lastupdated="",
+        source="odysee.com",
+        url=link,
+        duration="?",  # No duration, suprisingly.
+        description=description,
+        img_src=thumbnail_img,
+        iframe_src="",
+        views="?",
+        profile_img_src=thumbnail_img,
+    )
+    return o
+
+
+def fetch_odysee_today(channel_name: str, channel: str) -> List[VideoInfo]:
+    """Fetches the latest videos from odysee.com."""
+    url: str = f"https://lbryfeed.melroy.org/channel/odysee/{channel}"
+    channel_url: str = f"https://odysee.com/@{channel}"
+    resp = requests.get(url, timeout=_TIMEOUT)
+    now_str: str = iso_fmt(now_local())
+    resp.raise_for_status()
+    feed = feedparser.parse(resp.text)
+    out: List[VideoInfo] = []
+    for entry in feed.entries:
+        vo = _parse_rss_entry(entry)
+        vo.channel_name = channel_name
+        vo.channel_url = channel_url
+        vo.date_discovered = now_str
+        vo.date_lastupdated = now_str
+        if vo:
+            out.append(vo)
+    return out
```

### Comparing `vidcrawler-1.0.8/vidcrawler/rumble.py` & `vidcrawler-1.0.9/vidcrawler/rumble.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,108 +1,118 @@
-"""
-Rumble scrapper.
-"""
-
-# pylint: disable=line-too-long,missing-function-docstring,consider-using-f-string,too-many-locals,invalid-name,no-else-return,fixme
-
-import json
-import sys
-import traceback
-from typing import Dict, List, Tuple
-
-import requests
-from bs4 import BeautifulSoup  # type: ignore
-
-from .date import iso_fmt, now_local
-from .fetch_html import fetch_html_using_request_lib as fetch_html
-from .video_info import VideoInfo
-
-
-def parse_rumble_video_object(html_doc: str) -> Dict[str, str]:
-    soup_article = BeautifulSoup(html_doc, "html.parser")
-    script_dom = soup_article.find("script", {"type": "application/ld+json"})
-    json_string = script_dom.contents[0]
-    data = json.loads(json_string)  # type: ignore
-    return data[0]  # type: ignore
-
-
-def fetch_rumble(channel: str) -> Tuple[str, str]:
-    html_doc: str = ""
-    channel_url: str = "https://rumble.com/c/%s" % channel
-    url: str = "https://rumble.com/c/%s?date=this-month" % channel
-    try:
-        sys.stdout.write("Rumble visiting %s (%s)\n" % (channel, url))
-        html_doc = fetch_html(url)
-    except requests.exceptions.HTTPError:
-        channel_url = "https://rumble.com/user/%s" % channel
-        url = "https://rumble.com/user/%s" % channel
-        sys.stdout.write(f"Rumble alt visiting {channel} ({url})\n")
-        html_doc = fetch_html(url)
-    return (html_doc, channel_url)
-
-
-# type: ignore
-
-
-def fetch_rumble_channel_today(
-    channel_name: str, channel: str
-) -> List[VideoInfo]:
-    # TODO: Fine grained try...catch blocks.
-    output: List[VideoInfo] = []
-    html_doc: str = ""
-    channel_url: str = ""
-    html_doc, channel_url = fetch_rumble(channel)
-    # print(html_doc)
-    soup = BeautifulSoup(html_doc, "html.parser")
-    for article in soup.find_all("article", class_="video-item"):
-        try:
-            duration = article.find(class_="video-item--duration")["data-value"]
-            vid_src_suffix = article.find(class_="video-item--a")["href"]
-            vid_src = "https://rumble.com%s" % vid_src_suffix
-            sys.stdout.write("  visiting video %s (%s)\n" % (channel, vid_src))
-            html_doc2 = fetch_html(vid_src)
-            video_obj = parse_rumble_video_object(html_doc2)
-            title = video_obj["name"]
-            iframe_src = video_obj["embedUrl"]
-            desc_text = video_obj["description"]
-            publish_date = video_obj["uploadDate"]
-            try:
-                views = video_obj["interactionStatistic"]["userInteractionCount"]  # type: ignore
-            except KeyError:
-                views = "?"
-            # img_src = video_obj['thumbnailUrl']
-            img_src = article.find(class_="video-item--img")["src"]
-            now_datestr = iso_fmt(now_local())
-            o = VideoInfo(
-                channel_name=channel_name,
-                source="rumble.com",
-                date_published=publish_date,
-                date_discovered=now_datestr,
-                date_lastupdated=now_datestr,
-                url=vid_src,
-                channel_url=channel_url,
-                title=title,
-                duration=duration,
-                description=desc_text,
-                img_src=img_src,
-                iframe_src=iframe_src,
-                views=views,
-                profile_img_src="",
-            )
-            output.append(o)
-        except BaseException as e:  # pylint: disable=broad-except
-            s = "".join(traceback.format_exception(None, e, e.__traceback__))
-            sys.stdout.write(
-                "Error: %s\nCould not parse\n%s\n\n" % (str(s), str(article))
-            )
-    return output
-
-
-def interactive_test() -> None:
-    sys.stdout.write("Rumble user: ")
-    name: str = input()
-    rslt = fetch_rumble_channel_today(channel_name=name, channel=name)
-    print(rslt)
-
-
-if __name__ == "__main__":
-    interactive_test()
+"""
+Rumble scrapper.
+"""
+
+# pylint: disable=line-too-long,missing-function-docstring,consider-using-f-string,too-many-locals,invalid-name,no-else-return,fixme
+
+import json
+import sys
+import traceback
+from typing import Dict, List, Tuple
+
+import isodate  # type: ignore
+import requests
+from bs4 import BeautifulSoup  # type: ignore
+
+from .date import iso_fmt, now_local
+from .fetch_html import fetch_html_using_request_lib as fetch_html
+from .video_info import VideoInfo
+
+
+def parse_rumble_video_object(html_doc: str) -> Dict[str, str]:
+    soup_article = BeautifulSoup(html_doc, "html.parser")
+    script_dom = soup_article.find("script", {"type": "application/ld+json"})
+    json_string = script_dom.contents[0]
+    data = json.loads(json_string)  # type: ignore
+    return data[0]  # type: ignore
+
+
+def fetch_rumble(channel: str) -> Tuple[str, str]:
+    html_doc: str = ""
+    channel_url: str = "https://rumble.com/c/%s" % channel
+    url: str = "https://rumble.com/c/%s?date=this-month" % channel
+    try:
+        sys.stdout.write("Rumble visiting %s (%s)\n" % (channel, url))
+        html_doc = fetch_html(url)
+    except requests.exceptions.HTTPError:
+        channel_url = "https://rumble.com/user/%s" % channel
+        url = "https://rumble.com/user/%s" % channel
+        sys.stdout.write(f"Rumble alt visiting {channel} ({url})\n")
+        html_doc = fetch_html(url)
+    return (html_doc, channel_url)
+
+
+# type: ignore
+
+
+def fetch_rumble_channel_today(
+    channel_name: str, channel: str
+) -> List[VideoInfo]:
+    # TODO: Fine grained try...catch blocks.
+    output: List[VideoInfo] = []
+    html_doc: str = ""
+    channel_url: str = ""
+    html_doc, channel_url = fetch_rumble(channel)
+    # print(html_doc)
+    soup = BeautifulSoup(html_doc, "html.parser")
+    for article in soup.find_all("article", class_="video-item"):
+        try:
+            article_duration_dom = article.find(class_="video-item--duration")
+            duration = (
+                ""
+                if not article_duration_dom
+                else article_duration_dom["data-value"]
+            )
+            vid_src_suffix = article.find(class_="video-item--a")["href"]
+            vid_src = "https://rumble.com%s" % vid_src_suffix
+            sys.stdout.write("  visiting video %s (%s)\n" % (channel, vid_src))
+            html_doc2 = fetch_html(vid_src)
+            video_obj = parse_rumble_video_object(html_doc2)
+            title = video_obj["name"]
+            iframe_src = video_obj["embedUrl"]
+            desc_text = video_obj["description"]
+            publish_date = video_obj["uploadDate"]
+
+            if not duration:
+                duration_str = video_obj["duration"]
+                duration = isodate.parse_duration(duration_str).total_seconds()
+            try:
+                views = video_obj["interactionStatistic"]["userInteractionCount"]  # type: ignore
+            except KeyError:
+                views = "?"
+            # img_src = video_obj['thumbnailUrl']
+            img_src = article.find(class_="video-item--img")["src"]
+            now_datestr = iso_fmt(now_local())
+            o = VideoInfo(
+                channel_name=channel_name,
+                source="rumble.com",
+                date_published=publish_date,
+                date_discovered=now_datestr,
+                date_lastupdated=now_datestr,
+                url=vid_src,
+                channel_url=channel_url,
+                title=title,
+                duration=duration,
+                description=desc_text,
+                img_src=img_src,
+                iframe_src=iframe_src,
+                views=views,
+                profile_img_src="",
+            )
+            output.append(o)
+        except BaseException as e:  # pylint: disable=broad-except
+            s = "".join(traceback.format_exception(None, e, e.__traceback__))
+            sys.stdout.write(
+                "Error: %s\nCould not parse\n%s\n\n" % (str(s), str(article))
+            )
+    return output
+
+
+def interactive_test() -> None:
+    sys.stdout.write("Rumble user: ")
+    name: str = input()
+    rslt = fetch_rumble_channel_today(channel_name=name, channel=name)
+    print(rslt)
+
+
+if __name__ == "__main__":
+    interactive_test()
```

### Comparing `vidcrawler-1.0.8/vidcrawler/spider.py` & `vidcrawler-1.0.9/vidcrawler/spider.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,195 +1,195 @@
-"""Spider which crawls all the channels"""
-
-# pylint: disable=line-too-long,missing-function-docstring,consider-using-f-string,too-many-locals,invalid-name,no-else-return
-
-import json
-import queue
-import random
-import signal
-import sys
-import threading
-import time
-import traceback
-from typing import Any, Dict, List, Tuple
-
-from .bitchute import fetch_bitchute_today
-from .brighteon import fetch_brighteon_today
-from .gabtv import fetch_gabtv_today
-from .odysee import fetch_odysee_today
-from .rumble import fetch_rumble_channel_today
-from .spotify import fetch_spotify_today
-from .spreaker import fetch_spreaker_today
-from .video_info import VideoInfo
-from .youtube import fetch_youtube_today
-
-BRIGHTEON = "brighteon"
-YOUTUBE = "youtube"
-RUMBLE = "rumble"
-BITCHUTE = "bitchute"
-SPREAKER = "spreaker"
-ODYSEE = "odysee"
-GAB = "gab"
-SPOTIFY = "spotify"
-
-CRAWLER_MAP = {
-    RUMBLE: fetch_rumble_channel_today,
-    BITCHUTE: fetch_bitchute_today,
-    BRIGHTEON: fetch_brighteon_today,
-    YOUTUBE: fetch_youtube_today,
-    SPREAKER: fetch_spreaker_today,
-    ODYSEE: fetch_odysee_today,
-    GAB: fetch_gabtv_today,
-    SPOTIFY: fetch_spotify_today,
-}
-
-_SCRAPE_RANDOMIZE_ORDER = True
-_YT_SCRAPER_ENABLE_THREADS = True
-_YT_SCRAPER_ENABLE_THREADS = False
-
-# type: ignore
-
-
-def _fetch_all(
-    source_name: str,
-    fetch_list: List[Tuple[str, str]],
-    out_queue: queue.Queue,
-    bad_channels: queue.Queue,
-) -> None:
-    callback = CRAWLER_MAP[source_name]
-    if _SCRAPE_RANDOMIZE_ORDER:
-        random.shuffle(fetch_list)
-
-    def do_fetch(fetch_list: List, callback: Any) -> None:
-        for (channel_name, channel_id) in fetch_list:
-            try:
-                videos = callback(channel_name, channel_id)  # type: ignore
-                for vid in videos:
-                    out_queue.put(vid)
-            except KeyboardInterrupt:
-                sys.exit(1)
-            except BaseException as e:
-                traceback.print_exc()
-                entry = (channel_name, str(e))
-                bad_channels.put(entry)
-                continue
-
-    if source_name != YOUTUBE:
-        do_fetch(fetch_list, callback)
-        return
-    if not _YT_SCRAPER_ENABLE_THREADS:
-        do_fetch(fetch_list, callback)
-        return
-    # YouTube and threads enabled.
-    num_workers = 4
-    thread_data = [[] for _ in range(num_workers)]  # type: ignore
-    for i, data in enumerate(fetch_list):
-        idx = i % num_workers
-        thread_data[idx].append(data)
-    threads = []
-    for tdata in thread_data:
-        thread = threading.Thread(target=do_fetch, args=(tdata, callback))
-        thread.daemon = True
-        thread.start()
-        threads.append(thread)
-    for t in threads:
-        t.join()
-
-
-def _yield_thread_for_keyboard_interrupt() -> None:
-    if sys.platform == "win32":
-        time.sleep(0.1)
-    else:
-        try:
-            # might be missing on some platforms.
-            signal.pause()  # pylint: disable-all
-        except BaseException:
-            time.sleep(0.1)
-
-
-def _threaded_fetch_channels(
-    channels: List[Tuple[str, str, str]],
-    out_videos: List[VideoInfo],
-    out_bad_channels: List[Tuple[str, str]],
-) -> None:
-    # Partition the list by source type (bitchute, youtube, ...)
-    # for each source fetch all videos.
-    partitioned: Dict[str, Any] = {}
-    for (channel_name, source, channel_id) in channels:
-        partitioned.setdefault(source, [])
-        partitioned[source].append((channel_name, channel_id))
-    queue_out: queue.Queue = queue.Queue()
-    queue_bad_channels: queue.Queue = queue.Queue()
-    # Launch threads but also makes the main thread responsive to the keyboard interrupt.
-    threads = []
-    for source, array_data in partitioned.items():
-        thread = threading.Thread(
-            target=_fetch_all,
-            args=(source, array_data, queue_out, queue_bad_channels),
-        )
-        thread.daemon = True
-        thread.start()
-        threads.append(thread)
-    while True:  # Weird loop allows KeyboardInterrupt
-        finish_cnt = 0
-        for t in threads:
-            if t.is_alive():
-                finish_cnt += 1
-        if finish_cnt == len(threads):
-            break
-        _yield_thread_for_keyboard_interrupt()
-    # Busy loop here allows keyboard interrupts to filter through to the
-    # top and halt the execution of the program right away.
-    while len(threads):
-        for i, thread in enumerate(threads):
-            if not thread.is_alive():
-                thread.join()
-                threads.pop(i)
-                break  # Start the outer loop again
-        time.sleep(0.1)
-    while not queue_out.empty():
-        out_videos.append(queue_out.get_nowait())
-    for c in list(queue_bad_channels.queue):
-        out_bad_channels.append(c)
-
-
-def _singlethreaded_fetch(
-    channels: List[Tuple[str, str, str]],
-    out_videos: List[VideoInfo],
-    out_bad_channels: List[Tuple[str, str]],
-) -> None:
-    partitioned: Dict[str, Any] = {}
-    for (channel_name, source, channel_id) in channels:
-        partitioned.setdefault(source, [])
-        partitioned[source].append((channel_name, channel_id))
-    queue_out: queue.Queue = queue.Queue()
-    queue_bad_channels: queue.Queue = queue.Queue()
-    for source, array_data in partitioned.items():
-        _fetch_all(source, array_data, queue_out, queue_bad_channels)
-    while not queue_out.empty():
-        out_videos.append(queue_out.get_nowait())
-    for c in list(queue_bad_channels.queue):
-        out_bad_channels.append(c)
-
-
-def crawl_video_sites(channels: List[Tuple[str, str, str]], use_threads: bool = True) -> str:  # type: ignore
-    vid_infos: List[VideoInfo] = []
-    bad_channels: List[Tuple[str, str]] = []
-    if use_threads:
-        _threaded_fetch_channels(channels, vid_infos, bad_channels)
-    else:
-        _singlethreaded_fetch(channels, vid_infos, bad_channels)
-    # apply_fetch_images(vid_infos)
-    out_data: List[Dict] = VideoInfo.to_plain_list(vid_infos)  # type: ignore
-    json_str = json.dumps(
-        out_data, indent=2, sort_keys=True, ensure_ascii=False
-    )
-    bad_channels.sort()
-    if bad_channels:
-        print("#############")
-        print("# Bad channels:")
-        for name, err in bad_channels:
-            print(f"#  {name}: {err}")
-        print("#############")
-    else:
-        print("No bad channels detected!")
-    return json_str
+"""Spider which crawls all the channels"""
+
+# pylint: disable=line-too-long,missing-function-docstring,consider-using-f-string,too-many-locals,invalid-name,no-else-return
+
+import json
+import queue
+import random
+import signal
+import sys
+import threading
+import time
+import traceback
+from typing import Any, Dict, List, Tuple
+
+from .bitchute import fetch_bitchute_today
+from .brighteon import fetch_brighteon_today
+from .gabtv import fetch_gabtv_today
+from .odysee import fetch_odysee_today
+from .rumble import fetch_rumble_channel_today
+from .spotify import fetch_spotify_today
+from .spreaker import fetch_spreaker_today
+from .video_info import VideoInfo
+from .youtube import fetch_youtube_today
+
+BRIGHTEON = "brighteon"
+YOUTUBE = "youtube"
+RUMBLE = "rumble"
+BITCHUTE = "bitchute"
+SPREAKER = "spreaker"
+ODYSEE = "odysee"
+GAB = "gab"
+SPOTIFY = "spotify"
+
+CRAWLER_MAP = {
+    RUMBLE: fetch_rumble_channel_today,
+    BITCHUTE: fetch_bitchute_today,
+    BRIGHTEON: fetch_brighteon_today,
+    YOUTUBE: fetch_youtube_today,
+    SPREAKER: fetch_spreaker_today,
+    ODYSEE: fetch_odysee_today,
+    GAB: fetch_gabtv_today,
+    SPOTIFY: fetch_spotify_today,
+}
+
+_SCRAPE_RANDOMIZE_ORDER = True
+_YT_SCRAPER_ENABLE_THREADS = True
+_YT_SCRAPER_ENABLE_THREADS = False
+
+# type: ignore
+
+
+def _fetch_all(
+    source_name: str,
+    fetch_list: List[Tuple[str, str]],
+    out_queue: queue.Queue,
+    bad_channels: queue.Queue,
+) -> None:
+    callback = CRAWLER_MAP[source_name]
+    if _SCRAPE_RANDOMIZE_ORDER:
+        random.shuffle(fetch_list)
+
+    def do_fetch(fetch_list: List, callback: Any) -> None:
+        for (channel_name, channel_id) in fetch_list:
+            try:
+                videos = callback(channel_name, channel_id)  # type: ignore
+                for vid in videos:
+                    out_queue.put(vid)
+            except KeyboardInterrupt:
+                sys.exit(1)
+            except BaseException as e:
+                traceback.print_exc()
+                entry = (channel_name, str(e))
+                bad_channels.put(entry)
+                continue
+
+    if source_name != YOUTUBE:
+        do_fetch(fetch_list, callback)
+        return
+    if not _YT_SCRAPER_ENABLE_THREADS:
+        do_fetch(fetch_list, callback)
+        return
+    # YouTube and threads enabled.
+    num_workers = 4
+    thread_data = [[] for _ in range(num_workers)]  # type: ignore
+    for i, data in enumerate(fetch_list):
+        idx = i % num_workers
+        thread_data[idx].append(data)
+    threads = []
+    for tdata in thread_data:
+        thread = threading.Thread(target=do_fetch, args=(tdata, callback))
+        thread.daemon = True
+        thread.start()
+        threads.append(thread)
+    for t in threads:
+        t.join()
+
+
+def _yield_thread_for_keyboard_interrupt() -> None:
+    if sys.platform == "win32":
+        time.sleep(0.1)
+    else:
+        try:
+            # might be missing on some platforms.
+            signal.pause()  # pylint: disable-all
+        except BaseException:
+            time.sleep(0.1)
+
+
+def _threaded_fetch_channels(
+    channels: List[Tuple[str, str, str]],
+    out_videos: List[VideoInfo],
+    out_bad_channels: List[Tuple[str, str]],
+) -> None:
+    # Partition the list by source type (bitchute, youtube, ...)
+    # for each source fetch all videos.
+    partitioned: Dict[str, Any] = {}
+    for (channel_name, source, channel_id) in channels:
+        partitioned.setdefault(source, [])
+        partitioned[source].append((channel_name, channel_id))
+    queue_out: queue.Queue = queue.Queue()
+    queue_bad_channels: queue.Queue = queue.Queue()
+    # Launch threads but also makes the main thread responsive to the keyboard interrupt.
+    threads = []
+    for source, array_data in partitioned.items():
+        thread = threading.Thread(
+            target=_fetch_all,
+            args=(source, array_data, queue_out, queue_bad_channels),
+        )
+        thread.daemon = True
+        thread.start()
+        threads.append(thread)
+    while True:  # Weird loop allows KeyboardInterrupt
+        finish_cnt = 0
+        for t in threads:
+            if t.is_alive():
+                finish_cnt += 1
+        if finish_cnt == len(threads):
+            break
+        _yield_thread_for_keyboard_interrupt()
+    # Busy loop here allows keyboard interrupts to filter through to the
+    # top and halt the execution of the program right away.
+    while len(threads):
+        for i, thread in enumerate(threads):
+            if not thread.is_alive():
+                thread.join()
+                threads.pop(i)
+                break  # Start the outer loop again
+        time.sleep(0.1)
+    while not queue_out.empty():
+        out_videos.append(queue_out.get_nowait())
+    for c in list(queue_bad_channels.queue):
+        out_bad_channels.append(c)
+
+
+def _singlethreaded_fetch(
+    channels: List[Tuple[str, str, str]],
+    out_videos: List[VideoInfo],
+    out_bad_channels: List[Tuple[str, str]],
+) -> None:
+    partitioned: Dict[str, Any] = {}
+    for (channel_name, source, channel_id) in channels:
+        partitioned.setdefault(source, [])
+        partitioned[source].append((channel_name, channel_id))
+    queue_out: queue.Queue = queue.Queue()
+    queue_bad_channels: queue.Queue = queue.Queue()
+    for source, array_data in partitioned.items():
+        _fetch_all(source, array_data, queue_out, queue_bad_channels)
+    while not queue_out.empty():
+        out_videos.append(queue_out.get_nowait())
+    for c in list(queue_bad_channels.queue):
+        out_bad_channels.append(c)
+
+
+def crawl_video_sites(channels: List[Tuple[str, str, str]], use_threads: bool = True) -> str:  # type: ignore
+    vid_infos: List[VideoInfo] = []
+    bad_channels: List[Tuple[str, str]] = []
+    if use_threads:
+        _threaded_fetch_channels(channels, vid_infos, bad_channels)
+    else:
+        _singlethreaded_fetch(channels, vid_infos, bad_channels)
+    # apply_fetch_images(vid_infos)
+    out_data: List[Dict] = VideoInfo.to_plain_list(vid_infos)  # type: ignore
+    json_str = json.dumps(
+        out_data, indent=2, sort_keys=True, ensure_ascii=False
+    )
+    bad_channels.sort()
+    if bad_channels:
+        print("#############")
+        print("# Bad channels:")
+        for name, err in bad_channels:
+            print(f"#  {name}: {err}")
+        print("#############")
+    else:
+        print("No bad channels detected!")
+    return json_str
```

### Comparing `vidcrawler-1.0.8/vidcrawler/spotify.py` & `vidcrawler-1.0.9/vidcrawler/spotify.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-"""
-Spotify scraper
-"""
-
-# pylint: disable=line-too-long,missing-function-docstring,consider-using-f-string,too-many-locals,invalid-name,no-else-return,fixme
-
-import sys
-from datetime import datetime
-from typing import List
-
-from bs4 import BeautifulSoup  # type: ignore
-
-from .date import iso_fmt
-from .fetch_html import fetch_html_using_request_lib as fetch_html
-from .video_info import VideoInfo
-
-_TIMEOUT_EPISODE = 20  # Wow these can take a long time.
-
-# TODO: Allow spotify scraper to access the database and check to see if
-# the episode is already there.
-
-
-def now_local() -> datetime:
-    """Patch to allow code to work."""
-    return datetime.now()
-
-
-def fetch_spotify_today(channel_name: str, channel: str) -> List[VideoInfo]:
-    output: List[VideoInfo] = []
-    now_datestr = iso_fmt(now_local())
-    channel_url = f"https://open.spotify.com/show/{channel}"
-    sys.stdout.write(
-        f"Spotify crawler visiting {channel_name} ({channel_url})\n"
-    )
-    html_doc = fetch_html(channel_url)
-    html_dom = BeautifulSoup(html_doc, "html.parser")
-    music_doms = html_dom.findAll("meta", {"property": "music:song"})
-    episode_urls = [e.attrs["content"] for e in music_doms]
-    for episide_url in episode_urls:
-        sys.stdout.write(f"  Spotify crawler visiting episode {episide_url}\n")
-        episode_html = fetch_html(episide_url, timeout=_TIMEOUT_EPISODE)
-        episode_dom = BeautifulSoup(episode_html, "html.parser")
-
-        def extract_meta_property(name: str) -> str:
-            dom = episode_dom.find(  # pylint: disable=cell-var-from-loop
-                "meta", {"property": name}
-            )
-            return str(dom["content"])
-
-        img_url = extract_meta_property("og:image")
-        title = extract_meta_property("og:title")
-        description = extract_meta_property("og:description")
-        release_date = extract_meta_property("music:release_date")
-        duration = extract_meta_property("music:duration")
-        url = extract_meta_property("og:url")
-        # example:
-        #   "4rJBoD4BeeYFd8eLhrDRM" is extracted from
-        #   "https://open.spotify.com/episode/4rJBoD4BeeYFd8eLhrDRM"
-        spotify_id = url.split("episode")[1].replace("/", "")
-        title = extract_meta_property("og:title")
-        vid_url = f"https://open.spotify.com/episode/{spotify_id}"
-        iframe_url = f"https://open.spotify.com/embed/episode/{spotify_id}"
-        vid: VideoInfo = VideoInfo(
-            channel_name=channel_name,
-            source="spotify.com",
-            date_published=release_date,
-            date_discovered=now_datestr,
-            date_lastupdated=now_datestr,
-            url=vid_url,
-            channel_url=channel_url,
-            title=title,
-            duration=duration,
-            description=description,
-            img_src=img_url,
-            iframe_src=iframe_url,
-            views="?",
-            profile_img_src="",
-        )
-        output.append(vid)
-    return output
-
-
-def unit_test() -> None:
-    fetch_spotify_today(
-        channel_name="Joe Rogan", channel="4rOoJ6Egrf8K2IrywzwOMk"
-    )
-
-
-if __name__ == "__main__":
-    # Unit test
-    unit_test()
+"""
+Spotify scraper
+"""
+
+# pylint: disable=line-too-long,missing-function-docstring,consider-using-f-string,too-many-locals,invalid-name,no-else-return,fixme
+
+import sys
+from datetime import datetime
+from typing import List
+
+from bs4 import BeautifulSoup  # type: ignore
+
+from .date import iso_fmt
+from .fetch_html import fetch_html_using_request_lib as fetch_html
+from .video_info import VideoInfo
+
+_TIMEOUT_EPISODE = 20  # Wow these can take a long time.
+
+# TODO: Allow spotify scraper to access the database and check to see if
+# the episode is already there.
+
+
+def now_local() -> datetime:
+    """Patch to allow code to work."""
+    return datetime.now()
+
+
+def fetch_spotify_today(channel_name: str, channel: str) -> List[VideoInfo]:
+    output: List[VideoInfo] = []
+    now_datestr = iso_fmt(now_local())
+    channel_url = f"https://open.spotify.com/show/{channel}"
+    sys.stdout.write(
+        f"Spotify crawler visiting {channel_name} ({channel_url})\n"
+    )
+    html_doc = fetch_html(channel_url)
+    html_dom = BeautifulSoup(html_doc, "html.parser")
+    music_doms = html_dom.findAll("meta", {"name": "music:song"})
+    episode_urls = [e.attrs["content"] for e in music_doms]
+    for episide_url in episode_urls:
+        sys.stdout.write(f"  Spotify crawler visiting episode {episide_url}\n")
+        episode_html = fetch_html(episide_url, timeout=_TIMEOUT_EPISODE)
+        episode_dom = BeautifulSoup(episode_html, "html.parser")
+
+        def extract_meta_property(name: str) -> str:
+            dom = episode_dom.find(  # pylint: disable=cell-var-from-loop
+                "meta", {"name": name}
+            )
+            return str(dom["content"])
+
+        img_url = extract_meta_property("og:image")
+        title = extract_meta_property("og:title")
+        description = extract_meta_property("og:description")
+        release_date = extract_meta_property("music:release_date")
+        duration = extract_meta_property("music:duration")
+        url = extract_meta_property("og:url")
+        # example:
+        #   "4rJBoD4BeeYFd8eLhrDRM" is extracted from
+        #   "https://open.spotify.com/episode/4rJBoD4BeeYFd8eLhrDRM"
+        spotify_id = url.split("episode")[1].replace("/", "")
+        title = extract_meta_property("og:title")
+        vid_url = f"https://open.spotify.com/episode/{spotify_id}"
+        iframe_url = f"https://open.spotify.com/embed/episode/{spotify_id}"
+        vid: VideoInfo = VideoInfo(
+            channel_name=channel_name,
+            source="spotify.com",
+            date_published=release_date,
+            date_discovered=now_datestr,
+            date_lastupdated=now_datestr,
+            url=vid_url,
+            channel_url=channel_url,
+            title=title,
+            duration=duration,
+            description=description,
+            img_src=img_url,
+            iframe_src=iframe_url,
+            views="?",
+            profile_img_src="",
+        )
+        output.append(vid)
+    return output
+
+
+def unit_test() -> None:
+    fetch_spotify_today(
+        channel_name="Joe Rogan", channel="4rOoJ6Egrf8K2IrywzwOMk"
+    )
+
+
+if __name__ == "__main__":
+    # Unit test
+    unit_test()
```

### Comparing `vidcrawler-1.0.8/vidcrawler/spreaker.py` & `vidcrawler-1.0.9/vidcrawler/spreaker.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,69 @@
-"""
-Scraper for spreaker.com
-"""
-
-# pylint: disable=line-too-long,missing-function-docstring,consider-using-f-string,too-many-locals,invalid-name,no-else-return,R0801
-
-import sys
-from typing import List
-
-import feedparser  # type: ignore
-
-from vidcrawler.date import iso_fmt, now_local
-
-from .fetch_html import fetch_html_using_request_lib as fetch_html
-from .video_info import VideoInfo
-
-# EXPERIMENTAL - parses sara carter from spreaker.
-
-
-def rss_element_to_video_info(
-    channel_name: str, rss_element: dict
-) -> VideoInfo:
-    # content = rss_element.get('content')
-    thumbnail_img = rss_element["googleplay_image"]["href"]
-    link = rss_element["link"]
-    published = rss_element["published"]
-    title = rss_element["title"]
-    description = rss_element.get("subtitle") or rss_element.get("summary", "")
-    # summary = entry['summary']
-    duration = rss_element["itunes_duration"]
-    now_str = iso_fmt(now_local())
-    o = VideoInfo(
-        channel_name=channel_name,
-        title=title,
-        date_published=published,
-        date_discovered=now_str,
-        date_lastupdated=now_str,
-        source="spreaker.com",
-        url=link,
-        duration=duration,
-        description=f"{description}",
-        img_src=thumbnail_img,
-        iframe_src="",
-        views="?",
-        profile_img_src=thumbnail_img,
-    )
-    return o
-
-
-def fetch_spreaker_today(channel_name: str, channel: str) -> List[VideoInfo]:
-    url = f"https://www.spreaker.com/show/{channel}/episodes/feed"
-    sys.stdout.write("Spreaker visiting %s (%s)\n" % (channel, url))
-    content = fetch_html(url)
-    feed = feedparser.parse(content)
-    output: List[VideoInfo] = []
-    for entry in feed.entries:
-        try:
-            vid = rss_element_to_video_info(
-                channel_name=channel_name, rss_element=entry
-            )
-            output.append(vid)
-        except BaseException as err:  # pylint: disable=broad-except
-            sys.stderr.write(
-                f"{__file__}: Error while parsing {channel_name} entry:\n {str(entry)}:\n because of {err}"
-            )
-    return output
-
-
-if __name__ == "__main__":
-    print(fetch_spreaker_today("Sara Carter", "4495281"))
+"""
+Scraper for spreaker.com
+"""
+
+# pylint: disable=line-too-long,missing-function-docstring,consider-using-f-string,too-many-locals,invalid-name,no-else-return,R0801
+
+import sys
+from typing import List
+
+import feedparser  # type: ignore
+
+from vidcrawler.date import iso_fmt, now_local
+
+from .fetch_html import fetch_html_using_request_lib as fetch_html
+from .video_info import VideoInfo
+
+# EXPERIMENTAL - parses sara carter from spreaker.
+
+
+def rss_element_to_video_info(
+    channel_name: str, rss_element: dict
+) -> VideoInfo:
+    thumbnail_img = rss_element["image"]["href"]
+    link = rss_element["link"]
+    published = rss_element["published"]
+    title = rss_element["title"]
+    description = rss_element.get("subtitle") or rss_element.get("summary", "")
+    # summary = entry['summary']
+    duration = rss_element["itunes_duration"]
+    now_str = iso_fmt(now_local())
+    o = VideoInfo(
+        channel_name=channel_name,
+        title=title,
+        date_published=published,
+        date_discovered=now_str,
+        date_lastupdated=now_str,
+        source="spreaker.com",
+        url=link,
+        duration=duration,
+        description=f"{description}",
+        img_src=thumbnail_img,
+        iframe_src="",
+        views="?",
+        profile_img_src=thumbnail_img,
+    )
+    return o
+
+
+def fetch_spreaker_today(channel_name: str, channel: str) -> List[VideoInfo]:
+    url = f"https://www.spreaker.com/show/{channel}/episodes/feed"
+    sys.stdout.write("Spreaker visiting %s (%s)\n" % (channel, url))
+    content = fetch_html(url)
+    feed = feedparser.parse(content)
+    output: List[VideoInfo] = []
+    for entry in feed.entries:
+        try:
+            vid = rss_element_to_video_info(
+                channel_name=channel_name, rss_element=entry
+            )
+            output.append(vid)
+        except BaseException as err:  # pylint: disable=broad-except
+            sys.stderr.write(
+                f"{__file__}: Error while parsing {channel_name} entry:\n {str(entry['title'])}:\n because of {err}"
+            )
+    return output
+
+
+if __name__ == "__main__":
+    print(fetch_spreaker_today("Sara Carter", "4495281"))
```

### Comparing `vidcrawler-1.0.8/vidcrawler/testing/simple_http_server.py` & `vidcrawler-1.0.9/vidcrawler/testing/simple_http_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from http import HTTPStatus
 from typing import Any, Callable, Generator, List, Optional
 
 import requests
 
 StringFunctor = Callable[[], str]
 
+_TIMEOUT = 10
+
 
 def make_handler_class(response_text_fcn: StringFunctor) -> Any:
     class Handler(http.server.SimpleHTTPRequestHandler):
         def do_GET(self):
             self.send_response(HTTPStatus.OK)
             self.end_headers()
             data = response_text_fcn().encode("utf-8")
@@ -80,14 +82,14 @@
         server_thread.join()
 
 
 def unit_test() -> None:
     with simple_response_server_thread(
         port=53925, response_text_fcn=lambda: "this should match!!!!"
     ):
-        resp = requests.get("http://localhost:53925")
+        resp = requests.get("http://localhost:53925", timeout=_TIMEOUT)
         resp.raise_for_status()
         assert resp.text == "this should match!!!!"
 
 
 if __name__ == "__main__":
     unit_test()
```

### Comparing `vidcrawler-1.0.8/vidcrawler/testing/test_cmd.py` & `vidcrawler-1.0.9/vidcrawler/testing/test_cmd.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-"""
-Testing cmd
-"""
-
-
-# pylint: disable=line-too-long,missing-function-docstring,missing-class-docstring,super-with-arguments,invalid-name,R0801
-
-import os
-import subprocess
-import unittest
-from pprint import pprint
-
-HERE = os.path.dirname(os.path.abspath(__file__))
-FETCH_LIST = os.path.join(HERE, "fetch_list.json")
-OUT_LIST = os.path.join(HERE, "out_list.json")
-
-
-class IoTester(unittest.TestCase):
-    def test_env(self):  # pylint: disable
-        pprint(dict(os.environ))
-
-    def test_cmd(self):  # pylint: disable
-        subprocess.check_call(
-            "vidcrawler --help",
-            shell=True,
-            stdout=subprocess.DEVNULL,
-            stderr=subprocess.DEVNULL,
-        )
-
-    def test_process_test(self):  # pylint: disable
-        subprocess.check_call(
-            f'vidcrawler --input_crawl_json "{FETCH_LIST}" --output_json "{OUT_LIST}"',
-            shell=True,
-            stdout=subprocess.DEVNULL,
-            stderr=subprocess.DEVNULL,
-        )
-
-
-if __name__ == "__main__":
-    unittest.main()
+"""
+Testing cmd
+"""
+
+
+# pylint: disable=line-too-long,missing-function-docstring,missing-class-docstring,super-with-arguments,invalid-name,R0801
+
+import os
+import subprocess
+import unittest
+from pprint import pprint
+
+HERE = os.path.dirname(os.path.abspath(__file__))
+FETCH_LIST = os.path.join(HERE, "fetch_list.json")
+OUT_LIST = os.path.join(HERE, "out_list.json")
+
+
+class IoTester(unittest.TestCase):
+    def test_env(self):  # pylint: disable
+        pprint(dict(os.environ))
+
+    def test_cmd(self):  # pylint: disable
+        subprocess.check_call(
+            "vidcrawler --help",
+            shell=True,
+            stdout=subprocess.DEVNULL,
+            stderr=subprocess.DEVNULL,
+        )
+
+    def test_process_test(self):  # pylint: disable
+        subprocess.check_call(
+            f'vidcrawler --input_crawl_json "{FETCH_LIST}" --output_json "{OUT_LIST}"',
+            shell=True,
+            stdout=subprocess.DEVNULL,
+            stderr=subprocess.DEVNULL,
+        )
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `vidcrawler-1.0.8/vidcrawler/testing/test_io.py` & `vidcrawler-1.0.9/vidcrawler/testing/test_io.py`

 * *Files identical despite different names*

### Comparing `vidcrawler-1.0.8/vidcrawler/testing/test_scraper_bitchute.py` & `vidcrawler-1.0.9/vidcrawler/testing/test_scraper_bitchute.py`

 * *Files identical despite different names*

### Comparing `vidcrawler-1.0.8/vidcrawler/testing/test_scraper_gabtv.py` & `vidcrawler-1.0.9/vidcrawler/testing/test_scraper_gabtv.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# pylint: disable=missing-module-docstring,missing-class-docstring,missing-function-docstring
-
-import unittest
-from typing import List
-
-from vidcrawler.gabtv import fetch_gabtv_today, fetch_views
-from vidcrawler.video_info import VideoInfo
-
-
-class GabTvTester(unittest.TestCase):
-    def test_fetch_gabtv_views(self):
-        """Tests that we can fetch views."""
-        views = fetch_views(channel="LadyBee")
-        self.assertGreater(len(views), 0)
-
-    def test_fetch_gabtv_today(self):
-        vid_list: List[VideoInfo] = fetch_gabtv_today(
-            channel_name="Maryam Henein", channel_id="LadyBee"
-        )
-        self.assertGreater(len(vid_list), 0)
-
-
-if __name__ == "__main__":
-    unittest.main()
+# pylint: disable=missing-module-docstring,missing-class-docstring,missing-function-docstring
+
+import unittest
+from typing import List
+
+from vidcrawler.gabtv import fetch_gabtv_today, fetch_views
+from vidcrawler.video_info import VideoInfo
+
+
+class GabTvTester(unittest.TestCase):
+    def test_fetch_gabtv_views(self):
+        """Tests that we can fetch views."""
+        views = fetch_views(channel="LadyBee")
+        self.assertGreater(len(views), 0)
+
+    def test_fetch_gabtv_today(self):
+        vid_list: List[VideoInfo] = fetch_gabtv_today(
+            channel_name="Maryam Henein", channel_id="LadyBee"
+        )
+        self.assertGreater(len(vid_list), 0)
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `vidcrawler-1.0.8/vidcrawler/testing/test_scraper_odysee.py` & `vidcrawler-1.0.9/vidcrawler/testing/test_scraper_odysee.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,47 @@
-# pylint: disable=missing-module-docstring,missing-class-docstring,missing-function-docstring
-
-import re
-import unittest
-from typing import List
-
-from vidcrawler.odysee import fetch_odysee_today
-from vidcrawler.video_info import VideoInfo
-
-
-def is_valid_url(url: str) -> bool:
-    # Create a regex to match a url
-    regex = r"^(?:http(s)?:\/\/)?[\w.-]+(?:\.[\w\.-]+)+[\w\-\._~:/?#[\]@!\$&'\(\)\*\+,;=.]+$"
-    return re.match(regex, url) is not None
-
-
-class OdyseeScraperTester(unittest.TestCase):
-    def test_fetch_odysee_today(self):
-        # RSS FEED:
-        #   https://lbryfeed.melroy.org/channel/odysee/BretWeinstein
-        vid_list: List[VideoInfo] = fetch_odysee_today(
-            channel_name="BretWeinstein", channel="BretWeinstein"
-        )
-        self.assertGreater(len(vid_list), 0)
-
-    def test_odysee_bug(self):
-        # Test the fix for odysee bug:
-        #   https://github.com/zackees/blast.video/issues/1
-        vid_list: List[VideoInfo] = fetch_odysee_today(
-            channel_name="The Ripple Effect", channel="therippleeffectpodcast"
-        )
-        self.assertGreater(len(vid_list), 0)
-        for vid in vid_list:
-            self.assertEqual(vid.channel_name, "The Ripple Effect")
-            self.assertTrue(
-                is_valid_url(vid.img_src), f'"{vid.img_src}" is not a valid url'
-            )
-
-
-if __name__ == "__main__":
-    unittest.main()
+# pylint: disable=missing-module-docstring,missing-class-docstring,missing-function-docstring
+
+import re
+import unittest
+from typing import List
+
+from vidcrawler.odysee import fetch_odysee_today
+from vidcrawler.video_info import VideoInfo
+
+
+def is_valid_url(url: str) -> bool:
+    # Create a regex to match a url
+    regex = r"^(?:http(s)?:\/\/)?[\w.-]+(?:\.[\w\.-]+)+[\w\-\._~:/?#[\]@!\$&'\(\)\*\+,;=.]+$"
+    return re.match(regex, url) is not None
+
+
+class OdyseeScraperTester(unittest.TestCase):
+    def test_fetch_odysee_today(self):
+        # RSS FEED:
+        #   https://lbryfeed.melroy.org/channel/odysee/BretWeinstein
+        vid_list: List[VideoInfo] = fetch_odysee_today(
+            channel_name="BretWeinstein", channel="BretWeinstein"
+        )
+        self.assertGreater(len(vid_list), 0)
+
+    def test_union_of_the_unwanted(self):
+        vid_list: List[VideoInfo] = fetch_odysee_today(
+            channel_name="UOTU", channel="uotuw:e"
+        )
+        self.assertGreater(len(vid_list), 0)
+
+    def test_odysee_bug(self):
+        # Test the fix for odysee bug:
+        #   https://github.com/zackees/blast.video/issues/1
+        vid_list: List[VideoInfo] = fetch_odysee_today(
+            channel_name="The Ripple Effect", channel="therippleeffectpodcast"
+        )
+        self.assertGreater(len(vid_list), 0)
+        for vid in vid_list:
+            self.assertEqual(vid.channel_name, "The Ripple Effect")
+            self.assertTrue(
+                is_valid_url(vid.img_src), f'"{vid.img_src}" is not a valid url'
+            )
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `vidcrawler-1.0.8/vidcrawler/testing/test_scraper_rumble.py` & `vidcrawler-1.0.9/vidcrawler/testing/test_scraper_rumble.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-# pylint: disable=missing-module-docstring,missing-class-docstring,missing-function-docstring
-import unittest
-from datetime import datetime
-from typing import Optional
-
-from vidcrawler.date import now_local, parse_datetime
-from vidcrawler.rumble import fetch_rumble, fetch_rumble_channel_today
-from vidcrawler.video_info import VideoInfo
-
-
-class RumbleScraperTester(unittest.TestCase):
-    def test_fetch_rumble(self):
-        vid_list = fetch_rumble(channel="DiamondandSilk")
-        self.assertTrue(vid_list)
-
-    def test_fetch_alt_channel_url(self):
-        vid_list = fetch_rumble(channel="MaryamXHenein")
-        self.assertTrue(vid_list)
-
-    def test_fetch_bannon(self) -> None:
-        max_days = 4
-        vid_list = fetch_rumble_channel_today(
-            channel="BannonsWarRoom", channel_name="BannonsWarRoom"
-        )
-        most_recent_date: Optional[datetime] = None
-        vid: VideoInfo
-        for vid in vid_list:
-            if most_recent_date is None:
-                most_recent_date = parse_datetime(vid.date_published)
-                continue
-            new_datetime = parse_datetime(vid.date_published)
-            if new_datetime > most_recent_date:
-                most_recent_date = new_datetime
-        # get time delta between most recent date and now in days
-        bannons_last_show_in_days: float = 9999
-        if most_recent_date is not None:
-            bannons_last_show_in_days = (
-                now_local() - most_recent_date
-            ).total_seconds() / (3600 * 24)
-
-        self.assertLess(
-            bannons_last_show_in_days,
-            max_days,
-            f"Bannon's last show was {bannons_last_show_in_days} days ago.",
-        )
-
-
-if __name__ == "__main__":
-    unittest.main()
+# pylint: disable=missing-module-docstring,missing-class-docstring,missing-function-docstring
+import unittest
+from datetime import datetime
+from typing import Optional
+
+from vidcrawler.date import now_local, parse_datetime
+from vidcrawler.rumble import fetch_rumble, fetch_rumble_channel_today
+from vidcrawler.video_info import VideoInfo
+
+
+class RumbleScraperTester(unittest.TestCase):
+    def test_fetch_rumble(self):
+        vid_list = fetch_rumble(channel="DiamondandSilk")
+        self.assertTrue(vid_list)
+
+    def test_fetch_alt_channel_url(self):
+        vid_list = fetch_rumble(channel="MaryamXHenein")
+        self.assertTrue(vid_list)
+
+    def test_fetch_bannon(self) -> None:
+        max_days = 4
+        vid_list = fetch_rumble_channel_today(
+            channel="BannonsWarRoom", channel_name="BannonsWarRoom"
+        )
+        most_recent_date: Optional[datetime] = None
+        vid: VideoInfo
+        for vid in vid_list:
+            if most_recent_date is None:
+                most_recent_date = parse_datetime(vid.date_published)
+                continue
+            new_datetime = parse_datetime(vid.date_published)
+            if new_datetime > most_recent_date:
+                most_recent_date = new_datetime
+        # get time delta between most recent date and now in days
+        bannons_last_show_in_days: float = 9999
+        if most_recent_date is not None:
+            bannons_last_show_in_days = (
+                now_local() - most_recent_date
+            ).total_seconds() / (3600 * 24)
+
+        self.assertLess(
+            bannons_last_show_in_days,
+            max_days,
+            f"Bannon's last show was {bannons_last_show_in_days} days ago.",
+        )
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `vidcrawler-1.0.8/vidcrawler/testing/test_scraper_youtube.py` & `vidcrawler-1.0.9/vidcrawler/testing/test_scraper_youtube.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-# pylint: disable=all
-import os
-import tempfile
-import unittest
-from typing import List
-
-import requests
-from vidcrawler.fetch_html import fetch_html
-from vidcrawler.video_info import VideoInfo
-from vidcrawler.youtube import fetch_youtube_today, parse_youtube_video
-
-
-class YouTubeScraperTester(unittest.TestCase):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.cleanup = []
-
-    def tearDown(self):
-        for cleanup in self.cleanup:
-            try:
-                cleanup()
-            except BaseException as be:  # pylint: disable=broad-except
-                print(str(be))
-        self.cleanup = []
-
-    def create_tempfile_path(self) -> str:
-        tmp_file = tempfile.NamedTemporaryFile(suffix=".sqlite3", delete=False)
-        tmp_file.close()
-        self.cleanup.append(lambda: os.remove(tmp_file.name))
-        return os.path.abspath(tmp_file.name)
-
-    def test_fetch_video_info(self):
-        url: str = "https://www.youtube.com/watch?v=5nBqIK0mrFI"
-        content: str = fetch_html(url)
-        d = parse_youtube_video(content)
-        self.assertEqual("False", d["is_live"])
-        self.assertEqual(
-            "https://yt3.ggpht.com/ytc/AKedOLTYHbdYZYe2pG819bvJjRE9GJ518ROSVQ1T-ateXA=s176-c-k-c0x00ffffff-no-rj",
-            d["profile_thumbnail"],
-        )
-
-    def test_bad_content(self):
-        """Stephan Molynuex is banned. This should produce an error."""
-        try:
-            fetch_youtube_today(
-                channel_name="Stefan Molynuex",
-                channel_id="UCC3L8QaxqEGUiBC252GHy3w",
-                cache_path=None,
-            )
-        except OSError:
-            return  # expected result.
-        self.fail("Expected bad channel to raise exception.")
-
-    def test_maryam_henein(self):
-        out: List[VideoInfo] = fetch_youtube_today(
-            channel_name="Maryam Henein",
-            channel_id="UCkw3pE7PwWfQCFFP2YgKVIQ",
-            cache_path=None,
-            limit=1,
-        )
-        self.assertEqual(len(out), 1)
-
-    def test_lex_freemond(self):
-        out: List[VideoInfo] = fetch_youtube_today(
-            channel_name="Lex Fridman",
-            channel_id="UCSHZKyawb77ixDdsGog4iWA",
-            cache_path=None,
-            limit=1,
-        )
-        self.assertEqual(len(out), 1)
-
-    def test_fetch_channel_via_html(self):
-        out = fetch_youtube_today(
-            channel_name="Maryam Henein",
-            channel_id="UCkw3pE7PwWfQCFFP2YgKVIQ",
-            cache_path=None,
-            limit=1,
-        )
-        self.assertEqual(len(out), 1)
-
-    def test_video_xml_api(self):
-        """Tests a major entry point used by the scraper to get YT vids."""
-        # Links to tim pool channel.
-        url = "https://www.youtube.com/feeds/videos.xml?channel_id=UCG749Dj4V2fKa143f8sE60Q"
-        response = requests.get(url)
-        # Raise error if 404 or other error condition.
-        response.raise_for_status()
-
-
-if __name__ == "__main__":
-    unittest.main()
+# pylint: disable=all
+import os
+import tempfile
+import unittest
+from typing import List
+
+import requests
+from vidcrawler.fetch_html import fetch_html
+from vidcrawler.video_info import VideoInfo
+from vidcrawler.youtube import fetch_youtube_today, parse_youtube_video
+
+
+class YouTubeScraperTester(unittest.TestCase):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.cleanup = []
+
+    def tearDown(self):
+        for cleanup in self.cleanup:
+            try:
+                cleanup()
+            except BaseException as be:  # pylint: disable=broad-except
+                print(str(be))
+        self.cleanup = []
+
+    def create_tempfile_path(self) -> str:
+        tmp_file = tempfile.NamedTemporaryFile(suffix=".sqlite3", delete=False)
+        tmp_file.close()
+        self.cleanup.append(lambda: os.remove(tmp_file.name))
+        return os.path.abspath(tmp_file.name)
+
+    def test_fetch_video_info(self):
+        url: str = "https://www.youtube.com/watch?v=5nBqIK0mrFI"
+        content: str = fetch_html(url)
+        d = parse_youtube_video(content)
+        self.assertEqual("False", d["is_live"])
+        self.assertEqual(
+            "https://yt3.ggpht.com/ytc/AMLnZu8YcoqIA7-FfOC0tEwMjTDflDpiMjnJT6GvCXjunw=s176-c-k-c0x00ffffff-no-rj",
+            d["profile_thumbnail"],
+        )
+
+    def test_bad_content(self):
+        """Stephan Molynuex is banned. This should produce an error."""
+        try:
+            fetch_youtube_today(
+                channel_name="Stefan Molynuex",
+                channel_id="UCC3L8QaxqEGUiBC252GHy3w",
+                cache_path=None,
+            )
+        except OSError:
+            return  # expected result.
+        self.fail("Expected bad channel to raise exception.")
+
+    def test_maryam_henein(self):
+        out: List[VideoInfo] = fetch_youtube_today(
+            channel_name="Maryam Henein",
+            channel_id="UCkw3pE7PwWfQCFFP2YgKVIQ",
+            cache_path=None,
+            limit=1,
+        )
+        self.assertEqual(len(out), 1)
+
+    def test_lex_freemond(self):
+        out: List[VideoInfo] = fetch_youtube_today(
+            channel_name="Lex Fridman",
+            channel_id="UCSHZKyawb77ixDdsGog4iWA",
+            cache_path=None,
+            limit=1,
+        )
+        self.assertEqual(len(out), 1)
+
+    def test_fetch_channel_via_html(self):
+        out = fetch_youtube_today(
+            channel_name="Maryam Henein",
+            channel_id="UCkw3pE7PwWfQCFFP2YgKVIQ",
+            cache_path=None,
+            limit=1,
+        )
+        self.assertEqual(len(out), 1)
+
+    def test_video_xml_api(self):
+        """Tests a major entry point used by the scraper to get YT vids."""
+        # Links to tim pool channel.
+        url = "https://www.youtube.com/feeds/videos.xml?channel_id=UCG749Dj4V2fKa143f8sE60Q"
+        response = requests.get(url)
+        # Raise error if 404 or other error condition.
+        response.raise_for_status()
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `vidcrawler-1.0.8/vidcrawler/testing/test_videoinfo.py` & `vidcrawler-1.0.9/vidcrawler/testing/test_videoinfo.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# pylint: disable=all
-
-import unittest
-from typing import List
-
-from vidcrawler.date import now_local
-from vidcrawler.video_info import VideoInfo
-
-
-class VideoInfoTester(unittest.TestCase):
-    def test_one(self) -> None:
-        now_str = str(now_local().isoformat())
-        vid_list = []
-        vi = VideoInfo()
-        vi.title = "test_channel"
-        vi.img_src = "https://example.com/img_src.png"
-        vi.description = "My video description"
-        vi.iframe_src = "https://example/123/player.html"
-        vi.duration = "1:03:53"
-        vi.views = "1000"
-        vi.date_published = "2021-12-21T03:30:19+00:00"
-        vi.channel_url = "https://rumble.com/c/PeteSantilliInterviews"
-        vi.channel_name = "Pete Santilli Interviews"
-        vi.date_published = now_str
-        vi.date_discovered = now_str
-        vi.date_lastupdated = now_str
-        vid_list.append(vi)
-        data: List[List] = VideoInfo.to_compact_csv(vid_list)
-        vid_list2: List[VideoInfo] = VideoInfo.from_compact_csv(data)
-        vi2: VideoInfo = vid_list2[0]
-        self.assertEqual(vi, vi2)
-
-
-if __name__ == "__main__":
-    unittest.main()
+# pylint: disable=all
+
+import unittest
+from typing import List
+
+from vidcrawler.date import now_local
+from vidcrawler.video_info import VideoInfo
+
+
+class VideoInfoTester(unittest.TestCase):
+    def test_one(self) -> None:
+        now_str = str(now_local().isoformat())
+        vid_list = []
+        vi = VideoInfo()
+        vi.title = "test_channel"
+        vi.img_src = "https://example.com/img_src.png"
+        vi.description = "My video description"
+        vi.iframe_src = "https://example/123/player.html"
+        vi.duration = "1:03:53"
+        vi.views = "1000"
+        vi.date_published = "2021-12-21T03:30:19+00:00"
+        vi.channel_url = "https://rumble.com/c/PeteSantilliInterviews"
+        vi.channel_name = "Pete Santilli Interviews"
+        vi.date_published = now_str
+        vi.date_discovered = now_str
+        vi.date_lastupdated = now_str
+        vid_list.append(vi)
+        data: List[List] = VideoInfo.to_compact_csv(vid_list)
+        vid_list2: List[VideoInfo] = VideoInfo.from_compact_csv(data)
+        vi2: VideoInfo = vid_list2[0]
+        self.assertEqual(vi, vi2)
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `vidcrawler-1.0.8/vidcrawler.egg-info/PKG-INFO` & `vidcrawler-1.0.9/vidcrawler.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: vidcrawler
-Version: 1.0.8
+Version: 1.0.9
 Summary: Video Crawler
 Home-page: https://github.com/zackees/vidcrawler
 Author: Zach Vorhies
 Author-email: dont@email.me
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Environment :: Console
@@ -113,17 +112,15 @@
   {
       ...
   }
 ]
 ```
 
 # Releases
-
+  * 1.0.9: Fixes crawler for rumble and minor fixes + linting fixes.
   * 1.0.8: Readme correction.
   * 1.0.7: Fixes Odysee scraper by including image/webp thumbnail format.
   * 1.0.4: Fixes local_now() to be local timezone aware.
   * 1.0.3: Bump
   * 1.0.2: Updates testing
   * 1.0.1: improves command line
   * 1.0.0: Initial release
-
-
```

### Comparing `vidcrawler-1.0.8/vidcrawler.egg-info/SOURCES.txt` & `vidcrawler-1.0.9/vidcrawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*


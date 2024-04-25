# Comparing `tmp/mkt-retv-1.404.tar.gz` & `tmp/mkt-retv-1.405.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkt-retv-1.404.tar", last modified: Wed Apr 24 14:24:23 2024, max compression
+gzip compressed data, was "mkt-retv-1.405.tar", last modified: Thu Apr 25 12:53:14 2024, max compression
```

## Comparing `mkt-retv-1.404.tar` & `mkt-retv-1.405.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 14:24:23.649990 mkt-retv-1.404/
--rw-rw-rw-   0        0        0      697 2024-04-24 14:24:23.634365 mkt-retv-1.404/PKG-INFO
--rw-rw-rw-   0        0        0     1637 2024-01-28 21:55:38.000000 mkt-retv-1.404/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 14:24:23.576707 mkt-retv-1.404/market_research/
--rw-rw-rw-   0        0        0        2 2023-11-21 12:45:19.000000 mkt-retv-1.404/market_research/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:24:23.588588 mkt-retv-1.404/market_research/analysis/
--rw-rw-rw-   0        0        0      167 2024-01-28 14:21:17.000000 mkt-retv-1.404/market_research/analysis/__init__.py
--rw-rw-rw-   0        0        0     1285 2023-11-23 12:49:10.000000 mkt-retv-1.404/market_research/analysis/_analysis_scheme.py
--rw-rw-rw-   0        0        0    10414 2024-01-30 11:22:46.000000 mkt-retv-1.404/market_research/analysis/imgemanger.py
--rw-rw-rw-   0        0        0    11047 2023-12-02 10:26:16.000000 mkt-retv-1.404/market_research/analysis/sentimentmanager.py
--rw-rw-rw-   0        0        0     4939 2024-01-28 14:17:23.000000 mkt-retv-1.404/market_research/analysis/textmanager.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:24:23.592141 mkt-retv-1.404/market_research/scraper/
--rw-rw-rw-   0        0        0      451 2024-01-24 12:15:44.000000 mkt-retv-1.404/market_research/scraper/__init__.py
--rw-rw-rw-   0        0        0     2145 2023-11-21 13:39:46.000000 mkt-retv-1.404/market_research/scraper/_scaper_scheme.py
--rw-rw-rw-   0        0        0      497 2023-11-21 16:22:41.000000 mkt-retv-1.404/market_research/scraper/_visualizer_scheme.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:24:23.596195 mkt-retv-1.404/market_research/scraper/models/
--rw-rw-rw-   0        0        0        0 2023-11-21 12:44:57.000000 mkt-retv-1.404/market_research/scraper/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:24:23.601094 mkt-retv-1.404/market_research/scraper/models/pana/
--rw-rw-rw-   0        0        0        0 2023-11-21 12:44:12.000000 mkt-retv-1.404/market_research/scraper/models/pana/__init__.py
--rw-rw-rw-   0        0        0     6484 2024-01-24 12:45:30.000000 mkt-retv-1.404/market_research/scraper/models/pana/spec_p.py
--rw-rw-rw-   0        0        0    12563 2024-01-24 13:16:23.000000 mkt-retv-1.404/market_research/scraper/models/pana/spec_pjp.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:24:23.611956 mkt-retv-1.404/market_research/scraper/models/sony/
--rw-rw-rw-   0        0        0        4 2023-11-21 12:44:57.000000 mkt-retv-1.404/market_research/scraper/models/sony/__init__.py
--rw-rw-rw-   0        0        0     5203 2024-04-24 13:43:17.000000 mkt-retv-1.404/market_research/scraper/models/sony/cleanup_s.py
--rw-rw-rw-   0        0        0    10226 2024-01-24 12:45:30.000000 mkt-retv-1.404/market_research/scraper/models/sony/sepc_sjp.py
--rw-rw-rw-   0        0        0    11943 2024-04-24 13:28:28.000000 mkt-retv-1.404/market_research/scraper/models/sony/spec_s.py
--rw-rw-rw-   0        0        0     4060 2024-04-24 14:21:40.000000 mkt-retv-1.404/market_research/scraper/models/sony/visualizer_s.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:24:23.618728 mkt-retv-1.404/market_research/scraper/rtings/
--rw-rw-rw-   0        0        0      106 2023-11-19 08:24:51.000000 mkt-retv-1.404/market_research/scraper/rtings/__init__.py
--rw-rw-rw-   0        0        0    10290 2023-11-23 09:57:43.000000 mkt-retv-1.404/market_research/scraper/rtings/rtings.py
--rw-rw-rw-   0        0        0     6309 2023-11-26 10:28:52.000000 mkt-retv-1.404/market_research/scraper/rtings/rurlsearcher.py
--rw-rw-rw-   0        0        0    13793 2023-11-23 12:05:59.000000 mkt-retv-1.404/market_research/scraper/rtings/rvisualizer.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:24:23.618728 mkt-retv-1.404/market_research/tools/
--rw-rw-rw-   0        0        0      206 2023-11-16 08:38:53.000000 mkt-retv-1.404/market_research/tools/__init__.py
--rw-rw-rw-   0        0        0     1003 2023-11-18 14:03:46.000000 mkt-retv-1.404/market_research/tools/aimanager.py
--rw-rw-rw-   0        0        0     3371 2023-11-19 12:13:44.000000 mkt-retv-1.404/market_research/tools/filemanager.py
--rw-rw-rw-   0        0        0     3818 2023-11-14 14:05:22.000000 mkt-retv-1.404/market_research/tools/installer.py
--rw-rw-rw-   0        0        0     5509 2023-11-15 11:16:47.000000 mkt-retv-1.404/market_research/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:24:23.634365 mkt-retv-1.404/mkt_retv.egg-info/
--rw-rw-rw-   0        0        0      697 2024-04-24 14:24:23.000000 mkt-retv-1.404/mkt_retv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1351 2024-04-24 14:24:23.000000 mkt-retv-1.404/mkt_retv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 14:24:23.000000 mkt-retv-1.404/mkt_retv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-04-24 14:24:23.000000 mkt-retv-1.404/mkt_retv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      129 2024-04-24 14:24:23.000000 mkt-retv-1.404/mkt_retv.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-24 14:24:23.000000 mkt-retv-1.404/mkt_retv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 14:24:23.649990 mkt-retv-1.404/setup.cfg
--rw-rw-rw-   0        0        0      959 2024-04-24 14:24:16.000000 mkt-retv-1.404/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:53:14.781938 mkt-retv-1.405/
+-rw-rw-rw-   0        0        0      697 2024-04-25 12:53:14.779867 mkt-retv-1.405/PKG-INFO
+-rw-rw-rw-   0        0        0     1637 2024-01-28 21:55:38.000000 mkt-retv-1.405/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 12:53:14.268007 mkt-retv-1.405/market_research/
+-rw-rw-rw-   0        0        0        2 2023-11-21 12:45:19.000000 mkt-retv-1.405/market_research/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:53:14.346794 mkt-retv-1.405/market_research/analysis/
+-rw-rw-rw-   0        0        0      167 2024-01-28 14:21:17.000000 mkt-retv-1.405/market_research/analysis/__init__.py
+-rw-rw-rw-   0        0        0     1285 2023-11-23 12:49:10.000000 mkt-retv-1.405/market_research/analysis/_analysis_scheme.py
+-rw-rw-rw-   0        0        0    10414 2024-01-30 11:22:46.000000 mkt-retv-1.405/market_research/analysis/imgemanger.py
+-rw-rw-rw-   0        0        0    11047 2023-12-02 10:26:16.000000 mkt-retv-1.405/market_research/analysis/sentimentmanager.py
+-rw-rw-rw-   0        0        0     4939 2024-01-28 14:17:23.000000 mkt-retv-1.405/market_research/analysis/textmanager.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:53:14.390658 mkt-retv-1.405/market_research/scraper/
+-rw-rw-rw-   0        0        0      451 2024-01-24 12:15:44.000000 mkt-retv-1.405/market_research/scraper/__init__.py
+-rw-rw-rw-   0        0        0     2145 2023-11-21 13:39:46.000000 mkt-retv-1.405/market_research/scraper/_scaper_scheme.py
+-rw-rw-rw-   0        0        0      497 2023-11-21 16:22:41.000000 mkt-retv-1.405/market_research/scraper/_visualizer_scheme.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:53:14.394626 mkt-retv-1.405/market_research/scraper/models/
+-rw-rw-rw-   0        0        0        0 2023-11-21 12:44:57.000000 mkt-retv-1.405/market_research/scraper/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:53:14.440562 mkt-retv-1.405/market_research/scraper/models/pana/
+-rw-rw-rw-   0        0        0        0 2023-11-21 12:44:12.000000 mkt-retv-1.405/market_research/scraper/models/pana/__init__.py
+-rw-rw-rw-   0        0        0     6484 2024-01-24 12:45:30.000000 mkt-retv-1.405/market_research/scraper/models/pana/spec_p.py
+-rw-rw-rw-   0        0        0    12563 2024-01-24 13:16:23.000000 mkt-retv-1.405/market_research/scraper/models/pana/spec_pjp.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:53:14.550488 mkt-retv-1.405/market_research/scraper/models/sony/
+-rw-rw-rw-   0        0        0        4 2023-11-21 12:44:57.000000 mkt-retv-1.405/market_research/scraper/models/sony/__init__.py
+-rw-rw-rw-   0        0        0     5188 2024-04-25 12:49:51.000000 mkt-retv-1.405/market_research/scraper/models/sony/cleanup_s.py
+-rw-rw-rw-   0        0        0    10226 2024-01-24 12:45:30.000000 mkt-retv-1.405/market_research/scraper/models/sony/sepc_sjp.py
+-rw-rw-rw-   0        0        0    11943 2024-04-24 13:28:28.000000 mkt-retv-1.405/market_research/scraper/models/sony/spec_s.py
+-rw-rw-rw-   0        0        0     4033 2024-04-25 12:44:14.000000 mkt-retv-1.405/market_research/scraper/models/sony/visualizer_s.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:53:14.606327 mkt-retv-1.405/market_research/scraper/rtings/
+-rw-rw-rw-   0        0        0      106 2023-11-19 08:24:51.000000 mkt-retv-1.405/market_research/scraper/rtings/__init__.py
+-rw-rw-rw-   0        0        0    10290 2023-11-23 09:57:43.000000 mkt-retv-1.405/market_research/scraper/rtings/rtings.py
+-rw-rw-rw-   0        0        0     6309 2023-11-26 10:28:52.000000 mkt-retv-1.405/market_research/scraper/rtings/rurlsearcher.py
+-rw-rw-rw-   0        0        0    13793 2023-11-23 12:05:59.000000 mkt-retv-1.405/market_research/scraper/rtings/rvisualizer.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:53:14.714987 mkt-retv-1.405/market_research/tools/
+-rw-rw-rw-   0        0        0      206 2023-11-16 08:38:53.000000 mkt-retv-1.405/market_research/tools/__init__.py
+-rw-rw-rw-   0        0        0     1003 2023-11-18 14:03:46.000000 mkt-retv-1.405/market_research/tools/aimanager.py
+-rw-rw-rw-   0        0        0     3371 2023-11-19 12:13:44.000000 mkt-retv-1.405/market_research/tools/filemanager.py
+-rw-rw-rw-   0        0        0     3818 2023-11-14 14:05:22.000000 mkt-retv-1.405/market_research/tools/installer.py
+-rw-rw-rw-   0        0        0     5509 2023-11-15 11:16:47.000000 mkt-retv-1.405/market_research/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-04-25 12:53:14.775837 mkt-retv-1.405/mkt_retv.egg-info/
+-rw-rw-rw-   0        0        0      697 2024-04-25 12:53:14.000000 mkt-retv-1.405/mkt_retv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1351 2024-04-25 12:53:14.000000 mkt-retv-1.405/mkt_retv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 12:53:14.000000 mkt-retv-1.405/mkt_retv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-25 12:53:14.000000 mkt-retv-1.405/mkt_retv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      129 2024-04-25 12:53:14.000000 mkt-retv-1.405/mkt_retv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-25 12:53:14.000000 mkt-retv-1.405/mkt_retv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 12:53:14.782956 mkt-retv-1.405/setup.cfg
+-rw-rw-rw-   0        0        0      959 2024-04-25 12:51:00.000000 mkt-retv-1.405/setup.py
```

### Comparing `mkt-retv-1.404/PKG-INFO` & `mkt-retv-1.405/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.404
+Version: 1.405
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.404/README.md` & `mkt-retv-1.405/README.md`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.404/market_research/analysis/_analysis_scheme.py` & `mkt-retv-1.405/market_research/analysis/_analysis_scheme.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.404/market_research/analysis/imgemanger.py` & `mkt-retv-1.405/market_research/analysis/imgemanger.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.404/market_research/analysis/sentimentmanager.py` & `mkt-retv-1.405/market_research/analysis/sentimentmanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.404/market_research/analysis/textmanager.py` & `mkt-retv-1.405/market_research/analysis/textmanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.404/market_research/scraper/_scaper_scheme.py` & `mkt-retv-1.405/market_research/scraper/_scaper_scheme.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.404/market_research/scraper/models/pana/spec_p.py` & `mkt-retv-1.405/market_research/scraper/models/pana/spec_p.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.404/market_research/scraper/models/pana/spec_pjp.py` & `mkt-retv-1.405/market_research/scraper/models/pana/spec_pjp.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.404/market_research/scraper/models/sony/cleanup_s.py` & `mkt-retv-1.405/market_research/scraper/models/sony/cleanup_s.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,21 +28,23 @@
                            "input", "output", "caption", "headphone", "radio", "text", "internet", "dsee", "speaker",
                            "bluetooth", "accessories", "mercury", "remote", "smart", "acoustic", "support",
                            "wallmount", "mic", "network", "android", "ios", "miracast",
                            "operating", "store", "clock", "rs-232c", "menu", "mute", "4:3", "hdcp",
                            "built", "tuners", "demo", "presence", "switch", "reader", "face", "surround", "phase",
                            "batteries", "info", "Parental", "setup", "aspect", "dashboard", "formats", "accessibility",
                            "ci+",
-                           "bass", "master", "shut", "sorplas", "volume", "wireless", "china",
+                           "bass", "shut", "sorplas", "volume", "wireless", "china",
                            "hole", "program", "manual", "latency",
-                           "inversion","twin","h x v","bravia", "motion","calman","rate"]
+                           "inversion","twin","h x v", "motion","calman","rate"]
         return stop_words_list
 
 
 
+
+
     def _preprocess_df(self):
         self.df = self.df.sort_values(["year", "series", "size", "grade"], axis=0, ascending=False)
         self.df = (self.df.map(lambda x: x.replace("  ", " ") if isinstance(x, str) else x)  # 공백 2개는 하나로 변경
                    .map(lambda x: x.replace("™", "") if isinstance(x, str) else x)  # ™ 제거
                    .map(lambda x: x.replace("®", "") if isinstance(x, str) else x)  # ® 제거
                    .map(lambda x: x.replace("\n\n", "\n ") if isinstance(x, str) else x)
                    .map(lambda x: x.replace(" \n", "\n ") if isinstance(x, str) else x)
@@ -82,11 +84,11 @@
                     col_remove.append(column)
         self.df = self.df.drop(col_remove, axis=1)
         self.df = self.df.drop_duplicates()
         self.df = pd.merge(self.df_prices[['model', 'size']], self.df, left_index=True, right_index=True)
 
     def get_df_cleaned(self):
         if self.df is not None:
-            df = self.df.set_index(["year", "display type", "series"]).drop(
+            df = self.df.set_index(["year", "series", "display type"]).drop(
                 ["model", "size", "grade"], axis=1)
             # df = df.fillna("-")
             return df
```

### Comparing `mkt-retv-1.404/market_research/scraper/models/sony/sepc_sjp.py` & `mkt-retv-1.405/market_research/scraper/models/sony/sepc_sjp.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.404/market_research/scraper/models/sony/spec_s.py` & `mkt-retv-1.405/market_research/scraper/models/sony/spec_s.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.404/market_research/scraper/models/sony/visualizer_s.py` & `mkt-retv-1.405/market_research/scraper/models/sony/visualizer_s.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,32 +40,31 @@
         # cividis
         # inferno
         # magma
         # coolwarm
         # Blues
         """
         if col_selected is None:
-            col_selected = ['high peak Luminance','peak luminance',
+            col_selected = ['high peak luminance','peak luminance',
                             'contrast enhancement', 'pixel contrast booster', 'dynamic contrast enhancer','xr backlight master drive',
-                             'color enhancement', 'triluminos',
+                            'color enhancement', 'triluminos',
                             # 'live colour technology',
                              # 'clarity enhancement', 'dual database processing', 'video processing',
                              # 'object-based super resolution',
                              'viewing angle (x-wide angle)', 'x-wide angle',
                              'anti reflection (x-anti reflection)', 'x-anti reflection',
                              'picture processor', '4k processor',
                              # 'color space',
                              # 'eco friendly',
-                             'sony pictures core calibrated mode', 'netflix calibrated mode', 'prime video calibrated mode',
+                             'bravia core calibrated mode','sony pictures core calibrated mode', 'netflix calibrated mode', 'prime video calibrated mode',
                              'auto genre picture mode',
                              'features for playstation5 auto genre picture mode',
                              'auto hdr tone mapping',
                              'features for playstation5 auto hdr tone mapping',
                              'multi-view',
-                             'rated power consumption'
                              ]
 
 
         data_df = self.dc.get_df_cleaned()
         data_df = data_df[col_selected]
         if display_types is not None:
             condition = data_df.index.get_level_values('display type').str.contains('|'.join(display_types), case=False, na=False)
```

### Comparing `mkt-retv-1.404/market_research/scraper/rtings/rtings.py` & `mkt-retv-1.405/market_research/scraper/rtings/rtings.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.404/market_research/scraper/rtings/rurlsearcher.py` & `mkt-retv-1.405/market_research/scraper/rtings/rurlsearcher.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.404/market_research/scraper/rtings/rvisualizer.py` & `mkt-retv-1.405/market_research/scraper/rtings/rvisualizer.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.404/market_research/tools/aimanager.py` & `mkt-retv-1.405/market_research/tools/aimanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.404/market_research/tools/filemanager.py` & `mkt-retv-1.405/market_research/tools/filemanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.404/market_research/tools/installer.py` & `mkt-retv-1.405/market_research/tools/installer.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.404/market_research/tools/webdriver.py` & `mkt-retv-1.405/market_research/tools/webdriver.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.404/mkt_retv.egg-info/PKG-INFO` & `mkt-retv-1.405/mkt_retv.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.404
+Version: 1.405
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.404/mkt_retv.egg-info/SOURCES.txt` & `mkt-retv-1.405/mkt_retv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.404/setup.py` & `mkt-retv-1.405/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mkt-retv',
-    version='1.404',
+    version='1.405',
     author='xikest',
     description='market research TV ',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=[
         'numpy', 'pandas',
         'selenium','beautifulsoup4','requests',
```


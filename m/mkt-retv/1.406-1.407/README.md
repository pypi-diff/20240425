# Comparing `tmp/mkt-retv-1.406.tar.gz` & `tmp/mkt-retv-1.407.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkt-retv-1.406.tar", last modified: Thu Apr 25 13:00:22 2024, max compression
+gzip compressed data, was "mkt-retv-1.407.tar", last modified: Thu Apr 25 14:58:34 2024, max compression
```

## Comparing `mkt-retv-1.406.tar` & `mkt-retv-1.407.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 13:00:22.878032 mkt-retv-1.406/
--rw-rw-rw-   0        0        0      697 2024-04-25 13:00:22.878032 mkt-retv-1.406/PKG-INFO
--rw-rw-rw-   0        0        0     1637 2024-01-28 21:55:38.000000 mkt-retv-1.406/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 13:00:22.782859 mkt-retv-1.406/market_research/
--rw-rw-rw-   0        0        0        2 2023-11-21 12:45:19.000000 mkt-retv-1.406/market_research/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:00:22.798490 mkt-retv-1.406/market_research/analysis/
--rw-rw-rw-   0        0        0      167 2024-01-28 14:21:17.000000 mkt-retv-1.406/market_research/analysis/__init__.py
--rw-rw-rw-   0        0        0     1285 2023-11-23 12:49:10.000000 mkt-retv-1.406/market_research/analysis/_analysis_scheme.py
--rw-rw-rw-   0        0        0    10414 2024-01-30 11:22:46.000000 mkt-retv-1.406/market_research/analysis/imgemanger.py
--rw-rw-rw-   0        0        0    11047 2023-12-02 10:26:16.000000 mkt-retv-1.406/market_research/analysis/sentimentmanager.py
--rw-rw-rw-   0        0        0     4939 2024-01-28 14:17:23.000000 mkt-retv-1.406/market_research/analysis/textmanager.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:00:22.798490 mkt-retv-1.406/market_research/scraper/
--rw-rw-rw-   0        0        0      451 2024-01-24 12:15:44.000000 mkt-retv-1.406/market_research/scraper/__init__.py
--rw-rw-rw-   0        0        0     2145 2023-11-21 13:39:46.000000 mkt-retv-1.406/market_research/scraper/_scaper_scheme.py
--rw-rw-rw-   0        0        0      497 2023-11-21 16:22:41.000000 mkt-retv-1.406/market_research/scraper/_visualizer_scheme.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:00:22.798490 mkt-retv-1.406/market_research/scraper/models/
--rw-rw-rw-   0        0        0        0 2023-11-21 12:44:57.000000 mkt-retv-1.406/market_research/scraper/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:00:22.798490 mkt-retv-1.406/market_research/scraper/models/pana/
--rw-rw-rw-   0        0        0        0 2023-11-21 12:44:12.000000 mkt-retv-1.406/market_research/scraper/models/pana/__init__.py
--rw-rw-rw-   0        0        0     6484 2024-01-24 12:45:30.000000 mkt-retv-1.406/market_research/scraper/models/pana/spec_p.py
--rw-rw-rw-   0        0        0    12563 2024-01-24 13:16:23.000000 mkt-retv-1.406/market_research/scraper/models/pana/spec_pjp.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:00:22.814099 mkt-retv-1.406/market_research/scraper/models/sony/
--rw-rw-rw-   0        0        0        4 2023-11-21 12:44:57.000000 mkt-retv-1.406/market_research/scraper/models/sony/__init__.py
--rw-rw-rw-   0        0        0     5188 2024-04-25 12:49:51.000000 mkt-retv-1.406/market_research/scraper/models/sony/cleanup_s.py
--rw-rw-rw-   0        0        0    10226 2024-01-24 12:45:30.000000 mkt-retv-1.406/market_research/scraper/models/sony/sepc_sjp.py
--rw-rw-rw-   0        0        0    11943 2024-04-24 13:28:28.000000 mkt-retv-1.406/market_research/scraper/models/sony/spec_s.py
--rw-rw-rw-   0        0        0     4078 2024-04-25 12:58:16.000000 mkt-retv-1.406/market_research/scraper/models/sony/visualizer_s.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:00:22.814099 mkt-retv-1.406/market_research/scraper/rtings/
--rw-rw-rw-   0        0        0      106 2023-11-19 08:24:51.000000 mkt-retv-1.406/market_research/scraper/rtings/__init__.py
--rw-rw-rw-   0        0        0    10290 2023-11-23 09:57:43.000000 mkt-retv-1.406/market_research/scraper/rtings/rtings.py
--rw-rw-rw-   0        0        0     6309 2023-11-26 10:28:52.000000 mkt-retv-1.406/market_research/scraper/rtings/rurlsearcher.py
--rw-rw-rw-   0        0        0    13793 2023-11-23 12:05:59.000000 mkt-retv-1.406/market_research/scraper/rtings/rvisualizer.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:00:22.829788 mkt-retv-1.406/market_research/tools/
--rw-rw-rw-   0        0        0      206 2023-11-16 08:38:53.000000 mkt-retv-1.406/market_research/tools/__init__.py
--rw-rw-rw-   0        0        0     1003 2023-11-18 14:03:46.000000 mkt-retv-1.406/market_research/tools/aimanager.py
--rw-rw-rw-   0        0        0     3371 2023-11-19 12:13:44.000000 mkt-retv-1.406/market_research/tools/filemanager.py
--rw-rw-rw-   0        0        0     3818 2023-11-14 14:05:22.000000 mkt-retv-1.406/market_research/tools/installer.py
--rw-rw-rw-   0        0        0     5509 2023-11-15 11:16:47.000000 mkt-retv-1.406/market_research/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-04-25 13:00:22.878032 mkt-retv-1.406/mkt_retv.egg-info/
--rw-rw-rw-   0        0        0      697 2024-04-25 13:00:22.000000 mkt-retv-1.406/mkt_retv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1351 2024-04-25 13:00:22.000000 mkt-retv-1.406/mkt_retv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 13:00:22.000000 mkt-retv-1.406/mkt_retv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-04-25 13:00:22.000000 mkt-retv-1.406/mkt_retv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      129 2024-04-25 13:00:22.000000 mkt-retv-1.406/mkt_retv.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-25 13:00:22.000000 mkt-retv-1.406/mkt_retv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 13:00:22.878032 mkt-retv-1.406/setup.cfg
--rw-rw-rw-   0        0        0      959 2024-04-25 12:58:24.000000 mkt-retv-1.406/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:58:34.366094 mkt-retv-1.407/
+-rw-rw-rw-   0        0        0      697 2024-04-25 14:58:34.366094 mkt-retv-1.407/PKG-INFO
+-rw-rw-rw-   0        0        0     1637 2024-01-28 21:55:38.000000 mkt-retv-1.407/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 14:58:33.878100 mkt-retv-1.407/market_research/
+-rw-rw-rw-   0        0        0        2 2023-11-21 12:45:19.000000 mkt-retv-1.407/market_research/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:58:33.972791 mkt-retv-1.407/market_research/analysis/
+-rw-rw-rw-   0        0        0      167 2024-01-28 14:21:17.000000 mkt-retv-1.407/market_research/analysis/__init__.py
+-rw-rw-rw-   0        0        0     1285 2023-11-23 12:49:10.000000 mkt-retv-1.407/market_research/analysis/_analysis_scheme.py
+-rw-rw-rw-   0        0        0    10414 2024-01-30 11:22:46.000000 mkt-retv-1.407/market_research/analysis/imgemanger.py
+-rw-rw-rw-   0        0        0    11047 2023-12-02 10:26:16.000000 mkt-retv-1.407/market_research/analysis/sentimentmanager.py
+-rw-rw-rw-   0        0        0     4939 2024-01-28 14:17:23.000000 mkt-retv-1.407/market_research/analysis/textmanager.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:58:34.019623 mkt-retv-1.407/market_research/scraper/
+-rw-rw-rw-   0        0        0      451 2024-01-24 12:15:44.000000 mkt-retv-1.407/market_research/scraper/__init__.py
+-rw-rw-rw-   0        0        0     2145 2023-11-21 13:39:46.000000 mkt-retv-1.407/market_research/scraper/_scaper_scheme.py
+-rw-rw-rw-   0        0        0      497 2023-11-21 16:22:41.000000 mkt-retv-1.407/market_research/scraper/_visualizer_scheme.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:58:34.019623 mkt-retv-1.407/market_research/scraper/models/
+-rw-rw-rw-   0        0        0        0 2023-11-21 12:44:57.000000 mkt-retv-1.407/market_research/scraper/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:58:34.068391 mkt-retv-1.407/market_research/scraper/models/pana/
+-rw-rw-rw-   0        0        0        0 2023-11-21 12:44:12.000000 mkt-retv-1.407/market_research/scraper/models/pana/__init__.py
+-rw-rw-rw-   0        0        0     6484 2024-01-24 12:45:30.000000 mkt-retv-1.407/market_research/scraper/models/pana/spec_p.py
+-rw-rw-rw-   0        0        0    12563 2024-01-24 13:16:23.000000 mkt-retv-1.407/market_research/scraper/models/pana/spec_pjp.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:58:34.146841 mkt-retv-1.407/market_research/scraper/models/sony/
+-rw-rw-rw-   0        0        0        4 2023-11-21 12:44:57.000000 mkt-retv-1.407/market_research/scraper/models/sony/__init__.py
+-rw-rw-rw-   0        0        0     5265 2024-04-25 14:52:31.000000 mkt-retv-1.407/market_research/scraper/models/sony/cleanup_s.py
+-rw-rw-rw-   0        0        0    10226 2024-01-24 12:45:30.000000 mkt-retv-1.407/market_research/scraper/models/sony/sepc_sjp.py
+-rw-rw-rw-   0        0        0    12121 2024-04-25 13:55:31.000000 mkt-retv-1.407/market_research/scraper/models/sony/spec_s.py
+-rw-rw-rw-   0        0        0     4189 2024-04-25 14:57:40.000000 mkt-retv-1.407/market_research/scraper/models/sony/visualizer_s.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:58:34.225002 mkt-retv-1.407/market_research/scraper/rtings/
+-rw-rw-rw-   0        0        0      106 2023-11-19 08:24:51.000000 mkt-retv-1.407/market_research/scraper/rtings/__init__.py
+-rw-rw-rw-   0        0        0    10290 2023-11-23 09:57:43.000000 mkt-retv-1.407/market_research/scraper/rtings/rtings.py
+-rw-rw-rw-   0        0        0     6309 2023-11-26 10:28:52.000000 mkt-retv-1.407/market_research/scraper/rtings/rurlsearcher.py
+-rw-rw-rw-   0        0        0    13793 2023-11-23 12:05:59.000000 mkt-retv-1.407/market_research/scraper/rtings/rvisualizer.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:58:34.287507 mkt-retv-1.407/market_research/tools/
+-rw-rw-rw-   0        0        0      206 2023-11-16 08:38:53.000000 mkt-retv-1.407/market_research/tools/__init__.py
+-rw-rw-rw-   0        0        0     1003 2023-11-18 14:03:46.000000 mkt-retv-1.407/market_research/tools/aimanager.py
+-rw-rw-rw-   0        0        0     3371 2023-11-19 12:13:44.000000 mkt-retv-1.407/market_research/tools/filemanager.py
+-rw-rw-rw-   0        0        0     3818 2023-11-14 14:05:22.000000 mkt-retv-1.407/market_research/tools/installer.py
+-rw-rw-rw-   0        0        0     5509 2023-11-15 11:16:47.000000 mkt-retv-1.407/market_research/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:58:34.350440 mkt-retv-1.407/mkt_retv.egg-info/
+-rw-rw-rw-   0        0        0      697 2024-04-25 14:58:33.000000 mkt-retv-1.407/mkt_retv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1351 2024-04-25 14:58:33.000000 mkt-retv-1.407/mkt_retv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 14:58:33.000000 mkt-retv-1.407/mkt_retv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-25 14:58:33.000000 mkt-retv-1.407/mkt_retv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      129 2024-04-25 14:58:33.000000 mkt-retv-1.407/mkt_retv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-25 14:58:33.000000 mkt-retv-1.407/mkt_retv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 14:58:34.366094 mkt-retv-1.407/setup.cfg
+-rw-rw-rw-   0        0        0      959 2024-04-25 14:58:14.000000 mkt-retv-1.407/setup.py
```

### Comparing `mkt-retv-1.406/PKG-INFO` & `mkt-retv-1.407/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.406
+Version: 1.407
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.406/README.md` & `mkt-retv-1.407/README.md`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.406/market_research/analysis/_analysis_scheme.py` & `mkt-retv-1.407/market_research/analysis/_analysis_scheme.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.406/market_research/analysis/imgemanger.py` & `mkt-retv-1.407/market_research/analysis/imgemanger.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.406/market_research/analysis/sentimentmanager.py` & `mkt-retv-1.407/market_research/analysis/sentimentmanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.406/market_research/analysis/textmanager.py` & `mkt-retv-1.407/market_research/analysis/textmanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.406/market_research/scraper/_scaper_scheme.py` & `mkt-retv-1.407/market_research/scraper/_scaper_scheme.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.406/market_research/scraper/models/pana/spec_p.py` & `mkt-retv-1.407/market_research/scraper/models/pana/spec_p.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.406/market_research/scraper/models/pana/spec_pjp.py` & `mkt-retv-1.407/market_research/scraper/models/pana/spec_pjp.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.406/market_research/scraper/models/sony/cleanup_s.py` & `mkt-retv-1.407/market_research/scraper/models/sony/cleanup_s.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,29 +16,29 @@
         self.stop_words.extend(["model","size"])
         self._preprocess_df()
         self._create_price_df()
         self._cleanup_columns()
 
     def _call_stop_words(self):
         stop_words_list = ["price", "description",
-                           "weight", "dimension", "stand", "W x H", "W x H x D", "Wi-Fi", "atore", "audio",
-                           "frame", "length", "qty",
-                           "power", "usb", "channels", "language", "timer", "apple", "TALKBACK", "voice", "sensor",
-                           "system", "channel", "storage", "cable",
-                           "style", "protection", "hdmi", "energy", "sound", "camera", "subwoofer", "satellite",
-                           "input", "output", "caption", "headphone", "radio", "text", "internet", "dsee", "speaker",
-                           "bluetooth", "accessories", "mercury", "remote", "smart", "acoustic", "support",
-                           "wallmount", "mic", "network", "android", "ios", "miracast",
-                           "operating", "store", "clock", "rs-232c", "menu", "mute", "4:3", "hdcp",
-                           "built", "tuners", "demo", "presence", "switch", "reader", "face", "surround", "phase",
-                           "batteries", "info", "Parental", "setup", "aspect", "dashboard", "formats", "accessibility",
-                           "ci+",
-                           "bass", "shut", "sorplas", "volume", "wireless", "china",
-                           "hole", "program", "manual", "latency",
-                           "inversion","twin","h x v", "motion","calman","rate"]
+                                  "weight", "dimension", "stand", "W x H", "W x H x D", "Wi-Fi", "atore", "audio",
+                                  "frame", "length", "qty",
+                                  "power", "usb", "channels", "language", "timer", "apple", "TALKBACK", "voice", "sensor",
+                                  "system", "channel", "storage", "cable",
+                                  "style", "protection", "hdmi", "energy", "sound", "camera", "subwoofer", "satellite",
+                                  "input", "output", "caption", "headphone", "radio", "text", "internet", "dsee", "speaker",
+                                  "bluetooth", "accessories", "mercury", "remote", "smart", "acoustic", "support",
+                                  "wallmount", "network", "android", "ios", "miracast",
+                                  "operating", "store", "clock", "rs-232c", "menu", "mute", "4:3", "hdcp",
+                                  "built", "tuners", "demo", "presence", "switch", "reader", "face", "surround", "phase",
+                                  "batteries", "info", "Parental", "setup", "aspect", "dashboard", "formats", "accessibility",
+                                  "ci+",
+                                  "bass", "shut", "sorplas", "volume", "wireless", "china",
+                                  "hole", "program", "manual", "latency",
+                                  "twin","h x v", "motion","calman"]
         return stop_words_list
 
 
 
 
 
     def _preprocess_df(self):
@@ -87,8 +87,8 @@
         self.df = pd.merge(self.df_prices[['model', 'size']], self.df, left_index=True, right_index=True)
 
     def get_df_cleaned(self):
         if self.df is not None:
             df = self.df.set_index(["year", "series", "display type"]).drop(
                 ["model", "size", "grade"], axis=1)
             # df = df.fillna("-")
-            return df
+            return df
```

### Comparing `mkt-retv-1.406/market_research/scraper/models/sony/sepc_sjp.py` & `mkt-retv-1.407/market_research/scraper/models/sony/sepc_sjp.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.406/market_research/scraper/models/sony/spec_s.py` & `mkt-retv-1.407/market_research/scraper/models/sony/spec_s.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self.tracking_log = verbose
         self.wait_time = wait_time
         self.file_manager = FileManager
         self.log_dir = "logs/sony/models"
         if self.tracking_log:
             FileManager.make_dir(self.log_dir)
 
-    def get_models_info(self, foramt_output:str='df', fastmode:bool=False):
+    def get_models_info(self, foramt_output:str='df', fastmode:bool=False, temporary_year_marking=False):
         print("collecting models")
         url_series_set = self._get_url_series()
         url_series_dict = {}
         for url in url_series_set:
             url_models = self._get_models(url=url)
             url_series_dict.update(url_models)
         print("number of total model:", len(url_series_dict))
@@ -48,14 +48,16 @@
                 print(f"Failed to get info from {key}")
                 pass
 
         for model, url in visit_url_dict.items():  print(f"{model}: {url}")
 
         if foramt_output == "df":
             df_models = pd.DataFrame.from_dict(dict_models).T
+            if temporary_year_marking:
+                df_models['year'] = df_models['year'].fillna(2024) ## 임시
             FileManager.df_to_excel(df_models.reset_index(), file_name=self.output_xlsx_name, sheet_name="raw_na", mode='w')
             return df_models
         else:
             return dict_models
 
 
     def _get_url_series(self) -> set:
@@ -212,15 +214,16 @@
                     driver.save_screenshot(f"./{dir_model}/{stamp_url}_4_end_{stamp_today}.png")
                 driver.quit()
                 if self.tracking_log:
                     print(f"Received information from {url}")
                 return dict_spec
             except Exception as e:
                 print(f"An error occurred on page 3rd : {model} try {cnt_try + 1}/{try_total}")
-                print(e)
+                if self.tracking_log:
+                    print(e)
                 driver.quit()
                 pass
 
     def _extract_model_info(self, model):
         """
         Extract additional information from the model name.
         """
@@ -236,15 +239,15 @@
             'J': 2021,
             # Add additional mappings as needed
         }
 
         try:
             dict_info["year"] = year_mapping.get(dict_info.get("year"))
         except:
-            dict_info["year"] = "2024_" ## 임시
+            dict_info["year"] = None
 
         return dict_info
 
     def _soup_to_dict(self, soup):
         """
         Convert BeautifulSoup soup to dictionary.
         """
```

### Comparing `mkt-retv-1.406/market_research/scraper/models/sony/visualizer_s.py` & `mkt-retv-1.407/market_research/scraper/models/sony/visualizer_s.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,25 +65,28 @@
 
 
         data_df = self.dc.get_df_cleaned()
         data_df = data_df[col_selected]
         if display_types is not None:
             condition = data_df.index.get_level_values('display type').str.contains('|'.join(display_types), case=False, na=False)
             data_df = data_df[condition]
-        data_df = data_df.replace({"-": 0})
+        data_df = data_df.mask(data_df == '-', 0)
         data_df = data_df.map(lambda x: len(x.split(",")) if isinstance(x, str) else x)
         data_df = data_df.fillna(0)
+        idx_names = data_df.index.names
+        data_df = data_df.reset_index().drop_duplicates()
+        data_df = data_df.set_index(idx_names)
         data_df = data_df.sort_index(ascending=True)
-        data_df = data_df.drop_duplicates()
         # Use plt.subplots to get the axis for colorbar
         self.data_df = data_df
 
         # Use plt.subplots to get the axis for colorbar
         fig, ax = plt.subplots(figsize=figsize)
         sns.heatmap(data_df.T, cmap=cmap, cbar=cbar, ax=ax, vmax=1)
         plt.xticks(rotation=90)
         plt.title(title)
         if save_plot_name is None:
             save_plot_name = f"heatmap_for_{title}.png"
         plt.savefig(self.output_folder/save_plot_name, bbox_inches='tight')
         plt.show()
 
+
```

### Comparing `mkt-retv-1.406/market_research/scraper/rtings/rtings.py` & `mkt-retv-1.407/market_research/scraper/rtings/rtings.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.406/market_research/scraper/rtings/rurlsearcher.py` & `mkt-retv-1.407/market_research/scraper/rtings/rurlsearcher.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.406/market_research/scraper/rtings/rvisualizer.py` & `mkt-retv-1.407/market_research/scraper/rtings/rvisualizer.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.406/market_research/tools/aimanager.py` & `mkt-retv-1.407/market_research/tools/aimanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.406/market_research/tools/filemanager.py` & `mkt-retv-1.407/market_research/tools/filemanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.406/market_research/tools/installer.py` & `mkt-retv-1.407/market_research/tools/installer.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.406/market_research/tools/webdriver.py` & `mkt-retv-1.407/market_research/tools/webdriver.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.406/mkt_retv.egg-info/PKG-INFO` & `mkt-retv-1.407/mkt_retv.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.406
+Version: 1.407
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.406/mkt_retv.egg-info/SOURCES.txt` & `mkt-retv-1.407/mkt_retv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.406/setup.py` & `mkt-retv-1.407/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mkt-retv',
-    version='1.406',
+    version='1.407',
     author='xikest',
     description='market research TV ',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=[
         'numpy', 'pandas',
         'selenium','beautifulsoup4','requests',
```


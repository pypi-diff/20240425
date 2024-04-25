# Comparing `tmp/tiktok_uploader-1.0.16.tar.gz` & `tmp/tiktok_uploader-1.0.2.tar.gz`

## Comparing `tiktok_uploader-1.0.16.tar` & `tiktok_uploader-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,26 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/.DS_Store
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/LISCENSE
--rw-r--r--   0        0        0    11979 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/README.de.md
--rw-r--r--   0        0        0    11736 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/README.es.md
--rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/README.fr.md
--rw-r--r--   0        0        0    10497 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/README.zh-Hans.md
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/.github/FUNDING.yml
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/.github/workflows/build-hatch.yml
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/.github/workflows/link_checker.yml
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/examples/basic_upload.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/examples/multiple_videos_at_once.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/examples/series_upload.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/src/tiktok_uploader/__init__.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/src/tiktok_uploader/__main__.py
--rw-r--r--   0        0        0     7408 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/src/tiktok_uploader/auth.py
--rw-r--r--   0        0        0     5778 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/src/tiktok_uploader/browsers.py
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/src/tiktok_uploader/cli.py
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/src/tiktok_uploader/config.toml
--rw-r--r--   0        0        0    29156 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/src/tiktok_uploader/upload.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/src/tiktok_uploader/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/src/tiktok_uploader/proxy_auth_extension/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/src/tiktok_uploader/proxy_auth_extension/background.js
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/src/tiktok_uploader/proxy_auth_extension/manifest.json
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/src/tiktok_uploader/proxy_auth_extension/proxy_auth_extension.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/tests/__init__.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/tests/test_browsers.py
--rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/tests/test_upload.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/.gitignore
--rw-r--r--   0        0        0    10846 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/README.md
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/pyproject.toml
--rw-r--r--   0        0        0    11726 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.16/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/.DS_Store
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/LISCENSE
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/.github/workflows/build-hatch.yml
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/.github/workflows/link_checker.yml
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/examples/basic_upload.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/examples/multiple_videos_at_once.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/examples/series_upload.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/src/tiktok_uploader/__init__.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/src/tiktok_uploader/__main__.py
+-rw-r--r--   0        0        0     7408 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/src/tiktok_uploader/auth.py
+-rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/src/tiktok_uploader/browsers.py
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/src/tiktok_uploader/cli.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/src/tiktok_uploader/config.toml
+-rw-r--r--   0        0        0    26072 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/src/tiktok_uploader/upload.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/src/tiktok_uploader/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/src/tiktok_uploader/proxy_auth_extension/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/src/tiktok_uploader/proxy_auth_extension/background.js
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/src/tiktok_uploader/proxy_auth_extension/manifest.json
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/src/tiktok_uploader/proxy_auth_extension/proxy_auth_extension.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/tests/test_browsers.py
+-rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/tests/test_upload.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/.gitignore
+-rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/README.md
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    10495 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.2/PKG-INFO
```

### Comparing `tiktok_uploader-1.0.16/.DS_Store` & `tiktok_uploader-1.0.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.16/LISCENSE` & `tiktok_uploader-1.0.2/LISCENSE`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.16/.github/workflows/build-hatch.yml` & `tiktok_uploader-1.0.2/.github/workflows/build-hatch.yml`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.16/examples/multiple_videos_at_once.py` & `tiktok_uploader-1.0.2/examples/multiple_videos_at_once.py`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.16/examples/series_upload.py` & `tiktok_uploader-1.0.2/examples/series_upload.py`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.16/src/tiktok_uploader/__init__.py` & `tiktok_uploader-1.0.2/src/tiktok_uploader/__init__.py`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.16/src/tiktok_uploader/auth.py` & `tiktok_uploader-1.0.2/src/tiktok_uploader/auth.py`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.16/src/tiktok_uploader/browsers.py` & `tiktok_uploader-1.0.2/src/tiktok_uploader/browsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,17 +87,14 @@
     options.add_argument('--disable-blink-features=AutomationControlled')
     options.add_argument('--profile-directory=Default')
 
     ## experimental
     options.add_experimental_option('excludeSwitches', ['enable-automation'])
     options.add_experimental_option('useAutomationExtension', False)
 
-    ## add english language to avoid languages translation error
-    options.add_argument("--lang=en")
-    
     # headless
     if headless:
         options.add_argument('--headless=new')
     if proxy:
         if 'user' in proxy.keys() and 'pass' in proxy.keys():
             # This can fail if you are executing the function more than once in the same time
             extension_file = 'temp_proxy_auth_extension.zip'
```

### Comparing `tiktok_uploader-1.0.16/src/tiktok_uploader/cli.py` & `tiktok_uploader-1.0.2/src/tiktok_uploader/cli.py`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.16/src/tiktok_uploader/config.toml` & `tiktok_uploader-1.0.2/src/tiktok_uploader/config.toml`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 # Messing around with inputs
 valid_path_names = ["path", "filename", "video", "video_path"]
 valid_descriptions = ["description", "desc", "caption"]
 
 # Selenium Webdriver Waits
 implicit_wait = 5  # seconds
 explicit_wait = 60 # seconds
-uploading_wait = 180 # seconds
 
 supported_file_types = ["mp4", "mov", "avi", "wmv", "flv", "webm", "mkv", "m4v", "3gp", "3g2", "gif"]
 
 max_description_length = 150 # characters
 
 [paths]
 main = "https://www.tiktok.com/"
@@ -34,33 +33,35 @@
 	alert_user_if_failed = true # sends an alert and waits instead of failing
 	
 	cookie_of_interest = "sessionid" # cookie to check if login was successful
 	
 	[selectors.upload]
 	iframe = "//iframe"
 	
-	split_window = "//button[./div[text()='Not now']]"
 	upload_video = "//input[@type='file']"
-	upload_finished = "//div[contains(@class, 'btn-cancel')]"
- 	upload_confirmation = "//div[@title]"
- 	process_confirmation = "//div[contains(@class, 'cover-selector-image-container')]/img[contains(@class, 'cover-selector-image')]"
+	upload_in_progress = "//*[.='Cancel']"
+	upload_confirmation = "//video" 
+	process_confirmation = "//img[@draggable='false']"
+
 	description = "//div[@contenteditable='true']"
 
 	visibility = "//div[@class='tiktok-select-selector']"
 	options = ["Public", "Friends", "Private"]
 
-	mention_box = "//div[contains(@class, 'mention-list-popover')]"
-	mention_box_user_id = "//span[contains(@class, 'user-id')]"
+	hashtags = "//div[@class='mentionSuggestions']//*[contains(text(), '{}')]"
+	mentions = "//div[contains(concat(' ', normalize-space(@class), ' '), 'user-id') and .='{}']/.."
+
+	mention_box = "//input[contains(concat(' ', normalize-space(@class), ' '), 'search-friends')]"
 
 	comment = "//label[.='Comment']/following-sibling::div/input"
 	duet = "//label[.='Duet']/following-sibling::div/input"
 	stitch = "//label[.='Stitch']/following-sibling::div/input"
 
 	post = "//div[contains(@class, 'btn-post')]"
-	post_confirmation = "//div[contains(@class, 'tiktok-modal__modal-wrapper')]//div[contains(@class, 'tiktok-modal__modal-title') and contains(text(), 'Your videos are being posted to TikTok!')]"
+	post_confirmation = "//div[.='Your videos are being uploaded to TikTok!']"
 
 	[selectors.schedule]
 	switch = "//*[@id='tux-3']"
 
 	date_picker = "//div[contains(@class, 'date-picker-input')]"
 	calendar = "//div[contains(@class, 'calendar-wrapper')]"
 	calendar_month = "//span[contains(@class, 'month-title')]"
@@ -68,11 +69,7 @@
 	calendar_arrows = "//span[contains(@class, 'arrow')]"  # first last, second next
 
 	time_picker = "//div[contains(@class, 'time-picker-input')]"
 	time_picker_text = "//div[contains(@class, 'time-picker-input')]/*[1]"
 	time_picker_container = "//div[@class='tiktok-timepicker-time-picker-container']"
 	timepicker_hours = "//span[contains(@class, 'tiktok-timepicker-left')]"
 	timepicker_minutes = "//span[contains(@class, 'tiktok-timepicker-right')]"
-
-	[selectors.upload.cookies_banner]
-		banner = "tiktok-cookie-banner"
-		button = "div.button-wrapper"
```

### Comparing `tiktok_uploader-1.0.16/src/tiktok_uploader/upload.py` & `tiktok_uploader-1.0.2/src/tiktok_uploader/upload.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,39 +2,37 @@
 `tiktok_uploader` module for uploading videos to TikTok
 
 Key Functions
 -------------
 upload_video : Uploads a single TikTok video
 upload_videos : Uploads multiple TikTok videos
 """
-
 from os.path import abspath, exists
 from typing import List
 import time
 import pytz
 import datetime
-import threading
 
 from selenium.webdriver.common.by import By
 
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.keys import Keys
-from selenium.common.exceptions import ElementClickInterceptedException, TimeoutException
+from selenium.common.exceptions import ElementClickInterceptedException
 
 from tiktok_uploader.browsers import get_browser
 from tiktok_uploader.auth import AuthBackend
 from tiktok_uploader import config, logger
-from tiktok_uploader.utils import bold, cyan, green, red
+from tiktok_uploader.utils import bold, green
 from tiktok_uploader.proxy_auth_extension.proxy_auth_extension import proxy_is_working
 
 
-def upload_video(filename=None, description='', cookies='', schedule: datetime.datetime = None, username='',
-                 password='', sessionid=None, cookies_list=None, cookies_str=None, proxy=None, *args, **kwargs):
+def upload_video(filename=None, description='', schedule: datetime.datetime = None, username='',
+                 password='', cookies='', sessionid=None, cookies_list=None, cookies_str=None, proxy=None, *args, **kwargs):
     """
     Uploads a single TikTok video.
 
     Consider using `upload_videos` if using multiple videos
 
     Parameters
     ----------
@@ -58,15 +56,15 @@
             auth=auth,
             proxy=proxy,
             *args, **kwargs
         )
 
 
 def upload_videos(videos: list = None, auth: AuthBackend = None, proxy: dict = None, browser='chrome',
-                  browser_agent=None, on_complete=None, headless=False, num_retries : int = 1, skip_split_window=False, *args, **kwargs):
+                  browser_agent=None, on_complete=None, headless=False, num_retires : int = 1, *args, **kwargs):
     """
     Uploads multiple videos to TikTok
 
     Parameters
     ----------
     videos : list
         A list of dictionaries containing the video's ('path') and description ('description')
@@ -148,61 +146,43 @@
                 schedule = _get_valid_schedule_minute(schedule, valid_tiktok_minute_multiple)
                 if not _check_valid_schedule(schedule):
                     print(f'{schedule} is invalid, the schedule datetime must be as least 20 minutes in the future, and a maximum of 10 days, skipping')
                     failed.append(video)
                     continue
 
             complete_upload_form(driver, path, description, schedule,
-                                 num_retries=num_retries, 
-                                 skip_split_window=skip_split_window,
-                                 headless=headless,*args, **kwargs)
+                                 num_retires=num_retires, headless=headless,
+                                 *args, **kwargs)
         except Exception as exception:
             logger.error('Failed to upload %s', path)
             logger.error(exception)
             failed.append(video)
 
         if on_complete is callable: # calls the user-specified on-complete function
             on_complete(video)
 
     if config['quit_on_end']:
         driver.quit()
 
     return failed
 
 
-def complete_upload_form(driver, path: str, description: str, schedule: datetime.datetime, skip_split_window: bool, headless=False,  *args, **kwargs) -> None:
+def complete_upload_form(driver, path: str, description: str, schedule: datetime.datetime, headless=False, *args, **kwargs) -> None:
     """
     Actually uploads each video
 
     Parameters
     ----------
     driver : selenium.webdriver
         The selenium webdriver to use for uploading
     path : str
         The path to the video to upload
     """
     _go_to_upload(driver)
-    #  _remove_cookies_window(driver)
-    
-    upload_complete_event = threading.Event()
-    
-    # Function to call _set_video and set the event when it's done
-    def upload_video():
-        _set_video(driver, path=path, **kwargs)
-        upload_complete_event.set()
-    
-    # Start the upload_video function in a separate thread
-    upload_thread = threading.Thread(target=upload_video)
-    upload_thread.start()
-    
-    # Wait for the upload to complete before proceeding
-    upload_complete_event.wait()
-    
-    if not skip_split_window:
-        _remove_split_window(driver)
+    _set_video(driver, path=path, **kwargs)
     _set_interactivity(driver, **kwargs)
     _set_description(driver, description)
     if schedule:
         _set_schedule_video(driver, schedule)
     _post_video(driver)
 
 
@@ -220,37 +200,25 @@
     if driver.current_url != config['paths']['upload']:
         driver.get(config['paths']['upload'])
     # otherwise, refresh the page and accept the reload alert
     else:
         _refresh_with_alert(driver)
 
     # changes to the iframe
-    _change_to_upload_iframe(driver)
-
-    # waits for the iframe to load
-    root_selector = EC.presence_of_element_located((By.ID, 'root'))
-    WebDriverWait(driver, config['explicit_wait']).until(root_selector)
-
-    # Return to default webpage
-    driver.switch_to.default_content()
-
-def _change_to_upload_iframe(driver) -> None:
-    """
-    Switch to the iframe of the upload page
-
-    Parameters
-    ----------
-    driver : selenium.webdriver
-    """
     iframe_selector = EC.presence_of_element_located(
         (By.XPATH, config['selectors']['upload']['iframe'])
         )
     iframe = WebDriverWait(driver, config['explicit_wait']).until(iframe_selector)
     driver.switch_to.frame(iframe)
 
+    # waits for the iframe to load
+    root_selector = EC.presence_of_element_located((By.ID, 'root'))
+    WebDriverWait(driver, config['explicit_wait']).until(root_selector)
+
+
 def _set_description(driver, description: str) -> None:
     """
     Sets the description of the video
 
     Parameters
     ----------
     driver : selenium.webdriver
@@ -259,106 +227,86 @@
     """
     if description is None:
         # if no description is provided, filename
         return
 
     logger.debug(green('Setting description'))
 
-    # Remove any characters outside the BMP range (emojis, etc) & Fix accents
-    description = description.encode('utf-8', 'ignore').decode('utf-8')
+    # Remove any characters outside the BMP range (emojis, etc)
+    description = description.encode('ascii', 'ignore').decode('ascii')
 
     saved_description = description # save the description in case it fails
 
-    WebDriverWait(driver, config['implicit_wait']).until(EC.presence_of_element_located(
-                    (By.XPATH, config['selectors']['upload']['description'])
-                ))
-
     desc = driver.find_element(By.XPATH, config['selectors']['upload']['description'])
 
-    desc.click()
-
     # desc populates with filename before clearing
     WebDriverWait(driver, config['explicit_wait']).until(lambda driver: desc.text != '')
 
-    desc.send_keys(Keys.END)
     _clear(desc)
 
-    WebDriverWait(driver, config['explicit_wait']).until(lambda driver: desc.text == '')
-    
-    desc.click()
+    try:
+        while description:
+            nearest_mention = description.find('@')
+            nearest_hash = description.find('#')
+
+            if nearest_mention == 0 or nearest_hash == 0:
+                desc.send_keys('@' if nearest_mention == 0 else '#')
+
+                name = description[1:].split(' ')[0]
+                if nearest_mention == 0: # @ case
+                    mention_xpath = config['selectors']['upload']['mention_box']
+                    condition = EC.presence_of_element_located((By.XPATH, mention_xpath))
+                    mention_box = WebDriverWait(driver, config['explicit_wait']).until(condition)
+                    mention_box.send_keys(name)
+                else:
+                    desc.send_keys(name)
+
+                time.sleep(config['implicit_wait'])
 
-    time.sleep(1)
+                if nearest_mention == 0: # @ case
+                    mention_xpath = config['selectors']['upload']['mentions'].format('@' + name)
+                    condition = EC.presence_of_element_located((By.XPATH, mention_xpath))
+                else:
+                    hashtag_xpath = config['selectors']['upload']['hashtags'].format(name)
+                    condition = EC.presence_of_element_located((By.XPATH, hashtag_xpath))
 
-    try:
-        words = description.split(" ")
-        for word in words:
-            if word[0] == "#":
-                desc.send_keys(word)
-                desc.send_keys(' ' + Keys.BACKSPACE)
-                WebDriverWait(driver, config['implicit_wait']).until(EC.presence_of_element_located(
-                    (By.XPATH, config['selectors']['upload']['mention_box'])
-                ))
-                desc.send_keys(Keys.ENTER)
-            elif word[0] == "@":
-                logger.debug(green('- Adding Mention: ' + word))
-                desc.send_keys(word)
-                desc.send_keys(' ')
-                time.sleep(1)
-                desc.send_keys(Keys.BACKSPACE)
-
-                WebDriverWait(driver, config['explicit_wait']).until(EC.presence_of_element_located(
-                    (By.XPATH, config['selectors']['upload']['mention_box_user_id'])
-                ))
-                
-                found = False
-                waiting_interval = 0.5
-                timeout = 5
-                start_time = time.time()
-                
-                while not found and (time.time() - start_time < timeout):
-                    
-                    user_id_elements = driver.find_elements(By.XPATH, config['selectors']['upload']['mention_box_user_id'])
-                    time.sleep(1)
-                    
-                    for i in range(len(user_id_elements)):
-                        user_id_element = user_id_elements[i]
-                        if user_id_element and user_id_element.is_enabled:
-                            
-                            username = user_id_element.text.split(" ")[0]
-                            if username.lower() == word[1:].lower():
-                                found = True
-                                print("Matching User found : Clicking User")
-                                for j in range(i):
-                                    desc.send_keys(Keys.DOWN)
-                                desc.send_keys(Keys.ENTER)
-                                break
-
-                        if not found:
-                            print(f"No match. Waiting for {waiting_interval} seconds...")
-                            time.sleep(waiting_interval)
+                # if the element never appears (timeout exception) remove the tag and continue
+                try:
+                    elem = WebDriverWait(driver, config['implicit_wait']).until(condition)
+                except:
+                    desc.send_keys(Keys.BACKSPACE * (len(name) + 1))
+                    description = description[len(name) + 2:]
+                    continue
+
+                ActionChains(driver).move_to_element(elem).click(elem).perform()
 
+                description = description[len(name) + 2:]
             else:
-                desc.send_keys(word + ' ')
+                min_index = _get_splice_index(nearest_mention, nearest_hash, description)
 
+                desc.send_keys(description[:min_index])
+                description = description[min_index:]
     except Exception as exception:
         print('Failed to set description: ', exception)
         _clear(desc)
-        desc.send_keys(saved_description)
+        desc.send_keys(saved_description) # if fail, use saved description
+
 
 def _clear(element) -> None:
     """
     Clears the text of the element (an issue with the TikTok website when automating)
 
     Parameters
     ----------
     element
         The text box to clear
     """
     element.send_keys(2 * len(element.text) * Keys.BACKSPACE)
 
+
 def _set_video(driver, path: str = '', num_retries: int = 3, **kwargs) -> None:
     """
     Sets the video to upload
 
     Parameters
     ----------
     driver : selenium.webdriver
@@ -367,80 +315,45 @@
     num_retries : number of retries (can occasionally fail)
     """
     # uploads the element
     logger.debug(green('Uploading video file'))
 
     for _ in range(num_retries):
         try:
-            _change_to_upload_iframe(driver)
-            # Wait For Input File
-            driverWait = WebDriverWait(driver, config['explicit_wait'])
-            upload_boxWait = EC.presence_of_element_located(
-                (By.XPATH, config['selectors']['upload']['upload_video'])
-                )
-            driverWait.until(upload_boxWait)
             upload_box = driver.find_element(
                 By.XPATH, config['selectors']['upload']['upload_video']
             )
             upload_box.send_keys(path)
-            
+            # waits for the upload progress bar to disappear
+            upload_progress = EC.presence_of_element_located(
+                (By.XPATH, config['selectors']['upload']['upload_in_progress'])
+                )
+
+            WebDriverWait(driver, config['explicit_wait']).until(upload_progress)
+            WebDriverWait(driver, config['explicit_wait']).until_not(upload_progress)
+
+            # waits for the video to upload
+            upload_confirmation = EC.presence_of_element_located(
+                (By.XPATH, config['selectors']['upload']['upload_confirmation'])
+                )
+
+            # An exception throw here means the video failed to upload an a retry is needed
+            WebDriverWait(driver, config['explicit_wait']).until(upload_confirmation)
+
             # wait until a non-draggable image is found
             process_confirmation = EC.presence_of_element_located(
                 (By.XPATH, config['selectors']['upload']['process_confirmation'])
                 )
             WebDriverWait(driver, config['explicit_wait']).until(process_confirmation)
             return
-        except TimeoutException as exception:
-            print("TimeoutException occurred:\n", exception)
         except Exception as exception:
             print(exception)
-            raise FailedToUpload(exception)
-
 
-def _remove_cookies_window(driver) -> None:
-    """
-    Removes the cookies window if it is open
+    raise FailedToUpload()
 
-    Parameters
-    ----------
-    driver : selenium.webdriver
-    """
-
-    logger.debug(green(f'Removing cookies window'))
-    cookies_banner = WebDriverWait(driver, config['implicit_wait']).until(
-        EC.presence_of_element_located((By.TAG_NAME, config['selectors']['upload']['cookies_banner']['banner'])))
-    
-    item = WebDriverWait(driver, config['implicit_wait']).until(
-        EC.visibility_of(cookies_banner.shadow_root.find_element(By.CSS_SELECTOR, config['selectors']['upload']['cookies_banner']['button'])))
-
-    # Wait that the Decline all button is clickable
-    decline_button = WebDriverWait(driver, config['implicit_wait']).until(
-        EC.element_to_be_clickable(item.find_elements(By.TAG_NAME, 'button')[0]))
-
-    decline_button.click()
-
-def _remove_split_window(driver) -> None:
-    """
-    Remove the split window if it is open
-
-    Parameters
-    ----------
-    driver : selenium.webdriver
-    """
-    logger.debug(green(f'Removing split window'))
-    window_xpath = config['selectors']['upload']['split_window']
-    
-    try:
-        condition = EC.presence_of_element_located((By.XPATH, window_xpath))
-        window = WebDriverWait(driver, config['implicit_wait']).until(condition)
-        window.click()
-            
-    except TimeoutException:
-        logger.debug(red(f"Split window not found or operation timed out"))
-        
 
 def _set_interactivity(driver, comment=True, stitch=True, duet=True, *args, **kwargs) -> None:
     """
     Sets the interactivity settings of the video
 
     Parameters
     ----------
@@ -497,15 +410,16 @@
     try:
         switch = driver.find_element(By.XPATH, config['selectors']['schedule']['switch'])
         switch.click()
         __date_picker(driver, month, day)
         __time_picker(driver, hour, minute)
     except Exception as e:
         msg = f'Failed to set schedule: {e}'
-        logger.error(red(msg))
+        print(msg)
+        logger.error(msg)
         raise FailedToUpload()
 
 
 
 def __date_picker(driver, month: int, day: int) -> None:
     logger.debug(green('Picking date'))
 
@@ -576,21 +490,17 @@
     # 00 == 0, 05 == 1, 10 == 2, 15 == 3, 20 == 4, 25 == 5, 30 == 6, 35 == 7, 40 == 8, 45 == 9, 50 == 10, 55 == 11
     minute_options = driver.find_elements(By.XPATH, config['selectors']['schedule']['timepicker_minutes'])
 
     hour_to_click = hour_options[hour]
     minute_option_correct_index = int(minute / 5)
     minute_to_click = minute_options[minute_option_correct_index]
 
-    time.sleep(1) # temporay fix => might be better to use an explicit wait
     driver.execute_script("arguments[0].scrollIntoView({block: 'center', inline: 'nearest'});", hour_to_click)
-    time.sleep(1) # temporay fix => might be better to use an explicit wait
     hour_to_click.click()
-
     driver.execute_script("arguments[0].scrollIntoView({block: 'center', inline: 'nearest'});", minute_to_click)
-    time.sleep(2) # temporary fixed => Might be better to use an explicit wait
     minute_to_click.click()
 
     # click somewhere else to close the time picker
     time_picker.click()
 
     time.sleep(.5)  # wait for the DOM change
     __verify_time_picked_is_correct(driver, hour, minute)
@@ -603,14 +513,15 @@
 
     if time_selected_hour == hour and time_selected_minute == minute:
         logger.debug(green('Time picked correctly'))
     else:
         msg = f'Something went wrong with the time picker, ' \
               f'expected {hour:02d}:{minute:02d} ' \
               f'but got {time_selected_hour:02d}:{time_selected_minute:02d}'
+        logger.error(msg)
         raise Exception(msg)
 
 
 def _post_video(driver) -> None:
     """
     Posts the video by clicking the post button
 
@@ -618,15 +529,14 @@
     ----------
     driver : selenium.webdriver
     """
     logger.debug(green('Clicking the post button'))
 
     try:
         post = WebDriverWait(driver, config['implicit_wait']).until(EC.element_to_be_clickable((By.XPATH, config['selectors']['upload']['post'])))
-        driver.execute_script("arguments[0].scrollIntoView({block: 'center', inline: 'nearest'});", post)
         post.click()
     except ElementClickInterceptedException:
         logger.debug(green("Trying to click on the button again"))
         driver.execute_script('document.querySelector(".btn-post > button").click()')
 
     # waits for the video to upload
     post_confirmation = EC.presence_of_element_located(
```

### Comparing `tiktok_uploader-1.0.16/src/tiktok_uploader/proxy_auth_extension/background.js` & `tiktok_uploader-1.0.2/src/tiktok_uploader/proxy_auth_extension/background.js`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.16/src/tiktok_uploader/proxy_auth_extension/proxy_auth_extension.py` & `tiktok_uploader-1.0.2/src/tiktok_uploader/proxy_auth_extension/proxy_auth_extension.py`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.16/tests/test_browsers.py` & `tiktok_uploader-1.0.2/tests/test_browsers.py`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.16/tests/test_upload.py` & `tiktok_uploader-1.0.2/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.16/.gitignore` & `tiktok_uploader-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-1.0.16/README.md` & `tiktok_uploader-1.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,678 +1,656 @@
-00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-00000010: 223e 0a3c 696d 6720 7372 633d 2268 7474  ">.<img src="htt
-00000020: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000030: 776b 6169 7365 7274 6578 6173 2f74 696b  wkaisertexas/tik
-00000040: 746f 6b2d 7570 6c6f 6164 6572 2f61 7373  tok-uploader/ass
-00000050: 6574 732f 3237 3739 3530 3134 2f66 3939  ets/27795014/f99
-00000060: 3166 6463 372d 3238 3761 2d34 6333 622d  1fdc7-287a-4c3b-
-00000070: 3961 3834 2d32 3263 3761 6438 6135 3762  9a84-22c7ad8a57b
-00000080: 6622 2061 6c74 3d22 7669 6465 6f20 776f  f" alt="video wo
-00000090: 726b 696e 6722 202f 3e0a 3c2f 703e 0a0a  rking" />.</p>..
-000000a0: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
-000000b0: 7222 3e20 e2ac 86ef b88f 2054 696b 546f  r"> ...... TikTo
-000000c0: 6b20 5570 6c6f 6164 6572 203c 2f68 313e  k Uploader </h1>
-000000d0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
-000000e0: 7222 3e41 203c 7374 726f 6e67 3e53 656c  r">A <strong>Sel
-000000f0: 656e 6975 6d3c 2f73 7472 6f6e 673e 2d62  enium</strong>-b
-00000100: 6173 6564 2061 7574 6f6d 6174 6564 203c  ased automated <
-00000110: 7374 726f 6e67 3e54 696b 546f 6b3c 2f73  strong>TikTok</s
-00000120: 7472 6f6e 673e 2076 6964 656f 2075 706c  trong> video upl
-00000130: 6f61 6465 723c 2f70 3e0a 0a3c 7020 616c  oader</p>..<p al
-00000140: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
-00000150: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000160: 2f67 6974 6875 622e 636f 6d2f 776b 6169  /github.com/wkai
-00000170: 7365 7274 6578 6173 2f74 696b 746f 6b2d  sertexas/tiktok-
-00000180: 7570 6c6f 6164 6572 223e 3c73 7472 6f6e  uploader"><stron
-00000190: 673e 456e 676c 6973 683c 2f73 7472 6f6e  g>English</stron
-000001a0: 673e 3c2f 613e 20c2 b70a 2020 3c61 2068  g></a> ...  <a h
-000001b0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-000001c0: 6875 622e 636f 6d2f 776b 6169 7365 7274  hub.com/wkaisert
-000001d0: 6578 6173 2f74 696b 746f 6b2d 7570 6c6f  exas/tiktok-uplo
-000001e0: 6164 6572 2f62 6c6f 622f 6d61 696e 2f52  ader/blob/main/R
-000001f0: 4541 444d 452e 7a68 2d48 616e 732e 6d64  EADME.zh-Hans.md
-00000200: 223e 3c73 7472 6f6e 673e 4368 696e 6573  "><strong>Chines
-00000210: 6520 2853 696d 706c 6966 6965 6429 3c2f  e (Simplified)</
-00000220: 7374 726f 6e67 3e3c 2f61 3e20 c2b7 0a20  strong></a> ... 
-00000230: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00000240: 2f2f 6769 7468 7562 2e63 6f6d 2f77 6b61  //github.com/wka
-00000250: 6973 6572 7465 7861 732f 7469 6b74 6f6b  isertexas/tiktok
-00000260: 2d75 706c 6f61 6465 722f 626c 6f62 2f6d  -uploader/blob/m
-00000270: 6169 6e2f 5245 4144 4d45 2e66 722e 6d64  ain/README.fr.md
-00000280: 223e 3c73 7472 6f6e 673e 4672 656e 6368  "><strong>French
-00000290: 3c2f 7374 726f 6e67 3e3c 2f61 3e20 c2b7  </strong></a> ..
-000002a0: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
-000002b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f77  s://github.com/w
-000002c0: 6b61 6973 6572 7465 7861 732f 7469 6b74  kaisertexas/tikt
-000002d0: 6f6b 2d75 706c 6f61 6465 722f 626c 6f62  ok-uploader/blob
-000002e0: 2f6d 6169 6e2f 5245 4144 4d45 2e65 732e  /main/README.es.
-000002f0: 6d64 223e 3c73 7472 6f6e 673e 5370 616e  md"><strong>Span
-00000300: 6973 683c 2f73 7472 696e 673e 3c2f 613e  ish</string></a>
-00000310: 20c2 b70a 2020 3c61 2068 7265 663d 2268   ...  <a href="h
-00000320: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000330: 6d2f 776b 6169 7365 7274 6578 6173 2f74  m/wkaisertexas/t
-00000340: 696b 746f 6b2d 7570 6c6f 6164 6572 2f62  iktok-uploader/b
-00000350: 6c6f 622f 6d61 696e 2f52 4541 444d 452e  lob/main/README.
-00000360: 6465 2e6d 6422 3e3c 7374 726f 6e67 3e47  de.md"><strong>G
-00000370: 6572 6d61 6e3c 2f73 7472 6f6e 673e 3c2f  erman</strong></
-00000380: 613e 0a3c 2f70 3e0a 0a3c 7020 616c 6967  a>.</p>..<p alig
-00000390: 6e3d 2263 656e 7465 7222 3e0a 2020 3c69  n="center">.  <i
-000003a0: 6d67 2061 6c74 3d22 466f 726b 7322 2073  mg alt="Forks" s
-000003b0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-000003c0: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-000003d0: 622f 666f 726b 732f 776b 6169 7365 7274  b/forks/wkaisert
-000003e0: 6578 6173 2f74 696b 746f 6b2d 7570 6c6f  exas/tiktok-uplo
-000003f0: 6164 6572 2220 2f3e 0a20 203c 696d 6720  ader" />.  <img 
-00000400: 616c 743d 2253 7461 7273 2220 7372 633d  alt="Stars" src=
-00000410: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-00000420: 656c 6473 2e69 6f2f 6769 7468 7562 2f73  elds.io/github/s
-00000430: 7461 7273 2f77 6b61 6973 6572 7465 7861  tars/wkaisertexa
-00000440: 732f 7469 6b74 6f6b 2d75 706c 6f61 6465  s/tiktok-uploade
-00000450: 7222 202f 3e0a 2020 3c69 6d67 2061 6c74  r" />.  <img alt
-00000460: 3d22 5761 7463 6865 7273 2220 7372 633d  ="Watchers" src=
-00000470: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-00000480: 656c 6473 2e69 6f2f 6769 7468 7562 2f77  elds.io/github/w
-00000490: 6174 6368 6572 732f 776b 6169 7365 7274  atchers/wkaisert
-000004a0: 6578 6173 2f74 696b 746f 6b2d 7570 6c6f  exas/tiktok-uplo
-000004b0: 6164 6572 2220 2f3e 0a3c 2f70 3e0a 0a3c  ader" />.</p>..<
-000004c0: 6831 3e54 6162 6c65 206f 6620 436f 6e74  h1>Table of Cont
-000004d0: 656e 7473 3c2f 6831 3e0a 0a2d 205b 496e  ents</h1>..- [In
-000004e0: 7374 616c 6c61 7469 6f6e 5d28 2369 6e73  stallation](#ins
-000004f0: 7461 6c6c 6174 696f 6e29 0a20 202d 205b  tallation).  - [
-00000500: 4d61 634f 532c 2057 696e 646f 7773 2061  MacOS, Windows a
-00000510: 6e64 204c 696e 7578 5d28 236d 6163 6f73  nd Linux](#macos
-00000520: 2d77 696e 646f 7773 2d61 6e64 2d6c 696e  -windows-and-lin
-00000530: 7578 290a 2020 2020 2d20 5b44 6f77 6e6c  ux).    - [Downl
-00000540: 6f61 6469 6e67 2066 726f 6d20 5079 5049  oading from PyPI
-00000550: 2028 5265 636f 6d6d 656e 6465 6429 5d28   (Recommended)](
-00000560: 2370 7970 6929 0a20 2020 202d 205b 4275  #pypi).    - [Bu
-00000570: 696c 6469 6e67 2066 726f 6d20 736f 7572  ilding from sour
-00000580: 6365 5d28 2362 7569 6c64 696e 672d 6672  ce](#building-fr
-00000590: 6f6d 2d73 6f75 7263 6529 0a2d 205b 5573  om-source).- [Us
-000005a0: 6167 655d 2823 7573 6167 6529 0a20 202d  age](#usage).  -
-000005b0: 205b f09f 92bb 2043 6f6d 6d61 6e64 204c   [.... Command L
-000005c0: 696e 6520 496e 7465 7266 6163 6520 2843  ine Interface (C
-000005d0: 4c49 295d 2823 636c 6929 0a20 202d 205b  LI)](#cli).  - [
-000005e0: e2ac 8620 5570 6c6f 6164 696e 6720 5669  ... Uploading Vi
-000005f0: 6465 6f73 5d28 2375 706c 6f61 6469 6e67  deos](#uploading
-00000600: 2d76 6964 656f 7329 0a20 202d 205b f09f  -videos).  - [..
-00000610: abb5 204d 656e 7469 6f6e 7320 616e 6420  .. Mentions and 
-00000620: 4861 7368 7461 6773 5d28 236d 656e 7469  Hashtags](#menti
-00000630: 6f6e 732d 616e 642d 6861 7368 7461 6773  ons-and-hashtags
-00000640: 290a 2020 2d20 5bf0 9faa a120 5374 6974  ).  - [.... Stit
-00000650: 6368 6573 2c20 4475 6574 7320 616e 6420  ches, Duets and 
-00000660: 436f 6d6d 656e 7473 5d28 2373 7469 7463  Comments](#stitc
-00000670: 6865 732d 6475 6574 732d 616e 642d 636f  hes-duets-and-co
-00000680: 6d6d 656e 7473 290a 2020 2d20 5bf0 9f94  mments).  - [...
-00000690: 9020 4175 7468 656e 7469 6361 7469 6f6e  . Authentication
-000006a0: 5d28 2361 7574 6865 6e74 6963 6174 696f  ](#authenticatio
-000006b0: 6e29 0a20 202d 205b f09f 9180 2042 726f  n).  - [.... Bro
-000006c0: 7773 6572 2053 656c 6563 7469 6f6e 5d28  wser Selection](
-000006d0: 2362 726f 7773 6572 2d73 656c 6563 7469  #browser-selecti
-000006e0: 6f6e 290a 2020 2d20 5bf0 9f9a b220 4375  on).  - [.... Cu
-000006f0: 7374 6f6d 2057 6562 4472 6976 6572 204f  stom WebDriver O
-00000700: 7074 696f 6e73 5d28 2363 7573 746f 6d2d  ptions](#custom-
-00000710: 7765 6264 7269 7665 7229 0a20 202d 205b  webdriver).  - [
-00000720: f09f a4af 2048 6561 646c 6573 7320 4272  .... Headless Br
-00000730: 6f77 7365 7273 5d28 2368 6561 646c 6573  owsers](#headles
-00000740: 7329 0a20 202d 205b f09f 94a8 2049 6e69  s).  - [.... Ini
-00000750: 7469 616c 2053 6574 7570 5d28 2369 6e69  tial Setup](#ini
-00000760: 7469 616c 2d73 6574 7570 290a 2d20 5be2  tial-setup).- [.
-00000770: 99bb efb8 8f20 4578 616d 706c 6573 5d28  ..... Examples](
-00000780: 2365 7861 6d70 6c65 7329 0a2d 205b f09f  #examples).- [..
-00000790: 939d 204e 6f74 6573 5d28 236e 6f74 6573  .. Notes](#notes
-000007a0: 290a 2d20 5b41 6363 6f75 6e74 7320 6d61  ).- [Accounts ma
-000007b0: 6465 2077 6974 685d 2823 6d61 6465 2d77  de with](#made-w
-000007c0: 6974 6829 0a0a 2320 496e 7374 616c 6c61  ith)..# Installa
-000007d0: 7469 6f6e 0a0a 4120 7065 7271 7569 7369  tion..A perquisi
-000007e0: 7465 2074 6f20 7573 696e 6720 7468 6973  te to using this
-000007f0: 2070 726f 6772 616d 2069 7320 7468 6520   program is the 
-00000800: 696e 7374 616c 6c61 7469 6f6e 206f 6620  installation of 
-00000810: 6120 5b53 656c 656e 6975 6d2d 636f 6d70  a [Selenium-comp
-00000820: 6174 6962 6c65 5d28 6874 7470 733a 2f2f  atible](https://
-00000830: 7777 772e 7365 6c65 6e69 756d 2e64 6576  www.selenium.dev
-00000840: 2f64 6f63 756d 656e 7461 7469 6f6e 2f77  /documentation/w
-00000850: 6562 6472 6976 6572 2f67 6574 7469 6e67  ebdriver/getting
-00000860: 5f73 7461 7274 6564 2f69 6e73 7461 6c6c  _started/install
-00000870: 5f64 7269 7665 7273 2f29 2077 6562 2062  _drivers/) web b
-00000880: 726f 7773 6572 2e20 5b47 6f6f 676c 6520  rowser. [Google 
-00000890: 4368 726f 6d65 5d28 6874 7470 733a 2f2f  Chrome](https://
-000008a0: 7777 772e 676f 6f67 6c65 2e63 6f6d 2f63  www.google.com/c
-000008b0: 6872 6f6d 652f 2920 6973 2072 6563 6f6d  hrome/) is recom
-000008c0: 6d65 6e64 6564 2e0a 0a3c 6832 2069 643d  mended...<h2 id=
-000008d0: 226d 6163 6f73 2d77 696e 646f 7773 2d61  "macos-windows-a
-000008e0: 6e64 2d6c 696e 7578 223e 4d61 634f 532c  nd-linux">MacOS,
-000008f0: 2057 696e 646f 7773 2061 6e64 204c 696e   Windows and Lin
-00000900: 7578 3c2f 6832 3e0a 0a49 6e73 7461 6c6c  ux</h2>..Install
-00000910: 2050 7974 686f 6e20 3320 6f72 2067 7265   Python 3 or gre
-00000920: 6174 6572 2066 726f 6d20 5b70 7974 686f  ater from [pytho
-00000930: 6e2e 6f72 675d 2868 7474 7073 3a2f 2f77  n.org](https://w
-00000940: 7777 2e70 7974 686f 6e2e 6f72 672f 646f  ww.python.org/do
-00000950: 776e 6c6f 6164 732f 290a 0a3c 6833 2069  wnloads/)..<h3 i
-00000960: 643d 2270 7970 6922 3e44 6f77 6e6c 6f61  d="pypi">Downloa
-00000970: 6469 6e67 2066 726f 6d20 5079 5049 2028  ding from PyPI (
-00000980: 5265 636f 6d6d 656e 6465 6429 3c2f 6833  Recommended)</h3
-00000990: 3e0a 0a49 6e73 7461 6c6c 2060 7469 6b74  >..Install `tikt
-000009a0: 6f6b 2d75 706c 6f61 6465 7260 2075 7369  ok-uploader` usi
-000009b0: 6e67 2060 7069 7060 0a0a 6060 6062 6173  ng `pip`..```bas
-000009c0: 680a 7069 7020 696e 7374 616c 6c20 7469  h.pip install ti
-000009d0: 6b74 6f6b 2d75 706c 6f61 6465 720a 6060  ktok-uploader.``
-000009e0: 600a 0a3c 6833 2069 643d 2262 7569 6c64  `..<h3 id="build
-000009f0: 696e 672d 6672 6f6d 2d73 6f75 7263 6522  ing-from-source"
-00000a00: 3e42 7569 6c64 696e 6720 6672 6f6d 2073  >Building from s
-00000a10: 6f75 7263 653c 2f68 333e 0a0a 496e 7374  ource</h3>..Inst
-00000a20: 616c 6c69 6e67 2066 726f 6d20 736f 7572  alling from sour
-00000a30: 6365 2061 6c6c 6f77 7320 6772 6561 7465  ce allows greate
-00000a40: 7220 666c 6578 6962 696c 6974 7920 746f  r flexibility to
-00000a50: 206d 6f64 6966 7920 7468 6520 6d6f 6475   modify the modu
-00000a60: 6c65 2773 2063 6f64 6520 746f 2065 7874  le's code to ext
-00000a70: 656e 6420 6465 6661 756c 7420 6265 6861  end default beha
-00000a80: 7669 6f72 2e0a 0a46 6972 7374 2c20 6063  vior...First, `c
-00000a90: 6c6f 6e65 6020 616e 6420 6d6f 7665 2069  lone` and move i
-00000aa0: 6e74 6f20 7468 6520 7265 706f 7369 746f  nto the reposito
-00000ab0: 7279 2e20 4e65 7874 2c20 696e 7374 616c  ry. Next, instal
-00000ac0: 6c20 6068 6174 6368 602c 2074 6865 2062  l `hatch`, the b
-00000ad0: 7569 6c64 2074 6f6f 6c20 7573 6564 2066  uild tool used f
-00000ae0: 6f72 2074 6869 7320 7072 6f6a 6563 7420  or this project 
-00000af0: 5b5e 315d 2e20 5468 656e 2c20 6062 7569  [^1]. Then, `bui
-00000b00: 6c64 6020 7468 6520 7072 6f6a 6563 742e  ld` the project.
-00000b10: 2046 696e 616c 6c79 2c20 6069 6e73 7461   Finally, `insta
-00000b20: 6c6c 6020 7468 6520 7072 6f6a 6563 7420  ll` the project 
-00000b30: 7769 7468 2074 6865 2060 2d65 6020 6f72  with the `-e` or
-00000b40: 2065 6469 7461 626c 6520 666c 6167 2e0a   editable flag..
-00000b50: 0a60 6060 636f 6e73 6f6c 650a 6769 7420  .```console.git 
-00000b60: 636c 6f6e 6520 6874 7470 733a 2f2f 6769  clone https://gi
-00000b70: 7468 7562 2e63 6f6d 2f77 6b61 6973 6572  thub.com/wkaiser
-00000b80: 7465 7861 732f 7469 6b74 6f6b 2d75 706c  texas/tiktok-upl
-00000b90: 6f61 6465 722e 6769 740a 6364 2074 696b  oader.git.cd tik
-00000ba0: 746f 6b2d 7570 6c6f 6164 6572 0a70 6970  tok-uploader.pip
-00000bb0: 2069 6e73 7461 6c6c 2068 6174 6368 0a68   install hatch.h
-00000bc0: 6174 6368 2062 7569 6c64 0a70 6970 2069  atch build.pip i
-00000bd0: 6e73 7461 6c6c 202d 6520 2e0a 6060 600a  nstall -e ..```.
-00000be0: 0a3c 6831 2069 643d 2275 7361 6765 223e  .<h1 id="usage">
-00000bf0: 5573 6167 653c 2f68 313e 0a0a 6074 696b  Usage</h1>..`tik
-00000c00: 746f 6b2d 7570 6c6f 6164 6572 6020 776f  tok-uploader` wo
-00000c10: 726b 7320 6279 2064 7570 6c69 6361 7469  rks by duplicati
-00000c20: 6e67 2079 6f75 7220 6272 6f77 7365 7227  ng your browser'
-00000c30: 7320 2a2a 636f 6f6b 6965 732a 2a20 7768  s **cookies** wh
-00000c40: 6963 6820 7472 6963 6b73 202a 2a54 696b  ich tricks **Tik
-00000c50: 546f 6b2a 2a20 696e 746f 2062 656c 6965  Tok** into belie
-00000c60: 7669 6e67 2079 6f75 2061 7265 206c 6f67  ving you are log
-00000c70: 6765 6420 696e 206f 6e20 6120 7265 6d6f  ged in on a remo
-00000c80: 7465 2d63 6f6e 7472 6f6c 6c65 6420 6272  te-controlled br
-00000c90: 6f77 7365 722e 0a0a 3c68 3220 6964 3d22  owser...<h2 id="
-00000ca0: 636c 6922 3e20 f09f 92bb 2043 6f6d 6d61  cli"> .... Comma
-00000cb0: 6e64 204c 696e 6520 496e 7465 7266 6163  nd Line Interfac
-00000cc0: 6520 2843 4c49 293c 2f68 323e 0a0a 5573  e (CLI)</h2>..Us
-00000cd0: 696e 6720 7468 6520 434c 4920 6973 2061  ing the CLI is a
-00000ce0: 7320 7369 6d70 6c65 2061 7320 6361 6c6c  s simple as call
-00000cf0: 696e 6720 6074 696b 746f 6b2d 7570 6c6f  ing `tiktok-uplo
-00000d00: 6164 6572 6020 7769 7468 2079 6f75 7220  ader` with your 
-00000d10: 7669 6465 6f73 3a20 6070 6174 6860 2028  videos: `path` (
-00000d20: 2d76 292c 2060 6465 7363 7269 7074 696f  -v), `descriptio
-00000d30: 6e60 282d 6429 2061 6e64 2060 636f 6f6b  n`(-d) and `cook
-00000d40: 6965 7360 2028 2d63 290a 0a60 6060 6261  ies` (-c)..```ba
-00000d50: 7368 0a74 696b 746f 6b2d 7570 6c6f 6164  sh.tiktok-upload
-00000d60: 6572 202d 7620 7669 6465 6f2e 6d70 3420  er -v video.mp4 
-00000d70: 2d64 2022 7468 6973 2069 7320 6d79 2065  -d "this is my e
-00000d80: 7363 6170 6564 205c 2264 6573 6372 6970  scaped \"descrip
-00000d90: 7469 6f6e 5c22 2220 2d63 2063 6f6f 6b69  tion\"" -c cooki
-00000da0: 6573 2e74 7874 0a60 6060 0a0a 6060 6070  es.txt.```..```p
-00000db0: 7974 686f 6e0a 6672 6f6d 2074 696b 746f  ython.from tikto
-00000dc0: 6b5f 7570 6c6f 6164 6572 2e75 706c 6f61  k_uploader.uploa
-00000dd0: 6420 696d 706f 7274 2075 706c 6f61 645f  d import upload_
-00000de0: 7669 6465 6f2c 2075 706c 6f61 645f 7669  video, upload_vi
-00000df0: 6465 6f73 0a66 726f 6d20 7469 6b74 6f6b  deos.from tiktok
-00000e00: 5f75 706c 6f61 6465 722e 6175 7468 2069  _uploader.auth i
-00000e10: 6d70 6f72 7420 4175 7468 4261 636b 656e  mport AuthBacken
-00000e20: 640a 0a23 2073 696e 676c 6520 7669 6465  d..# single vide
-00000e30: 6f0a 7570 6c6f 6164 5f76 6964 656f 2827  o.upload_video('
-00000e40: 7669 6465 6f2e 6d70 3427 2c0a 2020 2020  video.mp4',.    
-00000e50: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-00000e60: 696f 6e3d 2774 6869 7320 6973 206d 7920  ion='this is my 
-00000e70: 6465 7363 7269 7074 696f 6e27 2c0a 2020  description',.  
-00000e80: 2020 2020 2020 2020 2020 636f 6f6b 6965            cookie
-00000e90: 733d 2763 6f6f 6b69 6573 2e74 7874 2729  s='cookies.txt')
-00000ea0: 0a0a 2320 4d75 6c74 6970 6c65 2056 6964  ..# Multiple Vid
-00000eb0: 656f 730a 7669 6465 6f73 203d 205b 0a20  eos.videos = [. 
-00000ec0: 2020 207b 0a20 2020 2020 2020 2027 7061     {.        'pa
-00000ed0: 7468 273a 2027 7669 6465 6f2e 6d70 3427  th': 'video.mp4'
-00000ee0: 2c0a 2020 2020 2020 2020 2764 6573 6372  ,.        'descr
-00000ef0: 6970 7469 6f6e 273a 2027 7468 6973 2069  iption': 'this i
-00000f00: 7320 6d79 2064 6573 6372 6970 7469 6f6e  s my description
-00000f10: 270a 2020 2020 7d2c 0a20 2020 207b 0a20  '.    },.    {. 
-00000f20: 2020 2020 2020 2027 7061 7468 273a 2027         'path': '
-00000f30: 7669 6465 6f32 2e6d 7034 272c 0a20 2020  video2.mp4',.   
-00000f40: 2020 2020 2027 6465 7363 7269 7074 696f       'descriptio
-00000f50: 6e27 3a20 2774 6869 7320 6973 2061 6c73  n': 'this is als
-00000f60: 6f20 6d79 2064 6573 6372 6970 7469 6f6e  o my description
-00000f70: 270a 2020 2020 7d0a 5d0a 0a61 7574 6820  '.    }.]..auth 
-00000f80: 3d20 4175 7468 4261 636b 656e 6428 636f  = AuthBackend(co
-00000f90: 6f6b 6965 733d 2763 6f6f 6b69 6573 2e74  okies='cookies.t
-00000fa0: 7874 2729 0a75 706c 6f61 645f 7669 6465  xt').upload_vide
-00000fb0: 6f73 2876 6964 656f 733d 7669 6465 6f73  os(videos=videos
-00000fc0: 2c20 6175 7468 3d61 7574 6829 0a60 6060  , auth=auth).```
-00000fd0: 0a0a 3c68 3220 6964 3d22 7570 6c6f 6164  ..<h2 id="upload
-00000fe0: 696e 672d 7669 6465 6f73 223e 20e2 ac86  ing-videos"> ...
-00000ff0: 2055 706c 6f61 6469 6e67 2056 6964 656f   Uploading Video
-00001000: 733c 2f68 323e 0a0a 5468 6973 206c 6962  s</h2>..This lib
-00001010: 7261 7279 2072 6576 6f6c 7665 7320 6172  rary revolves ar
-00001020: 6f75 6e64 2074 6865 2060 7570 6c6f 6164  ound the `upload
-00001030: 5f76 6964 656f 7360 2066 756e 6374 696f  _videos` functio
-00001040: 6e20 7768 6963 6820 7461 6b65 7320 696e  n which takes in
-00001050: 2061 206c 6973 7420 6f66 2076 6964 656f   a list of video
-00001060: 7320 7768 6963 6820 6861 7665 202a 2a66  s which have **f
-00001070: 696c 656e 616d 6573 2a2a 2061 6e64 202a  ilenames** and *
-00001080: 2a64 6573 6372 6970 7469 6f6e 732a 2a20  *descriptions** 
-00001090: 616e 6420 6172 6520 7061 7373 6564 2061  and are passed a
-000010a0: 7320 666f 6c6c 6f77 733a 0a0a 6060 6070  s follows:..```p
-000010b0: 7974 686f 6e0a 6672 6f6d 2074 696b 746f  ython.from tikto
-000010c0: 6b5f 7570 6c6f 6164 6572 2e75 706c 6f61  k_uploader.uploa
-000010d0: 6420 696d 706f 7274 2075 706c 6f61 645f  d import upload_
-000010e0: 7669 6465 6f73 0a66 726f 6d20 7469 6b74  videos.from tikt
-000010f0: 6f6b 5f75 706c 6f61 6465 722e 6175 7468  ok_uploader.auth
-00001100: 2069 6d70 6f72 7420 4175 7468 4261 636b   import AuthBack
-00001110: 656e 640a 0a76 6964 656f 7320 3d20 5b0a  end..videos = [.
-00001120: 2020 2020 7b0a 2020 2020 2020 2020 2776      {.        'v
-00001130: 6964 656f 273a 2027 7669 6465 6f30 2e6d  ideo': 'video0.m
-00001140: 7034 272c 0a20 2020 2020 2020 2027 6465  p4',.        'de
-00001150: 7363 7269 7074 696f 6e27 3a20 2756 6964  scription': 'Vid
-00001160: 656f 2031 2069 7320 6162 6f75 7420 2e2e  eo 1 is about ..
-00001170: 2e27 0a20 2020 207d 2c0a 2020 2020 7b0a  .'.    },.    {.
-00001180: 2020 2020 2020 2020 2776 6964 656f 273a          'video':
-00001190: 2027 7669 6465 6f31 2e6d 7034 272c 0a20   'video1.mp4',. 
-000011a0: 2020 2020 2020 2027 6465 7363 7269 7074         'descript
-000011b0: 696f 6e27 3a20 2756 6964 656f 2032 2069  ion': 'Video 2 i
-000011c0: 7320 6162 6f75 7420 2e2e 2e27 0a20 2020  s about ...'.   
-000011d0: 207d 0a5d 0a0a 6175 7468 203d 2041 7574   }.]..auth = Aut
-000011e0: 6842 6163 6b65 6e64 2863 6f6f 6b69 6573  hBackend(cookies
-000011f0: 3d27 636f 6f6b 6965 732e 7478 7427 290a  ='cookies.txt').
-00001200: 6661 696c 6564 5f76 6964 656f 7320 3d20  failed_videos = 
-00001210: 7570 6c6f 6164 5f76 6964 656f 7328 7669  upload_videos(vi
-00001220: 6465 6f73 3d76 6964 656f 732c 2061 7574  deos=videos, aut
-00001230: 683d 6175 7468 290a 0a66 6f72 2076 6964  h=auth)..for vid
-00001240: 656f 2069 6e20 6661 696c 6564 5f76 6964  eo in failed_vid
-00001250: 656f 733a 2023 2065 6163 6820 696e 7075  eos: # each inpu
-00001260: 7420 7669 6465 6f20 6f62 6a65 6374 2077  t video object w
-00001270: 6869 6368 2066 6169 6c65 640a 2020 2020  hich failed.    
-00001280: 7072 696e 7428 6627 7b76 6964 656f 5b27  print(f'{video['
-00001290: 7669 6465 6f27 5d7d 2077 6974 6820 6465  video']} with de
-000012a0: 7363 7269 7074 696f 6e20 227b 7669 6465  scription "{vide
-000012b0: 6f5b 2764 6573 6372 6970 7469 6f6e 275d  o['description']
-000012c0: 7d22 2066 6169 6c65 6427 290a 6060 600a  }" failed').```.
-000012d0: 0a3c 6832 2069 643d 226d 656e 7469 6f6e  .<h2 id="mention
-000012e0: 732d 616e 642d 6861 7368 7461 6773 223e  s-and-hashtags">
-000012f0: 20f0 9fab b520 4d65 6e74 696f 6e73 2061   .... Mentions a
-00001300: 6e64 2048 6173 6874 6167 733c 2f68 323e  nd Hashtags</h2>
-00001310: 0a0a 4d65 6e74 696f 6e73 2061 6e64 2048  ..Mentions and H
-00001320: 6173 6874 6167 7320 6e6f 7720 776f 726b  ashtags now work
-00001330: 2073 6f20 6c6f 6e67 2061 7320 7468 6579   so long as they
-00001340: 2061 7265 2066 6f6c 6c6f 7765 6420 6279   are followed by
-00001350: 2061 2073 7061 6365 2e20 486f 7765 7665   a space. Howeve
-00001360: 722c 2079 6f75 2061 7320 7468 6520 7573  r, you as the us
-00001370: 6572 2061 7265 2072 6573 706f 6e73 6962  er are responsib
-00001380: 6c65 2066 6f72 2076 6572 6966 7969 6e67  le for verifying
-00001390: 2061 206d 656e 7469 6f6e 206f 7220 6861   a mention or ha
-000013a0: 7368 7461 6720 6578 6973 7473 2062 6566  shtag exists bef
-000013b0: 6f72 6520 706f 7374 696e 670a 0a2a 2a45  ore posting..**E
-000013c0: 7861 6d70 6c65 3a2a 2a0a 0a60 6060 7079  xample:**..```py
-000013d0: 7468 6f6e 0a66 726f 6d20 7469 6b74 6f6b  thon.from tiktok
-000013e0: 5f75 706c 6f61 6465 722e 7570 6c6f 6164  _uploader.upload
-000013f0: 2069 6d70 6f72 7420 7570 6c6f 6164 5f76   import upload_v
-00001400: 6964 656f 0a0a 7570 6c6f 6164 5f76 6964  ideo..upload_vid
-00001410: 656f 2827 7669 6465 6f2e 6d70 3427 2c20  eo('video.mp4', 
-00001420: 2723 6679 7020 4069 6365 7370 6963 6565  '#fyp @icespicee
-00001430: 272c 2027 636f 6f6b 6965 732e 7478 7427  ', 'cookies.txt'
-00001440: 290a 6060 600a 0a3c 6832 2069 643d 2273  ).```..<h2 id="s
-00001450: 7469 7463 6865 732d 6475 6574 732d 616e  titches-duets-an
-00001460: 642d 636f 6d6d 656e 7473 223e 20f0 9faa  d-comments"> ...
-00001470: a120 5374 6974 6368 6573 2c20 4475 6574  . Stitches, Duet
-00001480: 7320 616e 6420 436f 6d6d 656e 7473 3c2f  s and Comments</
-00001490: 6832 3e0a 0a54 6f20 7365 7420 7768 6574  h2>..To set whet
-000014a0: 6865 7220 6f72 206e 6f74 2061 2076 6964  her or not a vid
-000014b0: 656f 2075 706c 6f61 6465 6420 616c 6c6f  eo uploaded allo
-000014c0: 7773 2073 7469 7463 6865 732c 2063 6f6d  ws stitches, com
-000014d0: 6d65 6e74 7320 6f72 2064 7565 742c 2073  ments or duet, s
-000014e0: 696d 706c 7920 7370 6563 6966 7920 6063  imply specify `c
-000014f0: 6f6d 6d65 6e74 602c 2060 7374 6974 6368  omment`, `stitch
-00001500: 6020 616e 642f 6f72 2060 6475 6574 6020  ` and/or `duet` 
-00001510: 6173 206b 6579 776f 7264 2061 7267 756d  as keyword argum
-00001520: 656e 7473 2074 6f20 6075 706c 6f61 645f  ents to `upload_
-00001530: 7669 6465 6f60 206f 7220 6075 706c 6f61  video` or `uploa
-00001540: 645f 7669 6465 6f73 602e 0a0a 6060 6070  d_videos`...```p
-00001550: 7974 686f 6e0a 7570 6c6f 6164 5f76 6964  ython.upload_vid
-00001560: 656f 282e 2e2e 2c20 636f 6d6d 656e 743d  eo(..., comment=
-00001570: 5472 7565 2c20 7374 6974 6368 3d54 7275  True, stitch=Tru
-00001580: 652c 2064 7565 743d 5472 7565 290a 6060  e, duet=True).``
-00001590: 600a 0a3e 2043 6f6d 6d65 6e74 732c 2053  `..> Comments, S
-000015a0: 7469 7463 6865 7320 616e 6420 4475 6574  titches and Duet
-000015b0: 7320 6172 6520 616c 6c6f 7765 6420 6279  s are allowed by
-000015c0: 202a 2a64 6566 6175 6c74 2a2a 0a0a 3c68   **default**..<h
-000015d0: 3220 6964 3d22 7072 6f78 7922 3e20 f09f  2 id="proxy"> ..
-000015e0: 8c90 2050 726f 7879 3c2f 6832 3e0a 0a54  .. Proxy</h2>..T
-000015f0: 6f20 7365 7420 6120 7072 6f78 792c 2063  o set a proxy, c
-00001600: 7572 7265 6e74 6c79 206f 6e6c 7920 776f  urrently only wo
-00001610: 726b 7320 7769 7468 2063 6872 6f6d 6520  rks with chrome 
-00001620: 6173 2074 6865 2062 726f 7773 6572 2c20  as the browser, 
-00001630: 616c 6c6f 7720 7573 6572 3a70 6173 7320  allow user:pass 
-00001640: 6175 7468 2e0a 0a60 6060 7079 7468 6f6e  auth...```python
-00001650: 0a23 2070 726f 7879 203d 207b 2775 7365  .# proxy = {'use
-00001660: 7227 3a20 276d 7975 7365 7227 2c20 2770  r': 'myuser', 'p
-00001670: 6173 7327 3a20 276d 7970 6173 7327 2c20  ass': 'mypass', 
-00001680: 2768 6f73 7427 3a20 2731 3131 2e31 3131  'host': '111.111
-00001690: 2e31 3131 272c 2027 706f 7274 273a 2027  .111', 'port': '
-000016a0: 3939 277d 2020 2320 7573 6572 3a70 6173  99'}  # user:pas
-000016b0: 730a 7072 6f78 7920 3d20 7b27 686f 7374  s.proxy = {'host
-000016c0: 273a 2027 3131 312e 3131 312e 3131 3127  ': '111.111.111'
-000016d0: 2c20 2770 6f72 7427 3a20 2739 3927 7d0a  , 'port': '99'}.
-000016e0: 7570 6c6f 6164 5f76 6964 656f 282e 2e2e  upload_video(...
-000016f0: 2c20 7072 6f78 793d 7072 6f78 7929 0a60  , proxy=proxy).`
-00001700: 6060 0a0a 3c68 3220 6964 3d22 7363 6865  ``..<h2 id="sche
-00001710: 6475 6c65 223e 20f0 9f93 8620 5363 6865  dule"> .... Sche
-00001720: 6475 6c65 3c2f 6832 3e0a 0a54 6865 2064  dule</h2>..The d
-00001730: 6174 6574 696d 6520 746f 2073 6368 6564  atetime to sched
-00001740: 756c 6520 7468 6520 7669 6465 6f20 7769  ule the video wi
-00001750: 6c6c 2062 6520 7472 6561 7465 6420 7769  ll be treated wi
-00001760: 7468 2074 6865 2055 5443 2074 696d 657a  th the UTC timez
-00001770: 6f6e 652e 203c 6272 3e0a 5468 6520 7363  one. <br>.The sc
-00001780: 6865 6475 6c65 6420 6461 7465 7469 6d65  heduled datetime
-00001790: 206d 7573 7420 6265 2061 7420 6c65 6173   must be at leas
-000017a0: 7420 3230 206d 696e 7574 6573 2069 6e20  t 20 minutes in 
-000017b0: 7468 6520 6675 7475 7265 2061 6e64 2061  the future and a
-000017c0: 206d 6178 696d 756d 206f 6620 3130 2064   maximum of 10 d
-000017d0: 6179 732e 0a0a 6060 6070 7974 686f 6e0a  ays...```python.
-000017e0: 696d 706f 7274 2064 6174 6574 696d 650a  import datetime.
-000017f0: 7363 6865 6475 6c65 203d 2064 6174 6574  schedule = datet
-00001800: 696d 652e 6461 7465 7469 6d65 2832 3032  ime.datetime(202
-00001810: 302c 2031 322c 2032 302c 2031 332c 2030  0, 12, 20, 13, 0
-00001820: 3029 0a75 706c 6f61 645f 7669 6465 6f28  0).upload_video(
-00001830: 2e2e 2e2c 2073 6368 6564 756c 653d 7363  ..., schedule=sc
-00001840: 6865 6475 6c65 290a 6060 600a 0a3c 6832  hedule).```..<h2
-00001850: 2069 643d 2261 7574 6865 6e74 6963 6174   id="authenticat
-00001860: 696f 6e22 3e20 f09f 9490 2041 7574 6865  ion"> .... Authe
-00001870: 6e74 6963 6174 696f 6e3c 2f68 323e 0a0a  ntication</h2>..
-00001880: 4175 7468 656e 7469 6361 7469 6f6e 2075  Authentication u
-00001890: 7365 7320 796f 7572 2062 726f 7773 6572  ses your browser
-000018a0: 2773 2063 6f6f 6b69 6573 2e20 5468 6973  's cookies. This
-000018b0: 2077 6f72 6b61 726f 756e 6420 7761 7320   workaround was 
-000018c0: 646f 6e65 2064 7565 2074 6f20 5469 6b54  done due to TikT
-000018d0: 6f6b 2773 2073 7472 6963 7465 7220 7374  ok's stricter st
-000018e0: 616e 6365 206f 6e20 6175 7468 656e 7469  ance on authenti
-000018f0: 6361 7469 6f6e 2062 7920 6120 5365 6c65  cation by a Sele
-00001900: 6e69 756d 2d63 6f6e 7472 6f6c 6c65 6420  nium-controlled 
-00001910: 6272 6f77 7365 722e 0a0a 596f 7572 2060  browser...Your `
-00001920: 7365 7373 696f 6e69 6460 2069 7320 616c  sessionid` is al
-00001930: 6c20 7468 6174 2069 7320 7265 7175 6972  l that is requir
-00001940: 6564 2066 6f72 2061 7574 6865 6e74 6963  ed for authentic
-00001950: 6174 696f 6e20 616e 6420 6361 6e20 6265  ation and can be
-00001960: 2070 6173 7365 6420 6173 2061 6e20 6172   passed as an ar
-00001970: 6775 6d65 6e74 2074 6f20 6e65 6172 6c79  gument to nearly
-00001980: 2061 6e79 2066 756e 6374 696f 6e0a 0a5b   any function..[
-00001990: f09f 8daa 2047 6574 2063 6f6f 6b69 6573  .... Get cookies
-000019a0: 2e74 7874 5d28 6874 7470 733a 2f2f 6769  .txt](https://gi
-000019b0: 7468 7562 2e63 6f6d 2f6b 6169 7269 3030  thub.com/kairi00
-000019c0: 332f 4765 742d 636f 6f6b 6965 732e 7478  3/Get-cookies.tx
-000019d0: 742d 4c4f 4341 4c4c 5929 206d 616b 6573  t-LOCALLY) makes
-000019e0: 2067 6574 7469 6e67 2063 6f6f 6b69 6573   getting cookies
-000019f0: 2069 6e20 6120 5b4e 6574 5363 6170 6520   in a [NetScape 
-00001a00: 636f 6f6b 6965 7320 666f 726d 6174 5d28  cookies format](
-00001a10: 6874 7470 3a2f 2f66 696c 6566 6f72 6d61  http://fileforma
-00001a20: 7473 2e61 7263 6869 7665 7465 616d 2e6f  ts.archiveteam.o
-00001a30: 7267 2f77 696b 692f 4e65 7473 6361 7065  rg/wiki/Netscape
-00001a40: 5f63 6f6f 6b69 6573 2e74 7874 292e 0a0a  _cookies.txt)...
-00001a50: 4166 7465 7220 696e 7374 616c 6c69 6e67  After installing
-00001a60: 2c20 6f70 656e 2074 6865 2065 7874 656e  , open the exten
-00001a70: 7369 6f6e 7320 6d65 6e75 206f 6e20 5b54  sions menu on [T
-00001a80: 696b 546f 6b2e 636f 6d5d 2868 7474 7073  ikTok.com](https
-00001a90: 3a2f 2f74 696b 746f 6b2e 636f 6d2f 2920  ://tiktok.com/) 
-00001aa0: 616e 6420 636c 6963 6b20 60f0 9f8d aa20  and click `.... 
-00001ab0: 4765 7420 636f 6f6b 6965 732e 7478 7460  Get cookies.txt`
-00001ac0: 2074 6f20 7265 7665 616c 2079 6f75 7220   to reveal your 
-00001ad0: 636f 6f6b 6965 732e 2053 656c 6563 7420  cookies. Select 
-00001ae0: 6045 7870 6f72 7420 4173 20e2 87a9 6020  `Export As ...` 
-00001af0: 616e 6420 7370 6563 6966 7920 6120 6c6f  and specify a lo
-00001b00: 6361 7469 6f6e 2061 6e64 206e 616d 6520  cation and name 
-00001b10: 746f 2073 6176 652e 0a0a 6060 6070 7974  to save...```pyt
-00001b20: 686f 6e0a 7570 6c6f 6164 5f76 6964 656f  hon.upload_video
-00001b30: 282e 2e2e 2c20 636f 6f6b 6965 733d 2763  (..., cookies='c
-00001b40: 6f6f 6b69 6573 2e74 7874 2729 0a60 6060  ookies.txt').```
-00001b50: 0a0a 2a2a 4f70 7469 6f6e 616c 6c79 2a2a  ..**Optionally**
-00001b60: 2c20 6063 6f6f 6b69 6573 5f6c 6973 7460  , `cookies_list`
-00001b70: 2069 7320 6120 6c69 7374 206f 6620 6469   is a list of di
-00001b80: 6374 696f 6e61 7269 6573 2077 6974 6820  ctionaries with 
-00001b90: 6b65 7973 2060 6e61 6d65 602c 2060 7661  keys `name`, `va
-00001ba0: 6c75 6560 2c20 6064 6f6d 6169 6e60 2c20  lue`, `domain`, 
-00001bb0: 6070 6174 6860 2061 6e64 2060 6578 7069  `path` and `expi
-00001bc0: 7279 6020 7768 6963 6820 616c 6c6f 7720  ry` which allow 
-00001bd0: 796f 7520 746f 2070 6173 7320 796f 7572  you to pass your
-00001be0: 206f 776e 2062 726f 7773 6572 2063 6f6f   own browser coo
-00001bf0: 6b69 6573 2e0a 0a2a 2a45 7861 6d70 6c65  kies...**Example
-00001c00: 3a2a 2a0a 0a60 6060 7079 7468 6f6e 0a63  :**..```python.c
-00001c10: 6f6f 6b69 6573 5f6c 6973 7420 3d20 5b0a  ookies_list = [.
-00001c20: 2020 2020 7b0a 2020 2020 2020 2020 276e      {.        'n
-00001c30: 616d 6527 3a20 2773 6573 7369 6f6e 6964  ame': 'sessionid
-00001c40: 272c 0a20 2020 2020 2020 2027 7661 6c75  ',.        'valu
-00001c50: 6527 3a20 272a 2a79 6f75 7220 7365 7373  e': '**your sess
-00001c60: 696f 6e20 6964 2a2a 272c 0a20 2020 2020  ion id**',.     
-00001c70: 2020 2027 646f 6d61 696e 273a 2027 6874     'domain': 'ht
-00001c80: 7470 733a 2f2f 7469 6b74 6f6b 2e63 6f6d  tps://tiktok.com
-00001c90: 272c 0a20 2020 2020 2020 2027 7061 7468  ',.        'path
-00001ca0: 273a 2027 2f27 2c0a 2020 2020 2020 2020  ': '/',.        
-00001cb0: 2765 7870 6972 7927 3a20 2731 302f 382f  'expiry': '10/8/
-00001cc0: 3230 3233 2c20 3132 3a31 383a 3538 2050  2023, 12:18:58 P
-00001cd0: 4d27 0a20 2020 207d 2c0a 2020 2020 2320  M'.    },.    # 
-00001ce0: 7468 6520 7265 7374 206f 6620 796f 7572  the rest of your
-00001cf0: 2063 6f6f 6b69 6573 2061 6c6c 2069 6e20   cookies all in 
-00001d00: 6120 6c69 7374 0a5d 0a0a 7570 6c6f 6164  a list.]..upload
-00001d10: 5f76 6964 656f 282e 2e2e 2c20 636f 6f6b  _video(..., cook
-00001d20: 6965 735f 6c69 7374 3d63 6f6f 6b69 6573  ies_list=cookies
-00001d30: 5f6c 6973 7429 0a60 6060 0a0a 3c68 3220  _list).```..<h2 
-00001d40: 6964 3d22 6272 6f77 7365 722d 7365 6c65  id="browser-sele
-00001d50: 6374 696f 6e22 3e20 f09f 9180 2042 726f  ction"> .... Bro
-00001d60: 7773 6572 2053 656c 6563 7469 6f6e 3c2f  wser Selection</
-00001d70: 6832 3e0a 0a5b 476f 6f67 6c65 2043 6872  h2>..[Google Chr
-00001d80: 6f6d 655d 2868 7474 7073 3a2f 2f77 7777  ome](https://www
-00001d90: 2e67 6f6f 676c 652e 636f 6d2f 6368 726f  .google.com/chro
-00001da0: 6d65 2920 6973 2074 6865 2070 7265 6665  me) is the prefe
-00001db0: 7272 6564 2062 726f 7773 6572 2066 6f72  rred browser for
-00001dc0: 202a 2a54 696b 546f 6b55 706c 6f61 6465   **TikTokUploade
-00001dd0: 722a 2a2e 2054 6865 2064 6566 6175 6c74  r**. The default
-00001de0: 2061 6e74 692d 6465 7465 6374 696f 6e20   anti-detection 
-00001df0: 7465 6368 6e69 7175 6573 2075 7365 6420  techniques used 
-00001e00: 696e 2074 6869 7320 7061 636b 6167 6564  in this packaged
-00001e10: 2061 7265 206f 7074 696d 697a 6564 2066   are optimized f
-00001e20: 6f72 2074 6869 732e 2048 6f77 6576 6572  or this. However
-00001e30: 2c20 6966 2079 6f75 2077 6973 6820 746f  , if you wish to
-00001e40: 2075 7365 2061 2064 6966 6665 7265 6e74   use a different
-00001e50: 2062 726f 7773 6572 2079 6f75 206d 6179   browser you may
-00001e60: 2073 7065 6369 6679 2074 6865 2060 6272   specify the `br
-00001e70: 6f77 7365 7260 2069 6e20 6075 706c 6f61  owser` in `uploa
-00001e80: 645f 7669 6465 6f60 206f 7220 6075 706c  d_video` or `upl
-00001e90: 6f61 645f 7669 6465 6f73 602e 0a0a 6060  oad_videos`...``
-00001ea0: 6070 7974 686f 6e0a 6672 6f6d 2074 696b  `python.from tik
-00001eb0: 746f 6b5f 7570 6c6f 6164 6572 2e75 706c  tok_uploader.upl
-00001ec0: 6f61 6420 696d 706f 7274 2075 706c 6f61  oad import uploa
-00001ed0: 645f 7669 6465 6f0a 0a66 726f 6d20 7261  d_video..from ra
-00001ee0: 6e64 6f6d 2069 6d70 6f72 7420 6368 6f69  ndom import choi
-00001ef0: 6365 0a0a 4252 4f57 5345 5253 203d 205b  ce..BROWSERS = [
-00001f00: 0a20 2020 2027 6368 726f 6d65 272c 0a20  .    'chrome',. 
-00001f10: 2020 2027 7361 6661 7269 272c 0a20 2020     'safari',.   
-00001f20: 2027 6368 726f 6d69 756d 272c 0a20 2020   'chromium',.   
-00001f30: 2027 6564 6765 272c 0a20 2020 2027 6669   'edge',.    'fi
-00001f40: 7265 666f 7827 0a5d 0a0a 2320 7261 6e64  refox'.]..# rand
-00001f50: 6f6d 6c79 2070 6963 6b73 2061 2077 6562  omly picks a web
-00001f60: 2062 726f 7773 6572 0a75 706c 6f61 645f   browser.upload_
-00001f70: 7669 6465 6f28 2e2e 2e2c 2062 726f 7773  video(..., brows
-00001f80: 6572 3d63 686f 6963 6528 4252 4f57 5345  er=choice(BROWSE
-00001f90: 5253 2929 0a60 6060 0a0a e29c 8520 5375  RS)).```..... Su
-00001fa0: 7070 6f72 7465 6420 4272 6f77 7365 7273  pported Browsers
-00001fb0: 3a0a 0a2d 202a 2a43 6872 6f6d 652a 2a20  :..- **Chrome** 
-00001fc0: 2852 6563 6f6d 6d65 6e64 6564 290a 2d20  (Recommended).- 
-00001fd0: 2a2a 5361 6661 7269 2a2a 0a2d 202a 2a43  **Safari**.- **C
-00001fe0: 6872 6f6d 6975 6d2a 2a0a 2d20 2a2a 4564  hromium**.- **Ed
-00001ff0: 6765 2a2a 0a2d 202a 2a46 6972 6546 6f78  ge**.- **FireFox
-00002000: 2a2a 0a0a 3c68 3220 6964 3d22 6375 7374  **..<h2 id="cust
-00002010: 6f6d 2d77 6562 6472 6976 6572 223e 20f0  om-webdriver"> .
-00002020: 9f9a b220 4375 7374 6f6d 2057 6562 4472  ... Custom WebDr
-00002030: 6976 6572 204f 7074 696f 6e73 3c2f 6832  iver Options</h2
-00002040: 3e0a 0a44 6566 6175 6c74 206d 6f64 6966  >..Default modif
-00002050: 6963 6174 696f 6e73 2074 6f20 5365 6c65  ications to Sele
-00002060: 6e69 756d 2061 7265 2061 7070 6c69 6564  nium are applied
-00002070: 2077 6869 6368 2068 656c 7020 6974 2061   which help it a
-00002080: 766f 6964 2062 6569 6e67 2064 6574 6563  void being detec
-00002090: 7465 6420 6279 2054 696b 546f 6b2e 0a0a  ted by TikTok...
-000020a0: 486f 7765 7665 722c 2079 6f75 202a 2a6d  However, you **m
-000020b0: 6179 2a2a 2070 6173 7320 6120 6375 7374  ay** pass a cust
-000020c0: 6f6d 2064 7269 7665 7220 636f 6e66 6967  om driver config
-000020d0: 7572 6174 696f 6e20 6f70 7469 6f6e 732e  uration options.
-000020e0: 2053 696d 706c 7920 7061 7373 2060 6f70   Simply pass `op
-000020f0: 7469 6f6e 7360 2061 7320 6120 6b65 7977  tions` as a keyw
-00002100: 6f72 6420 6172 6775 6d65 6e74 2074 6f20  ord argument to 
-00002110: 6569 7468 6572 2060 7570 6c6f 6164 5f76  either `upload_v
-00002120: 6964 656f 6020 6f72 2060 7570 6c6f 6164  ideo` or `upload
-00002130: 5f76 6964 656f 7360 2e0a 0a60 6060 7079  _videos`...```py
-00002140: 7468 6f6e 0a66 726f 6d20 7365 6c65 6e69  thon.from seleni
-00002150: 756d 2e77 6562 6472 6976 6572 2e63 6872  um.webdriver.chr
-00002160: 6f6d 652e 6f70 7469 6f6e 7320 696d 706f  ome.options impo
-00002170: 7274 204f 7074 696f 6e73 0a0a 6f70 7469  rt Options..opti
-00002180: 6f6e 7320 3d20 4f70 7469 6f6e 7328 290a  ons = Options().
-00002190: 0a6f 7074 696f 6e73 2e61 6464 5f61 7267  .options.add_arg
-000021a0: 756d 656e 7428 2773 7461 7274 2d6d 6178  ument('start-max
-000021b0: 696d 697a 6564 2729 0a0a 7570 6c6f 6164  imized')..upload
-000021c0: 5f76 6964 656f 7328 2e2e 2e2c 206f 7074  _videos(..., opt
-000021d0: 696f 6e73 3d6f 7074 696f 6e73 290a 6060  ions=options).``
-000021e0: 600a 0a3e 204e 6f74 653a 204d 616b 6520  `..> Note: Make 
-000021f0: 7375 7265 2074 6f20 7573 6520 7468 6520  sure to use the 
-00002200: 7269 6768 7420 7365 6c65 6e69 756d 206f  right selenium o
-00002210: 7074 696f 6e73 2066 6f72 2079 6f75 7220  ptions for your 
-00002220: 6272 6f77 7365 720a 0a3c 6832 2069 643d  browser..<h2 id=
-00002230: 2268 6561 646c 6573 7322 3e20 f09f a4af  "headless"> ....
-00002240: 2048 6561 646c 6573 7320 4272 6f77 7365   Headless Browse
-00002250: 7273 203c 2f68 323e 0a0a 4865 6164 6c65  rs </h2>..Headle
-00002260: 7373 2062 726f 7773 696e 6720 6f6e 6c79  ss browsing only
-00002270: 2077 6f72 6b73 206f 6e20 4368 726f 6d65   works on Chrome
-00002280: 2e20 5768 656e 2075 7369 6e67 2043 6872  . When using Chr
-00002290: 6f6d 652c 2061 6464 696e 6720 7468 6520  ome, adding the 
-000022a0: 602d 2d68 6561 646c 6573 7360 2066 6c61  `--headless` fla
-000022b0: 6720 7573 696e 6720 7468 6520 434c 4920  g using the CLI 
-000022c0: 6f72 2070 6173 7369 6e67 2060 6865 6164  or passing `head
-000022d0: 6c65 7373 6020 6173 2061 206b 6579 776f  less` as a keywo
-000022e0: 7264 2061 7267 756d 656e 7420 746f 2060  rd argument to `
-000022f0: 7570 6c6f 6164 5f76 6964 656f 6020 6f72  upload_video` or
-00002300: 2060 7570 6c6f 6164 5f76 6964 656f 7360   `upload_videos`
-00002310: 2069 7320 616c 6c20 7468 6174 2069 7320   is all that is 
-00002320: 7265 7175 6972 6564 2e0a 0a60 6060 7079  required...```py
-00002330: 7468 6f6e 0a75 706c 6f61 645f 7669 6465  thon.upload_vide
-00002340: 6f28 2e2e 2e2c 2068 6561 646c 6573 733d  o(..., headless=
-00002350: 5472 7565 290a 7570 6c6f 6164 5f76 6964  True).upload_vid
-00002360: 656f 7328 2e2e 2e2c 2068 6561 646c 6573  eos(..., headles
-00002370: 733d 5472 7565 290a 6060 600a 0a3c 6832  s=True).```..<h2
-00002380: 2069 643d 2269 6e69 7469 616c 2d73 6574   id="initial-set
-00002390: 7570 223e 20f0 9f94 a820 496e 6974 6961  up"> .... Initia
-000023a0: 6c20 5365 7475 703c 2f68 323e 0a0a 5b57  l Setup</h2>..[W
-000023b0: 6562 4472 6976 6572 4d61 6e61 6765 725d  ebDriverManager]
-000023c0: 2868 7474 7073 3a2f 2f62 6f6e 6967 6172  (https://bonigar
-000023d0: 6369 612e 6465 762f 7765 6264 7269 7665  cia.dev/webdrive
-000023e0: 726d 616e 6167 6572 2f29 2069 7320 7573  rmanager/) is us
-000023f0: 6564 2074 6f20 6d61 6e61 6765 2064 7269  ed to manage dri
-00002400: 7665 7220 7665 7273 696f 6e73 2e0a 0a4f  ver versions...O
-00002410: 6e20 696e 6974 6961 6c20 7374 6172 7475  n initial startu
-00002420: 702c 2079 6f75 202a 2a6d 6179 2a2a 2062  p, you **may** b
-00002430: 6520 7072 6f6d 7074 6564 2074 6f20 696e  e prompted to in
-00002440: 7374 616c 6c20 7468 6520 636f 7272 6563  stall the correc
-00002450: 7420 6472 6976 6572 2066 6f72 2079 6f75  t driver for you
-00002460: 7220 7365 6c65 6374 6564 2062 726f 7773  r selected brows
-00002470: 6572 2e20 486f 7765 7665 722c 2066 6f72  er. However, for
-00002480: 202a 2a43 6872 6f6d 652a 2a20 616e 6420   **Chrome** and 
-00002490: 2a2a 4564 6765 2a2a 2074 6865 2064 7269  **Edge** the dri
-000024a0: 7665 7220 6973 2061 7574 6f6d 6174 6963  ver is automatic
-000024b0: 616c 6c79 2069 6e73 7461 6c6c 6564 2e0a  ally installed..
-000024c0: 0a3c 6832 2069 643d 2265 7861 6d70 6c65  .<h2 id="example
-000024d0: 7322 3e20 e299 bb20 4578 616d 706c 6573  s"> ... Examples
-000024e0: 3c2f 6832 3e0a 0a2d 202a 2a5b 4261 7369  </h2>..- **[Basi
-000024f0: 6320 5570 6c6f 6164 2045 7861 6d70 6c65  c Upload Example
-00002500: 5d28 6578 616d 706c 6573 2f62 6173 6963  ](examples/basic
-00002510: 5f75 706c 6f61 642e 7079 293a 2a2a 2055  _upload.py):** U
-00002520: 7365 7320 6075 706c 6f61 645f 7669 6465  ses `upload_vide
-00002530: 6f60 2074 6f20 6d61 6b65 206f 6e65 2070  o` to make one p
-00002540: 6f73 742e 0a0a 2d20 2a2a 5b4d 756c 7469  ost...- **[Multi
-00002550: 706c 6520 5669 6465 6f73 2041 7420 4f6e  ple Videos At On
-00002560: 6365 5d28 6578 616d 706c 6573 2f6d 756c  ce](examples/mul
-00002570: 7469 706c 655f 7669 6465 6f73 5f61 745f  tiple_videos_at_
-00002580: 6f6e 6365 2e70 7929 3a2a 2a20 5570 6c6f  once.py):** Uplo
-00002590: 6164 7320 7468 6520 7361 6d65 2076 6964  ads the same vid
-000025a0: 656f 206d 756c 7469 706c 6520 7469 6d65  eo multiple time
-000025b0: 7320 7573 696e 6720 6075 706c 6f61 645f  s using `upload_
-000025c0: 7669 6465 6f73 602e 0a0a 2d20 2a2a 5b53  videos`...- **[S
-000025d0: 6572 6965 7320 5570 6c6f 6164 2045 7861  eries Upload Exa
-000025e0: 6d70 6c65 5d28 6578 616d 706c 6573 2f73  mple](examples/s
-000025f0: 6572 6965 735f 7570 6c6f 6164 2e70 7929  eries_upload.py)
-00002600: 3a2a 2a20 5669 6465 6f73 2061 7265 2072  :** Videos are r
-00002610: 6561 6420 6672 6f6d 2061 2043 5356 2066  ead from a CSV f
-00002620: 696c 6520 7573 696e 6720 5b50 616e 6461  ile using [Panda
-00002630: 735d 2868 7474 7073 3a2f 2f70 616e 6461  s](https://panda
-00002640: 732e 7079 6461 7461 2e6f 7267 292e 2041  s.pydata.org). A
-00002650: 2076 6964 656f 2075 706c 6f61 6420 6174   video upload at
-00002660: 7465 6d70 7420 6973 206d 6164 6520 616e  tempt is made an
-00002670: 6420 2a2a 6966 2061 6e64 206f 6e6c 7920  d **if and only 
-00002680: 6966 2a2a 2069 7420 6973 2073 7563 6365  if** it is succe
-00002690: 7373 6675 6c20 7769 6c6c 2074 6865 2076  ssful will the v
-000026a0: 6964 656f 2062 6520 6d61 726b 6564 2061  ideo be marked a
-000026b0: 7320 7570 6c6f 6164 6564 2e0a 0a3c 6831  s uploaded...<h1
-000026c0: 2069 643d 226e 6f74 6573 223e 20f0 9f93   id="notes"> ...
-000026d0: 9d20 4e6f 7465 733c 2f68 313e 0a0a 5468  . Notes</h1>..Th
-000026e0: 6973 2062 6f74 2069 7320 6e6f 7420 666f  is bot is not fo
-000026f0: 6f6c 2070 726f 6f66 2e20 5468 6f75 6768  ol proof. Though
-00002700: 2049 2068 6176 6520 6e6f 7420 676f 7474   I have not gott
-00002710: 656e 2061 6e20 6f66 6669 6369 616c 2062  en an official b
-00002720: 616e 2c20 7468 6520 7669 6465 6f20 7769  an, the video wi
-00002730: 6c6c 2066 6169 6c20 746f 2075 706c 6f61  ll fail to uploa
-00002740: 6420 6166 7465 7220 746f 6f20 6d61 6e79  d after too many
-00002750: 2075 706c 6f61 6473 2e20 496e 2074 6573   uploads. In tes
-00002760: 7469 6e67 2c20 7761 6974 696e 6720 7365  ting, waiting se
-00002770: 7665 7261 6c20 686f 7572 7320 7761 7320  veral hours was 
-00002780: 7375 6666 6963 6965 6e74 2074 6f20 6669  sufficient to fi
-00002790: 7820 7468 6973 2070 726f 626c 656d 2e20  x this problem. 
-000027a0: 466f 7220 7468 6973 2072 6561 736f 6e2c  For this reason,
-000027b0: 2070 6c65 6173 6520 7468 696e 6b20 6f66   please think of
-000027c0: 2074 6869 7320 6d6f 7265 2061 7320 6120   this more as a 
-000027d0: 7363 6865 6475 6c65 6420 7570 6c6f 6164  scheduled upload
-000027e0: 6572 2066 6f72 2054 696b 546f 6b20 7669  er for TikTok vi
-000027f0: 6465 6f73 2c20 7261 7468 6572 2074 6861  deos, rather tha
-00002800: 6e20 6120 7370 616d 2062 6f74 2e0a 0a3c  n a spam bot...<
-00002810: 6831 2069 643d 226d 6164 652d 7769 7468  h1 id="made-with
-00002820: 223e 2041 6363 6f75 6e74 7320 6d61 6465  "> Accounts made
-00002830: 2077 6974 683c 2f68 313e 0a0a 2d20 5b40   with</h1>..- [@
-00002840: 435f 5370 616e 5d28 6874 7470 733a 2f2f  C_Span](https://
-00002850: 7777 772e 7469 6b74 6f6b 2e63 6f6d 2f40  www.tiktok.com/@
-00002860: 635f 7370 616e 3f6c 616e 673d 656e 2920  c_span?lang=en) 
-00002870: 2d20 4120 7370 6c69 742d 7363 7265 656e  - A split-screen
-00002880: 2063 6861 6e6e 656c 2077 6974 6820 6d6f   channel with mo
-00002890: 6269 6c65 2067 616d 6573 2062 656c 6f77  bile games below
-000028a0: 2d66 6561 7475 7269 6e67 2063 6c69 7073  -featuring clips
-000028b0: 2066 726f 6d20 432d 5370 616e 2773 2059   from C-Span's Y
-000028c0: 6f75 5475 6265 2063 6861 6e6e 656c 0a2d  ouTube channel.-
-000028d0: 205b 4068 6162 6974 5f74 7261 636b 5d28   [@habit_track](
-000028e0: 6874 7470 733a 2f2f 7777 772e 7469 6b74  https://www.tikt
-000028f0: 6f6b 2e63 6f6d 2f40 6861 6269 745f 7472  ok.com/@habit_tr
-00002900: 6163 6b3f 6c61 6e67 3d65 6e29 202d 2041  ack?lang=en) - A
-00002910: 2052 6564 6469 7420 626f 7420 746f 2073   Reddit bot to s
-00002920: 6565 2077 6869 6368 2053 7562 5265 6464  ee which SubRedd
-00002930: 6974 2069 7320 6d6f 7374 2076 6972 616c  it is most viral
-00002940: 206f 6e20 5469 6b54 6f6b 0a0a 3e20 4966   on TikTok..> If
-00002950: 2079 6f75 206c 696b 6520 7468 6973 2070   you like this p
-00002960: 726f 6a65 6374 2c20 706c 6561 7365 20e2  roject, please .
-00002970: ad90 2069 7420 6f6e 2047 6974 4875 6220  .. it on GitHub 
-00002980: 746f 2073 686f 7720 796f 7572 2073 7570  to show your sup
-00002990: 706f 7274 2120 e29d a4ef b88f 0a0a 215b  port! ........![
-000029a0: 5374 6172 2048 6973 746f 7279 2043 6861  Star History Cha
-000029b0: 7274 5d28 6874 7470 733a 2f2f 6170 692e  rt](https://api.
-000029c0: 7374 6172 2d68 6973 746f 7279 2e63 6f6d  star-history.com
-000029d0: 2f73 7667 3f72 6570 6f73 3d77 6b61 6973  /svg?repos=wkais
-000029e0: 6572 7465 7861 732f 7469 6b74 6f6b 2d75  ertexas/tiktok-u
-000029f0: 706c 6f61 6465 7226 7479 7065 3d44 6174  ploader&type=Dat
-00002a00: 6529 0a0a 5b5e 315d 3a20 4966 2069 6e74  e)..[^1]: If int
-00002a10: 6572 6573 7465 6420 696e 2048 6174 6368  erested in Hatch
-00002a20: 2c20 6368 6563 6b6f 7574 2074 6865 205b  , checkout the [
-00002a30: 7765 6273 6974 655d 2868 7474 7073 3a2f  website](https:/
-00002a40: 2f68 6174 6368 2e70 7970 612e 696f 2f6c  /hatch.pypa.io/l
-00002a50: 6174 6573 742f 6275 696c 642f 290a       atest/build/).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7469 6b74  : 2.1.Name: tikt
+00000020: 6f6b 2d75 706c 6f61 6465 720a 5665 7273  ok-uploader.Vers
+00000030: 696f 6e3a 2031 2e30 2e32 0a53 756d 6d61  ion: 1.0.2.Summa
+00000040: 7279 3a20 416e 2061 7574 6f6d 6174 6963  ry: An automatic
+00000050: 2054 696b 546f 6b20 7669 6465 6f20 7570   TikTok video up
+00000060: 6c6f 6164 6572 2077 2f20 434c 492e 2055  loader w/ CLI. U
+00000070: 706c 6f61 6473 2076 6964 656f 7320 6175  ploads videos au
+00000080: 746f 6d61 7469 6361 6c6c 7920 7573 696e  tomatically usin
+00000090: 6720 616e 2061 7574 6f6d 6174 6564 2062  g an automated b
+000000a0: 726f 7773 6572 2061 6e64 2079 6f75 7220  rowser and your 
+000000b0: 636f 6f6b 6965 7320 666f 7220 6175 7468  cookies for auth
+000000c0: 656e 7469 6361 7469 6f6e 2e0a 5072 6f6a  entication..Proj
+000000d0: 6563 742d 5552 4c3a 2053 6f75 7263 6520  ect-URL: Source 
+000000e0: 436f 6465 2c20 6874 7470 733a 2f2f 6769  Code, https://gi
+000000f0: 7468 7562 2e63 6f6d 2f77 6b61 6973 6572  thub.com/wkaiser
+00000100: 7465 7861 732f 7469 6b74 6f6b 2d75 706c  texas/tiktok-upl
+00000110: 6f61 6465 720a 5072 6f6a 6563 742d 5552  oader.Project-UR
+00000120: 4c3a 2042 7567 2054 7261 636b 6572 2c20  L: Bug Tracker, 
+00000130: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000140: 6f6d 2f77 6b61 6973 6572 7465 7861 732f  om/wkaisertexas/
+00000150: 7469 6b74 6f6b 2d75 706c 6f61 6465 722f  tiktok-uploader/
+00000160: 6973 7375 6573 0a41 7574 686f 722d 656d  issues.Author-em
+00000170: 6169 6c3a 2057 696c 6c69 616d 204b 6169  ail: William Kai
+00000180: 7365 7220 3c77 6b61 6973 6572 7465 7861  ser <wkaisertexa
+00000190: 7340 676d 6169 6c2e 636f 6d3e 0a4b 6579  s@gmail.com>.Key
+000001a0: 776f 7264 733a 2041 7574 6f6d 6174 696f  words: Automatio
+000001b0: 6e2c 434c 492c 436f 6d6d 616e 6420 4c69  n,CLI,Command Li
+000001c0: 6e65 2c50 7974 686f 6e2c 5365 6c65 6e69  ne,Python,Seleni
+000001d0: 756d 2c54 696b 546f 6b2c 5570 6c6f 6164  um,TikTok,Upload
+000001e0: 2c56 6964 656f 0a43 6c61 7373 6966 6965  ,Video.Classifie
+000001f0: 723a 204c 6963 656e 7365 203a 3a20 4f53  r: License :: OS
+00000200: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
+00000210: 5420 4c69 6365 6e73 650a 436c 6173 7369  T License.Classi
+00000220: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
+00000230: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+00000240: 6570 656e 6465 6e74 0a43 6c61 7373 6966  ependent.Classif
+00000250: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000260: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000270: 686f 6e20 3a3a 2033 0a52 6571 7569 7265  hon :: 3.Require
+00000280: 732d 5079 7468 6f6e 3a20 3e3d 332e 300a  s-Python: >=3.0.
+00000290: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
+000002a0: 7974 7a0a 5265 7175 6972 6573 2d44 6973  ytz.Requires-Dis
+000002b0: 743a 2073 656c 656e 6975 6d0a 5265 7175  t: selenium.Requ
+000002c0: 6972 6573 2d44 6973 743a 2074 6f6d 6c0a  ires-Dist: toml.
+000002d0: 5265 7175 6972 6573 2d44 6973 743a 2077  Requires-Dist: w
+000002e0: 6562 6472 6976 6572 2d6d 616e 6167 6572  ebdriver-manager
+000002f0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
+00000300: 2074 6573 740a 5265 7175 6972 6573 2d44   test.Requires-D
+00000310: 6973 743a 2070 7974 6573 743b 2065 7874  ist: pytest; ext
+00000320: 7261 203d 3d20 2774 6573 7427 0a44 6573  ra == 'test'.Des
+00000330: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+00000340: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+00000350: 646f 776e 0a0a 3c70 2061 6c69 676e 3d22  down..<p align="
+00000360: 6365 6e74 6572 223e 0a3c 696d 6720 7372  center">.<img sr
+00000370: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
+00000380: 622e 636f 6d2f 776b 6169 7365 7274 6578  b.com/wkaisertex
+00000390: 6173 2f74 696b 746f 6b2d 7570 6c6f 6164  as/tiktok-upload
+000003a0: 6572 2f61 7373 6574 732f 3237 3739 3530  er/assets/277950
+000003b0: 3134 2f66 3939 3166 6463 372d 3238 3761  14/f991fdc7-287a
+000003c0: 2d34 6333 622d 3961 3834 2d32 3263 3761  -4c3b-9a84-22c7a
+000003d0: 6438 6135 3762 6622 2061 6c74 3d22 7669  d8a57bf" alt="vi
+000003e0: 6465 6f20 776f 726b 696e 6722 202f 3e0a  deo working" />.
+000003f0: 3c2f 703e 0a0a 3c68 3120 616c 6967 6e3d  </p>..<h1 align=
+00000400: 2263 656e 7465 7222 3e20 e2ac 86ef b88f  "center"> ......
+00000410: 2054 696b 546f 6b20 5570 6c6f 6164 6572   TikTok Uploader
+00000420: 203c 2f68 313e 0a3c 7020 616c 6967 6e3d   </h1>.<p align=
+00000430: 2263 656e 7465 7222 3e41 203c 7374 726f  "center">A <stro
+00000440: 6e67 3e53 656c 656e 6975 6d3c 2f73 7472  ng>Selenium</str
+00000450: 6f6e 673e 2d62 6173 6564 2061 7574 6f6d  ong>-based autom
+00000460: 6174 6564 203c 7374 726f 6e67 3e54 696b  ated <strong>Tik
+00000470: 546f 6b3c 2f73 7472 6f6e 673e 2076 6964  Tok</strong> vid
+00000480: 656f 2075 706c 6f61 6465 723c 2f70 3e0a  eo uploader</p>.
+00000490: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+000004a0: 7222 3e0a 2020 3c69 6d67 2061 6c74 3d22  r">.  <img alt="
+000004b0: 466f 726b 7322 2073 7263 3d22 6874 7470  Forks" src="http
+000004c0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000004d0: 696f 2f67 6974 6875 622f 666f 726b 732f  io/github/forks/
+000004e0: 776b 6169 7365 7274 6578 6173 2f74 696b  wkaisertexas/tik
+000004f0: 746f 6b2d 7570 6c6f 6164 6572 2220 2f3e  tok-uploader" />
+00000500: 0a20 203c 696d 6720 616c 743d 2253 7461  .  <img alt="Sta
+00000510: 7273 2220 7372 633d 2268 7474 7073 3a2f  rs" src="https:/
+00000520: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000530: 6769 7468 7562 2f73 7461 7273 2f77 6b61  github/stars/wka
+00000540: 6973 6572 7465 7861 732f 7469 6b74 6f6b  isertexas/tiktok
+00000550: 2d75 706c 6f61 6465 7222 202f 3e0a 2020  -uploader" />.  
+00000560: 3c69 6d67 2061 6c74 3d22 5761 7463 6865  <img alt="Watche
+00000570: 7273 2220 7372 633d 2268 7474 7073 3a2f  rs" src="https:/
+00000580: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000590: 6769 7468 7562 2f77 6174 6368 6572 732f  github/watchers/
+000005a0: 776b 6169 7365 7274 6578 6173 2f74 696b  wkaisertexas/tik
+000005b0: 746f 6b2d 7570 6c6f 6164 6572 2220 2f3e  tok-uploader" />
+000005c0: 0a3c 2f70 3e0a 0a23 2054 6162 6c65 206f  .</p>..# Table o
+000005d0: 6620 436f 6e74 656e 7473 0a2d 205b 496e  f Contents.- [In
+000005e0: 7374 616c 6c61 7469 6f6e 5d28 2369 6e73  stallation](#ins
+000005f0: 7461 6c6c 6174 696f 6e29 0a20 202d 205b  tallation).  - [
+00000600: 4d61 634f 532c 2057 696e 646f 7773 2061  MacOS, Windows a
+00000610: 6e64 204c 696e 7578 5d28 236d 6163 6f73  nd Linux](#macos
+00000620: 2d77 696e 646f 7773 2d61 6e64 2d6c 696e  -windows-and-lin
+00000630: 7578 290a 2020 2020 2d20 5b44 6f77 6e6c  ux).    - [Downl
+00000640: 6f61 6469 6e67 2066 726f 6d20 5079 5049  oading from PyPI
+00000650: 2028 5265 636f 6d6d 656e 6465 6429 5d28   (Recommended)](
+00000660: 2364 6f77 6e6c 6f61 6469 6e67 2d66 726f  #downloading-fro
+00000670: 6d2d 7079 7069 2d72 6563 6f6d 6d65 6e64  m-pypi-recommend
+00000680: 6564 290a 2020 2020 2d20 5b42 7569 6c64  ed).    - [Build
+00000690: 696e 6720 6672 6f6d 2073 6f75 7263 655d  ing from source]
+000006a0: 2823 6275 696c 6469 6e67 2d66 726f 6d2d  (#building-from-
+000006b0: 736f 7572 6365 290a 2d20 5b55 7361 6765  source).- [Usage
+000006c0: 5d28 2375 7361 6765 290a 2020 2d20 5bf0  ](#usage).  - [.
+000006d0: 9f92 bb20 436f 6d6d 616e 6420 4c69 6e65  ... Command Line
+000006e0: 2049 6e74 6572 6661 6365 2028 434c 4929   Interface (CLI)
+000006f0: 5d28 232d 636f 6d6d 6d61 6e64 2d6c 696e  ](#-commmand-lin
+00000700: 652d 696e 7465 7266 6163 652d 636c 6929  e-interface-cli)
+00000710: 0a20 202d 205b e2ac 8620 5570 6c6f 6164  .  - [... Upload
+00000720: 696e 6720 5669 6465 6f73 5d28 232d 7570  ing Videos](#-up
+00000730: 6c6f 6164 696e 672d 7669 6465 6f73 290a  loading-videos).
+00000740: 2020 2d20 5bf0 9fab b520 4d65 6e74 696f    - [.... Mentio
+00000750: 6e73 2061 6e64 2048 6173 6874 6167 735d  ns and Hashtags]
+00000760: 2823 2d6d 656e 7469 6f6e 732d 616e 642d  (#-mentions-and-
+00000770: 6861 7368 7461 6773 290a 2020 2d20 5bf0  hashtags).  - [.
+00000780: 9faa a120 5374 6974 6368 6573 2c20 4475  ... Stitches, Du
+00000790: 6574 7320 616e 6420 436f 6d6d 656e 7473  ets and Comments
+000007a0: 5d28 232d 7374 6974 6368 6573 2d64 7565  ](#-stitches-due
+000007b0: 7473 2d61 6e64 2d63 6f6d 6d65 6e74 7329  ts-and-comments)
+000007c0: 0a20 202d 205b f09f 9490 2041 7574 6865  .  - [.... Authe
+000007d0: 6e74 6963 6174 696f 6e5d 2823 2d61 7574  ntication](#-aut
+000007e0: 6865 6e74 6963 6174 696f 6e29 0a20 202d  hentication).  -
+000007f0: 205b f09f 9180 2042 726f 7773 6572 2053   [.... Browser S
+00000800: 656c 6563 7469 6f6e 5d28 232d 6272 6f77  election](#-brow
+00000810: 7365 722d 7365 6c65 6374 696f 6e29 0a20  ser-selection). 
+00000820: 202d 205b f09f 9ab2 2043 7573 746f 6d20   - [.... Custom 
+00000830: 5765 6244 7269 7665 7220 4472 6976 6572  WebDriver Driver
+00000840: 204f 7074 696f 6e73 5d28 232d 6375 7374   Options](#-cust
+00000850: 6f6d 2d77 6562 6472 6976 6572 2d64 7269  om-webdriver-dri
+00000860: 7665 722d 6f70 7469 6f6e 7329 0a20 202d  ver-options).  -
+00000870: 205b f09f a4af 2048 6561 646c 6573 7320   [.... Headless 
+00000880: 4272 6f77 7365 7273 5d28 232d 6865 6164  Browsers](#-head
+00000890: 6c65 7373 2d62 726f 7773 6572 7329 0a20  less-browsers). 
+000008a0: 202d 205b f09f 94a8 2049 6e69 7469 616c   - [.... Initial
+000008b0: 2053 6574 7570 5d28 232d 696e 6974 6961   Setup](#-initia
+000008c0: 6c2d 7365 7475 7029 0a2d 205b e299 bbef  l-setup).- [....
+000008d0: b88f 2045 7861 6d70 6c65 735d 2823 2d65  .. Examples](#-e
+000008e0: 7861 6d70 6c65 7329 0a2d 205b f09f 939d  xamples).- [....
+000008f0: 204e 6f74 6573 5d28 232d 6e6f 7465 7329   Notes](#-notes)
+00000900: 0a2d 205b 4163 636f 756e 7473 206d 6164  .- [Accounts mad
+00000910: 6520 7769 7468 5d28 2361 6363 6f75 6e74  e with](#account
+00000920: 732d 6d61 6465 2d75 7369 6e67 2d74 696b  s-made-using-tik
+00000930: 746f 6b2d 7570 6c6f 6164 6572 290a 2320  tok-uploader).# 
+00000940: 496e 7374 616c 6c61 7469 6f6e 0a0a 4120  Installation..A 
+00000950: 7065 7271 7569 7369 7465 2074 6f20 7573  perquisite to us
+00000960: 696e 6720 7468 6973 2070 726f 6772 616d  ing this program
+00000970: 2069 7320 7468 6520 696e 7374 616c 6c61   is the installa
+00000980: 7469 6f6e 206f 6620 6120 5b53 656c 656e  tion of a [Selen
+00000990: 6975 6d2d 636f 6d70 6174 6962 6c65 5d28  ium-compatible](
+000009a0: 6874 7470 733a 2f2f 7777 772e 7365 6c65  https://www.sele
+000009b0: 6e69 756d 2e64 6576 2f64 6f63 756d 656e  nium.dev/documen
+000009c0: 7461 7469 6f6e 2f77 6562 6472 6976 6572  tation/webdriver
+000009d0: 2f67 6574 7469 6e67 5f73 7461 7274 6564  /getting_started
+000009e0: 2f69 6e73 7461 6c6c 5f64 7269 7665 7273  /install_drivers
+000009f0: 2f29 2077 6562 2062 726f 7773 6572 2e20  /) web browser. 
+00000a00: 5b47 6f6f 676c 6520 4368 726f 6d65 5d28  [Google Chrome](
+00000a10: 6874 7470 733a 2f2f 7777 772e 676f 6f67  https://www.goog
+00000a20: 6c65 2e63 6f6d 2f63 6872 6f6d 652f 2920  le.com/chrome/) 
+00000a30: 6973 2072 6563 6f6d 6d65 6e64 6564 2e0a  is recommended..
+00000a40: 0a23 2320 4d61 634f 532c 2057 696e 646f  .## MacOS, Windo
+00000a50: 7773 2061 6e64 204c 696e 7578 0a0a 496e  ws and Linux..In
+00000a60: 7374 616c 6c20 5079 7468 6f6e 2033 206f  stall Python 3 o
+00000a70: 7220 6772 6561 7465 7220 6672 6f6d 205b  r greater from [
+00000a80: 7079 7468 6f6e 2e6f 7267 5d28 6874 7470  python.org](http
+00000a90: 733a 2f2f 7777 772e 7079 7468 6f6e 2e6f  s://www.python.o
+00000aa0: 7267 2f64 6f77 6e6c 6f61 6473 2f29 0a0a  rg/downloads/)..
+00000ab0: 2323 2320 446f 776e 6c6f 6164 696e 6720  ### Downloading 
+00000ac0: 6672 6f6d 2050 7950 4920 2852 6563 6f6d  from PyPI (Recom
+00000ad0: 6d65 6e64 6564 290a 0a49 6e73 7461 6c6c  mended)..Install
+00000ae0: 2060 7469 6b74 6f6b 2d75 706c 6f61 6465   `tiktok-uploade
+00000af0: 7260 2075 7369 6e67 2060 7069 7060 0a0a  r` using `pip`..
+00000b00: 6060 6062 6173 680a 7069 7020 696e 7374  ```bash.pip inst
+00000b10: 616c 6c20 7469 6b74 6f6b 2d75 706c 6f61  all tiktok-uploa
+00000b20: 6465 720a 6060 600a 0a23 2323 2042 7569  der.```..### Bui
+00000b30: 6c64 696e 6720 6672 6f6d 2073 6f75 7263  lding from sourc
+00000b40: 650a 0a49 6e73 7461 6c6c 696e 6720 6672  e..Installing fr
+00000b50: 6f6d 2073 6f75 7263 6520 616c 6c6f 7773  om source allows
+00000b60: 2067 7265 6174 6572 2066 6c65 7869 6269   greater flexibi
+00000b70: 6c69 7479 2074 6f20 6d6f 6469 6679 2074  lity to modify t
+00000b80: 6865 206d 6f64 756c 6527 7320 636f 6465  he module's code
+00000b90: 2074 6f20 6578 7465 6e64 2064 6566 6175   to extend defau
+00000ba0: 6c74 2062 6568 6176 696f 722e 200a 0a46  lt behavior. ..F
+00000bb0: 6972 7374 2c20 6063 6c6f 6e65 6020 616e  irst, `clone` an
+00000bc0: 6420 6d6f 7665 2069 6e74 6f20 7468 6520  d move into the 
+00000bd0: 7265 706f 7369 746f 7279 2e20 4e65 7874  repository. Next
+00000be0: 2c20 696e 7374 616c 6c20 6068 6174 6368  , install `hatch
+00000bf0: 602c 2074 6865 2062 7569 6c64 2074 6f6f  `, the build too
+00000c00: 6c20 7573 6564 2066 6f72 2074 6869 7320  l used for this 
+00000c10: 7072 6f6a 6563 7420 5b5e 315d 2e20 5468  project [^1]. Th
+00000c20: 656e 2c20 6062 7569 6c64 6020 7468 6520  en, `build` the 
+00000c30: 7072 6f6a 6563 742e 2046 696e 616c 6c79  project. Finally
+00000c40: 2c20 6069 6e73 7461 6c6c 6020 7468 6520  , `install` the 
+00000c50: 7072 6f6a 6563 7420 7769 7468 2074 6865  project with the
+00000c60: 2060 2d65 6020 6f72 2065 6469 7461 626c   `-e` or editabl
+00000c70: 6520 666c 6167 2e20 200a 6060 6063 6f6e  e flag.  .```con
+00000c80: 736f 6c65 0a67 6974 2063 6c6f 6e65 2068  sole.git clone h
+00000c90: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000ca0: 6d2f 776b 6169 7365 7274 6578 6173 2f74  m/wkaisertexas/t
+00000cb0: 696b 746f 6b2d 7570 6c6f 6164 6572 2e67  iktok-uploader.g
+00000cc0: 6974 0a63 6420 7469 6b74 6f6b 2d75 706c  it.cd tiktok-upl
+00000cd0: 6f61 6465 720a 7069 7020 696e 7374 616c  oader.pip instal
+00000ce0: 6c20 6861 7463 680a 6861 7463 6820 6275  l hatch.hatch bu
+00000cf0: 696c 640a 7069 7020 696e 7374 616c 6c20  ild.pip install 
+00000d00: 2d65 202e 200a 6060 600a 0a23 2055 7361  -e . .```..# Usa
+00000d10: 6765 0a0a 6074 696b 746f 6b2d 7570 6c6f  ge..`tiktok-uplo
+00000d20: 6164 6572 6020 776f 726b 7320 6279 2064  ader` works by d
+00000d30: 7570 6c69 6361 7469 6e67 2079 6f75 7220  uplicating your 
+00000d40: 6272 6f77 7365 7227 7320 2a2a 636f 6f6b  browser's **cook
+00000d50: 6965 732a 2a20 7768 6963 6820 7472 6963  ies** which tric
+00000d60: 6b73 202a 2a54 696b 546f 6b2a 2a20 696e  ks **TikTok** in
+00000d70: 746f 2062 656c 6965 7669 6e67 2079 6f75  to believing you
+00000d80: 2061 7265 206c 6f67 6765 6420 696e 206f   are logged in o
+00000d90: 6e20 6120 7265 6d6f 7465 2d63 6f6e 7472  n a remote-contr
+00000da0: 6f6c 6c65 6420 6272 6f77 7365 722e 0a0a  olled browser...
+00000db0: 2323 20f0 9f92 bb20 436f 6d6d 616e 6420  ## .... Command 
+00000dc0: 4c69 6e65 2049 6e74 6572 6661 6365 2028  Line Interface (
+00000dd0: 434c 4929 0a0a 5573 696e 6720 7468 6520  CLI)..Using the 
+00000de0: 434c 4920 6973 2061 7320 7369 6d70 6c65  CLI is as simple
+00000df0: 2061 7320 6361 6c6c 696e 6720 6074 696b   as calling `tik
+00000e00: 746f 6b2d 7570 6c6f 6164 6572 6020 7769  tok-uploader` wi
+00000e10: 7468 2079 6f75 7220 7669 6465 6f73 3a20  th your videos: 
+00000e20: 6070 6174 6860 2028 2d76 292c 2060 6465  `path` (-v), `de
+00000e30: 7363 7269 7074 696f 6e60 282d 6429 2061  scription`(-d) a
+00000e40: 6e64 2060 636f 6f6b 6965 7360 2028 2d63  nd `cookies` (-c
+00000e50: 290a 0a60 6060 6261 7368 0a74 696b 746f  )..```bash.tikto
+00000e60: 6b2d 7570 6c6f 6164 6572 202d 7620 7669  k-uploader -v vi
+00000e70: 6465 6f2e 6d70 3420 2d64 2022 7468 6973  deo.mp4 -d "this
+00000e80: 2069 7320 6d79 2065 7363 6170 6564 205c   is my escaped \
+00000e90: 2264 6573 6372 6970 7469 6f6e 5c22 2220  "description\"" 
+00000ea0: 2d63 2063 6f6f 6b69 6573 2e74 7874 0a60  -c cookies.txt.`
+00000eb0: 6060 0a0a 6060 6070 7974 686f 6e0a 6672  ``..```python.fr
+00000ec0: 6f6d 2074 696b 746f 6b5f 7570 6c6f 6164  om tiktok_upload
+00000ed0: 6572 2e75 706c 6f61 6420 696d 706f 7274  er.upload import
+00000ee0: 2075 706c 6f61 645f 7669 6465 6f2c 2075   upload_video, u
+00000ef0: 706c 6f61 645f 7669 6465 6f73 0a66 726f  pload_videos.fro
+00000f00: 6d20 7469 6b74 6f6b 5f75 706c 6f61 6465  m tiktok_uploade
+00000f10: 722e 6175 7468 2069 6d70 6f72 7420 4175  r.auth import Au
+00000f20: 7468 4261 636b 656e 640a 0a23 2073 696e  thBackend..# sin
+00000f30: 676c 6520 7669 6465 6f0a 7570 6c6f 6164  gle video.upload
+00000f40: 5f76 6964 656f 2827 7669 6465 6f2e 6d70  _video('video.mp
+00000f50: 3427 2c20 0a20 2020 2020 2020 2020 2020  4', .           
+00000f60: 2064 6573 6372 6970 7469 6f6e 3d27 7468   description='th
+00000f70: 6973 2069 7320 6d79 2064 6573 6372 6970  is is my descrip
+00000f80: 7469 6f6e 272c 200a 2020 2020 2020 2020  tion', .        
+00000f90: 2020 2020 636f 6f6b 6965 733d 2763 6f6f      cookies='coo
+00000fa0: 6b69 6573 2e74 7874 2729 0a0a 2320 4d75  kies.txt')..# Mu
+00000fb0: 6c74 6970 6c65 2056 6964 656f 730a 7669  ltiple Videos.vi
+00000fc0: 6465 6f73 203d 205b 0a20 2020 207b 0a20  deos = [.    {. 
+00000fd0: 2020 2020 2020 2027 7061 7468 273a 2027         'path': '
+00000fe0: 7669 6465 6f2e 6d70 3427 2c20 0a20 2020  video.mp4', .   
+00000ff0: 2020 2020 2027 6465 7363 7269 7074 696f       'descriptio
+00001000: 6e27 3a20 2774 6869 7320 6973 206d 7920  n': 'this is my 
+00001010: 6465 7363 7269 7074 696f 6e27 0a20 2020  description'.   
+00001020: 207d 2c0a 2020 2020 7b0a 2020 2020 2020   },.    {.      
+00001030: 2020 2770 6174 6827 3a20 2776 6964 656f    'path': 'video
+00001040: 322e 6d70 3427 2c20 0a20 2020 2020 2020  2.mp4', .       
+00001050: 2027 6465 7363 7269 7074 696f 6e27 3a20   'description': 
+00001060: 2774 6869 7320 6973 2061 6c73 6f20 6d79  'this is also my
+00001070: 2064 6573 6372 6970 7469 6f6e 270a 2020   description'.  
+00001080: 2020 7d0a 5d0a 0a61 7574 6820 3d20 4175    }.]..auth = Au
+00001090: 7468 4261 636b 656e 6428 636f 6f6b 6965  thBackend(cookie
+000010a0: 733d 2763 6f6f 6b69 6573 2e74 7874 2729  s='cookies.txt')
+000010b0: 0a75 706c 6f61 645f 7669 6465 6f73 2876  .upload_videos(v
+000010c0: 6964 656f 733d 7669 6465 6f73 2c20 6175  ideos=videos, au
+000010d0: 7468 3d61 7574 6829 0a60 6060 0a0a 2323  th=auth).```..##
+000010e0: 20e2 ac86 2055 706c 6f61 6469 6e67 2056   ... Uploading V
+000010f0: 6964 656f 730a 0a54 6869 7320 6c69 6272  ideos..This libr
+00001100: 6172 7920 7265 766f 6c76 6573 2061 726f  ary revolves aro
+00001110: 756e 6420 7468 6520 6075 706c 6f61 645f  und the `upload_
+00001120: 7669 6465 6f73 6020 6675 6e63 7469 6f6e  videos` function
+00001130: 2077 6869 6368 2074 616b 6573 2069 6e20   which takes in 
+00001140: 6120 6c69 7374 206f 6620 7669 6465 6f73  a list of videos
+00001150: 2077 6869 6368 2068 6176 6520 2a2a 6669   which have **fi
+00001160: 6c65 6e61 6d65 732a 2a20 616e 6420 2a2a  lenames** and **
+00001170: 6465 7363 7269 7074 696f 6e73 2a2a 2061  descriptions** a
+00001180: 6e64 2061 7265 2070 6173 7365 6420 6173  nd are passed as
+00001190: 2066 6f6c 6c6f 7773 3a0a 0a60 6060 7079   follows:..```py
+000011a0: 7468 6f6e 0a66 726f 6d20 7469 6b74 6f6b  thon.from tiktok
+000011b0: 5f75 706c 6f61 6465 722e 7570 6c6f 6164  _uploader.upload
+000011c0: 2069 6d70 6f72 7420 7570 6c6f 6164 5f76   import upload_v
+000011d0: 6964 656f 730a 6672 6f6d 2074 696b 746f  ideos.from tikto
+000011e0: 6b5f 7570 6c6f 6164 6572 2e61 7574 6820  k_uploader.auth 
+000011f0: 696d 706f 7274 2041 7574 6842 6163 6b65  import AuthBacke
+00001200: 6e64 0a0a 7669 6465 6f73 203d 205b 0a20  nd..videos = [. 
+00001210: 2020 207b 0a20 2020 2020 2020 2027 7669     {.        'vi
+00001220: 6465 6f27 3a20 2776 6964 656f 302e 6d70  deo': 'video0.mp
+00001230: 3427 2c0a 2020 2020 2020 2020 2764 6573  4',.        'des
+00001240: 6372 6970 7469 6f6e 273a 2027 5669 6465  cription': 'Vide
+00001250: 6f20 3120 6973 2061 626f 7574 202e 2e2e  o 1 is about ...
+00001260: 270a 2020 2020 7d2c 0a20 2020 207b 0a20  '.    },.    {. 
+00001270: 2020 2020 2020 2027 7669 6465 6f27 3a20         'video': 
+00001280: 2776 6964 656f 312e 6d70 3427 2c0a 2020  'video1.mp4',.  
+00001290: 2020 2020 2020 2764 6573 6372 6970 7469        'descripti
+000012a0: 6f6e 273a 2027 5669 6465 6f20 3220 6973  on': 'Video 2 is
+000012b0: 2061 626f 7574 202e 2e2e 270a 2020 2020   about ...'.    
+000012c0: 7d0a 5d0a 0a61 7574 6820 3d20 4175 7468  }.]..auth = Auth
+000012d0: 4261 636b 656e 6428 636f 6f6b 6965 733d  Backend(cookies=
+000012e0: 2763 6f6f 6b69 6573 2e74 7874 2729 0a66  'cookies.txt').f
+000012f0: 6169 6c65 645f 7669 6465 6f73 203d 2075  ailed_videos = u
+00001300: 706c 6f61 645f 7669 6465 6f73 2876 6964  pload_videos(vid
+00001310: 656f 733d 7669 6465 6f73 2c20 6175 7468  eos=videos, auth
+00001320: 3d61 7574 6829 0a0a 666f 7220 7669 6465  =auth)..for vide
+00001330: 6f20 696e 2066 6169 6c65 645f 7669 6465  o in failed_vide
+00001340: 6f73 3a20 2320 6561 6368 2069 6e70 7574  os: # each input
+00001350: 2076 6964 656f 206f 626a 6563 7420 7768   video object wh
+00001360: 6963 6820 6661 696c 6564 0a20 2020 2070  ich failed.    p
+00001370: 7269 6e74 2866 277b 7669 6465 6f5b 2776  rint(f'{video['v
+00001380: 6964 656f 275d 7d20 7769 7468 2064 6573  ideo']} with des
+00001390: 6372 6970 7469 6f6e 2022 7b76 6964 656f  cription "{video
+000013a0: 5b27 6465 7363 7269 7074 696f 6e27 5d7d  ['description']}
+000013b0: 2220 6661 696c 6564 2729 0a60 6060 0a0a  " failed').```..
+000013c0: 2323 20f0 9fab b520 4d65 6e74 696f 6e73  ## .... Mentions
+000013d0: 2061 6e64 2048 6173 6874 6167 730a 0a4d   and Hashtags..M
+000013e0: 656e 7469 6f6e 7320 616e 6420 4861 7368  entions and Hash
+000013f0: 7461 6773 206e 6f77 2077 6f72 6b20 736f  tags now work so
+00001400: 206c 6f6e 6720 6173 2074 6865 7920 6172   long as they ar
+00001410: 6520 666f 6c6c 6f77 6564 2062 7920 6120  e followed by a 
+00001420: 7370 6163 652e 2048 6f77 6576 6572 2c20  space. However, 
+00001430: 796f 7520 6173 2074 6865 2075 7365 7220  you as the user 
+00001440: 6172 6520 7265 7370 6f6e 7369 626c 6520  are responsible 
+00001450: 666f 7220 7665 7269 6679 696e 6720 6120  for verifying a 
+00001460: 6d65 6e74 696f 6e20 6f72 2068 6173 6874  mention or hasht
+00001470: 6167 2065 7869 7374 7320 6265 666f 7265  ag exists before
+00001480: 2070 6f73 7469 6e67 0a0a 2a2a 4578 616d   posting..**Exam
+00001490: 706c 653a 2a2a 0a60 6060 7079 7468 6f6e  ple:**.```python
+000014a0: 0a66 726f 6d20 7469 6b74 6f6b 5f75 706c  .from tiktok_upl
+000014b0: 6f61 6465 722e 7570 6c6f 6164 2069 6d70  oader.upload imp
+000014c0: 6f72 7420 7570 6c6f 6164 5f76 6964 656f  ort upload_video
+000014d0: 0a0a 7570 6c6f 6164 5f76 6964 656f 2827  ..upload_video('
+000014e0: 7669 6465 6f2e 6d70 3427 2c20 2723 6679  video.mp4', '#fy
+000014f0: 7020 4069 6365 7370 6963 6565 272c 2027  p @icespicee', '
+00001500: 636f 6f6b 6965 732e 7478 7427 290a 6060  cookies.txt').``
+00001510: 600a 0a23 2320 f09f aaa1 2053 7469 7463  `..## .... Stitc
+00001520: 6865 732c 2044 7565 7473 2061 6e64 2043  hes, Duets and C
+00001530: 6f6d 6d65 6e74 730a 0a54 6f20 7365 7420  omments..To set 
+00001540: 7768 6574 6865 7220 6f72 206e 6f74 2061  whether or not a
+00001550: 2076 6964 656f 2075 706c 6f61 6465 6420   video uploaded 
+00001560: 616c 6c6f 7773 2073 7469 7463 6865 732c  allows stitches,
+00001570: 2063 6f6d 6d65 6e74 7320 6f72 2064 7565   comments or due
+00001580: 742c 2073 696d 706c 7920 7370 6563 6966  t, simply specif
+00001590: 7920 6063 6f6d 6d65 6e74 602c 2060 7374  y `comment`, `st
+000015a0: 6974 6368 6020 616e 642f 6f72 2060 6475  itch` and/or `du
+000015b0: 6574 6020 6173 206b 6579 776f 7264 2061  et` as keyword a
+000015c0: 7267 756d 656e 7473 2074 6f20 6075 706c  rguments to `upl
+000015d0: 6f61 645f 7669 6465 6f60 206f 7220 6075  oad_video` or `u
+000015e0: 706c 6f61 645f 7669 6465 6f73 602e 0a0a  pload_videos`...
+000015f0: 6060 6070 7974 686f 6e0a 7570 6c6f 6164  ```python.upload
+00001600: 5f76 6964 656f 282e 2e2e 2c20 636f 6d6d  _video(..., comm
+00001610: 656e 743d 5472 7565 2c20 7374 6974 6368  ent=True, stitch
+00001620: 3d54 7275 652c 2064 7565 743d 5472 7565  =True, duet=True
+00001630: 290a 6060 600a 0a3e 2043 6f6d 6d65 6e74  ).```..> Comment
+00001640: 732c 2053 7469 7463 6865 7320 616e 6420  s, Stitches and 
+00001650: 4475 6574 7320 6172 6520 616c 6c6f 7765  Duets are allowe
+00001660: 6420 6279 202a 2a64 6566 6175 6c74 2a2a  d by **default**
+00001670: 0a0a 2323 20f0 9f8c 9020 5072 6f78 790a  ..## .... Proxy.
+00001680: 546f 2073 6574 2061 2070 726f 7879 2c20  To set a proxy, 
+00001690: 6375 7272 656e 746c 7920 6f6e 6c79 2077  currently only w
+000016a0: 6f72 6b73 2077 6974 6820 6368 726f 6d65  orks with chrome
+000016b0: 2061 7320 7468 6520 6272 6f77 7365 722c   as the browser,
+000016c0: 2061 6c6c 6f77 2075 7365 723a 7061 7373   allow user:pass
+000016d0: 2061 7574 682e 0a0a 6060 6070 7974 686f   auth...```pytho
+000016e0: 6e0a 2320 7072 6f78 7920 3d20 7b27 7573  n.# proxy = {'us
+000016f0: 6572 273a 2027 6d79 7573 6572 272c 2027  er': 'myuser', '
+00001700: 7061 7373 273a 2027 6d79 7061 7373 272c  pass': 'mypass',
+00001710: 2027 686f 7374 273a 2027 3131 312e 3131   'host': '111.11
+00001720: 312e 3131 3127 2c20 2770 6f72 7427 3a20  1.111', 'port': 
+00001730: 2739 3927 7d20 2023 2075 7365 723a 7061  '99'}  # user:pa
+00001740: 7373 0a70 726f 7879 203d 207b 2768 6f73  ss.proxy = {'hos
+00001750: 7427 3a20 2731 3131 2e31 3131 2e31 3131  t': '111.111.111
+00001760: 272c 2027 706f 7274 273a 2027 3939 277d  ', 'port': '99'}
+00001770: 0a75 706c 6f61 645f 7669 6465 6f28 2e2e  .upload_video(..
+00001780: 2e2c 2070 726f 7879 3d70 726f 7879 290a  ., proxy=proxy).
+00001790: 6060 600a 2323 20f0 9f93 8620 5363 6865  ```.## .... Sche
+000017a0: 6475 6c65 0a54 6865 2064 6174 6574 696d  dule.The datetim
+000017b0: 6520 746f 2073 6368 6564 756c 6520 7468  e to schedule th
+000017c0: 6520 7669 6465 6f20 7769 6c6c 2062 6520  e video will be 
+000017d0: 7472 6561 7465 6420 7769 7468 2074 6865  treated with the
+000017e0: 2055 5443 2074 696d 657a 6f6e 652e 203c   UTC timezone. <
+000017f0: 6272 3e0a 5468 6520 7363 6865 6475 6c65  br>.The schedule
+00001800: 6420 6461 7465 7469 6d65 206d 7573 7420  d datetime must 
+00001810: 6265 2061 7420 6c65 6173 7420 3230 206d  be at least 20 m
+00001820: 696e 7574 6573 2069 6e20 7468 6520 6675  inutes in the fu
+00001830: 7475 7265 2061 6e64 2061 206d 6178 696d  ture and a maxim
+00001840: 756d 206f 6620 3130 2064 6179 732e 0a0a  um of 10 days...
+00001850: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
+00001860: 2064 6174 6574 696d 650a 7363 6865 6475   datetime.schedu
+00001870: 6c65 203d 2064 6174 6574 696d 652e 6461  le = datetime.da
+00001880: 7465 7469 6d65 2832 3032 302c 2031 322c  tetime(2020, 12,
+00001890: 2032 302c 2031 332c 2030 3029 0a75 706c   20, 13, 00).upl
+000018a0: 6f61 645f 7669 6465 6f28 2e2e 2e2c 2073  oad_video(..., s
+000018b0: 6368 6564 756c 653d 7363 6865 6475 6c65  chedule=schedule
+000018c0: 290a 6060 600a 0a23 2320 f09f 9490 2041  ).```..## .... A
+000018d0: 7574 6865 6e74 6963 6174 696f 6e0a 4175  uthentication.Au
+000018e0: 7468 656e 7469 6361 7469 6f6e 2075 7365  thentication use
+000018f0: 7320 796f 7572 2062 726f 7773 6572 2773  s your browser's
+00001900: 2063 6f6f 6b69 6573 2e20 5468 6973 2077   cookies. This w
+00001910: 6f72 6b61 726f 756e 6420 7761 7320 646f  orkaround was do
+00001920: 6e65 2064 7565 2074 6f20 5469 6b54 6f6b  ne due to TikTok
+00001930: 2773 2073 7472 6963 7465 7220 7374 616e  's stricter stan
+00001940: 6365 206f 6e20 6175 7468 656e 7469 6361  ce on authentica
+00001950: 7469 6f6e 2062 7920 6120 5365 6c65 6e69  tion by a Seleni
+00001960: 756d 2d63 6f6e 7472 6f6c 6c65 6420 6272  um-controlled br
+00001970: 6f77 7365 722e 0a0a 596f 7572 2060 7365  owser...Your `se
+00001980: 7373 696f 6e69 6460 2069 7320 616c 6c20  ssionid` is all 
+00001990: 7468 6174 2069 7320 7265 7175 6972 6564  that is required
+000019a0: 2066 6f72 2061 7574 6865 6e74 6963 6174   for authenticat
+000019b0: 696f 6e20 616e 6420 6361 6e20 6265 2070  ion and can be p
+000019c0: 6173 7365 6420 6173 2061 6e20 6172 6775  assed as an argu
+000019d0: 6d65 6e74 2074 6f20 6e65 6172 6c79 2061  ment to nearly a
+000019e0: 6e79 2066 756e 6374 696f 6e0a 0a5b f09f  ny function..[..
+000019f0: 8daa 2047 6574 2063 6f6f 6b69 6573 2e74  .. Get cookies.t
+00001a00: 7874 5d28 6874 7470 733a 2f2f 6769 7468  xt](https://gith
+00001a10: 7562 2e63 6f6d 2f6b 6169 7269 3030 332f  ub.com/kairi003/
+00001a20: 4765 742d 636f 6f6b 6965 732e 7478 742d  Get-cookies.txt-
+00001a30: 4c4f 4341 4c4c 5929 206d 616b 6573 2067  LOCALLY) makes g
+00001a40: 6574 7469 6e67 2063 6f6f 6b69 6573 2069  etting cookies i
+00001a50: 6e20 6120 5b4e 6574 5363 6170 6520 636f  n a [NetScape co
+00001a60: 6f6b 6965 7320 666f 726d 6174 5d28 6874  okies format](ht
+00001a70: 7470 3a2f 2f66 696c 6566 6f72 6d61 7473  tp://fileformats
+00001a80: 2e61 7263 6869 7665 7465 616d 2e6f 7267  .archiveteam.org
+00001a90: 2f77 696b 692f 4e65 7473 6361 7065 5f63  /wiki/Netscape_c
+00001aa0: 6f6f 6b69 6573 2e74 7874 292e 0a0a 4166  ookies.txt)...Af
+00001ab0: 7465 7220 696e 7374 616c 6c69 6e67 2c20  ter installing, 
+00001ac0: 6f70 656e 2074 6865 2065 7874 656e 7369  open the extensi
+00001ad0: 6f6e 7320 6d65 6e75 206f 6e20 5b54 696b  ons menu on [Tik
+00001ae0: 546f 6b2e 636f 6d5d 2868 7474 7073 3a2f  Tok.com](https:/
+00001af0: 2f74 696b 746f 6b2e 636f 6d2f 2920 616e  /tiktok.com/) an
+00001b00: 6420 636c 6963 6b20 60f0 9f8d aa20 4765  d click `.... Ge
+00001b10: 7420 636f 6f6b 6965 732e 7478 7460 2074  t cookies.txt` t
+00001b20: 6f20 7265 7665 616c 2079 6f75 7220 636f  o reveal your co
+00001b30: 6f6b 6965 732e 2053 656c 6563 7420 6045  okies. Select `E
+00001b40: 7870 6f72 7420 4173 20e2 87a9 6020 616e  xport As ...` an
+00001b50: 6420 7370 6563 6966 7920 6120 6c6f 6361  d specify a loca
+00001b60: 7469 6f6e 2061 6e64 206e 616d 6520 746f  tion and name to
+00001b70: 2073 6176 652e 0a0a 2a2a 4f70 7469 6f6e   save...**Option
+00001b80: 616c 6c79 2a2a 2c20 6063 6f6f 6b69 6573  ally**, `cookies
+00001b90: 5f6c 6973 7460 2069 7320 6120 6c69 7374  _list` is a list
+00001ba0: 206f 6620 6469 6374 696f 6e61 7269 6573   of dictionaries
+00001bb0: 2077 6974 6820 6b65 7973 2060 6e61 6d65   with keys `name
+00001bc0: 602c 2060 7661 6c75 6560 2c20 6064 6f6d  `, `value`, `dom
+00001bd0: 6169 6e60 2c20 6070 6174 6860 2061 6e64  ain`, `path` and
+00001be0: 2060 6578 7069 7279 6020 7768 6963 6820   `expiry` which 
+00001bf0: 616c 6c6f 7720 796f 7520 746f 2070 6173  allow you to pas
+00001c00: 7320 796f 7572 206f 776e 2062 726f 7773  s your own brows
+00001c10: 6572 2063 6f6f 6b69 6573 2e20 0a0a 2a2a  er cookies. ..**
+00001c20: 4578 616d 706c 653a 2a2a 0a0a 6060 6070  Example:**..```p
+00001c30: 7974 686f 6e0a 636f 6f6b 6965 735f 6c69  ython.cookies_li
+00001c40: 7374 203d 205b 0a20 2020 207b 0a20 2020  st = [.    {.   
+00001c50: 2020 2020 2027 6e61 6d65 273a 2027 7365       'name': 'se
+00001c60: 7373 696f 6e69 6427 2c0a 2020 2020 2020  ssionid',.      
+00001c70: 2020 2776 616c 7565 273a 2027 2a2a 796f    'value': '**yo
+00001c80: 7572 2073 6573 7369 6f6e 2069 642a 2a27  ur session id**'
+00001c90: 2c0a 2020 2020 2020 2020 2764 6f6d 6169  ,.        'domai
+00001ca0: 6e27 3a20 2768 7474 7073 3a2f 2f74 696b  n': 'https://tik
+00001cb0: 746f 6b2e 636f 6d27 2c0a 2020 2020 2020  tok.com',.      
+00001cc0: 2020 2770 6174 6827 3a20 272f 272c 0a20    'path': '/',. 
+00001cd0: 2020 2020 2020 2027 6578 7069 7279 273a         'expiry':
+00001ce0: 2027 3130 2f38 2f32 3032 332c 2031 323a   '10/8/2023, 12:
+00001cf0: 3138 3a35 3820 504d 270a 2020 2020 7d0a  18:58 PM'.    }.
+00001d00: 5d0a 0a75 706c 6f61 645f 7669 6465 6f28  ]..upload_video(
+00001d10: 2e2e 2e2c 2063 6f6f 6b69 6573 5f6c 6973  ..., cookies_lis
+00001d20: 743d 636f 6f6b 6965 735f 6c69 7374 290a  t=cookies_list).
+00001d30: 6060 600a 0a23 2320 f09f 9180 2042 726f  ```..## .... Bro
+00001d40: 7773 6572 2053 656c 6563 7469 6f6e 0a0a  wser Selection..
+00001d50: 5b47 6f6f 676c 6520 4368 726f 6d65 5d28  [Google Chrome](
+00001d60: 6874 7470 733a 2f2f 7777 772e 676f 6f67  https://www.goog
+00001d70: 6c65 2e63 6f6d 2f63 6872 6f6d 6529 2069  le.com/chrome) i
+00001d80: 7320 7468 6520 7072 6566 6572 7265 6420  s the preferred 
+00001d90: 6272 6f77 7365 7220 666f 7220 2a2a 5469  browser for **Ti
+00001da0: 6b54 6f6b 5570 6c6f 6164 6572 2a2a 2e20  kTokUploader**. 
+00001db0: 5468 6520 6465 6661 756c 7420 616e 7469  The default anti
+00001dc0: 2d64 6574 6563 7469 6f6e 2074 6563 686e  -detection techn
+00001dd0: 6971 7565 7320 7573 6564 2069 6e20 7468  iques used in th
+00001de0: 6973 2070 6163 6b61 6765 6420 6172 6520  is packaged are 
+00001df0: 6f70 7469 6d69 7a65 6420 666f 7220 7468  optimized for th
+00001e00: 6973 2e20 486f 7765 7665 722c 2069 6620  is. However, if 
+00001e10: 796f 7520 7769 7368 2074 6f20 7573 6520  you wish to use 
+00001e20: 6120 6469 6666 6572 656e 7420 6272 6f77  a different brow
+00001e30: 7365 7220 796f 7520 6d61 7920 7370 6563  ser you may spec
+00001e40: 6966 7920 7468 6520 6062 726f 7773 6572  ify the `browser
+00001e50: 6020 696e 2060 7570 6c6f 6164 5f76 6964  ` in `upload_vid
+00001e60: 656f 6020 6f72 2060 7570 6c6f 6164 5f76  eo` or `upload_v
+00001e70: 6964 656f 7360 2e0a 0a60 6060 7079 7468  ideos`...```pyth
+00001e80: 6f6e 0a66 726f 6d20 7469 6b74 6f6b 5f75  on.from tiktok_u
+00001e90: 706c 6f61 6465 722e 7570 6c6f 6164 2069  ploader.upload i
+00001ea0: 6d70 6f72 7420 7570 6c6f 6164 5f76 6964  mport upload_vid
+00001eb0: 656f 0a0a 6672 6f6d 2072 616e 646f 6d20  eo..from random 
+00001ec0: 696d 706f 7274 2063 686f 6963 650a 0a42  import choice..B
+00001ed0: 524f 5753 4552 5320 3d20 5b0a 2020 2020  ROWSERS = [.    
+00001ee0: 2763 6872 6f6d 6527 2c0a 2020 2020 2773  'chrome',.    's
+00001ef0: 6166 6172 6927 2c0a 2020 2020 2763 6872  afari',.    'chr
+00001f00: 6f6d 6975 6d27 2c0a 2020 2020 2765 6467  omium',.    'edg
+00001f10: 6527 2c0a 2020 2020 2766 6972 6566 6f78  e',.    'firefox
+00001f20: 270a 5d0a 0a23 2072 616e 646f 6d6c 7920  '.]..# randomly 
+00001f30: 7069 636b 7320 6120 7765 6220 6272 6f77  picks a web brow
+00001f40: 7365 7220 0a75 706c 6f61 645f 7669 6465  ser .upload_vide
+00001f50: 6f28 2e2e 2e2c 2062 726f 7773 6572 3d63  o(..., browser=c
+00001f60: 686f 6963 6528 4252 4f57 5345 5253 2929  hoice(BROWSERS))
+00001f70: 0a60 6060 0a0a e29c 8520 5375 7070 6f72  .```..... Suppor
+00001f80: 7465 6420 4272 6f77 7365 7273 3a0a 2d20  ted Browsers:.- 
+00001f90: 2a2a 4368 726f 6d65 2a2a 2028 5265 636f  **Chrome** (Reco
+00001fa0: 6d6d 656e 6465 6429 0a2d 202a 2a53 6166  mmended).- **Saf
+00001fb0: 6172 692a 2a0a 2d20 2a2a 4368 726f 6d69  ari**.- **Chromi
+00001fc0: 756d 2a2a 0a2d 202a 2a45 6467 652a 2a0a  um**.- **Edge**.
+00001fd0: 2d20 2a2a 4669 7265 466f 782a 2a20 0a0a  - **FireFox** ..
+00001fe0: 2323 20f0 9f9a b220 4375 7374 6f6d 2057  ## .... Custom W
+00001ff0: 6562 4472 6976 6572 2044 7269 7665 7220  ebDriver Driver 
+00002000: 4f70 7469 6f6e 730a 0a44 6566 6175 6c74  Options..Default
+00002010: 206d 6f64 6966 6963 6174 696f 6e73 2074   modifications t
+00002020: 6f20 5365 6c65 6e69 756d 2061 7265 2061  o Selenium are a
+00002030: 7070 6c69 6564 2077 6869 6368 2068 656c  pplied which hel
+00002040: 7020 6974 2061 766f 6964 2062 6569 6e67  p it avoid being
+00002050: 2064 6574 6563 7465 6420 6279 2054 696b   detected by Tik
+00002060: 546f 6b2e 200a 0a48 6f77 6576 6572 2c20  Tok. ..However, 
+00002070: 796f 7520 2a2a 6d61 792a 2a20 7061 7373  you **may** pass
+00002080: 2061 2063 7573 746f 6d20 6472 6976 6572   a custom driver
+00002090: 2063 6f6e 6669 6775 7261 7469 6f6e 206f   configuration o
+000020a0: 7074 696f 6e73 2e20 5369 6d70 6c79 2070  ptions. Simply p
+000020b0: 6173 7320 606f 7074 696f 6e73 6020 6173  ass `options` as
+000020c0: 2061 206b 6579 776f 7264 2061 7267 756d   a keyword argum
+000020d0: 656e 7420 746f 2065 6974 6865 7220 6075  ent to either `u
+000020e0: 706c 6f61 645f 7669 6465 6f60 206f 7220  pload_video` or 
+000020f0: 6075 706c 6f61 645f 7669 6465 6f73 602e  `upload_videos`.
+00002100: 200a 0a60 6060 7079 7468 6f6e 0a66 726f   ..```python.fro
+00002110: 6d20 7365 6c65 6e69 756d 2e77 6562 6472  m selenium.webdr
+00002120: 6976 6572 2e63 6872 6f6d 652e 6f70 7469  iver.chrome.opti
+00002130: 6f6e 7320 696d 706f 7274 204f 7074 696f  ons import Optio
+00002140: 6e73 0a0a 6f70 7469 6f6e 7320 3d20 4f70  ns..options = Op
+00002150: 7469 6f6e 7328 290a 0a6f 7074 696f 6e73  tions()..options
+00002160: 2e61 6464 5f61 7267 756d 656e 7428 2773  .add_argument('s
+00002170: 7461 7274 2d6d 6178 696d 697a 6564 2729  tart-maximized')
+00002180: 0a0a 7570 6c6f 6164 5f76 6964 656f 7328  ..upload_videos(
+00002190: 2e2e 2e2c 206f 7074 696f 6e73 3d6f 7074  ..., options=opt
+000021a0: 696f 6e73 290a 6060 600a 0a3e 204e 6f74  ions).```..> Not
+000021b0: 653a 204d 616b 6520 7375 7265 2074 6f20  e: Make sure to 
+000021c0: 7573 6520 7468 6520 7269 6768 7420 7365  use the right se
+000021d0: 6c65 6e69 756d 206f 7074 696f 6e73 2066  lenium options f
+000021e0: 6f72 2079 6f75 7220 6272 6f77 7365 720a  or your browser.
+000021f0: 0a23 2320 f09f a4af 2048 6561 646c 6573  .## .... Headles
+00002200: 7320 4272 6f77 7365 7273 0a0a 4865 6164  s Browsers..Head
+00002210: 6c65 7373 2062 726f 7773 696e 6720 6f6e  less browsing on
+00002220: 6c79 2077 6f72 6b73 206f 6e20 4368 726f  ly works on Chro
+00002230: 6d65 2e20 5768 656e 2075 7369 6e67 2043  me. When using C
+00002240: 6872 6f6d 652c 2061 6464 696e 6720 7468  hrome, adding th
+00002250: 6520 602d 2d68 6561 646c 6573 7360 2066  e `--headless` f
+00002260: 6c61 6720 7573 696e 6720 7468 6520 434c  lag using the CL
+00002270: 4920 6f72 2070 6173 7369 6e67 2060 6865  I or passing `he
+00002280: 6164 6c65 7373 6020 6173 2061 206b 6579  adless` as a key
+00002290: 776f 7264 2061 7267 756d 656e 7420 746f  word argument to
+000022a0: 2060 7570 6c6f 6164 5f76 6964 656f 6020   `upload_video` 
+000022b0: 6f72 2060 7570 6c6f 6164 5f76 6964 656f  or `upload_video
+000022c0: 7360 2069 7320 616c 6c20 7468 6174 2069  s` is all that i
+000022d0: 7320 7265 7175 6972 6564 2e0a 0a60 6060  s required...```
+000022e0: 7079 7468 6f6e 0a75 706c 6f61 645f 7669  python.upload_vi
+000022f0: 6465 6f28 2e2e 2e2c 2068 6561 646c 6573  deo(..., headles
+00002300: 733d 5472 7565 290a 7570 6c6f 6164 5f76  s=True).upload_v
+00002310: 6964 656f 7328 2e2e 2e2c 2068 6561 646c  ideos(..., headl
+00002320: 6573 733d 5472 7565 290a 6060 600a 0a23  ess=True).```..#
+00002330: 2320 f09f 94a8 2049 6e69 7469 616c 2053  # .... Initial S
+00002340: 6574 7570 0a0a 5b57 6562 4472 6976 6572  etup..[WebDriver
+00002350: 4d61 6e61 6765 725d 2868 7474 7073 3a2f  Manager](https:/
+00002360: 2f62 6f6e 6967 6172 6369 612e 6465 762f  /bonigarcia.dev/
+00002370: 7765 6264 7269 7665 726d 616e 6167 6572  webdrivermanager
+00002380: 2f29 2069 7320 7573 6564 2074 6f20 6d61  /) is used to ma
+00002390: 6e61 6765 2064 7269 7665 7220 7665 7273  nage driver vers
+000023a0: 696f 6e73 2e20 0a0a 4f6e 2069 6e69 7469  ions. ..On initi
+000023b0: 616c 2073 7461 7274 7570 2c20 796f 7520  al startup, you 
+000023c0: 2a2a 6d61 792a 2a20 6265 2070 726f 6d70  **may** be promp
+000023d0: 7465 6420 746f 2069 6e73 7461 6c6c 2074  ted to install t
+000023e0: 6865 2063 6f72 7265 6374 2064 7269 7665  he correct drive
+000023f0: 7220 666f 7220 796f 7572 2073 656c 6563  r for your selec
+00002400: 7465 6420 6272 6f77 7365 722e 2048 6f77  ted browser. How
+00002410: 6576 6572 2c20 666f 7220 2a2a 4368 726f  ever, for **Chro
+00002420: 6d65 2a2a 2061 6e64 202a 2a45 6467 652a  me** and **Edge*
+00002430: 2a20 7468 6520 6472 6976 6572 2069 7320  * the driver is 
+00002440: 6175 746f 6d61 7469 6361 6c6c 7920 696e  automatically in
+00002450: 7374 616c 6c65 642e 0a0a 2320 e299 bb20  stalled...# ... 
+00002460: 4578 616d 706c 6573 0a0a 2d20 2a2a 5b42  Examples..- **[B
+00002470: 6173 6963 2055 706c 6f61 6420 4578 616d  asic Upload Exam
+00002480: 706c 655d 2865 7861 6d70 6c65 732f 6261  ple](examples/ba
+00002490: 7369 635f 7570 6c6f 6164 2e70 7929 3a2a  sic_upload.py):*
+000024a0: 2a20 5573 6573 2060 7570 6c6f 6164 5f76  * Uses `upload_v
+000024b0: 6964 656f 6020 746f 206d 616b 6520 6f6e  ideo` to make on
+000024c0: 6520 706f 7374 2e0a 0a2d 202a 2a5b 4d75  e post...- **[Mu
+000024d0: 6c74 6970 6c65 2056 6964 656f 7320 4174  ltiple Videos At
+000024e0: 204f 6e63 655d 2865 7861 6d70 6c65 732f   Once](examples/
+000024f0: 6d75 6c74 6970 6c65 5f76 6964 656f 735f  multiple_videos_
+00002500: 6174 5f6f 6e63 652e 7079 293a 2a2a 2055  at_once.py):** U
+00002510: 706c 6f61 6473 2074 6865 2073 616d 6520  ploads the same 
+00002520: 7669 6465 6f20 6d75 6c74 6970 6c65 2074  video multiple t
+00002530: 696d 6573 2075 7369 6e67 2060 7570 6c6f  imes using `uplo
+00002540: 6164 5f76 6964 656f 7360 2e0a 0a2d 202a  ad_videos`...- *
+00002550: 2a5b 5365 7269 6573 2055 706c 6f61 6420  *[Series Upload 
+00002560: 4578 616d 706c 655d 2865 7861 6d70 6c65  Example](example
+00002570: 732f 7365 7269 6573 5f75 706c 6f61 642e  s/series_upload.
+00002580: 7079 293a 2a2a 2056 6964 656f 7320 6172  py):** Videos ar
+00002590: 6520 7265 6164 2066 726f 6d20 6120 4353  e read from a CS
+000025a0: 5620 6669 6c65 2075 7369 6e67 205b 5061  V file using [Pa
+000025b0: 6e64 6173 5d28 6874 7470 733a 2f2f 7061  ndas](https://pa
+000025c0: 6e64 6173 2e70 7964 6174 612e 6f72 6729  ndas.pydata.org)
+000025d0: 2e20 4120 7669 6465 6f20 7570 6c6f 6164  . A video upload
+000025e0: 2061 7474 656d 7074 2069 7320 6d61 6465   attempt is made
+000025f0: 2061 6e64 202a 2a69 6620 616e 6420 6f6e   and **if and on
+00002600: 6c79 2069 662a 2a20 6974 2069 7320 7375  ly if** it is su
+00002610: 6363 6573 7366 756c 2077 696c 6c20 7468  ccessful will th
+00002620: 6520 7669 6465 6f20 6265 206d 6172 6b65  e video be marke
+00002630: 6420 6173 2075 706c 6f61 6465 642e 0a0a  d as uploaded...
+00002640: 2320 f09f 939d 204e 6f74 6573 0a0a 5468  # .... Notes..Th
+00002650: 6973 2062 6f74 2069 7320 6e6f 7420 666f  is bot is not fo
+00002660: 6f6c 2070 726f 6f66 2e20 5468 6f75 6768  ol proof. Though
+00002670: 2049 2068 6176 6520 6e6f 7420 676f 7474   I have not gott
+00002680: 656e 2061 6e20 6f66 6669 6369 616c 2062  en an official b
+00002690: 616e 2c20 7468 6520 7669 6465 6f20 7769  an, the video wi
+000026a0: 6c6c 2066 6169 6c20 746f 2075 706c 6f61  ll fail to uploa
+000026b0: 6420 6166 7465 7220 746f 6f20 6d61 6e79  d after too many
+000026c0: 2075 706c 6f61 6473 2e20 496e 2074 6573   uploads. In tes
+000026d0: 7469 6e67 2c20 7761 6974 696e 6720 7365  ting, waiting se
+000026e0: 7665 7261 6c20 686f 7572 7320 7761 7320  veral hours was 
+000026f0: 7375 6666 6963 6965 6e74 2074 6f20 6669  sufficient to fi
+00002700: 7820 7468 6973 2070 726f 626c 656d 2e20  x this problem. 
+00002710: 466f 7220 7468 6973 2072 6561 736f 6e2c  For this reason,
+00002720: 2070 6c65 6173 6520 7468 696e 6720 6f66   please thing of
+00002730: 2074 6869 7320 6d6f 7265 2061 7320 6120   this more as a 
+00002740: 7363 6865 6475 6c65 6420 7570 6c6f 6164  scheduled upload
+00002750: 6572 2066 6f72 2054 696b 546f 6b20 7669  er for TikTok vi
+00002760: 6465 6f73 2c20 7261 7468 6572 2074 6861  deos, rather tha
+00002770: 6e20 6120 7370 616d 2062 6f74 2e0a 0a23  n a spam bot...#
+00002780: 2041 6363 6f75 6e74 7320 6d61 6465 2077   Accounts made w
+00002790: 6974 680a 0a2d 205b 4043 5f53 7061 6e5d  ith..- [@C_Span]
+000027a0: 2868 7474 7073 3a2f 2f77 7777 2e74 696b  (https://www.tik
+000027b0: 746f 6b2e 636f 6d2f 4063 5f73 7061 6e3f  tok.com/@c_span?
+000027c0: 6c61 6e67 3d65 6e29 202d 2041 2073 706c  lang=en) - A spl
+000027d0: 6974 2d73 6372 6565 6e20 6368 616e 6e65  it-screen channe
+000027e0: 6c20 7769 7468 206d 6f62 696c 6520 6761  l with mobile ga
+000027f0: 6d65 7320 6265 6c6f 7720 6665 6174 7572  mes below featur
+00002800: 696e 6720 636c 6970 7320 6672 6f6d 2043  ing clips from C
+00002810: 2d53 7061 6e27 7320 596f 7554 7562 6520  -Span's YouTube 
+00002820: 6368 616e 6e65 6c0a 2d20 5b40 6861 6269  channel.- [@habi
+00002830: 745f 7472 6163 6b5d 2868 7474 7073 3a2f  t_track](https:/
+00002840: 2f77 7777 2e74 696b 746f 6b2e 636f 6d2f  /www.tiktok.com/
+00002850: 4068 6162 6974 5f74 7261 636b 3f6c 616e  @habit_track?lan
+00002860: 673d 656e 2920 2d20 4120 5265 6464 6974  g=en) - A Reddit
+00002870: 2062 6f74 2074 6f20 7365 6520 7768 6963   bot to see whic
+00002880: 6820 5375 6252 6564 6469 7420 6973 206d  h SubReddit is m
+00002890: 6f73 7420 7669 7261 6c20 6f6e 2054 696b  ost viral on Tik
+000028a0: 546f 6b0a 0a5b 5e31 5d3a 2049 6620 696e  Tok..[^1]: If in
+000028b0: 7465 7265 7374 6564 2069 6e20 4861 7463  terested in Hatc
+000028c0: 682c 2063 6865 636b 6f75 7420 7468 6520  h, checkout the 
+000028d0: 5b77 6562 7369 7465 5d28 6874 7470 733a  [website](https:
+000028e0: 2f2f 6861 7463 682e 7079 7061 2e69 6f2f  //hatch.pypa.io/
+000028f0: 6c61 7465 7374 2f62 7569 6c64 2f29 0a    latest/build/).
```

### Comparing `tiktok_uploader-1.0.16/pyproject.toml` & `tiktok_uploader-1.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tiktok-uploader"
-version = "1.0.16"
+version = "1.0.2"
 authors = [
   { name = "William Kaiser", email = "wkaisertexas@gmail.com" },
 ]
 description = "An automatic TikTok video uploader w/ CLI. Uploads videos automatically using an automated browser and your cookies for authentication."
 readme = "README.md"
 requires-python = ">=3.0"
 keywords = [
@@ -20,15 +20,14 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-  "pyperclip",
 	"selenium",
 	"webdriver_manager",
   "toml",
   "pytz"
 ]
 
 [build-system]
```

### Comparing `tiktok_uploader-1.0.16/PKG-INFO` & `tiktok_uploader-1.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,733 +1,603 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7469 6b74  : 2.1.Name: tikt
-00000020: 6f6b 2d75 706c 6f61 6465 720a 5665 7273  ok-uploader.Vers
-00000030: 696f 6e3a 2031 2e30 2e31 360a 5375 6d6d  ion: 1.0.16.Summ
-00000040: 6172 793a 2041 6e20 6175 746f 6d61 7469  ary: An automati
-00000050: 6320 5469 6b54 6f6b 2076 6964 656f 2075  c TikTok video u
-00000060: 706c 6f61 6465 7220 772f 2043 4c49 2e20  ploader w/ CLI. 
-00000070: 5570 6c6f 6164 7320 7669 6465 6f73 2061  Uploads videos a
-00000080: 7574 6f6d 6174 6963 616c 6c79 2075 7369  utomatically usi
-00000090: 6e67 2061 6e20 6175 746f 6d61 7465 6420  ng an automated 
-000000a0: 6272 6f77 7365 7220 616e 6420 796f 7572  browser and your
-000000b0: 2063 6f6f 6b69 6573 2066 6f72 2061 7574   cookies for aut
-000000c0: 6865 6e74 6963 6174 696f 6e2e 0a50 726f  hentication..Pro
-000000d0: 6a65 6374 2d55 524c 3a20 536f 7572 6365  ject-URL: Source
-000000e0: 2043 6f64 652c 2068 7474 7073 3a2f 2f67   Code, https://g
-000000f0: 6974 6875 622e 636f 6d2f 776b 6169 7365  ithub.com/wkaise
-00000100: 7274 6578 6173 2f74 696b 746f 6b2d 7570  rtexas/tiktok-up
-00000110: 6c6f 6164 6572 0a50 726f 6a65 6374 2d55  loader.Project-U
-00000120: 524c 3a20 4275 6720 5472 6163 6b65 722c  RL: Bug Tracker,
-00000130: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000140: 636f 6d2f 776b 6169 7365 7274 6578 6173  com/wkaisertexas
-00000150: 2f74 696b 746f 6b2d 7570 6c6f 6164 6572  /tiktok-uploader
-00000160: 2f69 7373 7565 730a 4175 7468 6f72 2d65  /issues.Author-e
-00000170: 6d61 696c 3a20 5769 6c6c 6961 6d20 4b61  mail: William Ka
-00000180: 6973 6572 203c 776b 6169 7365 7274 6578  iser <wkaisertex
-00000190: 6173 4067 6d61 696c 2e63 6f6d 3e0a 4b65  as@gmail.com>.Ke
-000001a0: 7977 6f72 6473 3a20 4175 746f 6d61 7469  ywords: Automati
-000001b0: 6f6e 2c43 4c49 2c43 6f6d 6d61 6e64 204c  on,CLI,Command L
-000001c0: 696e 652c 5079 7468 6f6e 2c53 656c 656e  ine,Python,Selen
-000001d0: 6975 6d2c 5469 6b54 6f6b 2c55 706c 6f61  ium,TikTok,Uploa
-000001e0: 642c 5669 6465 6f0a 436c 6173 7369 6669  d,Video.Classifi
-000001f0: 6572 3a20 4c69 6365 6e73 6520 3a3a 204f  er: License :: O
-00000200: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
-00000210: 4954 204c 6963 656e 7365 0a43 6c61 7373  IT License.Class
-00000220: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
-00000230: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
-00000240: 6465 7065 6e64 656e 740a 436c 6173 7369  dependent.Classi
-00000250: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000260: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000270: 7468 6f6e 203a 3a20 330a 5265 7175 6972  thon :: 3.Requir
-00000280: 6573 2d50 7974 686f 6e3a 203e 3d33 2e30  es-Python: >=3.0
-00000290: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000002a0: 7079 7065 7263 6c69 700a 5265 7175 6972  pyperclip.Requir
-000002b0: 6573 2d44 6973 743a 2070 7974 7a0a 5265  es-Dist: pytz.Re
-000002c0: 7175 6972 6573 2d44 6973 743a 2073 656c  quires-Dist: sel
-000002d0: 656e 6975 6d0a 5265 7175 6972 6573 2d44  enium.Requires-D
-000002e0: 6973 743a 2074 6f6d 6c0a 5265 7175 6972  ist: toml.Requir
-000002f0: 6573 2d44 6973 743a 2077 6562 6472 6976  es-Dist: webdriv
-00000300: 6572 2d6d 616e 6167 6572 0a50 726f 7669  er-manager.Provi
-00000310: 6465 732d 4578 7472 613a 2074 6573 740a  des-Extra: test.
-00000320: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
-00000330: 7974 6573 743b 2065 7874 7261 203d 3d20  ytest; extra == 
-00000340: 2774 6573 7427 0a44 6573 6372 6970 7469  'test'.Descripti
-00000350: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
-00000360: 2074 6578 742f 6d61 726b 646f 776e 0a0a   text/markdown..
-00000370: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-00000380: 223e 0a3c 696d 6720 7372 633d 2268 7474  ">.<img src="htt
-00000390: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000003a0: 776b 6169 7365 7274 6578 6173 2f74 696b  wkaisertexas/tik
-000003b0: 746f 6b2d 7570 6c6f 6164 6572 2f61 7373  tok-uploader/ass
-000003c0: 6574 732f 3237 3739 3530 3134 2f66 3939  ets/27795014/f99
-000003d0: 3166 6463 372d 3238 3761 2d34 6333 622d  1fdc7-287a-4c3b-
-000003e0: 3961 3834 2d32 3263 3761 6438 6135 3762  9a84-22c7ad8a57b
-000003f0: 6622 2061 6c74 3d22 7669 6465 6f20 776f  f" alt="video wo
-00000400: 726b 696e 6722 202f 3e0a 3c2f 703e 0a0a  rking" />.</p>..
-00000410: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
-00000420: 7222 3e20 e2ac 86ef b88f 2054 696b 546f  r"> ...... TikTo
-00000430: 6b20 5570 6c6f 6164 6572 203c 2f68 313e  k Uploader </h1>
-00000440: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
-00000450: 7222 3e41 203c 7374 726f 6e67 3e53 656c  r">A <strong>Sel
-00000460: 656e 6975 6d3c 2f73 7472 6f6e 673e 2d62  enium</strong>-b
-00000470: 6173 6564 2061 7574 6f6d 6174 6564 203c  ased automated <
-00000480: 7374 726f 6e67 3e54 696b 546f 6b3c 2f73  strong>TikTok</s
-00000490: 7472 6f6e 673e 2076 6964 656f 2075 706c  trong> video upl
-000004a0: 6f61 6465 723c 2f70 3e0a 0a3c 7020 616c  oader</p>..<p al
-000004b0: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
-000004c0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000004d0: 2f67 6974 6875 622e 636f 6d2f 776b 6169  /github.com/wkai
-000004e0: 7365 7274 6578 6173 2f74 696b 746f 6b2d  sertexas/tiktok-
-000004f0: 7570 6c6f 6164 6572 223e 3c73 7472 6f6e  uploader"><stron
-00000500: 673e 456e 676c 6973 683c 2f73 7472 6f6e  g>English</stron
-00000510: 673e 3c2f 613e 20c2 b70a 2020 3c61 2068  g></a> ...  <a h
-00000520: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00000530: 6875 622e 636f 6d2f 776b 6169 7365 7274  hub.com/wkaisert
-00000540: 6578 6173 2f74 696b 746f 6b2d 7570 6c6f  exas/tiktok-uplo
-00000550: 6164 6572 2f62 6c6f 622f 6d61 696e 2f52  ader/blob/main/R
-00000560: 4541 444d 452e 7a68 2d48 616e 732e 6d64  EADME.zh-Hans.md
-00000570: 223e 3c73 7472 6f6e 673e 4368 696e 6573  "><strong>Chines
-00000580: 6520 2853 696d 706c 6966 6965 6429 3c2f  e (Simplified)</
-00000590: 7374 726f 6e67 3e3c 2f61 3e20 c2b7 0a20  strong></a> ... 
-000005a0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-000005b0: 2f2f 6769 7468 7562 2e63 6f6d 2f77 6b61  //github.com/wka
-000005c0: 6973 6572 7465 7861 732f 7469 6b74 6f6b  isertexas/tiktok
-000005d0: 2d75 706c 6f61 6465 722f 626c 6f62 2f6d  -uploader/blob/m
-000005e0: 6169 6e2f 5245 4144 4d45 2e66 722e 6d64  ain/README.fr.md
-000005f0: 223e 3c73 7472 6f6e 673e 4672 656e 6368  "><strong>French
-00000600: 3c2f 7374 726f 6e67 3e3c 2f61 3e20 c2b7  </strong></a> ..
-00000610: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
-00000620: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f77  s://github.com/w
-00000630: 6b61 6973 6572 7465 7861 732f 7469 6b74  kaisertexas/tikt
-00000640: 6f6b 2d75 706c 6f61 6465 722f 626c 6f62  ok-uploader/blob
-00000650: 2f6d 6169 6e2f 5245 4144 4d45 2e65 732e  /main/README.es.
-00000660: 6d64 223e 3c73 7472 6f6e 673e 5370 616e  md"><strong>Span
-00000670: 6973 683c 2f73 7472 696e 673e 3c2f 613e  ish</string></a>
-00000680: 20c2 b70a 2020 3c61 2068 7265 663d 2268   ...  <a href="h
-00000690: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000006a0: 6d2f 776b 6169 7365 7274 6578 6173 2f74  m/wkaisertexas/t
-000006b0: 696b 746f 6b2d 7570 6c6f 6164 6572 2f62  iktok-uploader/b
-000006c0: 6c6f 622f 6d61 696e 2f52 4541 444d 452e  lob/main/README.
-000006d0: 6465 2e6d 6422 3e3c 7374 726f 6e67 3e47  de.md"><strong>G
-000006e0: 6572 6d61 6e3c 2f73 7472 6f6e 673e 3c2f  erman</strong></
-000006f0: 613e 0a3c 2f70 3e0a 0a3c 7020 616c 6967  a>.</p>..<p alig
-00000700: 6e3d 2263 656e 7465 7222 3e0a 2020 3c69  n="center">.  <i
-00000710: 6d67 2061 6c74 3d22 466f 726b 7322 2073  mg alt="Forks" s
-00000720: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000730: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-00000740: 622f 666f 726b 732f 776b 6169 7365 7274  b/forks/wkaisert
-00000750: 6578 6173 2f74 696b 746f 6b2d 7570 6c6f  exas/tiktok-uplo
-00000760: 6164 6572 2220 2f3e 0a20 203c 696d 6720  ader" />.  <img 
-00000770: 616c 743d 2253 7461 7273 2220 7372 633d  alt="Stars" src=
-00000780: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-00000790: 656c 6473 2e69 6f2f 6769 7468 7562 2f73  elds.io/github/s
-000007a0: 7461 7273 2f77 6b61 6973 6572 7465 7861  tars/wkaisertexa
-000007b0: 732f 7469 6b74 6f6b 2d75 706c 6f61 6465  s/tiktok-uploade
-000007c0: 7222 202f 3e0a 2020 3c69 6d67 2061 6c74  r" />.  <img alt
-000007d0: 3d22 5761 7463 6865 7273 2220 7372 633d  ="Watchers" src=
-000007e0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-000007f0: 656c 6473 2e69 6f2f 6769 7468 7562 2f77  elds.io/github/w
-00000800: 6174 6368 6572 732f 776b 6169 7365 7274  atchers/wkaisert
-00000810: 6578 6173 2f74 696b 746f 6b2d 7570 6c6f  exas/tiktok-uplo
-00000820: 6164 6572 2220 2f3e 0a3c 2f70 3e0a 0a3c  ader" />.</p>..<
-00000830: 6831 3e54 6162 6c65 206f 6620 436f 6e74  h1>Table of Cont
-00000840: 656e 7473 3c2f 6831 3e0a 0a2d 205b 496e  ents</h1>..- [In
-00000850: 7374 616c 6c61 7469 6f6e 5d28 2369 6e73  stallation](#ins
-00000860: 7461 6c6c 6174 696f 6e29 0a20 202d 205b  tallation).  - [
-00000870: 4d61 634f 532c 2057 696e 646f 7773 2061  MacOS, Windows a
-00000880: 6e64 204c 696e 7578 5d28 236d 6163 6f73  nd Linux](#macos
-00000890: 2d77 696e 646f 7773 2d61 6e64 2d6c 696e  -windows-and-lin
-000008a0: 7578 290a 2020 2020 2d20 5b44 6f77 6e6c  ux).    - [Downl
-000008b0: 6f61 6469 6e67 2066 726f 6d20 5079 5049  oading from PyPI
-000008c0: 2028 5265 636f 6d6d 656e 6465 6429 5d28   (Recommended)](
-000008d0: 2370 7970 6929 0a20 2020 202d 205b 4275  #pypi).    - [Bu
-000008e0: 696c 6469 6e67 2066 726f 6d20 736f 7572  ilding from sour
-000008f0: 6365 5d28 2362 7569 6c64 696e 672d 6672  ce](#building-fr
-00000900: 6f6d 2d73 6f75 7263 6529 0a2d 205b 5573  om-source).- [Us
-00000910: 6167 655d 2823 7573 6167 6529 0a20 202d  age](#usage).  -
-00000920: 205b f09f 92bb 2043 6f6d 6d61 6e64 204c   [.... Command L
-00000930: 696e 6520 496e 7465 7266 6163 6520 2843  ine Interface (C
-00000940: 4c49 295d 2823 636c 6929 0a20 202d 205b  LI)](#cli).  - [
-00000950: e2ac 8620 5570 6c6f 6164 696e 6720 5669  ... Uploading Vi
-00000960: 6465 6f73 5d28 2375 706c 6f61 6469 6e67  deos](#uploading
-00000970: 2d76 6964 656f 7329 0a20 202d 205b f09f  -videos).  - [..
-00000980: abb5 204d 656e 7469 6f6e 7320 616e 6420  .. Mentions and 
-00000990: 4861 7368 7461 6773 5d28 236d 656e 7469  Hashtags](#menti
-000009a0: 6f6e 732d 616e 642d 6861 7368 7461 6773  ons-and-hashtags
-000009b0: 290a 2020 2d20 5bf0 9faa a120 5374 6974  ).  - [.... Stit
-000009c0: 6368 6573 2c20 4475 6574 7320 616e 6420  ches, Duets and 
-000009d0: 436f 6d6d 656e 7473 5d28 2373 7469 7463  Comments](#stitc
-000009e0: 6865 732d 6475 6574 732d 616e 642d 636f  hes-duets-and-co
-000009f0: 6d6d 656e 7473 290a 2020 2d20 5bf0 9f94  mments).  - [...
-00000a00: 9020 4175 7468 656e 7469 6361 7469 6f6e  . Authentication
-00000a10: 5d28 2361 7574 6865 6e74 6963 6174 696f  ](#authenticatio
-00000a20: 6e29 0a20 202d 205b f09f 9180 2042 726f  n).  - [.... Bro
-00000a30: 7773 6572 2053 656c 6563 7469 6f6e 5d28  wser Selection](
-00000a40: 2362 726f 7773 6572 2d73 656c 6563 7469  #browser-selecti
-00000a50: 6f6e 290a 2020 2d20 5bf0 9f9a b220 4375  on).  - [.... Cu
-00000a60: 7374 6f6d 2057 6562 4472 6976 6572 204f  stom WebDriver O
-00000a70: 7074 696f 6e73 5d28 2363 7573 746f 6d2d  ptions](#custom-
-00000a80: 7765 6264 7269 7665 7229 0a20 202d 205b  webdriver).  - [
-00000a90: f09f a4af 2048 6561 646c 6573 7320 4272  .... Headless Br
-00000aa0: 6f77 7365 7273 5d28 2368 6561 646c 6573  owsers](#headles
-00000ab0: 7329 0a20 202d 205b f09f 94a8 2049 6e69  s).  - [.... Ini
-00000ac0: 7469 616c 2053 6574 7570 5d28 2369 6e69  tial Setup](#ini
-00000ad0: 7469 616c 2d73 6574 7570 290a 2d20 5be2  tial-setup).- [.
-00000ae0: 99bb efb8 8f20 4578 616d 706c 6573 5d28  ..... Examples](
-00000af0: 2365 7861 6d70 6c65 7329 0a2d 205b f09f  #examples).- [..
-00000b00: 939d 204e 6f74 6573 5d28 236e 6f74 6573  .. Notes](#notes
-00000b10: 290a 2d20 5b41 6363 6f75 6e74 7320 6d61  ).- [Accounts ma
-00000b20: 6465 2077 6974 685d 2823 6d61 6465 2d77  de with](#made-w
-00000b30: 6974 6829 0a0a 2320 496e 7374 616c 6c61  ith)..# Installa
-00000b40: 7469 6f6e 0a0a 4120 7065 7271 7569 7369  tion..A perquisi
-00000b50: 7465 2074 6f20 7573 696e 6720 7468 6973  te to using this
-00000b60: 2070 726f 6772 616d 2069 7320 7468 6520   program is the 
-00000b70: 696e 7374 616c 6c61 7469 6f6e 206f 6620  installation of 
-00000b80: 6120 5b53 656c 656e 6975 6d2d 636f 6d70  a [Selenium-comp
-00000b90: 6174 6962 6c65 5d28 6874 7470 733a 2f2f  atible](https://
-00000ba0: 7777 772e 7365 6c65 6e69 756d 2e64 6576  www.selenium.dev
-00000bb0: 2f64 6f63 756d 656e 7461 7469 6f6e 2f77  /documentation/w
-00000bc0: 6562 6472 6976 6572 2f67 6574 7469 6e67  ebdriver/getting
-00000bd0: 5f73 7461 7274 6564 2f69 6e73 7461 6c6c  _started/install
-00000be0: 5f64 7269 7665 7273 2f29 2077 6562 2062  _drivers/) web b
-00000bf0: 726f 7773 6572 2e20 5b47 6f6f 676c 6520  rowser. [Google 
-00000c00: 4368 726f 6d65 5d28 6874 7470 733a 2f2f  Chrome](https://
-00000c10: 7777 772e 676f 6f67 6c65 2e63 6f6d 2f63  www.google.com/c
-00000c20: 6872 6f6d 652f 2920 6973 2072 6563 6f6d  hrome/) is recom
-00000c30: 6d65 6e64 6564 2e0a 0a3c 6832 2069 643d  mended...<h2 id=
-00000c40: 226d 6163 6f73 2d77 696e 646f 7773 2d61  "macos-windows-a
-00000c50: 6e64 2d6c 696e 7578 223e 4d61 634f 532c  nd-linux">MacOS,
-00000c60: 2057 696e 646f 7773 2061 6e64 204c 696e   Windows and Lin
-00000c70: 7578 3c2f 6832 3e0a 0a49 6e73 7461 6c6c  ux</h2>..Install
-00000c80: 2050 7974 686f 6e20 3320 6f72 2067 7265   Python 3 or gre
-00000c90: 6174 6572 2066 726f 6d20 5b70 7974 686f  ater from [pytho
-00000ca0: 6e2e 6f72 675d 2868 7474 7073 3a2f 2f77  n.org](https://w
-00000cb0: 7777 2e70 7974 686f 6e2e 6f72 672f 646f  ww.python.org/do
-00000cc0: 776e 6c6f 6164 732f 290a 0a3c 6833 2069  wnloads/)..<h3 i
-00000cd0: 643d 2270 7970 6922 3e44 6f77 6e6c 6f61  d="pypi">Downloa
-00000ce0: 6469 6e67 2066 726f 6d20 5079 5049 2028  ding from PyPI (
-00000cf0: 5265 636f 6d6d 656e 6465 6429 3c2f 6833  Recommended)</h3
-00000d00: 3e0a 0a49 6e73 7461 6c6c 2060 7469 6b74  >..Install `tikt
-00000d10: 6f6b 2d75 706c 6f61 6465 7260 2075 7369  ok-uploader` usi
-00000d20: 6e67 2060 7069 7060 0a0a 6060 6062 6173  ng `pip`..```bas
-00000d30: 680a 7069 7020 696e 7374 616c 6c20 7469  h.pip install ti
-00000d40: 6b74 6f6b 2d75 706c 6f61 6465 720a 6060  ktok-uploader.``
-00000d50: 600a 0a3c 6833 2069 643d 2262 7569 6c64  `..<h3 id="build
-00000d60: 696e 672d 6672 6f6d 2d73 6f75 7263 6522  ing-from-source"
-00000d70: 3e42 7569 6c64 696e 6720 6672 6f6d 2073  >Building from s
-00000d80: 6f75 7263 653c 2f68 333e 0a0a 496e 7374  ource</h3>..Inst
-00000d90: 616c 6c69 6e67 2066 726f 6d20 736f 7572  alling from sour
-00000da0: 6365 2061 6c6c 6f77 7320 6772 6561 7465  ce allows greate
-00000db0: 7220 666c 6578 6962 696c 6974 7920 746f  r flexibility to
-00000dc0: 206d 6f64 6966 7920 7468 6520 6d6f 6475   modify the modu
-00000dd0: 6c65 2773 2063 6f64 6520 746f 2065 7874  le's code to ext
-00000de0: 656e 6420 6465 6661 756c 7420 6265 6861  end default beha
-00000df0: 7669 6f72 2e0a 0a46 6972 7374 2c20 6063  vior...First, `c
-00000e00: 6c6f 6e65 6020 616e 6420 6d6f 7665 2069  lone` and move i
-00000e10: 6e74 6f20 7468 6520 7265 706f 7369 746f  nto the reposito
-00000e20: 7279 2e20 4e65 7874 2c20 696e 7374 616c  ry. Next, instal
-00000e30: 6c20 6068 6174 6368 602c 2074 6865 2062  l `hatch`, the b
-00000e40: 7569 6c64 2074 6f6f 6c20 7573 6564 2066  uild tool used f
-00000e50: 6f72 2074 6869 7320 7072 6f6a 6563 7420  or this project 
-00000e60: 5b5e 315d 2e20 5468 656e 2c20 6062 7569  [^1]. Then, `bui
-00000e70: 6c64 6020 7468 6520 7072 6f6a 6563 742e  ld` the project.
-00000e80: 2046 696e 616c 6c79 2c20 6069 6e73 7461   Finally, `insta
-00000e90: 6c6c 6020 7468 6520 7072 6f6a 6563 7420  ll` the project 
-00000ea0: 7769 7468 2074 6865 2060 2d65 6020 6f72  with the `-e` or
-00000eb0: 2065 6469 7461 626c 6520 666c 6167 2e0a   editable flag..
-00000ec0: 0a60 6060 636f 6e73 6f6c 650a 6769 7420  .```console.git 
-00000ed0: 636c 6f6e 6520 6874 7470 733a 2f2f 6769  clone https://gi
-00000ee0: 7468 7562 2e63 6f6d 2f77 6b61 6973 6572  thub.com/wkaiser
-00000ef0: 7465 7861 732f 7469 6b74 6f6b 2d75 706c  texas/tiktok-upl
-00000f00: 6f61 6465 722e 6769 740a 6364 2074 696b  oader.git.cd tik
-00000f10: 746f 6b2d 7570 6c6f 6164 6572 0a70 6970  tok-uploader.pip
-00000f20: 2069 6e73 7461 6c6c 2068 6174 6368 0a68   install hatch.h
-00000f30: 6174 6368 2062 7569 6c64 0a70 6970 2069  atch build.pip i
-00000f40: 6e73 7461 6c6c 202d 6520 2e0a 6060 600a  nstall -e ..```.
-00000f50: 0a3c 6831 2069 643d 2275 7361 6765 223e  .<h1 id="usage">
-00000f60: 5573 6167 653c 2f68 313e 0a0a 6074 696b  Usage</h1>..`tik
-00000f70: 746f 6b2d 7570 6c6f 6164 6572 6020 776f  tok-uploader` wo
-00000f80: 726b 7320 6279 2064 7570 6c69 6361 7469  rks by duplicati
-00000f90: 6e67 2079 6f75 7220 6272 6f77 7365 7227  ng your browser'
-00000fa0: 7320 2a2a 636f 6f6b 6965 732a 2a20 7768  s **cookies** wh
-00000fb0: 6963 6820 7472 6963 6b73 202a 2a54 696b  ich tricks **Tik
-00000fc0: 546f 6b2a 2a20 696e 746f 2062 656c 6965  Tok** into belie
-00000fd0: 7669 6e67 2079 6f75 2061 7265 206c 6f67  ving you are log
-00000fe0: 6765 6420 696e 206f 6e20 6120 7265 6d6f  ged in on a remo
-00000ff0: 7465 2d63 6f6e 7472 6f6c 6c65 6420 6272  te-controlled br
-00001000: 6f77 7365 722e 0a0a 3c68 3220 6964 3d22  owser...<h2 id="
-00001010: 636c 6922 3e20 f09f 92bb 2043 6f6d 6d61  cli"> .... Comma
-00001020: 6e64 204c 696e 6520 496e 7465 7266 6163  nd Line Interfac
-00001030: 6520 2843 4c49 293c 2f68 323e 0a0a 5573  e (CLI)</h2>..Us
-00001040: 696e 6720 7468 6520 434c 4920 6973 2061  ing the CLI is a
-00001050: 7320 7369 6d70 6c65 2061 7320 6361 6c6c  s simple as call
-00001060: 696e 6720 6074 696b 746f 6b2d 7570 6c6f  ing `tiktok-uplo
-00001070: 6164 6572 6020 7769 7468 2079 6f75 7220  ader` with your 
-00001080: 7669 6465 6f73 3a20 6070 6174 6860 2028  videos: `path` (
-00001090: 2d76 292c 2060 6465 7363 7269 7074 696f  -v), `descriptio
-000010a0: 6e60 282d 6429 2061 6e64 2060 636f 6f6b  n`(-d) and `cook
-000010b0: 6965 7360 2028 2d63 290a 0a60 6060 6261  ies` (-c)..```ba
-000010c0: 7368 0a74 696b 746f 6b2d 7570 6c6f 6164  sh.tiktok-upload
-000010d0: 6572 202d 7620 7669 6465 6f2e 6d70 3420  er -v video.mp4 
-000010e0: 2d64 2022 7468 6973 2069 7320 6d79 2065  -d "this is my e
-000010f0: 7363 6170 6564 205c 2264 6573 6372 6970  scaped \"descrip
-00001100: 7469 6f6e 5c22 2220 2d63 2063 6f6f 6b69  tion\"" -c cooki
-00001110: 6573 2e74 7874 0a60 6060 0a0a 6060 6070  es.txt.```..```p
-00001120: 7974 686f 6e0a 6672 6f6d 2074 696b 746f  ython.from tikto
-00001130: 6b5f 7570 6c6f 6164 6572 2e75 706c 6f61  k_uploader.uploa
-00001140: 6420 696d 706f 7274 2075 706c 6f61 645f  d import upload_
-00001150: 7669 6465 6f2c 2075 706c 6f61 645f 7669  video, upload_vi
-00001160: 6465 6f73 0a66 726f 6d20 7469 6b74 6f6b  deos.from tiktok
-00001170: 5f75 706c 6f61 6465 722e 6175 7468 2069  _uploader.auth i
-00001180: 6d70 6f72 7420 4175 7468 4261 636b 656e  mport AuthBacken
-00001190: 640a 0a23 2073 696e 676c 6520 7669 6465  d..# single vide
-000011a0: 6f0a 7570 6c6f 6164 5f76 6964 656f 2827  o.upload_video('
-000011b0: 7669 6465 6f2e 6d70 3427 2c0a 2020 2020  video.mp4',.    
-000011c0: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-000011d0: 696f 6e3d 2774 6869 7320 6973 206d 7920  ion='this is my 
-000011e0: 6465 7363 7269 7074 696f 6e27 2c0a 2020  description',.  
-000011f0: 2020 2020 2020 2020 2020 636f 6f6b 6965            cookie
-00001200: 733d 2763 6f6f 6b69 6573 2e74 7874 2729  s='cookies.txt')
-00001210: 0a0a 2320 4d75 6c74 6970 6c65 2056 6964  ..# Multiple Vid
-00001220: 656f 730a 7669 6465 6f73 203d 205b 0a20  eos.videos = [. 
-00001230: 2020 207b 0a20 2020 2020 2020 2027 7061     {.        'pa
-00001240: 7468 273a 2027 7669 6465 6f2e 6d70 3427  th': 'video.mp4'
-00001250: 2c0a 2020 2020 2020 2020 2764 6573 6372  ,.        'descr
-00001260: 6970 7469 6f6e 273a 2027 7468 6973 2069  iption': 'this i
-00001270: 7320 6d79 2064 6573 6372 6970 7469 6f6e  s my description
-00001280: 270a 2020 2020 7d2c 0a20 2020 207b 0a20  '.    },.    {. 
-00001290: 2020 2020 2020 2027 7061 7468 273a 2027         'path': '
-000012a0: 7669 6465 6f32 2e6d 7034 272c 0a20 2020  video2.mp4',.   
-000012b0: 2020 2020 2027 6465 7363 7269 7074 696f       'descriptio
-000012c0: 6e27 3a20 2774 6869 7320 6973 2061 6c73  n': 'this is als
-000012d0: 6f20 6d79 2064 6573 6372 6970 7469 6f6e  o my description
-000012e0: 270a 2020 2020 7d0a 5d0a 0a61 7574 6820  '.    }.]..auth 
-000012f0: 3d20 4175 7468 4261 636b 656e 6428 636f  = AuthBackend(co
-00001300: 6f6b 6965 733d 2763 6f6f 6b69 6573 2e74  okies='cookies.t
-00001310: 7874 2729 0a75 706c 6f61 645f 7669 6465  xt').upload_vide
-00001320: 6f73 2876 6964 656f 733d 7669 6465 6f73  os(videos=videos
-00001330: 2c20 6175 7468 3d61 7574 6829 0a60 6060  , auth=auth).```
-00001340: 0a0a 3c68 3220 6964 3d22 7570 6c6f 6164  ..<h2 id="upload
-00001350: 696e 672d 7669 6465 6f73 223e 20e2 ac86  ing-videos"> ...
-00001360: 2055 706c 6f61 6469 6e67 2056 6964 656f   Uploading Video
-00001370: 733c 2f68 323e 0a0a 5468 6973 206c 6962  s</h2>..This lib
-00001380: 7261 7279 2072 6576 6f6c 7665 7320 6172  rary revolves ar
-00001390: 6f75 6e64 2074 6865 2060 7570 6c6f 6164  ound the `upload
-000013a0: 5f76 6964 656f 7360 2066 756e 6374 696f  _videos` functio
-000013b0: 6e20 7768 6963 6820 7461 6b65 7320 696e  n which takes in
-000013c0: 2061 206c 6973 7420 6f66 2076 6964 656f   a list of video
-000013d0: 7320 7768 6963 6820 6861 7665 202a 2a66  s which have **f
-000013e0: 696c 656e 616d 6573 2a2a 2061 6e64 202a  ilenames** and *
-000013f0: 2a64 6573 6372 6970 7469 6f6e 732a 2a20  *descriptions** 
-00001400: 616e 6420 6172 6520 7061 7373 6564 2061  and are passed a
-00001410: 7320 666f 6c6c 6f77 733a 0a0a 6060 6070  s follows:..```p
-00001420: 7974 686f 6e0a 6672 6f6d 2074 696b 746f  ython.from tikto
-00001430: 6b5f 7570 6c6f 6164 6572 2e75 706c 6f61  k_uploader.uploa
-00001440: 6420 696d 706f 7274 2075 706c 6f61 645f  d import upload_
-00001450: 7669 6465 6f73 0a66 726f 6d20 7469 6b74  videos.from tikt
-00001460: 6f6b 5f75 706c 6f61 6465 722e 6175 7468  ok_uploader.auth
-00001470: 2069 6d70 6f72 7420 4175 7468 4261 636b   import AuthBack
-00001480: 656e 640a 0a76 6964 656f 7320 3d20 5b0a  end..videos = [.
-00001490: 2020 2020 7b0a 2020 2020 2020 2020 2776      {.        'v
-000014a0: 6964 656f 273a 2027 7669 6465 6f30 2e6d  ideo': 'video0.m
-000014b0: 7034 272c 0a20 2020 2020 2020 2027 6465  p4',.        'de
-000014c0: 7363 7269 7074 696f 6e27 3a20 2756 6964  scription': 'Vid
-000014d0: 656f 2031 2069 7320 6162 6f75 7420 2e2e  eo 1 is about ..
-000014e0: 2e27 0a20 2020 207d 2c0a 2020 2020 7b0a  .'.    },.    {.
-000014f0: 2020 2020 2020 2020 2776 6964 656f 273a          'video':
-00001500: 2027 7669 6465 6f31 2e6d 7034 272c 0a20   'video1.mp4',. 
-00001510: 2020 2020 2020 2027 6465 7363 7269 7074         'descript
-00001520: 696f 6e27 3a20 2756 6964 656f 2032 2069  ion': 'Video 2 i
-00001530: 7320 6162 6f75 7420 2e2e 2e27 0a20 2020  s about ...'.   
-00001540: 207d 0a5d 0a0a 6175 7468 203d 2041 7574   }.]..auth = Aut
-00001550: 6842 6163 6b65 6e64 2863 6f6f 6b69 6573  hBackend(cookies
-00001560: 3d27 636f 6f6b 6965 732e 7478 7427 290a  ='cookies.txt').
-00001570: 6661 696c 6564 5f76 6964 656f 7320 3d20  failed_videos = 
-00001580: 7570 6c6f 6164 5f76 6964 656f 7328 7669  upload_videos(vi
-00001590: 6465 6f73 3d76 6964 656f 732c 2061 7574  deos=videos, aut
-000015a0: 683d 6175 7468 290a 0a66 6f72 2076 6964  h=auth)..for vid
-000015b0: 656f 2069 6e20 6661 696c 6564 5f76 6964  eo in failed_vid
-000015c0: 656f 733a 2023 2065 6163 6820 696e 7075  eos: # each inpu
-000015d0: 7420 7669 6465 6f20 6f62 6a65 6374 2077  t video object w
-000015e0: 6869 6368 2066 6169 6c65 640a 2020 2020  hich failed.    
-000015f0: 7072 696e 7428 6627 7b76 6964 656f 5b27  print(f'{video['
-00001600: 7669 6465 6f27 5d7d 2077 6974 6820 6465  video']} with de
-00001610: 7363 7269 7074 696f 6e20 227b 7669 6465  scription "{vide
-00001620: 6f5b 2764 6573 6372 6970 7469 6f6e 275d  o['description']
-00001630: 7d22 2066 6169 6c65 6427 290a 6060 600a  }" failed').```.
-00001640: 0a3c 6832 2069 643d 226d 656e 7469 6f6e  .<h2 id="mention
-00001650: 732d 616e 642d 6861 7368 7461 6773 223e  s-and-hashtags">
-00001660: 20f0 9fab b520 4d65 6e74 696f 6e73 2061   .... Mentions a
-00001670: 6e64 2048 6173 6874 6167 733c 2f68 323e  nd Hashtags</h2>
-00001680: 0a0a 4d65 6e74 696f 6e73 2061 6e64 2048  ..Mentions and H
-00001690: 6173 6874 6167 7320 6e6f 7720 776f 726b  ashtags now work
-000016a0: 2073 6f20 6c6f 6e67 2061 7320 7468 6579   so long as they
-000016b0: 2061 7265 2066 6f6c 6c6f 7765 6420 6279   are followed by
-000016c0: 2061 2073 7061 6365 2e20 486f 7765 7665   a space. Howeve
-000016d0: 722c 2079 6f75 2061 7320 7468 6520 7573  r, you as the us
-000016e0: 6572 2061 7265 2072 6573 706f 6e73 6962  er are responsib
-000016f0: 6c65 2066 6f72 2076 6572 6966 7969 6e67  le for verifying
-00001700: 2061 206d 656e 7469 6f6e 206f 7220 6861   a mention or ha
-00001710: 7368 7461 6720 6578 6973 7473 2062 6566  shtag exists bef
-00001720: 6f72 6520 706f 7374 696e 670a 0a2a 2a45  ore posting..**E
-00001730: 7861 6d70 6c65 3a2a 2a0a 0a60 6060 7079  xample:**..```py
-00001740: 7468 6f6e 0a66 726f 6d20 7469 6b74 6f6b  thon.from tiktok
-00001750: 5f75 706c 6f61 6465 722e 7570 6c6f 6164  _uploader.upload
-00001760: 2069 6d70 6f72 7420 7570 6c6f 6164 5f76   import upload_v
-00001770: 6964 656f 0a0a 7570 6c6f 6164 5f76 6964  ideo..upload_vid
-00001780: 656f 2827 7669 6465 6f2e 6d70 3427 2c20  eo('video.mp4', 
-00001790: 2723 6679 7020 4069 6365 7370 6963 6565  '#fyp @icespicee
-000017a0: 272c 2027 636f 6f6b 6965 732e 7478 7427  ', 'cookies.txt'
-000017b0: 290a 6060 600a 0a3c 6832 2069 643d 2273  ).```..<h2 id="s
-000017c0: 7469 7463 6865 732d 6475 6574 732d 616e  titches-duets-an
-000017d0: 642d 636f 6d6d 656e 7473 223e 20f0 9faa  d-comments"> ...
-000017e0: a120 5374 6974 6368 6573 2c20 4475 6574  . Stitches, Duet
-000017f0: 7320 616e 6420 436f 6d6d 656e 7473 3c2f  s and Comments</
-00001800: 6832 3e0a 0a54 6f20 7365 7420 7768 6574  h2>..To set whet
-00001810: 6865 7220 6f72 206e 6f74 2061 2076 6964  her or not a vid
-00001820: 656f 2075 706c 6f61 6465 6420 616c 6c6f  eo uploaded allo
-00001830: 7773 2073 7469 7463 6865 732c 2063 6f6d  ws stitches, com
-00001840: 6d65 6e74 7320 6f72 2064 7565 742c 2073  ments or duet, s
-00001850: 696d 706c 7920 7370 6563 6966 7920 6063  imply specify `c
-00001860: 6f6d 6d65 6e74 602c 2060 7374 6974 6368  omment`, `stitch
-00001870: 6020 616e 642f 6f72 2060 6475 6574 6020  ` and/or `duet` 
-00001880: 6173 206b 6579 776f 7264 2061 7267 756d  as keyword argum
-00001890: 656e 7473 2074 6f20 6075 706c 6f61 645f  ents to `upload_
-000018a0: 7669 6465 6f60 206f 7220 6075 706c 6f61  video` or `uploa
-000018b0: 645f 7669 6465 6f73 602e 0a0a 6060 6070  d_videos`...```p
-000018c0: 7974 686f 6e0a 7570 6c6f 6164 5f76 6964  ython.upload_vid
-000018d0: 656f 282e 2e2e 2c20 636f 6d6d 656e 743d  eo(..., comment=
-000018e0: 5472 7565 2c20 7374 6974 6368 3d54 7275  True, stitch=Tru
-000018f0: 652c 2064 7565 743d 5472 7565 290a 6060  e, duet=True).``
-00001900: 600a 0a3e 2043 6f6d 6d65 6e74 732c 2053  `..> Comments, S
-00001910: 7469 7463 6865 7320 616e 6420 4475 6574  titches and Duet
-00001920: 7320 6172 6520 616c 6c6f 7765 6420 6279  s are allowed by
-00001930: 202a 2a64 6566 6175 6c74 2a2a 0a0a 3c68   **default**..<h
-00001940: 3220 6964 3d22 7072 6f78 7922 3e20 f09f  2 id="proxy"> ..
-00001950: 8c90 2050 726f 7879 3c2f 6832 3e0a 0a54  .. Proxy</h2>..T
-00001960: 6f20 7365 7420 6120 7072 6f78 792c 2063  o set a proxy, c
-00001970: 7572 7265 6e74 6c79 206f 6e6c 7920 776f  urrently only wo
-00001980: 726b 7320 7769 7468 2063 6872 6f6d 6520  rks with chrome 
-00001990: 6173 2074 6865 2062 726f 7773 6572 2c20  as the browser, 
-000019a0: 616c 6c6f 7720 7573 6572 3a70 6173 7320  allow user:pass 
-000019b0: 6175 7468 2e0a 0a60 6060 7079 7468 6f6e  auth...```python
-000019c0: 0a23 2070 726f 7879 203d 207b 2775 7365  .# proxy = {'use
-000019d0: 7227 3a20 276d 7975 7365 7227 2c20 2770  r': 'myuser', 'p
-000019e0: 6173 7327 3a20 276d 7970 6173 7327 2c20  ass': 'mypass', 
-000019f0: 2768 6f73 7427 3a20 2731 3131 2e31 3131  'host': '111.111
-00001a00: 2e31 3131 272c 2027 706f 7274 273a 2027  .111', 'port': '
-00001a10: 3939 277d 2020 2320 7573 6572 3a70 6173  99'}  # user:pas
-00001a20: 730a 7072 6f78 7920 3d20 7b27 686f 7374  s.proxy = {'host
-00001a30: 273a 2027 3131 312e 3131 312e 3131 3127  ': '111.111.111'
-00001a40: 2c20 2770 6f72 7427 3a20 2739 3927 7d0a  , 'port': '99'}.
-00001a50: 7570 6c6f 6164 5f76 6964 656f 282e 2e2e  upload_video(...
-00001a60: 2c20 7072 6f78 793d 7072 6f78 7929 0a60  , proxy=proxy).`
-00001a70: 6060 0a0a 3c68 3220 6964 3d22 7363 6865  ``..<h2 id="sche
-00001a80: 6475 6c65 223e 20f0 9f93 8620 5363 6865  dule"> .... Sche
-00001a90: 6475 6c65 3c2f 6832 3e0a 0a54 6865 2064  dule</h2>..The d
-00001aa0: 6174 6574 696d 6520 746f 2073 6368 6564  atetime to sched
-00001ab0: 756c 6520 7468 6520 7669 6465 6f20 7769  ule the video wi
-00001ac0: 6c6c 2062 6520 7472 6561 7465 6420 7769  ll be treated wi
-00001ad0: 7468 2074 6865 2055 5443 2074 696d 657a  th the UTC timez
-00001ae0: 6f6e 652e 203c 6272 3e0a 5468 6520 7363  one. <br>.The sc
-00001af0: 6865 6475 6c65 6420 6461 7465 7469 6d65  heduled datetime
-00001b00: 206d 7573 7420 6265 2061 7420 6c65 6173   must be at leas
-00001b10: 7420 3230 206d 696e 7574 6573 2069 6e20  t 20 minutes in 
-00001b20: 7468 6520 6675 7475 7265 2061 6e64 2061  the future and a
-00001b30: 206d 6178 696d 756d 206f 6620 3130 2064   maximum of 10 d
-00001b40: 6179 732e 0a0a 6060 6070 7974 686f 6e0a  ays...```python.
-00001b50: 696d 706f 7274 2064 6174 6574 696d 650a  import datetime.
-00001b60: 7363 6865 6475 6c65 203d 2064 6174 6574  schedule = datet
-00001b70: 696d 652e 6461 7465 7469 6d65 2832 3032  ime.datetime(202
-00001b80: 302c 2031 322c 2032 302c 2031 332c 2030  0, 12, 20, 13, 0
-00001b90: 3029 0a75 706c 6f61 645f 7669 6465 6f28  0).upload_video(
-00001ba0: 2e2e 2e2c 2073 6368 6564 756c 653d 7363  ..., schedule=sc
-00001bb0: 6865 6475 6c65 290a 6060 600a 0a3c 6832  hedule).```..<h2
-00001bc0: 2069 643d 2261 7574 6865 6e74 6963 6174   id="authenticat
-00001bd0: 696f 6e22 3e20 f09f 9490 2041 7574 6865  ion"> .... Authe
-00001be0: 6e74 6963 6174 696f 6e3c 2f68 323e 0a0a  ntication</h2>..
-00001bf0: 4175 7468 656e 7469 6361 7469 6f6e 2075  Authentication u
-00001c00: 7365 7320 796f 7572 2062 726f 7773 6572  ses your browser
-00001c10: 2773 2063 6f6f 6b69 6573 2e20 5468 6973  's cookies. This
-00001c20: 2077 6f72 6b61 726f 756e 6420 7761 7320   workaround was 
-00001c30: 646f 6e65 2064 7565 2074 6f20 5469 6b54  done due to TikT
-00001c40: 6f6b 2773 2073 7472 6963 7465 7220 7374  ok's stricter st
-00001c50: 616e 6365 206f 6e20 6175 7468 656e 7469  ance on authenti
-00001c60: 6361 7469 6f6e 2062 7920 6120 5365 6c65  cation by a Sele
-00001c70: 6e69 756d 2d63 6f6e 7472 6f6c 6c65 6420  nium-controlled 
-00001c80: 6272 6f77 7365 722e 0a0a 596f 7572 2060  browser...Your `
-00001c90: 7365 7373 696f 6e69 6460 2069 7320 616c  sessionid` is al
-00001ca0: 6c20 7468 6174 2069 7320 7265 7175 6972  l that is requir
-00001cb0: 6564 2066 6f72 2061 7574 6865 6e74 6963  ed for authentic
-00001cc0: 6174 696f 6e20 616e 6420 6361 6e20 6265  ation and can be
-00001cd0: 2070 6173 7365 6420 6173 2061 6e20 6172   passed as an ar
-00001ce0: 6775 6d65 6e74 2074 6f20 6e65 6172 6c79  gument to nearly
-00001cf0: 2061 6e79 2066 756e 6374 696f 6e0a 0a5b   any function..[
-00001d00: f09f 8daa 2047 6574 2063 6f6f 6b69 6573  .... Get cookies
-00001d10: 2e74 7874 5d28 6874 7470 733a 2f2f 6769  .txt](https://gi
-00001d20: 7468 7562 2e63 6f6d 2f6b 6169 7269 3030  thub.com/kairi00
-00001d30: 332f 4765 742d 636f 6f6b 6965 732e 7478  3/Get-cookies.tx
-00001d40: 742d 4c4f 4341 4c4c 5929 206d 616b 6573  t-LOCALLY) makes
-00001d50: 2067 6574 7469 6e67 2063 6f6f 6b69 6573   getting cookies
-00001d60: 2069 6e20 6120 5b4e 6574 5363 6170 6520   in a [NetScape 
-00001d70: 636f 6f6b 6965 7320 666f 726d 6174 5d28  cookies format](
-00001d80: 6874 7470 3a2f 2f66 696c 6566 6f72 6d61  http://fileforma
-00001d90: 7473 2e61 7263 6869 7665 7465 616d 2e6f  ts.archiveteam.o
-00001da0: 7267 2f77 696b 692f 4e65 7473 6361 7065  rg/wiki/Netscape
-00001db0: 5f63 6f6f 6b69 6573 2e74 7874 292e 0a0a  _cookies.txt)...
-00001dc0: 4166 7465 7220 696e 7374 616c 6c69 6e67  After installing
-00001dd0: 2c20 6f70 656e 2074 6865 2065 7874 656e  , open the exten
-00001de0: 7369 6f6e 7320 6d65 6e75 206f 6e20 5b54  sions menu on [T
-00001df0: 696b 546f 6b2e 636f 6d5d 2868 7474 7073  ikTok.com](https
-00001e00: 3a2f 2f74 696b 746f 6b2e 636f 6d2f 2920  ://tiktok.com/) 
-00001e10: 616e 6420 636c 6963 6b20 60f0 9f8d aa20  and click `.... 
-00001e20: 4765 7420 636f 6f6b 6965 732e 7478 7460  Get cookies.txt`
-00001e30: 2074 6f20 7265 7665 616c 2079 6f75 7220   to reveal your 
-00001e40: 636f 6f6b 6965 732e 2053 656c 6563 7420  cookies. Select 
-00001e50: 6045 7870 6f72 7420 4173 20e2 87a9 6020  `Export As ...` 
-00001e60: 616e 6420 7370 6563 6966 7920 6120 6c6f  and specify a lo
-00001e70: 6361 7469 6f6e 2061 6e64 206e 616d 6520  cation and name 
-00001e80: 746f 2073 6176 652e 0a0a 6060 6070 7974  to save...```pyt
-00001e90: 686f 6e0a 7570 6c6f 6164 5f76 6964 656f  hon.upload_video
-00001ea0: 282e 2e2e 2c20 636f 6f6b 6965 733d 2763  (..., cookies='c
-00001eb0: 6f6f 6b69 6573 2e74 7874 2729 0a60 6060  ookies.txt').```
-00001ec0: 0a0a 2a2a 4f70 7469 6f6e 616c 6c79 2a2a  ..**Optionally**
-00001ed0: 2c20 6063 6f6f 6b69 6573 5f6c 6973 7460  , `cookies_list`
-00001ee0: 2069 7320 6120 6c69 7374 206f 6620 6469   is a list of di
-00001ef0: 6374 696f 6e61 7269 6573 2077 6974 6820  ctionaries with 
-00001f00: 6b65 7973 2060 6e61 6d65 602c 2060 7661  keys `name`, `va
-00001f10: 6c75 6560 2c20 6064 6f6d 6169 6e60 2c20  lue`, `domain`, 
-00001f20: 6070 6174 6860 2061 6e64 2060 6578 7069  `path` and `expi
-00001f30: 7279 6020 7768 6963 6820 616c 6c6f 7720  ry` which allow 
-00001f40: 796f 7520 746f 2070 6173 7320 796f 7572  you to pass your
-00001f50: 206f 776e 2062 726f 7773 6572 2063 6f6f   own browser coo
-00001f60: 6b69 6573 2e0a 0a2a 2a45 7861 6d70 6c65  kies...**Example
-00001f70: 3a2a 2a0a 0a60 6060 7079 7468 6f6e 0a63  :**..```python.c
-00001f80: 6f6f 6b69 6573 5f6c 6973 7420 3d20 5b0a  ookies_list = [.
-00001f90: 2020 2020 7b0a 2020 2020 2020 2020 276e      {.        'n
-00001fa0: 616d 6527 3a20 2773 6573 7369 6f6e 6964  ame': 'sessionid
-00001fb0: 272c 0a20 2020 2020 2020 2027 7661 6c75  ',.        'valu
-00001fc0: 6527 3a20 272a 2a79 6f75 7220 7365 7373  e': '**your sess
-00001fd0: 696f 6e20 6964 2a2a 272c 0a20 2020 2020  ion id**',.     
-00001fe0: 2020 2027 646f 6d61 696e 273a 2027 6874     'domain': 'ht
-00001ff0: 7470 733a 2f2f 7469 6b74 6f6b 2e63 6f6d  tps://tiktok.com
-00002000: 272c 0a20 2020 2020 2020 2027 7061 7468  ',.        'path
-00002010: 273a 2027 2f27 2c0a 2020 2020 2020 2020  ': '/',.        
-00002020: 2765 7870 6972 7927 3a20 2731 302f 382f  'expiry': '10/8/
-00002030: 3230 3233 2c20 3132 3a31 383a 3538 2050  2023, 12:18:58 P
-00002040: 4d27 0a20 2020 207d 2c0a 2020 2020 2320  M'.    },.    # 
-00002050: 7468 6520 7265 7374 206f 6620 796f 7572  the rest of your
-00002060: 2063 6f6f 6b69 6573 2061 6c6c 2069 6e20   cookies all in 
-00002070: 6120 6c69 7374 0a5d 0a0a 7570 6c6f 6164  a list.]..upload
-00002080: 5f76 6964 656f 282e 2e2e 2c20 636f 6f6b  _video(..., cook
-00002090: 6965 735f 6c69 7374 3d63 6f6f 6b69 6573  ies_list=cookies
-000020a0: 5f6c 6973 7429 0a60 6060 0a0a 3c68 3220  _list).```..<h2 
-000020b0: 6964 3d22 6272 6f77 7365 722d 7365 6c65  id="browser-sele
-000020c0: 6374 696f 6e22 3e20 f09f 9180 2042 726f  ction"> .... Bro
-000020d0: 7773 6572 2053 656c 6563 7469 6f6e 3c2f  wser Selection</
-000020e0: 6832 3e0a 0a5b 476f 6f67 6c65 2043 6872  h2>..[Google Chr
-000020f0: 6f6d 655d 2868 7474 7073 3a2f 2f77 7777  ome](https://www
-00002100: 2e67 6f6f 676c 652e 636f 6d2f 6368 726f  .google.com/chro
-00002110: 6d65 2920 6973 2074 6865 2070 7265 6665  me) is the prefe
-00002120: 7272 6564 2062 726f 7773 6572 2066 6f72  rred browser for
-00002130: 202a 2a54 696b 546f 6b55 706c 6f61 6465   **TikTokUploade
-00002140: 722a 2a2e 2054 6865 2064 6566 6175 6c74  r**. The default
-00002150: 2061 6e74 692d 6465 7465 6374 696f 6e20   anti-detection 
-00002160: 7465 6368 6e69 7175 6573 2075 7365 6420  techniques used 
-00002170: 696e 2074 6869 7320 7061 636b 6167 6564  in this packaged
-00002180: 2061 7265 206f 7074 696d 697a 6564 2066   are optimized f
-00002190: 6f72 2074 6869 732e 2048 6f77 6576 6572  or this. However
-000021a0: 2c20 6966 2079 6f75 2077 6973 6820 746f  , if you wish to
-000021b0: 2075 7365 2061 2064 6966 6665 7265 6e74   use a different
-000021c0: 2062 726f 7773 6572 2079 6f75 206d 6179   browser you may
-000021d0: 2073 7065 6369 6679 2074 6865 2060 6272   specify the `br
-000021e0: 6f77 7365 7260 2069 6e20 6075 706c 6f61  owser` in `uploa
-000021f0: 645f 7669 6465 6f60 206f 7220 6075 706c  d_video` or `upl
-00002200: 6f61 645f 7669 6465 6f73 602e 0a0a 6060  oad_videos`...``
-00002210: 6070 7974 686f 6e0a 6672 6f6d 2074 696b  `python.from tik
-00002220: 746f 6b5f 7570 6c6f 6164 6572 2e75 706c  tok_uploader.upl
-00002230: 6f61 6420 696d 706f 7274 2075 706c 6f61  oad import uploa
-00002240: 645f 7669 6465 6f0a 0a66 726f 6d20 7261  d_video..from ra
-00002250: 6e64 6f6d 2069 6d70 6f72 7420 6368 6f69  ndom import choi
-00002260: 6365 0a0a 4252 4f57 5345 5253 203d 205b  ce..BROWSERS = [
-00002270: 0a20 2020 2027 6368 726f 6d65 272c 0a20  .    'chrome',. 
-00002280: 2020 2027 7361 6661 7269 272c 0a20 2020     'safari',.   
-00002290: 2027 6368 726f 6d69 756d 272c 0a20 2020   'chromium',.   
-000022a0: 2027 6564 6765 272c 0a20 2020 2027 6669   'edge',.    'fi
-000022b0: 7265 666f 7827 0a5d 0a0a 2320 7261 6e64  refox'.]..# rand
-000022c0: 6f6d 6c79 2070 6963 6b73 2061 2077 6562  omly picks a web
-000022d0: 2062 726f 7773 6572 0a75 706c 6f61 645f   browser.upload_
-000022e0: 7669 6465 6f28 2e2e 2e2c 2062 726f 7773  video(..., brows
-000022f0: 6572 3d63 686f 6963 6528 4252 4f57 5345  er=choice(BROWSE
-00002300: 5253 2929 0a60 6060 0a0a e29c 8520 5375  RS)).```..... Su
-00002310: 7070 6f72 7465 6420 4272 6f77 7365 7273  pported Browsers
-00002320: 3a0a 0a2d 202a 2a43 6872 6f6d 652a 2a20  :..- **Chrome** 
-00002330: 2852 6563 6f6d 6d65 6e64 6564 290a 2d20  (Recommended).- 
-00002340: 2a2a 5361 6661 7269 2a2a 0a2d 202a 2a43  **Safari**.- **C
-00002350: 6872 6f6d 6975 6d2a 2a0a 2d20 2a2a 4564  hromium**.- **Ed
-00002360: 6765 2a2a 0a2d 202a 2a46 6972 6546 6f78  ge**.- **FireFox
-00002370: 2a2a 0a0a 3c68 3220 6964 3d22 6375 7374  **..<h2 id="cust
-00002380: 6f6d 2d77 6562 6472 6976 6572 223e 20f0  om-webdriver"> .
-00002390: 9f9a b220 4375 7374 6f6d 2057 6562 4472  ... Custom WebDr
-000023a0: 6976 6572 204f 7074 696f 6e73 3c2f 6832  iver Options</h2
-000023b0: 3e0a 0a44 6566 6175 6c74 206d 6f64 6966  >..Default modif
-000023c0: 6963 6174 696f 6e73 2074 6f20 5365 6c65  ications to Sele
-000023d0: 6e69 756d 2061 7265 2061 7070 6c69 6564  nium are applied
-000023e0: 2077 6869 6368 2068 656c 7020 6974 2061   which help it a
-000023f0: 766f 6964 2062 6569 6e67 2064 6574 6563  void being detec
-00002400: 7465 6420 6279 2054 696b 546f 6b2e 0a0a  ted by TikTok...
-00002410: 486f 7765 7665 722c 2079 6f75 202a 2a6d  However, you **m
-00002420: 6179 2a2a 2070 6173 7320 6120 6375 7374  ay** pass a cust
-00002430: 6f6d 2064 7269 7665 7220 636f 6e66 6967  om driver config
-00002440: 7572 6174 696f 6e20 6f70 7469 6f6e 732e  uration options.
-00002450: 2053 696d 706c 7920 7061 7373 2060 6f70   Simply pass `op
-00002460: 7469 6f6e 7360 2061 7320 6120 6b65 7977  tions` as a keyw
-00002470: 6f72 6420 6172 6775 6d65 6e74 2074 6f20  ord argument to 
-00002480: 6569 7468 6572 2060 7570 6c6f 6164 5f76  either `upload_v
-00002490: 6964 656f 6020 6f72 2060 7570 6c6f 6164  ideo` or `upload
-000024a0: 5f76 6964 656f 7360 2e0a 0a60 6060 7079  _videos`...```py
-000024b0: 7468 6f6e 0a66 726f 6d20 7365 6c65 6e69  thon.from seleni
-000024c0: 756d 2e77 6562 6472 6976 6572 2e63 6872  um.webdriver.chr
-000024d0: 6f6d 652e 6f70 7469 6f6e 7320 696d 706f  ome.options impo
-000024e0: 7274 204f 7074 696f 6e73 0a0a 6f70 7469  rt Options..opti
-000024f0: 6f6e 7320 3d20 4f70 7469 6f6e 7328 290a  ons = Options().
-00002500: 0a6f 7074 696f 6e73 2e61 6464 5f61 7267  .options.add_arg
-00002510: 756d 656e 7428 2773 7461 7274 2d6d 6178  ument('start-max
-00002520: 696d 697a 6564 2729 0a0a 7570 6c6f 6164  imized')..upload
-00002530: 5f76 6964 656f 7328 2e2e 2e2c 206f 7074  _videos(..., opt
-00002540: 696f 6e73 3d6f 7074 696f 6e73 290a 6060  ions=options).``
-00002550: 600a 0a3e 204e 6f74 653a 204d 616b 6520  `..> Note: Make 
-00002560: 7375 7265 2074 6f20 7573 6520 7468 6520  sure to use the 
-00002570: 7269 6768 7420 7365 6c65 6e69 756d 206f  right selenium o
-00002580: 7074 696f 6e73 2066 6f72 2079 6f75 7220  ptions for your 
-00002590: 6272 6f77 7365 720a 0a3c 6832 2069 643d  browser..<h2 id=
-000025a0: 2268 6561 646c 6573 7322 3e20 f09f a4af  "headless"> ....
-000025b0: 2048 6561 646c 6573 7320 4272 6f77 7365   Headless Browse
-000025c0: 7273 203c 2f68 323e 0a0a 4865 6164 6c65  rs </h2>..Headle
-000025d0: 7373 2062 726f 7773 696e 6720 6f6e 6c79  ss browsing only
-000025e0: 2077 6f72 6b73 206f 6e20 4368 726f 6d65   works on Chrome
-000025f0: 2e20 5768 656e 2075 7369 6e67 2043 6872  . When using Chr
-00002600: 6f6d 652c 2061 6464 696e 6720 7468 6520  ome, adding the 
-00002610: 602d 2d68 6561 646c 6573 7360 2066 6c61  `--headless` fla
-00002620: 6720 7573 696e 6720 7468 6520 434c 4920  g using the CLI 
-00002630: 6f72 2070 6173 7369 6e67 2060 6865 6164  or passing `head
-00002640: 6c65 7373 6020 6173 2061 206b 6579 776f  less` as a keywo
-00002650: 7264 2061 7267 756d 656e 7420 746f 2060  rd argument to `
-00002660: 7570 6c6f 6164 5f76 6964 656f 6020 6f72  upload_video` or
-00002670: 2060 7570 6c6f 6164 5f76 6964 656f 7360   `upload_videos`
-00002680: 2069 7320 616c 6c20 7468 6174 2069 7320   is all that is 
-00002690: 7265 7175 6972 6564 2e0a 0a60 6060 7079  required...```py
-000026a0: 7468 6f6e 0a75 706c 6f61 645f 7669 6465  thon.upload_vide
-000026b0: 6f28 2e2e 2e2c 2068 6561 646c 6573 733d  o(..., headless=
-000026c0: 5472 7565 290a 7570 6c6f 6164 5f76 6964  True).upload_vid
-000026d0: 656f 7328 2e2e 2e2c 2068 6561 646c 6573  eos(..., headles
-000026e0: 733d 5472 7565 290a 6060 600a 0a3c 6832  s=True).```..<h2
-000026f0: 2069 643d 2269 6e69 7469 616c 2d73 6574   id="initial-set
-00002700: 7570 223e 20f0 9f94 a820 496e 6974 6961  up"> .... Initia
-00002710: 6c20 5365 7475 703c 2f68 323e 0a0a 5b57  l Setup</h2>..[W
-00002720: 6562 4472 6976 6572 4d61 6e61 6765 725d  ebDriverManager]
-00002730: 2868 7474 7073 3a2f 2f62 6f6e 6967 6172  (https://bonigar
-00002740: 6369 612e 6465 762f 7765 6264 7269 7665  cia.dev/webdrive
-00002750: 726d 616e 6167 6572 2f29 2069 7320 7573  rmanager/) is us
-00002760: 6564 2074 6f20 6d61 6e61 6765 2064 7269  ed to manage dri
-00002770: 7665 7220 7665 7273 696f 6e73 2e0a 0a4f  ver versions...O
-00002780: 6e20 696e 6974 6961 6c20 7374 6172 7475  n initial startu
-00002790: 702c 2079 6f75 202a 2a6d 6179 2a2a 2062  p, you **may** b
-000027a0: 6520 7072 6f6d 7074 6564 2074 6f20 696e  e prompted to in
-000027b0: 7374 616c 6c20 7468 6520 636f 7272 6563  stall the correc
-000027c0: 7420 6472 6976 6572 2066 6f72 2079 6f75  t driver for you
-000027d0: 7220 7365 6c65 6374 6564 2062 726f 7773  r selected brows
-000027e0: 6572 2e20 486f 7765 7665 722c 2066 6f72  er. However, for
-000027f0: 202a 2a43 6872 6f6d 652a 2a20 616e 6420   **Chrome** and 
-00002800: 2a2a 4564 6765 2a2a 2074 6865 2064 7269  **Edge** the dri
-00002810: 7665 7220 6973 2061 7574 6f6d 6174 6963  ver is automatic
-00002820: 616c 6c79 2069 6e73 7461 6c6c 6564 2e0a  ally installed..
-00002830: 0a3c 6832 2069 643d 2265 7861 6d70 6c65  .<h2 id="example
-00002840: 7322 3e20 e299 bb20 4578 616d 706c 6573  s"> ... Examples
-00002850: 3c2f 6832 3e0a 0a2d 202a 2a5b 4261 7369  </h2>..- **[Basi
-00002860: 6320 5570 6c6f 6164 2045 7861 6d70 6c65  c Upload Example
-00002870: 5d28 6578 616d 706c 6573 2f62 6173 6963  ](examples/basic
-00002880: 5f75 706c 6f61 642e 7079 293a 2a2a 2055  _upload.py):** U
-00002890: 7365 7320 6075 706c 6f61 645f 7669 6465  ses `upload_vide
-000028a0: 6f60 2074 6f20 6d61 6b65 206f 6e65 2070  o` to make one p
-000028b0: 6f73 742e 0a0a 2d20 2a2a 5b4d 756c 7469  ost...- **[Multi
-000028c0: 706c 6520 5669 6465 6f73 2041 7420 4f6e  ple Videos At On
-000028d0: 6365 5d28 6578 616d 706c 6573 2f6d 756c  ce](examples/mul
-000028e0: 7469 706c 655f 7669 6465 6f73 5f61 745f  tiple_videos_at_
-000028f0: 6f6e 6365 2e70 7929 3a2a 2a20 5570 6c6f  once.py):** Uplo
-00002900: 6164 7320 7468 6520 7361 6d65 2076 6964  ads the same vid
-00002910: 656f 206d 756c 7469 706c 6520 7469 6d65  eo multiple time
-00002920: 7320 7573 696e 6720 6075 706c 6f61 645f  s using `upload_
-00002930: 7669 6465 6f73 602e 0a0a 2d20 2a2a 5b53  videos`...- **[S
-00002940: 6572 6965 7320 5570 6c6f 6164 2045 7861  eries Upload Exa
-00002950: 6d70 6c65 5d28 6578 616d 706c 6573 2f73  mple](examples/s
-00002960: 6572 6965 735f 7570 6c6f 6164 2e70 7929  eries_upload.py)
-00002970: 3a2a 2a20 5669 6465 6f73 2061 7265 2072  :** Videos are r
-00002980: 6561 6420 6672 6f6d 2061 2043 5356 2066  ead from a CSV f
-00002990: 696c 6520 7573 696e 6720 5b50 616e 6461  ile using [Panda
-000029a0: 735d 2868 7474 7073 3a2f 2f70 616e 6461  s](https://panda
-000029b0: 732e 7079 6461 7461 2e6f 7267 292e 2041  s.pydata.org). A
-000029c0: 2076 6964 656f 2075 706c 6f61 6420 6174   video upload at
-000029d0: 7465 6d70 7420 6973 206d 6164 6520 616e  tempt is made an
-000029e0: 6420 2a2a 6966 2061 6e64 206f 6e6c 7920  d **if and only 
-000029f0: 6966 2a2a 2069 7420 6973 2073 7563 6365  if** it is succe
-00002a00: 7373 6675 6c20 7769 6c6c 2074 6865 2076  ssful will the v
-00002a10: 6964 656f 2062 6520 6d61 726b 6564 2061  ideo be marked a
-00002a20: 7320 7570 6c6f 6164 6564 2e0a 0a3c 6831  s uploaded...<h1
-00002a30: 2069 643d 226e 6f74 6573 223e 20f0 9f93   id="notes"> ...
-00002a40: 9d20 4e6f 7465 733c 2f68 313e 0a0a 5468  . Notes</h1>..Th
-00002a50: 6973 2062 6f74 2069 7320 6e6f 7420 666f  is bot is not fo
-00002a60: 6f6c 2070 726f 6f66 2e20 5468 6f75 6768  ol proof. Though
-00002a70: 2049 2068 6176 6520 6e6f 7420 676f 7474   I have not gott
-00002a80: 656e 2061 6e20 6f66 6669 6369 616c 2062  en an official b
-00002a90: 616e 2c20 7468 6520 7669 6465 6f20 7769  an, the video wi
-00002aa0: 6c6c 2066 6169 6c20 746f 2075 706c 6f61  ll fail to uploa
-00002ab0: 6420 6166 7465 7220 746f 6f20 6d61 6e79  d after too many
-00002ac0: 2075 706c 6f61 6473 2e20 496e 2074 6573   uploads. In tes
-00002ad0: 7469 6e67 2c20 7761 6974 696e 6720 7365  ting, waiting se
-00002ae0: 7665 7261 6c20 686f 7572 7320 7761 7320  veral hours was 
-00002af0: 7375 6666 6963 6965 6e74 2074 6f20 6669  sufficient to fi
-00002b00: 7820 7468 6973 2070 726f 626c 656d 2e20  x this problem. 
-00002b10: 466f 7220 7468 6973 2072 6561 736f 6e2c  For this reason,
-00002b20: 2070 6c65 6173 6520 7468 696e 6b20 6f66   please think of
-00002b30: 2074 6869 7320 6d6f 7265 2061 7320 6120   this more as a 
-00002b40: 7363 6865 6475 6c65 6420 7570 6c6f 6164  scheduled upload
-00002b50: 6572 2066 6f72 2054 696b 546f 6b20 7669  er for TikTok vi
-00002b60: 6465 6f73 2c20 7261 7468 6572 2074 6861  deos, rather tha
-00002b70: 6e20 6120 7370 616d 2062 6f74 2e0a 0a3c  n a spam bot...<
-00002b80: 6831 2069 643d 226d 6164 652d 7769 7468  h1 id="made-with
-00002b90: 223e 2041 6363 6f75 6e74 7320 6d61 6465  "> Accounts made
-00002ba0: 2077 6974 683c 2f68 313e 0a0a 2d20 5b40   with</h1>..- [@
-00002bb0: 435f 5370 616e 5d28 6874 7470 733a 2f2f  C_Span](https://
-00002bc0: 7777 772e 7469 6b74 6f6b 2e63 6f6d 2f40  www.tiktok.com/@
-00002bd0: 635f 7370 616e 3f6c 616e 673d 656e 2920  c_span?lang=en) 
-00002be0: 2d20 4120 7370 6c69 742d 7363 7265 656e  - A split-screen
-00002bf0: 2063 6861 6e6e 656c 2077 6974 6820 6d6f   channel with mo
-00002c00: 6269 6c65 2067 616d 6573 2062 656c 6f77  bile games below
-00002c10: 2d66 6561 7475 7269 6e67 2063 6c69 7073  -featuring clips
-00002c20: 2066 726f 6d20 432d 5370 616e 2773 2059   from C-Span's Y
-00002c30: 6f75 5475 6265 2063 6861 6e6e 656c 0a2d  ouTube channel.-
-00002c40: 205b 4068 6162 6974 5f74 7261 636b 5d28   [@habit_track](
-00002c50: 6874 7470 733a 2f2f 7777 772e 7469 6b74  https://www.tikt
-00002c60: 6f6b 2e63 6f6d 2f40 6861 6269 745f 7472  ok.com/@habit_tr
-00002c70: 6163 6b3f 6c61 6e67 3d65 6e29 202d 2041  ack?lang=en) - A
-00002c80: 2052 6564 6469 7420 626f 7420 746f 2073   Reddit bot to s
-00002c90: 6565 2077 6869 6368 2053 7562 5265 6464  ee which SubRedd
-00002ca0: 6974 2069 7320 6d6f 7374 2076 6972 616c  it is most viral
-00002cb0: 206f 6e20 5469 6b54 6f6b 0a0a 3e20 4966   on TikTok..> If
-00002cc0: 2079 6f75 206c 696b 6520 7468 6973 2070   you like this p
-00002cd0: 726f 6a65 6374 2c20 706c 6561 7365 20e2  roject, please .
-00002ce0: ad90 2069 7420 6f6e 2047 6974 4875 6220  .. it on GitHub 
-00002cf0: 746f 2073 686f 7720 796f 7572 2073 7570  to show your sup
-00002d00: 706f 7274 2120 e29d a4ef b88f 0a0a 215b  port! ........![
-00002d10: 5374 6172 2048 6973 746f 7279 2043 6861  Star History Cha
-00002d20: 7274 5d28 6874 7470 733a 2f2f 6170 692e  rt](https://api.
-00002d30: 7374 6172 2d68 6973 746f 7279 2e63 6f6d  star-history.com
-00002d40: 2f73 7667 3f72 6570 6f73 3d77 6b61 6973  /svg?repos=wkais
-00002d50: 6572 7465 7861 732f 7469 6b74 6f6b 2d75  ertexas/tiktok-u
-00002d60: 706c 6f61 6465 7226 7479 7065 3d44 6174  ploader&type=Dat
-00002d70: 6529 0a0a 5b5e 315d 3a20 4966 2069 6e74  e)..[^1]: If int
-00002d80: 6572 6573 7465 6420 696e 2048 6174 6368  erested in Hatch
-00002d90: 2c20 6368 6563 6b6f 7574 2074 6865 205b  , checkout the [
-00002da0: 7765 6273 6974 655d 2868 7474 7073 3a2f  website](https:/
-00002db0: 2f68 6174 6368 2e70 7970 612e 696f 2f6c  /hatch.pypa.io/l
-00002dc0: 6174 6573 742f 6275 696c 642f 290a       atest/build/).
+00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000010: 223e 0a3c 696d 6720 7372 633d 2268 7474  ">.<img src="htt
+00000020: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000030: 776b 6169 7365 7274 6578 6173 2f74 696b  wkaisertexas/tik
+00000040: 746f 6b2d 7570 6c6f 6164 6572 2f61 7373  tok-uploader/ass
+00000050: 6574 732f 3237 3739 3530 3134 2f66 3939  ets/27795014/f99
+00000060: 3166 6463 372d 3238 3761 2d34 6333 622d  1fdc7-287a-4c3b-
+00000070: 3961 3834 2d32 3263 3761 6438 6135 3762  9a84-22c7ad8a57b
+00000080: 6622 2061 6c74 3d22 7669 6465 6f20 776f  f" alt="video wo
+00000090: 726b 696e 6722 202f 3e0a 3c2f 703e 0a0a  rking" />.</p>..
+000000a0: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
+000000b0: 7222 3e20 e2ac 86ef b88f 2054 696b 546f  r"> ...... TikTo
+000000c0: 6b20 5570 6c6f 6164 6572 203c 2f68 313e  k Uploader </h1>
+000000d0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+000000e0: 7222 3e41 203c 7374 726f 6e67 3e53 656c  r">A <strong>Sel
+000000f0: 656e 6975 6d3c 2f73 7472 6f6e 673e 2d62  enium</strong>-b
+00000100: 6173 6564 2061 7574 6f6d 6174 6564 203c  ased automated <
+00000110: 7374 726f 6e67 3e54 696b 546f 6b3c 2f73  strong>TikTok</s
+00000120: 7472 6f6e 673e 2076 6964 656f 2075 706c  trong> video upl
+00000130: 6f61 6465 723c 2f70 3e0a 0a3c 7020 616c  oader</p>..<p al
+00000140: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+00000150: 3c69 6d67 2061 6c74 3d22 466f 726b 7322  <img alt="Forks"
+00000160: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00000170: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+00000180: 6875 622f 666f 726b 732f 776b 6169 7365  hub/forks/wkaise
+00000190: 7274 6578 6173 2f74 696b 746f 6b2d 7570  rtexas/tiktok-up
+000001a0: 6c6f 6164 6572 2220 2f3e 0a20 203c 696d  loader" />.  <im
+000001b0: 6720 616c 743d 2253 7461 7273 2220 7372  g alt="Stars" sr
+000001c0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+000001d0: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
+000001e0: 2f73 7461 7273 2f77 6b61 6973 6572 7465  /stars/wkaiserte
+000001f0: 7861 732f 7469 6b74 6f6b 2d75 706c 6f61  xas/tiktok-uploa
+00000200: 6465 7222 202f 3e0a 2020 3c69 6d67 2061  der" />.  <img a
+00000210: 6c74 3d22 5761 7463 6865 7273 2220 7372  lt="Watchers" sr
+00000220: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000230: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
+00000240: 2f77 6174 6368 6572 732f 776b 6169 7365  /watchers/wkaise
+00000250: 7274 6578 6173 2f74 696b 746f 6b2d 7570  rtexas/tiktok-up
+00000260: 6c6f 6164 6572 2220 2f3e 0a3c 2f70 3e0a  loader" />.</p>.
+00000270: 0a23 2054 6162 6c65 206f 6620 436f 6e74  .# Table of Cont
+00000280: 656e 7473 0a2d 205b 496e 7374 616c 6c61  ents.- [Installa
+00000290: 7469 6f6e 5d28 2369 6e73 7461 6c6c 6174  tion](#installat
+000002a0: 696f 6e29 0a20 202d 205b 4d61 634f 532c  ion).  - [MacOS,
+000002b0: 2057 696e 646f 7773 2061 6e64 204c 696e   Windows and Lin
+000002c0: 7578 5d28 236d 6163 6f73 2d77 696e 646f  ux](#macos-windo
+000002d0: 7773 2d61 6e64 2d6c 696e 7578 290a 2020  ws-and-linux).  
+000002e0: 2020 2d20 5b44 6f77 6e6c 6f61 6469 6e67    - [Downloading
+000002f0: 2066 726f 6d20 5079 5049 2028 5265 636f   from PyPI (Reco
+00000300: 6d6d 656e 6465 6429 5d28 2364 6f77 6e6c  mmended)](#downl
+00000310: 6f61 6469 6e67 2d66 726f 6d2d 7079 7069  oading-from-pypi
+00000320: 2d72 6563 6f6d 6d65 6e64 6564 290a 2020  -recommended).  
+00000330: 2020 2d20 5b42 7569 6c64 696e 6720 6672    - [Building fr
+00000340: 6f6d 2073 6f75 7263 655d 2823 6275 696c  om source](#buil
+00000350: 6469 6e67 2d66 726f 6d2d 736f 7572 6365  ding-from-source
+00000360: 290a 2d20 5b55 7361 6765 5d28 2375 7361  ).- [Usage](#usa
+00000370: 6765 290a 2020 2d20 5bf0 9f92 bb20 436f  ge).  - [.... Co
+00000380: 6d6d 616e 6420 4c69 6e65 2049 6e74 6572  mmand Line Inter
+00000390: 6661 6365 2028 434c 4929 5d28 232d 636f  face (CLI)](#-co
+000003a0: 6d6d 6d61 6e64 2d6c 696e 652d 696e 7465  mmmand-line-inte
+000003b0: 7266 6163 652d 636c 6929 0a20 202d 205b  rface-cli).  - [
+000003c0: e2ac 8620 5570 6c6f 6164 696e 6720 5669  ... Uploading Vi
+000003d0: 6465 6f73 5d28 232d 7570 6c6f 6164 696e  deos](#-uploadin
+000003e0: 672d 7669 6465 6f73 290a 2020 2d20 5bf0  g-videos).  - [.
+000003f0: 9fab b520 4d65 6e74 696f 6e73 2061 6e64  ... Mentions and
+00000400: 2048 6173 6874 6167 735d 2823 2d6d 656e   Hashtags](#-men
+00000410: 7469 6f6e 732d 616e 642d 6861 7368 7461  tions-and-hashta
+00000420: 6773 290a 2020 2d20 5bf0 9faa a120 5374  gs).  - [.... St
+00000430: 6974 6368 6573 2c20 4475 6574 7320 616e  itches, Duets an
+00000440: 6420 436f 6d6d 656e 7473 5d28 232d 7374  d Comments](#-st
+00000450: 6974 6368 6573 2d64 7565 7473 2d61 6e64  itches-duets-and
+00000460: 2d63 6f6d 6d65 6e74 7329 0a20 202d 205b  -comments).  - [
+00000470: f09f 9490 2041 7574 6865 6e74 6963 6174  .... Authenticat
+00000480: 696f 6e5d 2823 2d61 7574 6865 6e74 6963  ion](#-authentic
+00000490: 6174 696f 6e29 0a20 202d 205b f09f 9180  ation).  - [....
+000004a0: 2042 726f 7773 6572 2053 656c 6563 7469   Browser Selecti
+000004b0: 6f6e 5d28 232d 6272 6f77 7365 722d 7365  on](#-browser-se
+000004c0: 6c65 6374 696f 6e29 0a20 202d 205b f09f  lection).  - [..
+000004d0: 9ab2 2043 7573 746f 6d20 5765 6244 7269  .. Custom WebDri
+000004e0: 7665 7220 4472 6976 6572 204f 7074 696f  ver Driver Optio
+000004f0: 6e73 5d28 232d 6375 7374 6f6d 2d77 6562  ns](#-custom-web
+00000500: 6472 6976 6572 2d64 7269 7665 722d 6f70  driver-driver-op
+00000510: 7469 6f6e 7329 0a20 202d 205b f09f a4af  tions).  - [....
+00000520: 2048 6561 646c 6573 7320 4272 6f77 7365   Headless Browse
+00000530: 7273 5d28 232d 6865 6164 6c65 7373 2d62  rs](#-headless-b
+00000540: 726f 7773 6572 7329 0a20 202d 205b f09f  rowsers).  - [..
+00000550: 94a8 2049 6e69 7469 616c 2053 6574 7570  .. Initial Setup
+00000560: 5d28 232d 696e 6974 6961 6c2d 7365 7475  ](#-initial-setu
+00000570: 7029 0a2d 205b e299 bbef b88f 2045 7861  p).- [...... Exa
+00000580: 6d70 6c65 735d 2823 2d65 7861 6d70 6c65  mples](#-example
+00000590: 7329 0a2d 205b f09f 939d 204e 6f74 6573  s).- [.... Notes
+000005a0: 5d28 232d 6e6f 7465 7329 0a2d 205b 4163  ](#-notes).- [Ac
+000005b0: 636f 756e 7473 206d 6164 6520 7769 7468  counts made with
+000005c0: 5d28 2361 6363 6f75 6e74 732d 6d61 6465  ](#accounts-made
+000005d0: 2d75 7369 6e67 2d74 696b 746f 6b2d 7570  -using-tiktok-up
+000005e0: 6c6f 6164 6572 290a 2320 496e 7374 616c  loader).# Instal
+000005f0: 6c61 7469 6f6e 0a0a 4120 7065 7271 7569  lation..A perqui
+00000600: 7369 7465 2074 6f20 7573 696e 6720 7468  site to using th
+00000610: 6973 2070 726f 6772 616d 2069 7320 7468  is program is th
+00000620: 6520 696e 7374 616c 6c61 7469 6f6e 206f  e installation o
+00000630: 6620 6120 5b53 656c 656e 6975 6d2d 636f  f a [Selenium-co
+00000640: 6d70 6174 6962 6c65 5d28 6874 7470 733a  mpatible](https:
+00000650: 2f2f 7777 772e 7365 6c65 6e69 756d 2e64  //www.selenium.d
+00000660: 6576 2f64 6f63 756d 656e 7461 7469 6f6e  ev/documentation
+00000670: 2f77 6562 6472 6976 6572 2f67 6574 7469  /webdriver/getti
+00000680: 6e67 5f73 7461 7274 6564 2f69 6e73 7461  ng_started/insta
+00000690: 6c6c 5f64 7269 7665 7273 2f29 2077 6562  ll_drivers/) web
+000006a0: 2062 726f 7773 6572 2e20 5b47 6f6f 676c   browser. [Googl
+000006b0: 6520 4368 726f 6d65 5d28 6874 7470 733a  e Chrome](https:
+000006c0: 2f2f 7777 772e 676f 6f67 6c65 2e63 6f6d  //www.google.com
+000006d0: 2f63 6872 6f6d 652f 2920 6973 2072 6563  /chrome/) is rec
+000006e0: 6f6d 6d65 6e64 6564 2e0a 0a23 2320 4d61  ommended...## Ma
+000006f0: 634f 532c 2057 696e 646f 7773 2061 6e64  cOS, Windows and
+00000700: 204c 696e 7578 0a0a 496e 7374 616c 6c20   Linux..Install 
+00000710: 5079 7468 6f6e 2033 206f 7220 6772 6561  Python 3 or grea
+00000720: 7465 7220 6672 6f6d 205b 7079 7468 6f6e  ter from [python
+00000730: 2e6f 7267 5d28 6874 7470 733a 2f2f 7777  .org](https://ww
+00000740: 772e 7079 7468 6f6e 2e6f 7267 2f64 6f77  w.python.org/dow
+00000750: 6e6c 6f61 6473 2f29 0a0a 2323 2320 446f  nloads/)..### Do
+00000760: 776e 6c6f 6164 696e 6720 6672 6f6d 2050  wnloading from P
+00000770: 7950 4920 2852 6563 6f6d 6d65 6e64 6564  yPI (Recommended
+00000780: 290a 0a49 6e73 7461 6c6c 2060 7469 6b74  )..Install `tikt
+00000790: 6f6b 2d75 706c 6f61 6465 7260 2075 7369  ok-uploader` usi
+000007a0: 6e67 2060 7069 7060 0a0a 6060 6062 6173  ng `pip`..```bas
+000007b0: 680a 7069 7020 696e 7374 616c 6c20 7469  h.pip install ti
+000007c0: 6b74 6f6b 2d75 706c 6f61 6465 720a 6060  ktok-uploader.``
+000007d0: 600a 0a23 2323 2042 7569 6c64 696e 6720  `..### Building 
+000007e0: 6672 6f6d 2073 6f75 7263 650a 0a49 6e73  from source..Ins
+000007f0: 7461 6c6c 696e 6720 6672 6f6d 2073 6f75  talling from sou
+00000800: 7263 6520 616c 6c6f 7773 2067 7265 6174  rce allows great
+00000810: 6572 2066 6c65 7869 6269 6c69 7479 2074  er flexibility t
+00000820: 6f20 6d6f 6469 6679 2074 6865 206d 6f64  o modify the mod
+00000830: 756c 6527 7320 636f 6465 2074 6f20 6578  ule's code to ex
+00000840: 7465 6e64 2064 6566 6175 6c74 2062 6568  tend default beh
+00000850: 6176 696f 722e 200a 0a46 6972 7374 2c20  avior. ..First, 
+00000860: 6063 6c6f 6e65 6020 616e 6420 6d6f 7665  `clone` and move
+00000870: 2069 6e74 6f20 7468 6520 7265 706f 7369   into the reposi
+00000880: 746f 7279 2e20 4e65 7874 2c20 696e 7374  tory. Next, inst
+00000890: 616c 6c20 6068 6174 6368 602c 2074 6865  all `hatch`, the
+000008a0: 2062 7569 6c64 2074 6f6f 6c20 7573 6564   build tool used
+000008b0: 2066 6f72 2074 6869 7320 7072 6f6a 6563   for this projec
+000008c0: 7420 5b5e 315d 2e20 5468 656e 2c20 6062  t [^1]. Then, `b
+000008d0: 7569 6c64 6020 7468 6520 7072 6f6a 6563  uild` the projec
+000008e0: 742e 2046 696e 616c 6c79 2c20 6069 6e73  t. Finally, `ins
+000008f0: 7461 6c6c 6020 7468 6520 7072 6f6a 6563  tall` the projec
+00000900: 7420 7769 7468 2074 6865 2060 2d65 6020  t with the `-e` 
+00000910: 6f72 2065 6469 7461 626c 6520 666c 6167  or editable flag
+00000920: 2e20 200a 6060 6063 6f6e 736f 6c65 0a67  .  .```console.g
+00000930: 6974 2063 6c6f 6e65 2068 7474 7073 3a2f  it clone https:/
+00000940: 2f67 6974 6875 622e 636f 6d2f 776b 6169  /github.com/wkai
+00000950: 7365 7274 6578 6173 2f74 696b 746f 6b2d  sertexas/tiktok-
+00000960: 7570 6c6f 6164 6572 2e67 6974 0a63 6420  uploader.git.cd 
+00000970: 7469 6b74 6f6b 2d75 706c 6f61 6465 720a  tiktok-uploader.
+00000980: 7069 7020 696e 7374 616c 6c20 6861 7463  pip install hatc
+00000990: 680a 6861 7463 6820 6275 696c 640a 7069  h.hatch build.pi
+000009a0: 7020 696e 7374 616c 6c20 2d65 202e 200a  p install -e . .
+000009b0: 6060 600a 0a23 2055 7361 6765 0a0a 6074  ```..# Usage..`t
+000009c0: 696b 746f 6b2d 7570 6c6f 6164 6572 6020  iktok-uploader` 
+000009d0: 776f 726b 7320 6279 2064 7570 6c69 6361  works by duplica
+000009e0: 7469 6e67 2079 6f75 7220 6272 6f77 7365  ting your browse
+000009f0: 7227 7320 2a2a 636f 6f6b 6965 732a 2a20  r's **cookies** 
+00000a00: 7768 6963 6820 7472 6963 6b73 202a 2a54  which tricks **T
+00000a10: 696b 546f 6b2a 2a20 696e 746f 2062 656c  ikTok** into bel
+00000a20: 6965 7669 6e67 2079 6f75 2061 7265 206c  ieving you are l
+00000a30: 6f67 6765 6420 696e 206f 6e20 6120 7265  ogged in on a re
+00000a40: 6d6f 7465 2d63 6f6e 7472 6f6c 6c65 6420  mote-controlled 
+00000a50: 6272 6f77 7365 722e 0a0a 2323 20f0 9f92  browser...## ...
+00000a60: bb20 436f 6d6d 616e 6420 4c69 6e65 2049  . Command Line I
+00000a70: 6e74 6572 6661 6365 2028 434c 4929 0a0a  nterface (CLI)..
+00000a80: 5573 696e 6720 7468 6520 434c 4920 6973  Using the CLI is
+00000a90: 2061 7320 7369 6d70 6c65 2061 7320 6361   as simple as ca
+00000aa0: 6c6c 696e 6720 6074 696b 746f 6b2d 7570  lling `tiktok-up
+00000ab0: 6c6f 6164 6572 6020 7769 7468 2079 6f75  loader` with you
+00000ac0: 7220 7669 6465 6f73 3a20 6070 6174 6860  r videos: `path`
+00000ad0: 2028 2d76 292c 2060 6465 7363 7269 7074   (-v), `descript
+00000ae0: 696f 6e60 282d 6429 2061 6e64 2060 636f  ion`(-d) and `co
+00000af0: 6f6b 6965 7360 2028 2d63 290a 0a60 6060  okies` (-c)..```
+00000b00: 6261 7368 0a74 696b 746f 6b2d 7570 6c6f  bash.tiktok-uplo
+00000b10: 6164 6572 202d 7620 7669 6465 6f2e 6d70  ader -v video.mp
+00000b20: 3420 2d64 2022 7468 6973 2069 7320 6d79  4 -d "this is my
+00000b30: 2065 7363 6170 6564 205c 2264 6573 6372   escaped \"descr
+00000b40: 6970 7469 6f6e 5c22 2220 2d63 2063 6f6f  iption\"" -c coo
+00000b50: 6b69 6573 2e74 7874 0a60 6060 0a0a 6060  kies.txt.```..``
+00000b60: 6070 7974 686f 6e0a 6672 6f6d 2074 696b  `python.from tik
+00000b70: 746f 6b5f 7570 6c6f 6164 6572 2e75 706c  tok_uploader.upl
+00000b80: 6f61 6420 696d 706f 7274 2075 706c 6f61  oad import uploa
+00000b90: 645f 7669 6465 6f2c 2075 706c 6f61 645f  d_video, upload_
+00000ba0: 7669 6465 6f73 0a66 726f 6d20 7469 6b74  videos.from tikt
+00000bb0: 6f6b 5f75 706c 6f61 6465 722e 6175 7468  ok_uploader.auth
+00000bc0: 2069 6d70 6f72 7420 4175 7468 4261 636b   import AuthBack
+00000bd0: 656e 640a 0a23 2073 696e 676c 6520 7669  end..# single vi
+00000be0: 6465 6f0a 7570 6c6f 6164 5f76 6964 656f  deo.upload_video
+00000bf0: 2827 7669 6465 6f2e 6d70 3427 2c20 0a20  ('video.mp4', . 
+00000c00: 2020 2020 2020 2020 2020 2064 6573 6372             descr
+00000c10: 6970 7469 6f6e 3d27 7468 6973 2069 7320  iption='this is 
+00000c20: 6d79 2064 6573 6372 6970 7469 6f6e 272c  my description',
+00000c30: 200a 2020 2020 2020 2020 2020 2020 636f   .            co
+00000c40: 6f6b 6965 733d 2763 6f6f 6b69 6573 2e74  okies='cookies.t
+00000c50: 7874 2729 0a0a 2320 4d75 6c74 6970 6c65  xt')..# Multiple
+00000c60: 2056 6964 656f 730a 7669 6465 6f73 203d   Videos.videos =
+00000c70: 205b 0a20 2020 207b 0a20 2020 2020 2020   [.    {.       
+00000c80: 2027 7061 7468 273a 2027 7669 6465 6f2e   'path': 'video.
+00000c90: 6d70 3427 2c20 0a20 2020 2020 2020 2027  mp4', .        '
+00000ca0: 6465 7363 7269 7074 696f 6e27 3a20 2774  description': 't
+00000cb0: 6869 7320 6973 206d 7920 6465 7363 7269  his is my descri
+00000cc0: 7074 696f 6e27 0a20 2020 207d 2c0a 2020  ption'.    },.  
+00000cd0: 2020 7b0a 2020 2020 2020 2020 2770 6174    {.        'pat
+00000ce0: 6827 3a20 2776 6964 656f 322e 6d70 3427  h': 'video2.mp4'
+00000cf0: 2c20 0a20 2020 2020 2020 2027 6465 7363  , .        'desc
+00000d00: 7269 7074 696f 6e27 3a20 2774 6869 7320  ription': 'this 
+00000d10: 6973 2061 6c73 6f20 6d79 2064 6573 6372  is also my descr
+00000d20: 6970 7469 6f6e 270a 2020 2020 7d0a 5d0a  iption'.    }.].
+00000d30: 0a61 7574 6820 3d20 4175 7468 4261 636b  .auth = AuthBack
+00000d40: 656e 6428 636f 6f6b 6965 733d 2763 6f6f  end(cookies='coo
+00000d50: 6b69 6573 2e74 7874 2729 0a75 706c 6f61  kies.txt').uploa
+00000d60: 645f 7669 6465 6f73 2876 6964 656f 733d  d_videos(videos=
+00000d70: 7669 6465 6f73 2c20 6175 7468 3d61 7574  videos, auth=aut
+00000d80: 6829 0a60 6060 0a0a 2323 20e2 ac86 2055  h).```..## ... U
+00000d90: 706c 6f61 6469 6e67 2056 6964 656f 730a  ploading Videos.
+00000da0: 0a54 6869 7320 6c69 6272 6172 7920 7265  .This library re
+00000db0: 766f 6c76 6573 2061 726f 756e 6420 7468  volves around th
+00000dc0: 6520 6075 706c 6f61 645f 7669 6465 6f73  e `upload_videos
+00000dd0: 6020 6675 6e63 7469 6f6e 2077 6869 6368  ` function which
+00000de0: 2074 616b 6573 2069 6e20 6120 6c69 7374   takes in a list
+00000df0: 206f 6620 7669 6465 6f73 2077 6869 6368   of videos which
+00000e00: 2068 6176 6520 2a2a 6669 6c65 6e61 6d65   have **filename
+00000e10: 732a 2a20 616e 6420 2a2a 6465 7363 7269  s** and **descri
+00000e20: 7074 696f 6e73 2a2a 2061 6e64 2061 7265  ptions** and are
+00000e30: 2070 6173 7365 6420 6173 2066 6f6c 6c6f   passed as follo
+00000e40: 7773 3a0a 0a60 6060 7079 7468 6f6e 0a66  ws:..```python.f
+00000e50: 726f 6d20 7469 6b74 6f6b 5f75 706c 6f61  rom tiktok_uploa
+00000e60: 6465 722e 7570 6c6f 6164 2069 6d70 6f72  der.upload impor
+00000e70: 7420 7570 6c6f 6164 5f76 6964 656f 730a  t upload_videos.
+00000e80: 6672 6f6d 2074 696b 746f 6b5f 7570 6c6f  from tiktok_uplo
+00000e90: 6164 6572 2e61 7574 6820 696d 706f 7274  ader.auth import
+00000ea0: 2041 7574 6842 6163 6b65 6e64 0a0a 7669   AuthBackend..vi
+00000eb0: 6465 6f73 203d 205b 0a20 2020 207b 0a20  deos = [.    {. 
+00000ec0: 2020 2020 2020 2027 7669 6465 6f27 3a20         'video': 
+00000ed0: 2776 6964 656f 302e 6d70 3427 2c0a 2020  'video0.mp4',.  
+00000ee0: 2020 2020 2020 2764 6573 6372 6970 7469        'descripti
+00000ef0: 6f6e 273a 2027 5669 6465 6f20 3120 6973  on': 'Video 1 is
+00000f00: 2061 626f 7574 202e 2e2e 270a 2020 2020   about ...'.    
+00000f10: 7d2c 0a20 2020 207b 0a20 2020 2020 2020  },.    {.       
+00000f20: 2027 7669 6465 6f27 3a20 2776 6964 656f   'video': 'video
+00000f30: 312e 6d70 3427 2c0a 2020 2020 2020 2020  1.mp4',.        
+00000f40: 2764 6573 6372 6970 7469 6f6e 273a 2027  'description': '
+00000f50: 5669 6465 6f20 3220 6973 2061 626f 7574  Video 2 is about
+00000f60: 202e 2e2e 270a 2020 2020 7d0a 5d0a 0a61   ...'.    }.]..a
+00000f70: 7574 6820 3d20 4175 7468 4261 636b 656e  uth = AuthBacken
+00000f80: 6428 636f 6f6b 6965 733d 2763 6f6f 6b69  d(cookies='cooki
+00000f90: 6573 2e74 7874 2729 0a66 6169 6c65 645f  es.txt').failed_
+00000fa0: 7669 6465 6f73 203d 2075 706c 6f61 645f  videos = upload_
+00000fb0: 7669 6465 6f73 2876 6964 656f 733d 7669  videos(videos=vi
+00000fc0: 6465 6f73 2c20 6175 7468 3d61 7574 6829  deos, auth=auth)
+00000fd0: 0a0a 666f 7220 7669 6465 6f20 696e 2066  ..for video in f
+00000fe0: 6169 6c65 645f 7669 6465 6f73 3a20 2320  ailed_videos: # 
+00000ff0: 6561 6368 2069 6e70 7574 2076 6964 656f  each input video
+00001000: 206f 626a 6563 7420 7768 6963 6820 6661   object which fa
+00001010: 696c 6564 0a20 2020 2070 7269 6e74 2866  iled.    print(f
+00001020: 277b 7669 6465 6f5b 2776 6964 656f 275d  '{video['video']
+00001030: 7d20 7769 7468 2064 6573 6372 6970 7469  } with descripti
+00001040: 6f6e 2022 7b76 6964 656f 5b27 6465 7363  on "{video['desc
+00001050: 7269 7074 696f 6e27 5d7d 2220 6661 696c  ription']}" fail
+00001060: 6564 2729 0a60 6060 0a0a 2323 20f0 9fab  ed').```..## ...
+00001070: b520 4d65 6e74 696f 6e73 2061 6e64 2048  . Mentions and H
+00001080: 6173 6874 6167 730a 0a4d 656e 7469 6f6e  ashtags..Mention
+00001090: 7320 616e 6420 4861 7368 7461 6773 206e  s and Hashtags n
+000010a0: 6f77 2077 6f72 6b20 736f 206c 6f6e 6720  ow work so long 
+000010b0: 6173 2074 6865 7920 6172 6520 666f 6c6c  as they are foll
+000010c0: 6f77 6564 2062 7920 6120 7370 6163 652e  owed by a space.
+000010d0: 2048 6f77 6576 6572 2c20 796f 7520 6173   However, you as
+000010e0: 2074 6865 2075 7365 7220 6172 6520 7265   the user are re
+000010f0: 7370 6f6e 7369 626c 6520 666f 7220 7665  sponsible for ve
+00001100: 7269 6679 696e 6720 6120 6d65 6e74 696f  rifying a mentio
+00001110: 6e20 6f72 2068 6173 6874 6167 2065 7869  n or hashtag exi
+00001120: 7374 7320 6265 666f 7265 2070 6f73 7469  sts before posti
+00001130: 6e67 0a0a 2a2a 4578 616d 706c 653a 2a2a  ng..**Example:**
+00001140: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
+00001150: 7469 6b74 6f6b 5f75 706c 6f61 6465 722e  tiktok_uploader.
+00001160: 7570 6c6f 6164 2069 6d70 6f72 7420 7570  upload import up
+00001170: 6c6f 6164 5f76 6964 656f 0a0a 7570 6c6f  load_video..uplo
+00001180: 6164 5f76 6964 656f 2827 7669 6465 6f2e  ad_video('video.
+00001190: 6d70 3427 2c20 2723 6679 7020 4069 6365  mp4', '#fyp @ice
+000011a0: 7370 6963 6565 272c 2027 636f 6f6b 6965  spicee', 'cookie
+000011b0: 732e 7478 7427 290a 6060 600a 0a23 2320  s.txt').```..## 
+000011c0: f09f aaa1 2053 7469 7463 6865 732c 2044  .... Stitches, D
+000011d0: 7565 7473 2061 6e64 2043 6f6d 6d65 6e74  uets and Comment
+000011e0: 730a 0a54 6f20 7365 7420 7768 6574 6865  s..To set whethe
+000011f0: 7220 6f72 206e 6f74 2061 2076 6964 656f  r or not a video
+00001200: 2075 706c 6f61 6465 6420 616c 6c6f 7773   uploaded allows
+00001210: 2073 7469 7463 6865 732c 2063 6f6d 6d65   stitches, comme
+00001220: 6e74 7320 6f72 2064 7565 742c 2073 696d  nts or duet, sim
+00001230: 706c 7920 7370 6563 6966 7920 6063 6f6d  ply specify `com
+00001240: 6d65 6e74 602c 2060 7374 6974 6368 6020  ment`, `stitch` 
+00001250: 616e 642f 6f72 2060 6475 6574 6020 6173  and/or `duet` as
+00001260: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
+00001270: 7473 2074 6f20 6075 706c 6f61 645f 7669  ts to `upload_vi
+00001280: 6465 6f60 206f 7220 6075 706c 6f61 645f  deo` or `upload_
+00001290: 7669 6465 6f73 602e 0a0a 6060 6070 7974  videos`...```pyt
+000012a0: 686f 6e0a 7570 6c6f 6164 5f76 6964 656f  hon.upload_video
+000012b0: 282e 2e2e 2c20 636f 6d6d 656e 743d 5472  (..., comment=Tr
+000012c0: 7565 2c20 7374 6974 6368 3d54 7275 652c  ue, stitch=True,
+000012d0: 2064 7565 743d 5472 7565 290a 6060 600a   duet=True).```.
+000012e0: 0a3e 2043 6f6d 6d65 6e74 732c 2053 7469  .> Comments, Sti
+000012f0: 7463 6865 7320 616e 6420 4475 6574 7320  tches and Duets 
+00001300: 6172 6520 616c 6c6f 7765 6420 6279 202a  are allowed by *
+00001310: 2a64 6566 6175 6c74 2a2a 0a0a 2323 20f0  *default**..## .
+00001320: 9f8c 9020 5072 6f78 790a 546f 2073 6574  ... Proxy.To set
+00001330: 2061 2070 726f 7879 2c20 6375 7272 656e   a proxy, curren
+00001340: 746c 7920 6f6e 6c79 2077 6f72 6b73 2077  tly only works w
+00001350: 6974 6820 6368 726f 6d65 2061 7320 7468  ith chrome as th
+00001360: 6520 6272 6f77 7365 722c 2061 6c6c 6f77  e browser, allow
+00001370: 2075 7365 723a 7061 7373 2061 7574 682e   user:pass auth.
+00001380: 0a0a 6060 6070 7974 686f 6e0a 2320 7072  ..```python.# pr
+00001390: 6f78 7920 3d20 7b27 7573 6572 273a 2027  oxy = {'user': '
+000013a0: 6d79 7573 6572 272c 2027 7061 7373 273a  myuser', 'pass':
+000013b0: 2027 6d79 7061 7373 272c 2027 686f 7374   'mypass', 'host
+000013c0: 273a 2027 3131 312e 3131 312e 3131 3127  ': '111.111.111'
+000013d0: 2c20 2770 6f72 7427 3a20 2739 3927 7d20  , 'port': '99'} 
+000013e0: 2023 2075 7365 723a 7061 7373 0a70 726f   # user:pass.pro
+000013f0: 7879 203d 207b 2768 6f73 7427 3a20 2731  xy = {'host': '1
+00001400: 3131 2e31 3131 2e31 3131 272c 2027 706f  11.111.111', 'po
+00001410: 7274 273a 2027 3939 277d 0a75 706c 6f61  rt': '99'}.uploa
+00001420: 645f 7669 6465 6f28 2e2e 2e2c 2070 726f  d_video(..., pro
+00001430: 7879 3d70 726f 7879 290a 6060 600a 2323  xy=proxy).```.##
+00001440: 20f0 9f93 8620 5363 6865 6475 6c65 0a54   .... Schedule.T
+00001450: 6865 2064 6174 6574 696d 6520 746f 2073  he datetime to s
+00001460: 6368 6564 756c 6520 7468 6520 7669 6465  chedule the vide
+00001470: 6f20 7769 6c6c 2062 6520 7472 6561 7465  o will be treate
+00001480: 6420 7769 7468 2074 6865 2055 5443 2074  d with the UTC t
+00001490: 696d 657a 6f6e 652e 203c 6272 3e0a 5468  imezone. <br>.Th
+000014a0: 6520 7363 6865 6475 6c65 6420 6461 7465  e scheduled date
+000014b0: 7469 6d65 206d 7573 7420 6265 2061 7420  time must be at 
+000014c0: 6c65 6173 7420 3230 206d 696e 7574 6573  least 20 minutes
+000014d0: 2069 6e20 7468 6520 6675 7475 7265 2061   in the future a
+000014e0: 6e64 2061 206d 6178 696d 756d 206f 6620  nd a maximum of 
+000014f0: 3130 2064 6179 732e 0a0a 6060 6070 7974  10 days...```pyt
+00001500: 686f 6e0a 696d 706f 7274 2064 6174 6574  hon.import datet
+00001510: 696d 650a 7363 6865 6475 6c65 203d 2064  ime.schedule = d
+00001520: 6174 6574 696d 652e 6461 7465 7469 6d65  atetime.datetime
+00001530: 2832 3032 302c 2031 322c 2032 302c 2031  (2020, 12, 20, 1
+00001540: 332c 2030 3029 0a75 706c 6f61 645f 7669  3, 00).upload_vi
+00001550: 6465 6f28 2e2e 2e2c 2073 6368 6564 756c  deo(..., schedul
+00001560: 653d 7363 6865 6475 6c65 290a 6060 600a  e=schedule).```.
+00001570: 0a23 2320 f09f 9490 2041 7574 6865 6e74  .## .... Authent
+00001580: 6963 6174 696f 6e0a 4175 7468 656e 7469  ication.Authenti
+00001590: 6361 7469 6f6e 2075 7365 7320 796f 7572  cation uses your
+000015a0: 2062 726f 7773 6572 2773 2063 6f6f 6b69   browser's cooki
+000015b0: 6573 2e20 5468 6973 2077 6f72 6b61 726f  es. This workaro
+000015c0: 756e 6420 7761 7320 646f 6e65 2064 7565  und was done due
+000015d0: 2074 6f20 5469 6b54 6f6b 2773 2073 7472   to TikTok's str
+000015e0: 6963 7465 7220 7374 616e 6365 206f 6e20  icter stance on 
+000015f0: 6175 7468 656e 7469 6361 7469 6f6e 2062  authentication b
+00001600: 7920 6120 5365 6c65 6e69 756d 2d63 6f6e  y a Selenium-con
+00001610: 7472 6f6c 6c65 6420 6272 6f77 7365 722e  trolled browser.
+00001620: 0a0a 596f 7572 2060 7365 7373 696f 6e69  ..Your `sessioni
+00001630: 6460 2069 7320 616c 6c20 7468 6174 2069  d` is all that i
+00001640: 7320 7265 7175 6972 6564 2066 6f72 2061  s required for a
+00001650: 7574 6865 6e74 6963 6174 696f 6e20 616e  uthentication an
+00001660: 6420 6361 6e20 6265 2070 6173 7365 6420  d can be passed 
+00001670: 6173 2061 6e20 6172 6775 6d65 6e74 2074  as an argument t
+00001680: 6f20 6e65 6172 6c79 2061 6e79 2066 756e  o nearly any fun
+00001690: 6374 696f 6e0a 0a5b f09f 8daa 2047 6574  ction..[.... Get
+000016a0: 2063 6f6f 6b69 6573 2e74 7874 5d28 6874   cookies.txt](ht
+000016b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000016c0: 2f6b 6169 7269 3030 332f 4765 742d 636f  /kairi003/Get-co
+000016d0: 6f6b 6965 732e 7478 742d 4c4f 4341 4c4c  okies.txt-LOCALL
+000016e0: 5929 206d 616b 6573 2067 6574 7469 6e67  Y) makes getting
+000016f0: 2063 6f6f 6b69 6573 2069 6e20 6120 5b4e   cookies in a [N
+00001700: 6574 5363 6170 6520 636f 6f6b 6965 7320  etScape cookies 
+00001710: 666f 726d 6174 5d28 6874 7470 3a2f 2f66  format](http://f
+00001720: 696c 6566 6f72 6d61 7473 2e61 7263 6869  ileformats.archi
+00001730: 7665 7465 616d 2e6f 7267 2f77 696b 692f  veteam.org/wiki/
+00001740: 4e65 7473 6361 7065 5f63 6f6f 6b69 6573  Netscape_cookies
+00001750: 2e74 7874 292e 0a0a 4166 7465 7220 696e  .txt)...After in
+00001760: 7374 616c 6c69 6e67 2c20 6f70 656e 2074  stalling, open t
+00001770: 6865 2065 7874 656e 7369 6f6e 7320 6d65  he extensions me
+00001780: 6e75 206f 6e20 5b54 696b 546f 6b2e 636f  nu on [TikTok.co
+00001790: 6d5d 2868 7474 7073 3a2f 2f74 696b 746f  m](https://tikto
+000017a0: 6b2e 636f 6d2f 2920 616e 6420 636c 6963  k.com/) and clic
+000017b0: 6b20 60f0 9f8d aa20 4765 7420 636f 6f6b  k `.... Get cook
+000017c0: 6965 732e 7478 7460 2074 6f20 7265 7665  ies.txt` to reve
+000017d0: 616c 2079 6f75 7220 636f 6f6b 6965 732e  al your cookies.
+000017e0: 2053 656c 6563 7420 6045 7870 6f72 7420   Select `Export 
+000017f0: 4173 20e2 87a9 6020 616e 6420 7370 6563  As ...` and spec
+00001800: 6966 7920 6120 6c6f 6361 7469 6f6e 2061  ify a location a
+00001810: 6e64 206e 616d 6520 746f 2073 6176 652e  nd name to save.
+00001820: 0a0a 2a2a 4f70 7469 6f6e 616c 6c79 2a2a  ..**Optionally**
+00001830: 2c20 6063 6f6f 6b69 6573 5f6c 6973 7460  , `cookies_list`
+00001840: 2069 7320 6120 6c69 7374 206f 6620 6469   is a list of di
+00001850: 6374 696f 6e61 7269 6573 2077 6974 6820  ctionaries with 
+00001860: 6b65 7973 2060 6e61 6d65 602c 2060 7661  keys `name`, `va
+00001870: 6c75 6560 2c20 6064 6f6d 6169 6e60 2c20  lue`, `domain`, 
+00001880: 6070 6174 6860 2061 6e64 2060 6578 7069  `path` and `expi
+00001890: 7279 6020 7768 6963 6820 616c 6c6f 7720  ry` which allow 
+000018a0: 796f 7520 746f 2070 6173 7320 796f 7572  you to pass your
+000018b0: 206f 776e 2062 726f 7773 6572 2063 6f6f   own browser coo
+000018c0: 6b69 6573 2e20 0a0a 2a2a 4578 616d 706c  kies. ..**Exampl
+000018d0: 653a 2a2a 0a0a 6060 6070 7974 686f 6e0a  e:**..```python.
+000018e0: 636f 6f6b 6965 735f 6c69 7374 203d 205b  cookies_list = [
+000018f0: 0a20 2020 207b 0a20 2020 2020 2020 2027  .    {.        '
+00001900: 6e61 6d65 273a 2027 7365 7373 696f 6e69  name': 'sessioni
+00001910: 6427 2c0a 2020 2020 2020 2020 2776 616c  d',.        'val
+00001920: 7565 273a 2027 2a2a 796f 7572 2073 6573  ue': '**your ses
+00001930: 7369 6f6e 2069 642a 2a27 2c0a 2020 2020  sion id**',.    
+00001940: 2020 2020 2764 6f6d 6169 6e27 3a20 2768      'domain': 'h
+00001950: 7474 7073 3a2f 2f74 696b 746f 6b2e 636f  ttps://tiktok.co
+00001960: 6d27 2c0a 2020 2020 2020 2020 2770 6174  m',.        'pat
+00001970: 6827 3a20 272f 272c 0a20 2020 2020 2020  h': '/',.       
+00001980: 2027 6578 7069 7279 273a 2027 3130 2f38   'expiry': '10/8
+00001990: 2f32 3032 332c 2031 323a 3138 3a35 3820  /2023, 12:18:58 
+000019a0: 504d 270a 2020 2020 7d0a 5d0a 0a75 706c  PM'.    }.]..upl
+000019b0: 6f61 645f 7669 6465 6f28 2e2e 2e2c 2063  oad_video(..., c
+000019c0: 6f6f 6b69 6573 5f6c 6973 743d 636f 6f6b  ookies_list=cook
+000019d0: 6965 735f 6c69 7374 290a 6060 600a 0a23  ies_list).```..#
+000019e0: 2320 f09f 9180 2042 726f 7773 6572 2053  # .... Browser S
+000019f0: 656c 6563 7469 6f6e 0a0a 5b47 6f6f 676c  election..[Googl
+00001a00: 6520 4368 726f 6d65 5d28 6874 7470 733a  e Chrome](https:
+00001a10: 2f2f 7777 772e 676f 6f67 6c65 2e63 6f6d  //www.google.com
+00001a20: 2f63 6872 6f6d 6529 2069 7320 7468 6520  /chrome) is the 
+00001a30: 7072 6566 6572 7265 6420 6272 6f77 7365  preferred browse
+00001a40: 7220 666f 7220 2a2a 5469 6b54 6f6b 5570  r for **TikTokUp
+00001a50: 6c6f 6164 6572 2a2a 2e20 5468 6520 6465  loader**. The de
+00001a60: 6661 756c 7420 616e 7469 2d64 6574 6563  fault anti-detec
+00001a70: 7469 6f6e 2074 6563 686e 6971 7565 7320  tion techniques 
+00001a80: 7573 6564 2069 6e20 7468 6973 2070 6163  used in this pac
+00001a90: 6b61 6765 6420 6172 6520 6f70 7469 6d69  kaged are optimi
+00001aa0: 7a65 6420 666f 7220 7468 6973 2e20 486f  zed for this. Ho
+00001ab0: 7765 7665 722c 2069 6620 796f 7520 7769  wever, if you wi
+00001ac0: 7368 2074 6f20 7573 6520 6120 6469 6666  sh to use a diff
+00001ad0: 6572 656e 7420 6272 6f77 7365 7220 796f  erent browser yo
+00001ae0: 7520 6d61 7920 7370 6563 6966 7920 7468  u may specify th
+00001af0: 6520 6062 726f 7773 6572 6020 696e 2060  e `browser` in `
+00001b00: 7570 6c6f 6164 5f76 6964 656f 6020 6f72  upload_video` or
+00001b10: 2060 7570 6c6f 6164 5f76 6964 656f 7360   `upload_videos`
+00001b20: 2e0a 0a60 6060 7079 7468 6f6e 0a66 726f  ...```python.fro
+00001b30: 6d20 7469 6b74 6f6b 5f75 706c 6f61 6465  m tiktok_uploade
+00001b40: 722e 7570 6c6f 6164 2069 6d70 6f72 7420  r.upload import 
+00001b50: 7570 6c6f 6164 5f76 6964 656f 0a0a 6672  upload_video..fr
+00001b60: 6f6d 2072 616e 646f 6d20 696d 706f 7274  om random import
+00001b70: 2063 686f 6963 650a 0a42 524f 5753 4552   choice..BROWSER
+00001b80: 5320 3d20 5b0a 2020 2020 2763 6872 6f6d  S = [.    'chrom
+00001b90: 6527 2c0a 2020 2020 2773 6166 6172 6927  e',.    'safari'
+00001ba0: 2c0a 2020 2020 2763 6872 6f6d 6975 6d27  ,.    'chromium'
+00001bb0: 2c0a 2020 2020 2765 6467 6527 2c0a 2020  ,.    'edge',.  
+00001bc0: 2020 2766 6972 6566 6f78 270a 5d0a 0a23    'firefox'.]..#
+00001bd0: 2072 616e 646f 6d6c 7920 7069 636b 7320   randomly picks 
+00001be0: 6120 7765 6220 6272 6f77 7365 7220 0a75  a web browser .u
+00001bf0: 706c 6f61 645f 7669 6465 6f28 2e2e 2e2c  pload_video(...,
+00001c00: 2062 726f 7773 6572 3d63 686f 6963 6528   browser=choice(
+00001c10: 4252 4f57 5345 5253 2929 0a60 6060 0a0a  BROWSERS)).```..
+00001c20: e29c 8520 5375 7070 6f72 7465 6420 4272  ... Supported Br
+00001c30: 6f77 7365 7273 3a0a 2d20 2a2a 4368 726f  owsers:.- **Chro
+00001c40: 6d65 2a2a 2028 5265 636f 6d6d 656e 6465  me** (Recommende
+00001c50: 6429 0a2d 202a 2a53 6166 6172 692a 2a0a  d).- **Safari**.
+00001c60: 2d20 2a2a 4368 726f 6d69 756d 2a2a 0a2d  - **Chromium**.-
+00001c70: 202a 2a45 6467 652a 2a0a 2d20 2a2a 4669   **Edge**.- **Fi
+00001c80: 7265 466f 782a 2a20 0a0a 2323 20f0 9f9a  reFox** ..## ...
+00001c90: b220 4375 7374 6f6d 2057 6562 4472 6976  . Custom WebDriv
+00001ca0: 6572 2044 7269 7665 7220 4f70 7469 6f6e  er Driver Option
+00001cb0: 730a 0a44 6566 6175 6c74 206d 6f64 6966  s..Default modif
+00001cc0: 6963 6174 696f 6e73 2074 6f20 5365 6c65  ications to Sele
+00001cd0: 6e69 756d 2061 7265 2061 7070 6c69 6564  nium are applied
+00001ce0: 2077 6869 6368 2068 656c 7020 6974 2061   which help it a
+00001cf0: 766f 6964 2062 6569 6e67 2064 6574 6563  void being detec
+00001d00: 7465 6420 6279 2054 696b 546f 6b2e 200a  ted by TikTok. .
+00001d10: 0a48 6f77 6576 6572 2c20 796f 7520 2a2a  .However, you **
+00001d20: 6d61 792a 2a20 7061 7373 2061 2063 7573  may** pass a cus
+00001d30: 746f 6d20 6472 6976 6572 2063 6f6e 6669  tom driver confi
+00001d40: 6775 7261 7469 6f6e 206f 7074 696f 6e73  guration options
+00001d50: 2e20 5369 6d70 6c79 2070 6173 7320 606f  . Simply pass `o
+00001d60: 7074 696f 6e73 6020 6173 2061 206b 6579  ptions` as a key
+00001d70: 776f 7264 2061 7267 756d 656e 7420 746f  word argument to
+00001d80: 2065 6974 6865 7220 6075 706c 6f61 645f   either `upload_
+00001d90: 7669 6465 6f60 206f 7220 6075 706c 6f61  video` or `uploa
+00001da0: 645f 7669 6465 6f73 602e 200a 0a60 6060  d_videos`. ..```
+00001db0: 7079 7468 6f6e 0a66 726f 6d20 7365 6c65  python.from sele
+00001dc0: 6e69 756d 2e77 6562 6472 6976 6572 2e63  nium.webdriver.c
+00001dd0: 6872 6f6d 652e 6f70 7469 6f6e 7320 696d  hrome.options im
+00001de0: 706f 7274 204f 7074 696f 6e73 0a0a 6f70  port Options..op
+00001df0: 7469 6f6e 7320 3d20 4f70 7469 6f6e 7328  tions = Options(
+00001e00: 290a 0a6f 7074 696f 6e73 2e61 6464 5f61  )..options.add_a
+00001e10: 7267 756d 656e 7428 2773 7461 7274 2d6d  rgument('start-m
+00001e20: 6178 696d 697a 6564 2729 0a0a 7570 6c6f  aximized')..uplo
+00001e30: 6164 5f76 6964 656f 7328 2e2e 2e2c 206f  ad_videos(..., o
+00001e40: 7074 696f 6e73 3d6f 7074 696f 6e73 290a  ptions=options).
+00001e50: 6060 600a 0a3e 204e 6f74 653a 204d 616b  ```..> Note: Mak
+00001e60: 6520 7375 7265 2074 6f20 7573 6520 7468  e sure to use th
+00001e70: 6520 7269 6768 7420 7365 6c65 6e69 756d  e right selenium
+00001e80: 206f 7074 696f 6e73 2066 6f72 2079 6f75   options for you
+00001e90: 7220 6272 6f77 7365 720a 0a23 2320 f09f  r browser..## ..
+00001ea0: a4af 2048 6561 646c 6573 7320 4272 6f77  .. Headless Brow
+00001eb0: 7365 7273 0a0a 4865 6164 6c65 7373 2062  sers..Headless b
+00001ec0: 726f 7773 696e 6720 6f6e 6c79 2077 6f72  rowsing only wor
+00001ed0: 6b73 206f 6e20 4368 726f 6d65 2e20 5768  ks on Chrome. Wh
+00001ee0: 656e 2075 7369 6e67 2043 6872 6f6d 652c  en using Chrome,
+00001ef0: 2061 6464 696e 6720 7468 6520 602d 2d68   adding the `--h
+00001f00: 6561 646c 6573 7360 2066 6c61 6720 7573  eadless` flag us
+00001f10: 696e 6720 7468 6520 434c 4920 6f72 2070  ing the CLI or p
+00001f20: 6173 7369 6e67 2060 6865 6164 6c65 7373  assing `headless
+00001f30: 6020 6173 2061 206b 6579 776f 7264 2061  ` as a keyword a
+00001f40: 7267 756d 656e 7420 746f 2060 7570 6c6f  rgument to `uplo
+00001f50: 6164 5f76 6964 656f 6020 6f72 2060 7570  ad_video` or `up
+00001f60: 6c6f 6164 5f76 6964 656f 7360 2069 7320  load_videos` is 
+00001f70: 616c 6c20 7468 6174 2069 7320 7265 7175  all that is requ
+00001f80: 6972 6564 2e0a 0a60 6060 7079 7468 6f6e  ired...```python
+00001f90: 0a75 706c 6f61 645f 7669 6465 6f28 2e2e  .upload_video(..
+00001fa0: 2e2c 2068 6561 646c 6573 733d 5472 7565  ., headless=True
+00001fb0: 290a 7570 6c6f 6164 5f76 6964 656f 7328  ).upload_videos(
+00001fc0: 2e2e 2e2c 2068 6561 646c 6573 733d 5472  ..., headless=Tr
+00001fd0: 7565 290a 6060 600a 0a23 2320 f09f 94a8  ue).```..## ....
+00001fe0: 2049 6e69 7469 616c 2053 6574 7570 0a0a   Initial Setup..
+00001ff0: 5b57 6562 4472 6976 6572 4d61 6e61 6765  [WebDriverManage
+00002000: 725d 2868 7474 7073 3a2f 2f62 6f6e 6967  r](https://bonig
+00002010: 6172 6369 612e 6465 762f 7765 6264 7269  arcia.dev/webdri
+00002020: 7665 726d 616e 6167 6572 2f29 2069 7320  vermanager/) is 
+00002030: 7573 6564 2074 6f20 6d61 6e61 6765 2064  used to manage d
+00002040: 7269 7665 7220 7665 7273 696f 6e73 2e20  river versions. 
+00002050: 0a0a 4f6e 2069 6e69 7469 616c 2073 7461  ..On initial sta
+00002060: 7274 7570 2c20 796f 7520 2a2a 6d61 792a  rtup, you **may*
+00002070: 2a20 6265 2070 726f 6d70 7465 6420 746f  * be prompted to
+00002080: 2069 6e73 7461 6c6c 2074 6865 2063 6f72   install the cor
+00002090: 7265 6374 2064 7269 7665 7220 666f 7220  rect driver for 
+000020a0: 796f 7572 2073 656c 6563 7465 6420 6272  your selected br
+000020b0: 6f77 7365 722e 2048 6f77 6576 6572 2c20  owser. However, 
+000020c0: 666f 7220 2a2a 4368 726f 6d65 2a2a 2061  for **Chrome** a
+000020d0: 6e64 202a 2a45 6467 652a 2a20 7468 6520  nd **Edge** the 
+000020e0: 6472 6976 6572 2069 7320 6175 746f 6d61  driver is automa
+000020f0: 7469 6361 6c6c 7920 696e 7374 616c 6c65  tically installe
+00002100: 642e 0a0a 2320 e299 bb20 4578 616d 706c  d...# ... Exampl
+00002110: 6573 0a0a 2d20 2a2a 5b42 6173 6963 2055  es..- **[Basic U
+00002120: 706c 6f61 6420 4578 616d 706c 655d 2865  pload Example](e
+00002130: 7861 6d70 6c65 732f 6261 7369 635f 7570  xamples/basic_up
+00002140: 6c6f 6164 2e70 7929 3a2a 2a20 5573 6573  load.py):** Uses
+00002150: 2060 7570 6c6f 6164 5f76 6964 656f 6020   `upload_video` 
+00002160: 746f 206d 616b 6520 6f6e 6520 706f 7374  to make one post
+00002170: 2e0a 0a2d 202a 2a5b 4d75 6c74 6970 6c65  ...- **[Multiple
+00002180: 2056 6964 656f 7320 4174 204f 6e63 655d   Videos At Once]
+00002190: 2865 7861 6d70 6c65 732f 6d75 6c74 6970  (examples/multip
+000021a0: 6c65 5f76 6964 656f 735f 6174 5f6f 6e63  le_videos_at_onc
+000021b0: 652e 7079 293a 2a2a 2055 706c 6f61 6473  e.py):** Uploads
+000021c0: 2074 6865 2073 616d 6520 7669 6465 6f20   the same video 
+000021d0: 6d75 6c74 6970 6c65 2074 696d 6573 2075  multiple times u
+000021e0: 7369 6e67 2060 7570 6c6f 6164 5f76 6964  sing `upload_vid
+000021f0: 656f 7360 2e0a 0a2d 202a 2a5b 5365 7269  eos`...- **[Seri
+00002200: 6573 2055 706c 6f61 6420 4578 616d 706c  es Upload Exampl
+00002210: 655d 2865 7861 6d70 6c65 732f 7365 7269  e](examples/seri
+00002220: 6573 5f75 706c 6f61 642e 7079 293a 2a2a  es_upload.py):**
+00002230: 2056 6964 656f 7320 6172 6520 7265 6164   Videos are read
+00002240: 2066 726f 6d20 6120 4353 5620 6669 6c65   from a CSV file
+00002250: 2075 7369 6e67 205b 5061 6e64 6173 5d28   using [Pandas](
+00002260: 6874 7470 733a 2f2f 7061 6e64 6173 2e70  https://pandas.p
+00002270: 7964 6174 612e 6f72 6729 2e20 4120 7669  ydata.org). A vi
+00002280: 6465 6f20 7570 6c6f 6164 2061 7474 656d  deo upload attem
+00002290: 7074 2069 7320 6d61 6465 2061 6e64 202a  pt is made and *
+000022a0: 2a69 6620 616e 6420 6f6e 6c79 2069 662a  *if and only if*
+000022b0: 2a20 6974 2069 7320 7375 6363 6573 7366  * it is successf
+000022c0: 756c 2077 696c 6c20 7468 6520 7669 6465  ul will the vide
+000022d0: 6f20 6265 206d 6172 6b65 6420 6173 2075  o be marked as u
+000022e0: 706c 6f61 6465 642e 0a0a 2320 f09f 939d  ploaded...# ....
+000022f0: 204e 6f74 6573 0a0a 5468 6973 2062 6f74   Notes..This bot
+00002300: 2069 7320 6e6f 7420 666f 6f6c 2070 726f   is not fool pro
+00002310: 6f66 2e20 5468 6f75 6768 2049 2068 6176  of. Though I hav
+00002320: 6520 6e6f 7420 676f 7474 656e 2061 6e20  e not gotten an 
+00002330: 6f66 6669 6369 616c 2062 616e 2c20 7468  official ban, th
+00002340: 6520 7669 6465 6f20 7769 6c6c 2066 6169  e video will fai
+00002350: 6c20 746f 2075 706c 6f61 6420 6166 7465  l to upload afte
+00002360: 7220 746f 6f20 6d61 6e79 2075 706c 6f61  r too many uploa
+00002370: 6473 2e20 496e 2074 6573 7469 6e67 2c20  ds. In testing, 
+00002380: 7761 6974 696e 6720 7365 7665 7261 6c20  waiting several 
+00002390: 686f 7572 7320 7761 7320 7375 6666 6963  hours was suffic
+000023a0: 6965 6e74 2074 6f20 6669 7820 7468 6973  ient to fix this
+000023b0: 2070 726f 626c 656d 2e20 466f 7220 7468   problem. For th
+000023c0: 6973 2072 6561 736f 6e2c 2070 6c65 6173  is reason, pleas
+000023d0: 6520 7468 696e 6720 6f66 2074 6869 7320  e thing of this 
+000023e0: 6d6f 7265 2061 7320 6120 7363 6865 6475  more as a schedu
+000023f0: 6c65 6420 7570 6c6f 6164 6572 2066 6f72  led uploader for
+00002400: 2054 696b 546f 6b20 7669 6465 6f73 2c20   TikTok videos, 
+00002410: 7261 7468 6572 2074 6861 6e20 6120 7370  rather than a sp
+00002420: 616d 2062 6f74 2e0a 0a23 2041 6363 6f75  am bot...# Accou
+00002430: 6e74 7320 6d61 6465 2077 6974 680a 0a2d  nts made with..-
+00002440: 205b 4043 5f53 7061 6e5d 2868 7474 7073   [@C_Span](https
+00002450: 3a2f 2f77 7777 2e74 696b 746f 6b2e 636f  ://www.tiktok.co
+00002460: 6d2f 4063 5f73 7061 6e3f 6c61 6e67 3d65  m/@c_span?lang=e
+00002470: 6e29 202d 2041 2073 706c 6974 2d73 6372  n) - A split-scr
+00002480: 6565 6e20 6368 616e 6e65 6c20 7769 7468  een channel with
+00002490: 206d 6f62 696c 6520 6761 6d65 7320 6265   mobile games be
+000024a0: 6c6f 7720 6665 6174 7572 696e 6720 636c  low featuring cl
+000024b0: 6970 7320 6672 6f6d 2043 2d53 7061 6e27  ips from C-Span'
+000024c0: 7320 596f 7554 7562 6520 6368 616e 6e65  s YouTube channe
+000024d0: 6c0a 2d20 5b40 6861 6269 745f 7472 6163  l.- [@habit_trac
+000024e0: 6b5d 2868 7474 7073 3a2f 2f77 7777 2e74  k](https://www.t
+000024f0: 696b 746f 6b2e 636f 6d2f 4068 6162 6974  iktok.com/@habit
+00002500: 5f74 7261 636b 3f6c 616e 673d 656e 2920  _track?lang=en) 
+00002510: 2d20 4120 5265 6464 6974 2062 6f74 2074  - A Reddit bot t
+00002520: 6f20 7365 6520 7768 6963 6820 5375 6252  o see which SubR
+00002530: 6564 6469 7420 6973 206d 6f73 7420 7669  eddit is most vi
+00002540: 7261 6c20 6f6e 2054 696b 546f 6b0a 0a5b  ral on TikTok..[
+00002550: 5e31 5d3a 2049 6620 696e 7465 7265 7374  ^1]: If interest
+00002560: 6564 2069 6e20 4861 7463 682c 2063 6865  ed in Hatch, che
+00002570: 636b 6f75 7420 7468 6520 5b77 6562 7369  ckout the [websi
+00002580: 7465 5d28 6874 7470 733a 2f2f 6861 7463  te](https://hatc
+00002590: 682e 7079 7061 2e69 6f2f 6c61 7465 7374  h.pypa.io/latest
+000025a0: 2f62 7569 6c64 2f29 0a                   /build/).
```


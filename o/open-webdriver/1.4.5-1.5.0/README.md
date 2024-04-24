# Comparing `tmp/open_webdriver-1.4.5.tar.gz` & `tmp/open_webdriver-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_webdriver-1.4.5.tar", last modified: Thu Feb  8 03:32:55 2024, max compression
+gzip compressed data, was "open_webdriver-1.5.0.tar", last modified: Wed Apr 24 22:39:55 2024, max compression
```

## Comparing `open_webdriver-1.4.5.tar` & `open_webdriver-1.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-02-08 03:32:55.467891 open_webdriver-1.4.5/
--rw-rw-rw-   0        0        0     1064 2023-06-19 02:37:47.000000 open_webdriver-1.4.5/LICENSE
--rw-rw-rw-   0        0        0      196 2023-06-19 02:37:47.000000 open_webdriver-1.4.5/MANIFEST.in
--rw-rw-rw-   0        0        0     8775 2024-02-08 03:32:55.467891 open_webdriver-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     7936 2024-02-08 03:32:21.000000 open_webdriver-1.4.5/README.md
-drwxrwxrwx   0        0        0        0 2024-02-08 03:32:55.456923 open_webdriver-1.4.5/open_webdriver/
--rw-rw-rw-   0        0        0      326 2023-06-19 02:37:48.000000 open_webdriver-1.4.5/open_webdriver/__init__.py
--rw-rw-rw-   0        0        0      416 2023-06-19 02:37:48.000000 open_webdriver-1.4.5/open_webdriver/demo_app.py
--rw-rw-rw-   0        0        0     4645 2024-02-07 23:58:04.000000 open_webdriver-1.4.5/open_webdriver/download_chromium.py
--rw-rw-rw-   0        0        0     3895 2024-02-08 03:30:58.000000 open_webdriver-1.4.5/open_webdriver/main.py
--rw-rw-rw-   0        0        0      272 2023-06-19 02:37:48.000000 open_webdriver-1.4.5/open_webdriver/path.py
-drwxrwxrwx   0        0        0        0 2024-02-08 03:32:55.465623 open_webdriver-1.4.5/open_webdriver/tests/
--rw-rw-rw-   0        0        0        0 2023-06-19 02:37:48.000000 open_webdriver-1.4.5/open_webdriver/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-08 03:32:55.466626 open_webdriver-1.4.5/open_webdriver/tests/unit/
--rw-rw-rw-   0        0        0        0 2023-06-19 02:37:48.000000 open_webdriver-1.4.5/open_webdriver/tests/unit/__init__.py
--rw-rw-rw-   0        0        0     1796 2023-06-19 02:37:48.000000 open_webdriver-1.4.5/open_webdriver/tests/unit/test_webdriver.py
--rw-rw-rw-   0        0        0       65 2024-02-08 03:31:44.000000 open_webdriver-1.4.5/open_webdriver/version.py
-drwxrwxrwx   0        0        0        0 2024-02-08 03:32:55.464622 open_webdriver-1.4.5/open_webdriver.egg-info/
--rw-rw-rw-   0        0        0     8775 2024-02-08 03:32:55.000000 open_webdriver-1.4.5/open_webdriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      587 2024-02-08 03:32:55.000000 open_webdriver-1.4.5/open_webdriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-08 03:32:55.000000 open_webdriver-1.4.5/open_webdriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-02-08 03:32:55.000000 open_webdriver-1.4.5/open_webdriver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      119 2024-02-08 03:32:55.000000 open_webdriver-1.4.5/open_webdriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-02-08 03:32:55.000000 open_webdriver-1.4.5/open_webdriver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       43 2023-06-19 02:37:48.000000 open_webdriver-1.4.5/requirements.testing.txt
--rw-rw-rw-   0        0        0      104 2024-02-07 22:54:45.000000 open_webdriver-1.4.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-02-08 03:32:55.468863 open_webdriver-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0     3124 2024-02-07 22:58:12.000000 open_webdriver-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:39:55.116387 open_webdriver-1.5.0/
+-rw-rw-rw-   0        0        0     1064 2023-06-19 02:37:47.000000 open_webdriver-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0      196 2023-06-19 02:37:47.000000 open_webdriver-1.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9167 2024-04-24 22:39:55.115388 open_webdriver-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8088 2024-04-24 22:38:30.000000 open_webdriver-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 22:39:55.097265 open_webdriver-1.5.0/open_webdriver/
+-rw-rw-rw-   0        0        0      326 2023-06-19 02:37:48.000000 open_webdriver-1.5.0/open_webdriver/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-06-19 02:37:48.000000 open_webdriver-1.5.0/open_webdriver/demo_app.py
+-rw-rw-rw-   0        0        0     4645 2024-02-07 23:58:04.000000 open_webdriver-1.5.0/open_webdriver/download_chromium.py
+-rw-rw-rw-   0        0        0     4015 2024-04-24 22:19:02.000000 open_webdriver-1.5.0/open_webdriver/main.py
+-rw-rw-rw-   0        0        0      272 2023-06-19 02:37:48.000000 open_webdriver-1.5.0/open_webdriver/path.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:39:55.108359 open_webdriver-1.5.0/open_webdriver/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-19 02:37:48.000000 open_webdriver-1.5.0/open_webdriver/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:39:55.111870 open_webdriver-1.5.0/open_webdriver/tests/unit/
+-rw-rw-rw-   0        0        0        0 2023-06-19 02:37:48.000000 open_webdriver-1.5.0/open_webdriver/tests/unit/__init__.py
+-rw-rw-rw-   0        0        0     1796 2023-06-19 02:37:48.000000 open_webdriver-1.5.0/open_webdriver/tests/unit/test_webdriver.py
+-rw-rw-rw-   0        0        0       65 2024-04-24 22:38:46.000000 open_webdriver-1.5.0/open_webdriver/version.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:39:55.113871 open_webdriver-1.5.0/open_webdriver.egg-info/
+-rw-rw-rw-   0        0        0     9167 2024-04-24 22:39:54.000000 open_webdriver-1.5.0/open_webdriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      587 2024-04-24 22:39:54.000000 open_webdriver-1.5.0/open_webdriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 22:39:54.000000 open_webdriver-1.5.0/open_webdriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-24 22:39:54.000000 open_webdriver-1.5.0/open_webdriver.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      101 2024-04-24 22:39:54.000000 open_webdriver-1.5.0/open_webdriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-24 22:39:54.000000 open_webdriver-1.5.0/open_webdriver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       43 2023-06-19 02:37:48.000000 open_webdriver-1.5.0/requirements.testing.txt
+-rw-rw-rw-   0        0        0       86 2024-04-24 22:20:24.000000 open_webdriver-1.5.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 22:39:55.116387 open_webdriver-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     3124 2024-02-07 22:58:12.000000 open_webdriver-1.5.0/setup.py
```

### Comparing `open_webdriver-1.4.5/LICENSE` & `open_webdriver-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open_webdriver-1.4.5/PKG-INFO` & `open_webdriver-1.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 Metadata-Version: 2.1
 Name: open_webdriver
-Version: 1.4.5
+Version: 1.5.0
 Summary: Easiest zero-config selenium webdriver for Python
 Home-page: https://github.com/zackees/open-webdriver
 Author: Zach Vorhies
 Author-email: dont@email.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Environment :: Console
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: webdriver-manager==4.0.1
+Requires-Dist: selenium==4.20.0
+Requires-Dist: download
+Requires-Dist: filelock
+Requires-Dist: py7zr==0.20.2
+Requires-Dist: certifi
+Requires-Dist: six
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 # open-webdriver
 
 ## The simplest and easiest way to get a scriptable chrome browser running using selenium webdriver.
 
 Note that this package uses a pinned dependency for urllib3 and should be installed in an isolated environment.
 
@@ -34,14 +42,15 @@
 import os
 from open_webdriver import open_webdriver
 # Needed or else exceptions will be thrown when executed from github actions.
 IS_HEADLESS = os.environ.get("GITHUB_ACTIONS") == "true"
 
 def main():
     with open_webdriver(headless=IS_HEADLESS) as driver:
+        driver.set_window_size(1440, 900) # Needed for headless mode.
         # All Chromium / web driver dependencies are now installed.
         driver.get("https://www.google.com")
         assert driver.title == "Google"
 
 if __name__ == "__main__":
     main()
 ```
@@ -134,14 +143,15 @@
 
 
 Pull requests are welcome for this code base. When you submit your pull request you will need to have the following:
   * New code must have a unit/test.
   * Must pass the linting requirements. Run `tox` (also run on your pull request).
 
 # Changes
+  * 1.5.0: Upgraded dependencies. No longer depends on ancient version of urllib.
   * 1.4.5: `Driver` returned from `open_webdriver` is now of WebDriver type instead of one of the base classes. Should help linting.
   * 1.4.4: Fixed nuitka build process with breaking dependencies introduced by python-dotenv 1.0.1
   * 1.4.3: Updated nuitka package and fixed breaking build from urllib3 update.
   * 1.4.2: Prints log if chrome driver fails to launch.
   * 1.4.1: Try and fix failed upload on last version.
   * 1.4.0: Adds default user agent string, fixes running headless mode which uses a different user agent string.
   * 1.3.6: Remove mac m1 runner, which doesn't exist on github
```

### Comparing `open_webdriver-1.4.5/README.md` & `open_webdriver-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import os
 from open_webdriver import open_webdriver
 # Needed or else exceptions will be thrown when executed from github actions.
 IS_HEADLESS = os.environ.get("GITHUB_ACTIONS") == "true"
 
 def main():
     with open_webdriver(headless=IS_HEADLESS) as driver:
+        driver.set_window_size(1440, 900) # Needed for headless mode.
         # All Chromium / web driver dependencies are now installed.
         driver.get("https://www.google.com")
         assert driver.title == "Google"
 
 if __name__ == "__main__":
     main()
 ```
@@ -114,14 +115,15 @@
 
 
 Pull requests are welcome for this code base. When you submit your pull request you will need to have the following:
   * New code must have a unit/test.
   * Must pass the linting requirements. Run `tox` (also run on your pull request).
 
 # Changes
+  * 1.5.0: Upgraded dependencies. No longer depends on ancient version of urllib.
   * 1.4.5: `Driver` returned from `open_webdriver` is now of WebDriver type instead of one of the base classes. Should help linting.
   * 1.4.4: Fixed nuitka build process with breaking dependencies introduced by python-dotenv 1.0.1
   * 1.4.3: Updated nuitka package and fixed breaking build from urllib3 update.
   * 1.4.2: Prints log if chrome driver fails to launch.
   * 1.4.1: Try and fix failed upload on last version.
   * 1.4.0: Adds default user agent string, fixes running headless mode which uses a different user agent string.
   * 1.3.6: Remove mac m1 runner, which doesn't exist on github
```

### Comparing `open_webdriver-1.4.5/open_webdriver/download_chromium.py` & `open_webdriver-1.5.0/open_webdriver/download_chromium.py`

 * *Files identical despite different names*

### Comparing `open_webdriver-1.4.5/open_webdriver/main.py` & `open_webdriver-1.5.0/open_webdriver/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 import filelock  # type: ignore
 import urllib3  # type: ignore
 from selenium import webdriver  # type: ignore
 from selenium.webdriver import ChromeOptions  # type: ignore
 from selenium.webdriver.remote.webdriver import WebDriver as Driver  # type: ignore
 from webdriver_manager.chrome import ChromeDriverManager  # type: ignore
+from webdriver_manager.core.driver_cache import DriverCacheManager
 
 from open_webdriver.download_chromium import get_chromium_exe
 from open_webdriver.path import LOG_FILE, WDM_DIR
 
 urllib3.disable_warnings()
 
 ssl._create_default_https_context = ssl._create_unverified_context
@@ -79,26 +80,27 @@
     lock = filelock.FileLock(LOCK_FILE)
     with lock.acquire(timeout=timeout):
         if verbose:
             print("  Installing web driver...")
         chromium_exe = get_chromium_exe()
         if verbose:
             print("  Finished installing web driver: ", chromium_exe)
+        cache_manager = DriverCacheManager(
+            root_dir=WDM_DIR, valid_range=CACHE_TIMEOUT_DAYS
+        )
         opts.binary_location = chromium_exe
         driver_path = ChromeDriverManager(
-            cache_valid_range=CACHE_TIMEOUT_DAYS, version=CHROME_VERSION, path=WDM_DIR
+            cache_manager=cache_manager, driver_version=CHROME_VERSION
         ).install()
     if verbose:
         print(f"\n  Using ChromeDriver: {driver_path}")
     try:
         if os.path.exists(LOG_FILE):
             os.remove(LOG_FILE)
-        driver = webdriver.Chrome(
-            executable_path=driver_path, options=opts, service_log_path=LOG_FILE
-        )
+        driver = webdriver.Chrome(options=opts)  # , service_log_path=LOG_FILE)
         return driver
     except Exception as err:  # pylint: disable=broad-except
         traceback.print_exc()
         log_file_text = ""
         if os.path.exists(LOG_FILE):
             with open(LOG_FILE, encoding="utf-8", mode="r") as filed:
                 log_file_text = filed.read()
```

### Comparing `open_webdriver-1.4.5/open_webdriver/tests/unit/test_webdriver.py` & `open_webdriver-1.5.0/open_webdriver/tests/unit/test_webdriver.py`

 * *Files identical despite different names*

### Comparing `open_webdriver-1.4.5/open_webdriver.egg-info/PKG-INFO` & `open_webdriver-1.5.0/open_webdriver.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 Metadata-Version: 2.1
-Name: open-webdriver
-Version: 1.4.5
+Name: open_webdriver
+Version: 1.5.0
 Summary: Easiest zero-config selenium webdriver for Python
 Home-page: https://github.com/zackees/open-webdriver
 Author: Zach Vorhies
 Author-email: dont@email.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Environment :: Console
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: webdriver-manager==4.0.1
+Requires-Dist: selenium==4.20.0
+Requires-Dist: download
+Requires-Dist: filelock
+Requires-Dist: py7zr==0.20.2
+Requires-Dist: certifi
+Requires-Dist: six
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 # open-webdriver
 
 ## The simplest and easiest way to get a scriptable chrome browser running using selenium webdriver.
 
 Note that this package uses a pinned dependency for urllib3 and should be installed in an isolated environment.
 
@@ -34,14 +42,15 @@
 import os
 from open_webdriver import open_webdriver
 # Needed or else exceptions will be thrown when executed from github actions.
 IS_HEADLESS = os.environ.get("GITHUB_ACTIONS") == "true"
 
 def main():
     with open_webdriver(headless=IS_HEADLESS) as driver:
+        driver.set_window_size(1440, 900) # Needed for headless mode.
         # All Chromium / web driver dependencies are now installed.
         driver.get("https://www.google.com")
         assert driver.title == "Google"
 
 if __name__ == "__main__":
     main()
 ```
@@ -134,14 +143,15 @@
 
 
 Pull requests are welcome for this code base. When you submit your pull request you will need to have the following:
   * New code must have a unit/test.
   * Must pass the linting requirements. Run `tox` (also run on your pull request).
 
 # Changes
+  * 1.5.0: Upgraded dependencies. No longer depends on ancient version of urllib.
   * 1.4.5: `Driver` returned from `open_webdriver` is now of WebDriver type instead of one of the base classes. Should help linting.
   * 1.4.4: Fixed nuitka build process with breaking dependencies introduced by python-dotenv 1.0.1
   * 1.4.3: Updated nuitka package and fixed breaking build from urllib3 update.
   * 1.4.2: Prints log if chrome driver fails to launch.
   * 1.4.1: Try and fix failed upload on last version.
   * 1.4.0: Adds default user agent string, fixes running headless mode which uses a different user agent string.
   * 1.3.6: Remove mac m1 runner, which doesn't exist on github
```

### Comparing `open_webdriver-1.4.5/open_webdriver.egg-info/SOURCES.txt` & `open_webdriver-1.5.0/open_webdriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open_webdriver-1.4.5/setup.py` & `open_webdriver-1.5.0/setup.py`

 * *Files identical despite different names*


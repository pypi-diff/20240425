# Comparing `tmp/discover-overlay-0.7.3.tar.gz` & `tmp/discover_overlay-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discover-overlay-0.7.3.tar", last modified: Wed Apr  3 21:45:23 2024, max compression
+gzip compressed data, was "discover_overlay-0.7.4.tar", last modified: Wed Apr 24 23:31:01 2024, max compression
```

## Comparing `discover-overlay-0.7.3.tar` & `discover_overlay-0.7.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.012823 discover-overlay-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-04-03 21:45:23.012823 discover-overlay-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover-overlay-default.png
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover-overlay-default.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover-overlay-tray.png
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover-overlay-tray.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover-overlay.png
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover-overlay.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.008823 discover-overlay-0.7.3/discover_overlay/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/audio_assist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/autostart.py
--rw-r--r--   0 runner    (1001) docker     (127)    30399 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/discord_connector.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23229 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/discover_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/draggable_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/draggable_window_wayland.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.008823 discover-overlay-0.7.3/discover_overlay/glade/
--rw-r--r--   0 runner    (1001) docker     (127)   128883 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/glade/settings.glade
--rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/image_getter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.004823 discover-overlay-0.7.3/discover_overlay/locales/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.004823 discover-overlay-0.7.3/discover_overlay/locales/cy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.008823 discover-overlay-0.7.3/discover_overlay/locales/cy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/locales/cy/LC_MESSAGES/default.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.004823 discover-overlay-0.7.3/discover_overlay/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.008823 discover-overlay-0.7.3/discover_overlay/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/locales/de/LC_MESSAGES/default.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.004823 discover-overlay-0.7.3/discover_overlay/locales/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.008823 discover-overlay-0.7.3/discover_overlay/locales/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/locales/en/LC_MESSAGES/default.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.004823 discover-overlay-0.7.3/discover_overlay/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.012823 discover-overlay-0.7.3/discover_overlay/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/locales/fr/LC_MESSAGES/default.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.004823 discover-overlay-0.7.3/discover_overlay/locales/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.012823 discover-overlay-0.7.3/discover_overlay/locales/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/locales/tr/LC_MESSAGES/default.mo
--rw-r--r--   0 runner    (1001) docker     (127)    19938 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/notification_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)    16667 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)    55041 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/settings_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    13788 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/text_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)    43733 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/voice_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay.desktop
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.012823 discover-overlay-0.7.3/discover_overlay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-04-03 21:45:22.000000 discover-overlay-0.7.3/discover_overlay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-03 21:45:22.000000 discover-overlay-0.7.3/discover_overlay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:45:22.000000 discover-overlay-0.7.3/discover_overlay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 21:45:22.000000 discover-overlay-0.7.3/discover_overlay.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 21:45:22.000000 discover-overlay-0.7.3/discover_overlay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 21:45:22.000000 discover-overlay-0.7.3/discover_overlay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay_configure.desktop
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 21:45:23.012823 discover-overlay-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:31:01.304898 discover_overlay-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-04-24 23:31:01.304898 discover_overlay-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover-overlay-default.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover-overlay-default.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover-overlay-tray.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover-overlay-tray.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover-overlay.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover-overlay.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:31:01.300898 discover_overlay-0.7.4/discover_overlay/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover_overlay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover_overlay/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover_overlay/audio_assist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover_overlay/autostart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30399 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover_overlay/discord_connector.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23469 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover_overlay/discover_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover_overlay/draggable_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover_overlay/draggable_window_wayland.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:31:01.300898 discover_overlay-0.7.4/discover_overlay/glade/
+-rw-r--r--   0 runner    (1001) docker     (127)   128883 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover_overlay/glade/settings.glade
+-rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover_overlay/image_getter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:31:01.296898 discover_overlay-0.7.4/discover_overlay/locales/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:31:01.292898 discover_overlay-0.7.4/discover_overlay/locales/cy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:31:01.300898 discover_overlay-0.7.4/discover_overlay/locales/cy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover_overlay/locales/cy/LC_MESSAGES/default.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:31:01.292898 discover_overlay-0.7.4/discover_overlay/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:31:01.300898 discover_overlay-0.7.4/discover_overlay/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover_overlay/locales/de/LC_MESSAGES/default.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:31:01.292898 discover_overlay-0.7.4/discover_overlay/locales/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:31:01.300898 discover_overlay-0.7.4/discover_overlay/locales/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover_overlay/locales/en/LC_MESSAGES/default.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:31:01.296898 discover_overlay-0.7.4/discover_overlay/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:31:01.300898 discover_overlay-0.7.4/discover_overlay/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover_overlay/locales/fr/LC_MESSAGES/default.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:31:01.296898 discover_overlay-0.7.4/discover_overlay/locales/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:31:01.300898 discover_overlay-0.7.4/discover_overlay/locales/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover_overlay/locales/tr/LC_MESSAGES/default.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    20309 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover_overlay/notification_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17200 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover_overlay/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56132 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover_overlay/settings_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14403 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover_overlay/text_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43903 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover_overlay/voice_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover_overlay.desktop
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:31:01.304898 discover_overlay-0.7.4/discover_overlay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-04-24 23:31:01.000000 discover_overlay-0.7.4/discover_overlay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-24 23:31:01.000000 discover_overlay-0.7.4/discover_overlay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 23:31:01.000000 discover_overlay-0.7.4/discover_overlay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-24 23:31:01.000000 discover_overlay-0.7.4/discover_overlay.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-24 23:31:01.000000 discover_overlay-0.7.4/discover_overlay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 23:31:01.000000 discover_overlay-0.7.4/discover_overlay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/discover_overlay_configure.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 23:31:01.304898 discover_overlay-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-24 23:30:50.000000 discover_overlay-0.7.4/setup.py
```

### Comparing `discover-overlay-0.7.3/LICENSE` & `discover_overlay-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.3/PKG-INFO` & `discover_overlay-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discover-overlay
-Version: 0.7.3
+Version: 0.7.4
 Summary: Voice chat overlay
 Home-page: https://github.com/trigg/Discover
 Author: trigg
 Author-email: 
 License: GPLv3+
 Keywords: discord overlay voice linux
 Classifier: Development Status :: 4 - Beta
```

### Comparing `discover-overlay-0.7.3/README.md` & `discover_overlay-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.3/discover-overlay-default.png` & `discover_overlay-0.7.4/discover-overlay-default.png`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.3/discover-overlay-default.svg` & `discover_overlay-0.7.4/discover-overlay-default.svg`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.3/discover-overlay-tray.png` & `discover_overlay-0.7.4/discover-overlay-tray.png`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.3/discover-overlay-tray.svg` & `discover_overlay-0.7.4/discover-overlay-tray.svg`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.3/discover-overlay.png` & `discover_overlay-0.7.4/discover-overlay.png`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.3/discover-overlay.svg` & `discover_overlay-0.7.4/discover-overlay.svg`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.3/discover_overlay/__init__.py` & `discover_overlay-0.7.4/discover_overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.3/discover_overlay/__main__.py` & `discover_overlay-0.7.4/discover_overlay/__main__.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.3/discover_overlay/audio_assist.py` & `discover_overlay-0.7.4/discover_overlay/audio_assist.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,29 +88,31 @@
         for sink in await pulse.sink_list():
             if sink.description == self.sink:
                 if sink.mute == 1 or sink.volume.values[0] == 0.0:
                     deaf = True
                 elif sink.mute == 0:
                     deaf = False
 
+        if deaf != self.last_set_deaf:
+            self.last_set_deaf = deaf
+            self.discover.set_deaf_async(deaf)
+            self.last_set_mute = None
+            # At this point mute is undefined state
+
         for source in await pulse.source_list():
             if source.description == self.source:
                 if source.mute == 1 or source.volume.values[0] == 0.0:
                     mute = True
                 elif sink.mute == 0:
                     mute = False
 
         if mute != self.last_set_mute:
             self.last_set_mute = mute
             self.discover.set_mute_async(mute)
 
-        if deaf != self.last_set_deaf:
-            self.last_set_deaf = deaf
-            self.discover.set_deaf_async(deaf)
-
     async def print_events(self, pulse, ev):
         if not self.enabled:
             return
         # Sink and Source events are fired for changes to output and ints
         # Server is fired when default sink or source changes.
         match ev.facility:
             case 'sink':
```

### Comparing `discover-overlay-0.7.3/discover_overlay/autostart.py` & `discover_overlay-0.7.4/discover_overlay/autostart.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.3/discover_overlay/discord_connector.py` & `discover_overlay-0.7.4/discover_overlay/discord_connector.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.3/discover_overlay/discover_overlay.py` & `discover_overlay-0.7.4/discover_overlay/discover_overlay.py`

 * *Files 4% similar despite different names*

```diff
@@ -237,18 +237,18 @@
         except:
             pass
         self.voice_overlay.set_vert_edge_padding(config.getint(
             "main", "vert_edge_padding", fallback=0))
         self.voice_overlay.set_horz_edge_padding(config.getint(
             "main", "horz_edge_padding", fallback=0))
         floating = config.getboolean("main", "floating", fallback=False)
-        floating_x = config.getint("main", "floating_x", fallback=0)
-        floating_y = config.getint("main", "floating_y", fallback=0)
-        floating_w = config.getint("main", "floating_w", fallback=400)
-        floating_h = config.getint("main", "floating_h", fallback=400)
+        floating_x = config.getfloat("main", "floating_x", fallback=0.0)
+        floating_y = config.getfloat("main", "floating_y", fallback=0.0)
+        floating_w = config.getfloat("main", "floating_w", fallback=0.1)
+        floating_h = config.getfloat("main", "floating_h", fallback=0.1)
         self.voice_overlay.set_order(
             config.getint("main", "order", fallback=0))
         self.voice_overlay.set_hide_on_mouseover(
             config.getboolean("main", "autohide", fallback=False))
         self.voice_overlay.set_mouseover_timer(
             config.getint("main", "autohide_timer", fallback=1))
 
@@ -305,18 +305,18 @@
             config.getint("text", "topalign", fallback=2))
         monitor = 0
         try:
             monitor = config.getint("text", "monitor", fallback=0)
         except:
             pass
         floating = config.getboolean("text", "floating", fallback=True)
-        floating_x = config.getint("text", "floating_x", fallback=0)
-        floating_y = config.getint("text", "floating_y", fallback=0)
-        floating_w = config.getint("text", "floating_w", fallback=400)
-        floating_h = config.getint("text", "floating_h", fallback=400)
+        floating_x = config.getfloat("text", "floating_x", fallback=0.0)
+        floating_y = config.getfloat("text", "floating_y", fallback=0.0)
+        floating_w = config.getfloat("text", "floating_w", fallback=0.1)
+        floating_h = config.getfloat("text", "floating_h", fallback=0.1)
 
         channel = config.get("text", "channel", fallback="0")
         guild = config.get("text", "guild", fallback="0")
         self.connection.set_text_channel(channel, guild)
 
         self.font = config.get("text", "font", fallback=None)
         self.text_overlay.set_bg(json.loads(config.get(
@@ -353,22 +353,22 @@
         monitor = 0
         try:
             monitor = config.getint("notification", "monitor", fallback=0)
         except:
             pass
         floating = config.getboolean(
             "notification", "floating", fallback=False)
-        floating_x = config.getint(
-            "notification", "floating_x", fallback=0)
-        floating_y = config.getint(
-            "notification", "floating_y", fallback=0)
-        floating_w = config.getint(
-            "notification", "floating_w", fallback=400)
-        floating_h = config.getint(
-            "notification", "floating_h", fallback=400)
+        floating_x = config.getfloat(
+            "notification", "floating_x", fallback=0.0)
+        floating_y = config.getfloat(
+            "notification", "floating_y", fallback=0.0)
+        floating_w = config.getfloat(
+            "notification", "floating_w", fallback=0.1)
+        floating_h = config.getfloat(
+            "notification", "floating_h", fallback=0.1)
         font = config.get("notification", "font", fallback=None)
         self.notification_overlay.set_bg(json.loads(config.get(
             "notification", "bg_col", fallback="[0.0,0.0,0.0,0.5]")))
         self.notification_overlay.set_fg(json.loads(config.get(
             "notification", "fg_col", fallback="[1.0,1.0,1.0,1.0]")))
         self.notification_overlay.set_text_time(config.getint(
             "notification", "text_time", fallback=10))
@@ -514,14 +514,19 @@
         logging.basicConfig(filename=debug_file, format=FORMAT)
     else:
         logging.basicConfig(format=FORMAT)
     log = logging.getLogger(__name__)
     log.info("Starting Discover Overlay: %s",
              pkg_resources.get_distribution('discover_overlay').version)
 
+    # Hedge against the bet gamescope ships with some WAYLAND_DISPLAY
+    # Compatibility and we're not ready yet
+    if 'GAMESCOPE_WAYLAND_DISPLAY' in os.environ:
+        os.unsetenv("WAYLAND_DISPLAY")
+
     # Catch any errors and log them
     try:
         if "--rpc" in sys.argv:
             # Send command to overlay
             line = ""
             for arg in sys.argv[1:]:
                 line = "%s %s" % (line, arg)
```

### Comparing `discover-overlay-0.7.3/discover_overlay/draggable_window.py` & `discover_overlay-0.7.4/discover_overlay/draggable_window.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,20 +20,22 @@
 
 log = logging.getLogger(__name__)
 
 
 class DraggableWindow(Gtk.Window):
     """An X11 window which can be moved and resized"""
 
-    def __init__(self, pos_x=0, pos_y=0, width=300, height=300, message="Message", settings=None):
+    def __init__(self, pos_x=0.0, pos_y=0.0, width=0.1, height=0.1, message="Message", settings=None, monitor=None):
         Gtk.Window.__init__(self, type=Gtk.WindowType.POPUP)
-        self.pos_x = pos_x
-        self.pos_y = pos_y
-        self.width = max(100, width)
-        self.height = max(100, height)
+        self.monitor = monitor
+        (screen_x, screen_y, screen_width, screen_height) = self.get_display_coords()
+        self.pos_x = pos_x * screen_width
+        self.pos_y = pos_y * screen_height
+        self.width = max(40, width * screen_width)
+        self.height = max(40, height * screen_height)
         self.settings = settings
         self.message = message
         self.set_size_request(50, 50)
 
         self.connect('draw', self.dodraw)
         self.connect('motion-notify-event', self.drag)
         self.connect('button-press-event', self.button_press)
@@ -46,51 +48,62 @@
         if visual:
             # Set the visual even if we can't use it right now
             self.set_visual(visual)
         if screen.is_composited():
             self.compositing = True
 
         self.set_app_paintable(True)
-        self.monitor = 0
 
         self.drag_type = None
         self.drag_x = 0
         self.drag_y = 0
         self.force_location()
         self.show_all()
 
     def force_location(self):
         """
         Move the window to previously given co-ords.
         Also double check sanity on layer & decorations
         """
         self.set_decorated(False)
         self.set_keep_above(True)
-        self.move(self.pos_x, self.pos_y)
+
+        (screen_x, screen_y, screen_width, screen_height) = self.get_display_coords()
+
+        self.width = min(self.width, screen_width)
+        self.height = min(self.height, screen_height)
+        self.pos_x = max(0, self.pos_x)
+        self.pos_x = min(screen_width - self.width, self.pos_x)
+        self.pos_y = max(0, self.pos_y)
+        self.pos_y = min(screen_height - self.height, self.pos_y)
+
+        self.move(self.pos_x + screen_x, self.pos_y + screen_y)
         self.resize(self.width, self.height)
 
     def drag(self, _w, event):
         """Called by GTK while mouse is moving over window. Used to resize and move"""
         if event.state & Gdk.ModifierType.BUTTON1_MASK:
             if self.drag_type == 1:
                 # Center is move
-                self.pos_x = event.x_root - self.drag_x
-                self.pos_y = event.y_root - self.drag_y
+                (screen_x, screen_y, screen_width,
+                 screen_height) = self.get_display_coords()
+                self.pos_x = (event.x_root - screen_x) - self.drag_x
+                self.pos_y = (event.y_root - screen_y) - self.drag_y
                 self.force_location()
             elif self.drag_type == 2:
                 # Right edge
                 self.width += event.x - self.drag_x
                 self.drag_x = event.x
                 self.force_location()
             elif self.drag_type == 3:
                 # Bottom edge
                 self.height += event.y - self.drag_y
                 self.drag_y = event.y
                 self.force_location()
-            else:
+            elif self.drag_type == 4:
                 # Bottom Right
                 self.width += event.x - self.drag_x
                 self.height += event.y - self.drag_y
                 self.drag_x = event.x
                 self.drag_y = event.y
                 self.force_location()
 
@@ -133,15 +146,29 @@
         context.set_source_rgba(0.0, 0.0, 1.0, 0.5)
         context.rectangle(window_width - 32, 0, 32, window_height)
         context.fill()
 
         context.rectangle(0, window_height - 32, window_width, 32)
         context.fill()
 
+    def get_display_coords(self):
+        display = Gdk.Display.get_default()
+        if "get_monitor" in dir(display):
+            monitor = display.get_monitor(self.monitor)
+            if monitor:
+                geometry = monitor.get_geometry()
+                return (geometry.x, geometry.y, geometry.width, geometry.height)
+        return (0, 0, 1920, 1080)  # We're in trouble
+
     def get_coords(self):
         """Return window position and size"""
+        (screen_x, screen_y, screen_width, screen_height) = self.get_display_coords()
         scale = self.get_scale_factor()
         (pos_x, pos_y) = self.get_position()
+        pos_x = float(max(0, pos_x - screen_x))
+        pos_y = float(max(0, pos_y - screen_y))
         (width, height) = self.get_size()
+        width = float(width)
+        height = float(height)
         pos_x = pos_x / scale
         pos_y = pos_y / scale
-        return (pos_x, pos_y, width, height)
+        return (pos_x / screen_width, pos_y / screen_height, width / screen_width, height / screen_height)
```

### Comparing `discover-overlay-0.7.3/discover_overlay/glade/settings.glade` & `discover_overlay-0.7.4/discover_overlay/glade/settings.glade`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.3/discover_overlay/image_getter.py` & `discover_overlay-0.7.4/discover_overlay/image_getter.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.3/discover_overlay/locales/cy/LC_MESSAGES/default.mo` & `discover_overlay-0.7.4/discover_overlay/locales/cy/LC_MESSAGES/default.mo`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.3/discover_overlay/locales/de/LC_MESSAGES/default.mo` & `discover_overlay-0.7.4/discover_overlay/locales/de/LC_MESSAGES/default.mo`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.3/discover_overlay/locales/fr/LC_MESSAGES/default.mo` & `discover_overlay-0.7.4/discover_overlay/locales/fr/LC_MESSAGES/default.mo`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.3/discover_overlay/locales/tr/LC_MESSAGES/default.mo` & `discover_overlay-0.7.4/discover_overlay/locales/tr/LC_MESSAGES/default.mo`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.3/discover_overlay/notification_overlay.py` & `discover_overlay-0.7.4/discover_overlay/notification_overlay.py`

 * *Files 5% similar despite different names*

```diff
@@ -254,15 +254,17 @@
         else:
             m_with_body = "<span>%s</span>"
             message = m_with_body % (self.sanitize_string(line["title"]))
         layout = self.create_pango_layout(message)
         layout.set_auto_dir(True)
         layout.set_markup(message, -1)
         attr = layout.get_attributes()
-        width = self.limit_width if self.width > self.limit_width else self.width
+        (floating_x, floating_y, floating_width,
+         floating_height) = self.get_floating_coords()
+        width = self.limit_width if floating_width > self.limit_width else floating_width
         layout.set_width((Pango.SCALE * (width -
                          (self.border_radius * 4 + icon_width + icon_pad))))
         layout.set_spacing(Pango.SCALE * 3)
         if self.text_font:
             font = Pango.FontDescription(self.text_font)
             layout.set_font_description(font)
         text_width, text_height = layout.get_pixel_size()
@@ -300,19 +302,21 @@
         self.tick()
         context.save()
         if self.is_wayland or self.piggyback_parent or self.discover.steamos:
             # Special case!
             # The window is full-screen regardless of what the user has selected.
             # We need to set a clip and a transform to imitate original behaviour
             # Used in wlroots & gamescope
-            width = self.width
-            height = self.height
-            context.translate(self.pos_x, self.pos_y)
-            context.rectangle(0, 0, width, height)
-            context.clip()
+            (floating_x, floating_y, floating_width,
+             floating_height) = self.get_floating_coords()
+            if self.floating:
+                context.new_path()
+                context.translate(floating_x, floating_y)
+                context.rectangle(0, 0, floating_width, floating_height)
+                context.clip()
 
         current_y = height
         if self.align_vert == 0:
             current_y = 0
         if self.align_vert == 1:  # Center. Oh god why
             current_y = (height/2.0) - (self.calc_all_height() / 2.0)
         tnow = time.time()
@@ -363,15 +367,17 @@
             icon_width = 0
 
         layout = self.create_pango_layout(text)
         layout.set_auto_dir(True)
         layout.set_markup(text, -1)
         attr = layout.get_attributes()
 
-        width = self.limit_width if self.width > self.limit_width else self.width
+        (floating_x, floating_y, floating_width,
+         floating_height) = self.get_floating_coords()
+        width = self.limit_width if floating_width > self.limit_width else floating_width
         layout.set_width((Pango.SCALE * (width -
                          (self.border_radius * 4 + icon_width + icon_pad))))
         layout.set_spacing(Pango.SCALE * 3)
         if self.text_font:
             font = Pango.FontDescription(self.text_font)
             layout.set_font_description(font)
         text_width, text_height = layout.get_pixel_size()
@@ -384,15 +390,15 @@
         if text_height < icon_width:
             text_height = icon_width
         shape_height = text_height + self.border_radius * 4
         shape_width = text_width + self.border_radius*4 + icon_width + icon_pad
 
         left = 0
         if self.align_right:
-            left = self.width - shape_width
+            left = floating_width - shape_width
 
         self.context.save()
         # Draw Background
         self.context.translate(left, top)
         # self.context.rectangle(self.border_radius, 0,
         #                       shape_width - (self.border_radius*2), shape_height)
         # self.context.fill()
```

### Comparing `discover-overlay-0.7.3/discover_overlay/overlay.py` & `discover_overlay-0.7.4/discover_overlay/overlay.py`

 * *Files 4% similar despite different names*

```diff
@@ -218,18 +218,28 @@
             self.text_font = font
             self.set_needs_redraw()
 
     def set_floating(self, floating, pos_x, pos_y, width, height):
         """
         Set if the window is floating and what dimensions to use
         """
+        if width > 1.0 and height > 1.0:
+            # Old data.
+            (screen_x, screen_y, screen_width,
+             screen_height) = self.get_display_coords()
+            pos_x = float(pos_x) / screen_width
+            pos_y = float(pos_y) / screen_height
+            width = float(width) / screen_width
+            height = float(height) / screen_height
+
         if self.floating != floating or self.pos_x != pos_x or self.pos_y != pos_y or self.width != width or self.height != height:
             # Special case for Cinnamon desktop : see https://github.com/trigg/Discover/issues/322
             if 'XDG_SESSION_DESKTOP' in os.environ and os.environ['XDG_SESSION_DESKTOP'] == 'cinnamon':
                 floating = True
+
             self.floating = floating
             self.pos_x = pos_x
             self.pos_y = pos_y
             self.width = width
             self.height = height
             self.force_location()
 
@@ -268,59 +278,61 @@
     def force_location(self):
         """
         On X11 enforce the location and sane defaults
         On Wayland just store for later
         On Gamescope enforce size of display but only if it's the primary overlay
         """
         if self.discover.steamos and not self.piggyback_parent:
-            display = Gdk.Display.get_default()
-            if "get_monitor" in dir(display):
-                monitor = display.get_monitor(self.monitor)
-                if monitor:
-                    geometry = monitor.get_geometry()
-                    scale_factor = monitor.get_scale_factor()
-                    width = geometry.width
-                    height = geometry.height
-                    self.resize(width, height)
-                    self.set_needs_redraw()
-                return
+            (floating_x, floating_y, floating_width,
+             floating_height) = self.get_floating_coords()
+            self.resize(floating_width, floating_height)
+            self.set_needs_redraw()
+            return
         if not self.is_wayland:
             self.set_decorated(False)
             self.set_keep_above(True)
-            display = Gdk.Display.get_default()
-            if "get_monitor" in dir(display):
-                monitor = display.get_monitor(self.monitor)
-                if monitor:
-                    geometry = monitor.get_geometry()
-                    scale_factor = monitor.get_scale_factor()
-                    if not self.floating:
-                        width = geometry.width
-                        height = geometry.height
-                        pos_x = geometry.x
-                        pos_y = geometry.y
-                        self.resize(width, height)
-                        self.move(pos_x, pos_y)
-                    else:
-                        self.move(self.pos_x, self.pos_y)
-                        self.resize(self.width, self.height)
-            else:
-                if self.floating:
-                    self.move(self.pos_x, self.pos_y)
-                    self.resize(self.width, self.height)
 
-        if not self.floating:
-            (width, height) = self.get_size()
-            self.width = width
-            self.height = height
+            (floating_x, floating_y, floating_width,
+             floating_height) = self.get_floating_coords()
+            self.resize(floating_width, floating_height)
+            self.move(floating_x, floating_y)
+
         self.set_needs_redraw()
 
-    def set_needs_redraw(self):
-        if not self.hidden and self.enabled:
+    def get_display_coords(self):
+        if self.piggyback_parent:
+            return self.piggyback_parent.get_display_coords()
+        display = Gdk.Display.get_default()
+        if "get_monitor" in dir(display):
+            if self.monitor == None or self.monitor < 0:
+                monitor = display.get_monitor(0)
+            else:
+                monitor = display.get_monitor(self.monitor)
+            if monitor:
+                geometry = monitor.get_geometry()
+                return (geometry.x, geometry.y, geometry.width, geometry.height)
+        log.warn("No monitor found! This is going to go badly")
+        return (0, 0, 1920, 1080)  # We're in trouble
+
+    def get_floating_coords(self):
+        (screen_x, screen_y, screen_width, screen_height) = self.get_display_coords()
+        if self.floating:
+            if self.pos_x == None or self.pos_y == None or self.width == None or self.height == None:
+                log.error("No usable floating position")
+
+            if not self.is_wayland:
+                return (screen_x + self.pos_x * screen_width, screen_y + self.pos_y * screen_height, self.width * screen_width, self.height * screen_height)
+            return (self.pos_x * screen_width, self.pos_y * screen_height, self.width * screen_width, self.height * screen_height)
+        else:
+            return (0, 0, screen_width, screen_height)
+
+    def set_needs_redraw(self, be_pushy=False):
+        if (not self.hidden and self.enabled) or be_pushy:
             if self.piggyback_parent:
-                self.piggyback_parent.set_needs_redraw()
+                self.piggyback_parent.set_needs_redraw(be_pushy=True)
 
             if self.redraw_id == None:
                 self.redraw_id = GLib.idle_add(self.redraw)
             else:
                 log.debug("Already awaiting paint")
 
             # If this overlay has data that expires after draw, plan for that here
@@ -334,18 +346,14 @@
         so that we only cut out clear sections
         """
         self.redraw_id = None
         gdkwin = self.get_window()
         if self.piggyback_parent:
             self.piggyback_parent.redraw()
             return
-        if not self.floating:
-            (width, height) = self.get_size()
-            self.width = width
-            self.height = height
         if gdkwin:
             compositing = self.get_screen().is_composited()
             if not compositing or self.force_xshape:
                 (width, height) = self.get_size()
                 surface = cairo.ImageSurface(
                     cairo.FORMAT_ARGB32, width, height)
                 surface_ctx = cairo.Context(surface)
@@ -421,22 +429,24 @@
             self.force_xshape = False
 
     def set_enabled(self, enabled):
         """
         Set if this overlay should be visible
         """
         self.enabled = enabled
-        if enabled and not self.hidden and not self.piggyback_parent:
+        if self.piggyback_parent or self.piggyback:
+            self.set_needs_redraw()
+
+            if not self.piggyback_parent:
+                self.set_gamescope_xatom(1 if enabled else 0)
+            return
+        if enabled and not self.hidden:
             self.show_all()
             self.set_untouchable()
-            if self.discover.steamos:
-                self.set_gamescope_xatom(1)
         else:
-            if self.discover.steamos:
-                self.set_gamescope_xatom(0)
             self.hide()
 
     def set_task(self, visible):
         self.set_skip_pager_hint(not visible)
         self.set_skip_taskbar_hint(not visible)
 
     def check_composite(self, _a=None, _b=None):
```

### Comparing `discover-overlay-0.7.3/discover_overlay/settings_window.py` & `discover_overlay-0.7.4/discover_overlay/settings_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
         builder = Gtk.Builder.new_from_file(pkg_resources.resource_filename(
             'discover_overlay', 'glade/settings.glade'))
         window = builder.get_object("settings_window")
         window.connect("destroy", self.close_window)
         window.connect("delete-event", self.close_window)
 
-        window.set_default_size(280, 180)
+        window.set_default_size(1280, 800)
 
         # Make an array of all named widgets
         self.widget = {}
         for widget in builder.get_objects():
             if widget.find_property("name"):
                 name = widget.get_property("name")
                 if name == "":
@@ -115,25 +115,31 @@
             _("Welcome to Discover Overlay"),
             pkg_resources.get_distribution('discover_overlay').version,
             _("Discover-Overlay is a GTK3 overlay written in Python3. It can be configured to show who is currently talking on discord or it can be set to display text and images from a preconfigured channel. It is fully customisable and can be configured to display anywhere on the screen. We fully support X11 and wlroots based environments. We felt the need to make this project due to the shortcomings in support on Linux by the official discord client."),
             _("Please visit our discord"),
             _(" for support. Or open an issue on our GitHub ")
         ))
 
+        screen = window.get_screen()
+        screen_type = "%s" % (screen)
+        self.is_wayland = False
+        if "Wayland" in screen_type:
+            self.is_wayland = True
+        self.window = window
+
         if "GAMESCOPE_WAYLAND_DISPLAY" in os.environ:
             self.steamos = True
             log.info(
                 "GameScope session detected. Enabling steam and gamescope integration")
             self.steamos = True
             settings = Gtk.Settings.get_default()
             if settings:
                 settings.set_property(
                     "gtk-application-prefer-dark-theme", Gtk.true)
-            # TODO Not assume the display size. Probably poll it from GDK Display?
-            window.set_default_size(1280, 800)
+            self.set_steamos_window_size()
 
             # Larger fonts needed
             css = Gtk.CssProvider.new()
             css.load_from_data(bytes("* { font-size:18px; }", "utf-8"))
             window.get_style_context().add_provider(
                 css, Gtk.STYLE_PROVIDER_PRIORITY_USER)
         else:
@@ -142,21 +148,14 @@
         self.super_focus = Gtk.CssProvider.new()
         self.super_focus.load_from_data(
             bytes(
                 """scale { background-color: rgba(100%, 0%, 0%, 0.3); background-image:unset; }
                    spinbutton { background-color: rgba(100%, 0%, 0%, 0.3); background-image:unset;}
                 """, "utf-8"))
 
-        screen = window.get_screen()
-        screen_type = "%s" % (screen)
-        self.is_wayland = False
-        if "Wayland" in screen_type:
-            self.is_wayland = True
-        self.window = window
-
         # Fill monitor & guild menus
         self.populate_monitor_menus()
         window.get_screen().connect("monitors-changed", self.populate_monitor_menus)
 
         channel_file = Gio.File.new_for_path(channel_file)
         self.monitor_channel = channel_file.monitor_file(0, None)
         self.monitor_channel.connect("changed", self.populate_guild_menu)
@@ -181,14 +180,27 @@
             window.show()
 
         if self.icon_name != 'discover-overlay':
             self.widget['overview_image'].set_from_icon_name(
                 self.icon_name, Gtk.IconSize.DIALOG)
             self.widget['window'].set_default_icon_name(self.icon_name)
 
+    def set_steamos_window_size(self):
+        # Huge bunch of assumptions.
+        # Gamescope only has one monitor
+        # Gamescope has no scale factor
+        display = Gdk.Display.get_default()
+        if "get_monitor" in dir(display):
+            monitor = display.get_monitor(0)
+            if monitor:
+                geometry = monitor.get_geometry()
+                scale_factor = monitor.get_scale_factor()
+                log.info("%d %d" % (geometry.width, geometry.height))
+                self.window.set_size_request(geometry.width, geometry.height)
+
     def keypress_in_settings(self, window, event):
         if self.spinning_focus:
             match event.keyval:
                 case Gdk.KEY_Right:
                     step = self.spinning_focus.get_increments().step
                     value = self.spinning_focus.get_value()
                     self.spinning_focus.set_value(value + step)
@@ -310,24 +322,38 @@
         c.handler_unblock(self.channel_handler)
 
     def populate_monitor_menus(self, _a=None, _b=None):
         v = self.widget['voice_monitor']
         t = self.widget['text_monitor']
         m = self.widget['notification_monitor']
 
+        v_value = v.get_active()
+        t_value = t.get_active()
+        m_value = m.get_active()
+
         v.remove_all()
         t.remove_all()
         m.remove_all()
 
+        v.append_text("Any")
+        t.append_text("Any")
+        m.append_text("Any")
+
         display = Gdk.Display.get_default()
         if "get_n_monitors" in dir(display):
-            for i in range(0, display.get_n_monitors()):
-                v.append_text(display.get_monitor(i).get_model())
-                t.append_text(display.get_monitor(i).get_model())
-                m.append_text(display.get_monitor(i).get_model())
+            count_monitors = display.get_n_monitors()
+            if count_monitors >= 1:
+                for i in range(0, count_monitors):
+                    v.append_text(display.get_monitor(i).get_model())
+                    t.append_text(display.get_monitor(i).get_model())
+                    m.append_text(display.get_monitor(i).get_model())
+
+        v.set_active(v_value)
+        t.set_active(t_value)
+        m.set_active(m_value)
 
     def close_window(self, widget=None, event=None):
         """
         Hide the settings window for use at a later date
         """
         self.window.hide()
         if self.ind == None and self.tray == None:
@@ -380,19 +406,21 @@
 
         # Read config and put into gui
         config = ConfigParser(interpolation=None)
         config.read(self.config_file)
 
         # Read Voice section
 
-        self.voice_floating_x = config.getint("main", "floating_x", fallback=0)
-        self.voice_floating_y = config.getint("main", "floating_y", fallback=0)
-        self.voice_floating_w = config.getint(
+        self.voice_floating_x = config.getfloat(
+            "main", "floating_x", fallback=0)
+        self.voice_floating_y = config.getfloat(
+            "main", "floating_y", fallback=0)
+        self.voice_floating_w = config.getfloat(
             "main", "floating_w", fallback=400)
-        self.voice_floating_h = config.getint(
+        self.voice_floating_h = config.getfloat(
             "main", "floating_h", fallback=400)
 
         self.widget['voice_anchor_float'].set_active(
             0 if config.getboolean("main", "floating", fallback=False) else 1)
         self.update_floating_ahchor()
 
         self.widget['voice_align_1'].set_active(
@@ -402,15 +430,15 @@
 
         monitor = 0
         try:
             config.getint("main", "monitor", fallback=0)
         except:
             pass
 
-        self.widget['voice_monitor'].set_active(monitor)
+        self.widget['voice_monitor'].set_active(monitor+1)
 
         font = config.get("main", "font", fallback=None)
         if font:
             self.widget['voice_font'].set_font(font)
         title_font = config.get("main", "title_font", fallback=None)
         if title_font:
             self.widget['voice_title_font'].set_font(title_font)
@@ -535,19 +563,21 @@
         )
         self.widget['voice_show_mouseover'].set_value(
             config.getint("main", "autohide_timer", fallback=5)
         )
 
         # Read Text section
 
-        self.text_floating_x = config.getint("text", "floating_x", fallback=0)
-        self.text_floating_y = config.getint("text", "floating_y", fallback=0)
-        self.text_floating_w = config.getint(
+        self.text_floating_x = config.getfloat(
+            "text", "floating_x", fallback=0)
+        self.text_floating_y = config.getfloat(
+            "text", "floating_y", fallback=0)
+        self.text_floating_w = config.getfloat(
             "text", "floating_w", fallback=400)
-        self.text_floating_h = config.getint(
+        self.text_floating_h = config.getfloat(
             "text", "floating_h", fallback=400)
 
         self.widget['text_enable'].set_active(
             config.getboolean("text", "enabled", fallback=False))
 
         self.widget['text_popup_style'].set_active(
             config.getboolean("text", "popup_style", fallback=False))
@@ -572,15 +602,15 @@
 
         monitor = 0
         try:
             config.getint("text", "monitor", fallback=0)
         except:
             pass
 
-        self.widget['text_monitor'].set_active(monitor)
+        self.widget['text_monitor'].set_active(monitor+1)
 
         self.widget['text_show_attachments'].set_active(config.getboolean(
             "text", "show_attach", fallback=True))
 
         self.widget['text_line_limit'].set_value(
             config.getint("text", "line_limit", fallback=20))
 
@@ -615,15 +645,15 @@
 
         monitor = 0
         try:
             config.getint("notification", "monitor", fallback=0)
         except:
             pass
 
-        self.widget['notification_monitor'].set_active(monitor)
+        self.widget['notification_monitor'].set_active(monitor+1)
 
         self.widget['notification_align_1'].set_active(config.getboolean(
             "notification", "rightalign", fallback=True))
 
         self.widget['notification_align_2'].set_active(
             config.getint("notification", "topalign", fallback=2))
 
@@ -676,15 +706,15 @@
             "general", "start_min", fallback=False)
 
         self.widget['core_settings_min'].set_active(self.start_minimized)
 
         self.widget['core_settings_min'].set_sensitive(self.show_sys_tray_icon)
 
         if 'XDG_SESSION_DESKTOP' in os.environ and os.environ['XDG_SESSION_DESKTOP'] == 'cinnamon':
-            self.widget['voice_anchor_to_edge_button'].set_sensitive(False)
+            self.widget['voice_anchor_float'].set_sensitive(False)
 
         self.widget['core_audio_assist'].set_active(
             config.getboolean("general", "audio_assist", fallback=False))
 
         self.loading_config = False
 
     def make_colour(self, col):
@@ -716,23 +746,25 @@
             gi.require_version('AppIndicator3', '0.1')
             # pylint: disable=import-outside-toplevel
             from gi.repository import AppIndicator3
             self.ind = AppIndicator3.Indicator.new(
                 "discover_overlay",
                 self.tray_icon_name,
                 AppIndicator3.IndicatorCategory.APPLICATION_STATUS)
+            self.ind.set_title(_("Discover Overlay Configuration"))
             # Hide for now since we don't know if it should be shown yet
             self.ind.set_status(AppIndicator3.IndicatorStatus.PASSIVE)
             self.ind.set_menu(menu)
         except (ImportError, ValueError) as exception:
             # Create System Tray
             log.info("Falling back to Systray : %s", exception)
             self.tray = Gtk.StatusIcon.new_from_icon_name(
                 self.tray_icon_name)
             self.tray.connect('popup-menu', self.show_menu)
+            self.tray.set_title(_("Discover Overlay Configuration"))
             # Hide for now since we don't know if it should be shown yet
             self.tray.set_visible(False)
 
     def show_menu(self, obj, button, time):
         """
         Show menu when System Tray icon is clicked
         """
@@ -815,22 +847,22 @@
             self.voice_floating_w = width
             self.voice_floating_h = height
 
             config = ConfigParser(interpolation=None)
             config.read(self.config_file)
             if not "main" in config.sections():
                 config.add_section("main")
-            config.set("main", "floating_x", "%s" %
-                       (int(self.voice_floating_x)))
-            config.set("main", "floating_y", "%s" %
-                       (int(self.voice_floating_y)))
-            config.set("main", "floating_w", "%s" %
-                       (int(self.voice_floating_w)))
-            config.set("main", "floating_h", "%s" %
-                       (int(self.voice_floating_h)))
+            config.set("main", "floating_x", "%f" %
+                       (self.voice_floating_x))
+            config.set("main", "floating_y", "%f" %
+                       (self.voice_floating_y))
+            config.set("main", "floating_w", "%f" %
+                       (self.voice_floating_w))
+            config.set("main", "floating_h", "%f" %
+                       (self.voice_floating_h))
 
             with open(self.config_file, 'w') as file:
                 config.write(file)
             if button:
                 button.set_label(_("Place Window"))
             self.voice_placement_window.close()
             self.voice_placement_window = None
@@ -841,20 +873,20 @@
                 self.window.hide()
             if self.is_wayland or self.steamos:
                 self.voice_placement_window = DraggableWindowWayland(
                     pos_x=self.voice_floating_x, pos_y=self.voice_floating_y,
                     width=self.voice_floating_w, height=self.voice_floating_h,
                     message=_("Place & resize this window then press Green!"), settings=self,
                     steamos=self.steamos,
-                    monitor=self.get_monitor_obj(self.widget['voice_monitor'].get_active()))
+                    monitor=self.widget['voice_monitor'].get_active()-1)
             else:
                 self.voice_placement_window = DraggableWindow(
                     pos_x=self.voice_floating_x, pos_y=self.voice_floating_y,
                     width=self.voice_floating_w, height=self.voice_floating_h,
-                    message=_("Place & resize this window then press Save!"), settings=self)
+                    message=_("Place & resize this window then press Save!"), settings=self, monitor=self.widget['voice_monitor'].get_active()-1)
                 if button:
                     button.set_label(_("Save this position"))
 
     def text_place_window(self, button):
         if self.text_placement_window:
             (pos_x, pos_y, width, height) = self.text_placement_window.get_coords()
             self.text_floating_x = pos_x
@@ -862,22 +894,22 @@
             self.text_floating_w = width
             self.text_floating_h = height
 
             config = ConfigParser(interpolation=None)
             config.read(self.config_file)
             if not "text" in config.sections():
                 config.add_section("text")
-            config.set("text", "floating_x", "%s" %
-                       (int(self.text_floating_x)))
-            config.set("text", "floating_y", "%s" %
-                       (int(self.text_floating_y)))
-            config.set("text", "floating_w", "%s" %
-                       (int(self.text_floating_w)))
-            config.set("text", "floating_h", "%s" %
-                       (int(self.text_floating_h)))
+            config.set("text", "floating_x", "%f" %
+                       (self.text_floating_x))
+            config.set("text", "floating_y", "%f" %
+                       (self.text_floating_y))
+            config.set("text", "floating_w", "%f" %
+                       (self.text_floating_w))
+            config.set("text", "floating_h", "%f" %
+                       (self.text_floating_h))
 
             with open(self.config_file, 'w') as file:
                 config.write(file)
             if button:
                 button.set_label(_("Place Window"))
             self.text_placement_window.close()
             self.text_placement_window = None
@@ -888,20 +920,20 @@
                 self.window.hide()
             if self.is_wayland or self.steamos:
                 self.text_placement_window = DraggableWindowWayland(
                     pos_x=self.text_floating_x, pos_y=self.text_floating_y,
                     width=self.text_floating_w, height=self.text_floating_h,
                     message=_("Place & resize this window then press Green!"), settings=self,
                     steamos=self.steamos,
-                    monitor=self.get_monitor_obj(self.widget['text_monitor'].get_active()))
+                    monitor=self.widget['text_monitor'].get_active()-1)
             else:
                 self.text_placement_window = DraggableWindow(
                     pos_x=self.text_floating_x, pos_y=self.text_floating_y,
                     width=self.text_floating_w, height=self.text_floating_h,
-                    message=_("Place & resize this window then press Save!"), settings=self)
+                    message=_("Place & resize this window then press Save!"), settings=self, monitor=self.widget['text_monitor'].get_active()-1)
                 if button:
                     button.set_label(_("Save this position"))
 
     def change_placement(self, placement_window):
         if placement_window == self.text_placement_window:
             self.text_place_window(None)
         elif placement_window == self.voice_placement_window:
@@ -946,15 +978,15 @@
             self.widget['voice_place_window_button'].show()
         else:
             self.widget['voice_align_1'].show()
             self.widget['voice_align_2'].show()
             self.widget['voice_place_window_button'].hide()
 
     def voice_monitor_changed(self, button):
-        self.config_set("main", "monitor", "%s" % (button.get_active()))
+        self.config_set("main", "monitor", "%s" % (button.get_active()-1))
 
     def voice_align_1_changed(self, button):
         self.config_set("main", "rightalign", "%s" % (button.get_active()))
 
     def voice_align_2_changed(self, button):
         self.config_set("main", "topalign", "%s" % (button.get_active()))
 
@@ -1163,15 +1195,15 @@
 
     def text_background_colour_changed(self, button):
         colour = button.get_rgba()
         colour = [colour.red, colour.green, colour.blue, colour.alpha]
         self.config_set("text", "bg_col", json.dumps(colour))
 
     def text_monitor_changed(self, button):
-        self.config_set("text", "monitor", "%s" % (button.get_active()))
+        self.config_set("text", "monitor", "%s" % (button.get_active()-1))
 
     def text_show_attachments_changed(self, button):
         self.config_set("text", "show_attach", "%s" % (button.get_active()))
 
     def text_line_limit_changed(self, button):
         self.config_set("text", "line_limit", "%s" % (int(button.get_value())))
 
@@ -1201,15 +1233,15 @@
     def notification_background_colour_changed(self, button):
         colour = button.get_rgba()
         colour = [colour.red, colour.green, colour.blue, colour.alpha]
         self.config_set("notification", "bg_col", json.dumps(colour))
 
     def notification_monitor_changed(self, button):
         self.config_set("notification", "monitor", "%s" %
-                        (button.get_active()))
+                        (button.get_active()-1))
 
     def notification_align_1_changed(self, button):
         self.config_set("notification", "rightalign", "%s" %
                         (button.get_active()))
 
     def notification_align_2_changed(self, button):
         self.config_set("notification", "topalign", "%s" %
```

### Comparing `discover-overlay-0.7.3/discover_overlay/text_overlay.py` & `discover_overlay-0.7.4/discover_overlay/text_overlay.py`

 * *Files 6% similar despite different names*

```diff
@@ -193,14 +193,16 @@
         """
         Called when an image has been downloaded by image_getter
         """
         self.attachment[identifier] = pix
         self.set_needs_redraw()
 
     def has_content(self):
+        if self.piggyback and self.piggyback.has_content():
+            return True
         if not self.enabled:
             return False
         if self.hidden:
             return False
         return self.content
 
     def overlay_draw(self, w, context, data=None):
@@ -221,21 +223,25 @@
         self.tick()
         context.save()
         if self.is_wayland or self.piggyback_parent or self.discover.steamos:
             # Special case!
             # The window is full-screen regardless of what the user has selected.
             # We need to set a clip and a transform to imitate original behaviour
             # Used in wlroots & gamescope
-            width = self.width
-            height = self.height
-            context.translate(self.pos_x, self.pos_y)
-            context.rectangle(0, 0, width, height)
-            context.clip()
-
-        current_y = height
+            (floating_x, floating_y, floating_width,
+             floating_height) = self.get_floating_coords()
+            if self.floating:
+                context.new_path()
+                context.translate(floating_x, floating_y)
+                context.rectangle(0, 0, floating_width, floating_height)
+                context.clip()
+            pass
+        (floating_x, floating_y, floating_width,
+         floating_height) = self.get_floating_coords()
+        current_y = floating_height
         tnow = time.time()
         for line in reversed(self.content):
             if self.popup_style and tnow - line['time'] > self.text_time:
                 break
             out_line = ""
             self.image_list = []
 
@@ -272,23 +278,25 @@
         context.restore()
         self.context = None
 
     def draw_attach(self, pos_y, url):
         """
         Draw an attachment
         """
+        (floating_x, floating_y, floating_width,
+         floating_height) = self.get_floating_coords()
         if url in self.attachment and self.attachment[url]:
             pix = self.attachment[url]
-            image_width = min(pix.get_width(), self.width)
-            image_height = min(pix.get_height(), (self.height * .7))
+            image_width = min(pix.get_width(), floating_width)
+            image_height = min(pix.get_height(), (floating_height * .7))
             (_ax, _ay, _aw, aspect_height) = get_aspected_size(
                 pix, image_width, image_height)
             self.col(self.bg_col)
             self.context.rectangle(0, pos_y - aspect_height,
-                                   self.width, aspect_height)
+                                   floating_width, aspect_height)
 
             self.context.fill()
             self.context.set_operator(cairo.OPERATOR_OVER)
             _new_w, new_h = draw_img_to_rect(
                 pix, self.context, 0, pos_y - image_height, image_width, image_height, aspect=True)
             return pos_y - new_h
         return pos_y
@@ -298,22 +306,25 @@
         Draw a text message, returning the Y position of the next message
         """
         layout = self.create_pango_layout(text)
         layout.set_auto_dir(True)
         layout.set_markup(text, -1)
         attr = layout.get_attributes()
 
-        layout.set_width(Pango.SCALE * self.width)
+        (floating_x, floating_y, floating_width,
+         floating_height) = self.get_floating_coords()
+        layout.set_width(Pango.SCALE * floating_width)
         layout.set_spacing(Pango.SCALE * 3)
         if self.text_font:
             font = Pango.FontDescription(self.text_font)
             layout.set_font_description(font)
         _tw, text_height = layout.get_pixel_size()
         self.col(self.bg_col)
-        self.context.rectangle(0, pos_y - text_height, self.width, text_height)
+        self.context.rectangle(0, pos_y - text_height,
+                               floating_width, text_height)
         self.context.fill()
         self.context.set_operator(cairo.OPERATOR_OVER)
         self.col(self.fg_col)
 
         self.context.move_to(0, pos_y - text_height)
         PangoCairo.context_set_shape_renderer(
             self.get_pango_context(), self.render_custom, None)
```

### Comparing `discover-overlay-0.7.3/discover_overlay/voice_overlay.py` & `discover_overlay-0.7.4/discover_overlay/voice_overlay.py`

 * *Files 4% similar despite different names*

```diff
@@ -547,25 +547,26 @@
         self.set_wind_col()
         # Don't layer drawing over each other, always replace
         context.set_operator(cairo.OPERATOR_SOURCE)
         context.paint()
         context.save()
         if self.piggyback:
             self.piggyback.overlay_draw(w, context, data)
+        (floating_x, floating_y, floating_width,
+         floating_height) = self.get_floating_coords()
         if self.is_wayland or self.piggyback_parent or self.discover.steamos:
             # Special case!
             # The window is full-screen regardless of what the user has selected.
             # We need to set a clip and a transform to imitate original behaviour
             # Used in wlroots & gamescope
-            width = self.width
-            height = self.height
+
             if self.floating:
                 context.new_path()
-                context.translate(self.pos_x, self.pos_y)
-                context.rectangle(0, 0, width, height)
+                context.translate(floating_x, floating_y)
+                context.rectangle(0, 0, floating_width, floating_height)
                 context.clip()
 
         context.set_operator(cairo.OPERATOR_OVER)
         if not self.show_disconnected and self.connection_status == "DISCONNECTED" and not self.use_dummy:
             return
 
         connection = self.discover.connection
@@ -695,15 +696,15 @@
                         avatar_size = 8
 
             current_x = 0 + self.horz_edge_padding
             offset_x_mult = 1
             offset_x = avatar_size + self.horz_edge_padding
             if self.align_right:
                 offset_x_mult = -1
-                current_x = self.width - avatar_size - self.horz_edge_padding
+                current_x = floating_width - avatar_size - self.horz_edge_padding
 
             # Choose where to start drawing
             current_y = 0 + self.vert_edge_padding
             if self.align_vert == 1:
                 current_y = (height / 2) - (needed_height / 2)
             elif self.align_vert == 2:
                 current_y = height - needed_height - self.vert_edge_padding
@@ -913,16 +914,17 @@
         if self.nick_length < 32 and len(string) > self.nick_length:
             string = string[:(self.nick_length-1)] + u"\u2026"
 
         context.save()
         layout = self.create_pango_layout(string)
         layout.set_auto_dir(True)
         layout.set_markup(string, -1)
-
-        layout.set_width(Pango.SCALE * self.width)
+        (floating_x, floating_y, floating_width,
+         floating_height) = self.get_floating_coords()
+        layout.set_width(Pango.SCALE * floating_width)
         layout.set_spacing(Pango.SCALE * 3)
         if font:
             font = Pango.FontDescription(font)
             layout.set_font_description(font)
         (_ink_rect, logical_rect) = layout.get_pixel_extents()
         text_height = logical_rect.height
         text_width = logical_rect.width
```

### Comparing `discover-overlay-0.7.3/discover_overlay.egg-info/PKG-INFO` & `discover_overlay-0.7.4/discover_overlay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discover-overlay
-Version: 0.7.3
+Version: 0.7.4
 Summary: Voice chat overlay
 Home-page: https://github.com/trigg/Discover
 Author: trigg
 Author-email: 
 License: GPLv3+
 Keywords: discord overlay voice linux
 Classifier: Development Status :: 4 - Beta
```

### Comparing `discover-overlay-0.7.3/discover_overlay.egg-info/SOURCES.txt` & `discover_overlay-0.7.4/discover_overlay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.3/discover_overlay_configure.desktop` & `discover_overlay-0.7.4/discover_overlay_configure.desktop`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.3/setup.py` & `discover_overlay-0.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     return open('README.md', 'r').read()
 
 
 setup(
     name='discover-overlay',
     author='trigg',
     author_email='',
-    version='0.7.3',
+    version='0.7.4',
     description='Voice chat overlay',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/trigg/Discover',
     packages=find_namespace_packages(),
     include_package_data=True,
     data_files=[
```


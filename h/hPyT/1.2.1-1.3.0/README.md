# Comparing `tmp/hPyT-1.2.1.tar.gz` & `tmp/hpyt-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hPyT-1.2.1.tar", last modified: Wed Feb 28 09:18:19 2024, max compression
+gzip compressed data, was "hpyt-1.3.0.tar", last modified: Thu Apr 25 15:37:19 2024, max compression
```

## Comparing `hPyT-1.2.1.tar` & `hpyt-1.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:18:19.294634 hPyT-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-28 09:18:05.000000 hPyT-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9930 2024-02-28 09:18:19.294634 hPyT-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-02-28 09:18:05.000000 hPyT-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:18:19.290634 hPyT-1.2.1/hPyT/
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-02-28 09:18:05.000000 hPyT-1.2.1/hPyT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17817 2024-02-28 09:18:05.000000 hPyT-1.2.1/hPyT/hPyT.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:18:19.290634 hPyT-1.2.1/hPyT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9930 2024-02-28 09:18:19.000000 hPyT-1.2.1/hPyT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-28 09:18:19.000000 hPyT-1.2.1/hPyT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 09:18:19.000000 hPyT-1.2.1/hPyT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-28 09:18:19.000000 hPyT-1.2.1/hPyT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 09:18:19.294634 hPyT-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-02-28 09:18:05.000000 hPyT-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:37:19.331043 hpyt-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-25 15:37:12.000000 hpyt-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11057 2024-04-25 15:37:19.331043 hpyt-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10021 2024-04-25 15:37:12.000000 hpyt-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:37:19.331043 hpyt-1.3.0/hPyT/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-25 15:37:12.000000 hpyt-1.3.0/hPyT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23028 2024-04-25 15:37:12.000000 hpyt-1.3.0/hPyT/hPyT.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:37:19.331043 hpyt-1.3.0/hPyT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11057 2024-04-25 15:37:19.000000 hpyt-1.3.0/hPyT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-25 15:37:19.000000 hpyt-1.3.0/hPyT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:37:19.000000 hpyt-1.3.0/hPyT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 15:37:19.000000 hpyt-1.3.0/hPyT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:37:19.331043 hpyt-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-25 15:37:12.000000 hpyt-1.3.0/setup.py
```

### Comparing `hPyT-1.2.1/LICENSE` & `hpyt-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hPyT-1.2.1/PKG-INFO` & `hpyt-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hPyT
-Version: 1.2.1
+Version: 1.3.0
 Summary: Hack Python Titlebar - A package to manipulate windows and titlebar of GUI applications made using python.
 Home-page: https://github.com/zingzy/hPyT
 Author: zingzy
 License: MIT
 Keywords: Tkinter wxpython pyqt pyside GUI window controls decorations hide show titlebar
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,58 +13,62 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hPyT - Hack Python Titlebar
 
 A package to manipulate windows and titlebar of GUI applications made using python
 **Supports Both Windows 11 and 10**
 
-https://github.com/Zingzy/hPyT/assets/90309290/c61b3142-80d6-4c07-b8e3-65694faf945b
+https://github.com/Zingzy/hPyT/assets/90309290/f86df1c7-b75b-4477-974a-eb34cc117df3
 
-**You can download the above app from the [github releases](https://github.com/Zingzy/hPyT/releases/tag/v1.1.0/) to test out the package before installing/using it in your projects**
+**You can download the above app from the [github releases](https://github.com/Zingzy/hPyT/releases/tag/hPyT-preview/) to test out the package before installing/using it in your projects**
 
 <br>
 
 <details>
 
 <summary>📖 Table of Contents</summary>
 
 - [hPyT - Hack Python Titlebar](#hpyt---hack-python-titlebar)
 	- [📚 Supported Libraries](#-supported-libraries)
 	- [📦 Installing](#-installing)
 	- [📥 Importing](#-importing)
 	- [Hide/Unhide Title Bar](#hideunhide-title-bar)
 	- [🌈 Rainbow TitleBar](#-rainbow-titlebar)
+	- [🌈 Rainbow Border](#-rainbow-border)
 	- [Hide/Unhide both Maximize and Minimize Buttons (Completely Hides both buttons)](#hideunhide-both-maximize-and-minimize-buttons-completely-hides-both-buttons)
 	- [Hide/Unhide All Buttons or Stuffs](#hideunhide-all-buttons-or-stuffs)
 	- [Enable/Disable Maximize Button](#enabledisable-maximize-button)
 	- [Enable/Disable Minimize Button](#enabledisable-minimize-button)
 	- [Opacity](#opacity)
 	- [⚡ Flashing Window](#-flashing-window)
 	- [🎨 Custom TitleBar Color](#-custom-titlebar-color)
 	- [🖌️ Custom TitleBar Text Color](#️-custom-titlebar-text-color)
+	- [🖌️ Custom Border Color](#️-custom-border-color)
 	- [💻 Window Management](#-window-management)
 		- [Center a window on the screen](#center-a-window-on-the-screen)
 		- [Center a secondary window relative to the primary window](#center-a-secondary-window-relative-to-the-primary-window)
 		- [Other basic window management functions](#other-basic-window-management-functions)
 	- [✨ Window Animations](#-window-animations)
 		- [Circle Motion](#circle-motion)
 		- [Verical Shake](#verical-shake)
 		- [Horizontal Shake](#horizontal-shake)
 	- [✏️ Stylize text](#️-stylize-text)
 		- [Miscellaneous](#miscellaneous)
 	- [📜 hPyT Changelog](#-hpyt-changelog)
+		- [v1.3.0](#v130)
 		- [v1.2.1](#v121)
 		- [v1.2.0](#v120)
 		- [v1.1.3](#v113)
 		- [v1.1.2](#v112)
 		- [v1.1.1](#v111)
 		- [v1.1.0](#v110)
 </details>
@@ -78,15 +82,15 @@
 - PySide
 - WxPython
 - support for more libraries soon...
 
 ## 📦 Installing
 
 ```powershell
-pip install hPyT==1.2.1
+pip install hPyT==1.3.0
 ```
 
 ## 📥 Importing
 
 ```python
 from hPyT import *
 from customtkinter import * # you can use any other library from the above mentioned list
@@ -97,27 +101,37 @@
 ## Hide/Unhide Title Bar
 
 ```python
 title_bar.hide(window) # hides full titlebar
 # title_bar.unhide(window)
 ```
 
-![Hidden Title Bar](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/titlebar.png)
+![image](https://github.com/littlewhitecloud/hPyT/assets/71159641/03e533fe-c42a-4d84-b138-176a73ad7977)
 
 ## 🌈 Rainbow TitleBar
 
 ```python
 rainbow_title_bar.start(window, interval=5) # starts the rainbow titlebar
 # rainbow_title_bar.stop(window) # stops the rainbow titlebar
 ```
 
-*`interval` is the time in milliseconds in which the color would change*
+> [!NOTE]
+> *`interval` is the time in milliseconds in which the color would change*
 
 ![Rainbow TitleBar](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/rainbow_titlebar.gif)
 
+## 🌈 Rainbow Border
+
+```python
+rainbow_border.start(window, interval=4) # starts the rainbow border
+# rainbow_border.stop(window) # stops the rainbow border
+```
+
+![Rainbow Border](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/rainbow_border.gif)
+
 ## Hide/Unhide both Maximize and Minimize Buttons (Completely Hides both buttons)
 
 ```python
 maximize_minimize_button.hide(window) # hides both maximize and minimize button
 # maximize_minimize_button.unhide(window)
 ```
 
@@ -172,30 +186,40 @@
 
 ![Flashing Window](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/flashing.gif)
 
 ## 🎨 Custom TitleBar Color
 
 ```python
 title_bar_color.set(window, '#ff00ff') # sets the titlebar color to magenta
+# title_bar_color.reset(window) # resets the titlebar color to default
 ```
 
-*You can pass any valid color in `Hex` or `RGB` format*
+> [!NOTE]
+> *You can pass any valid color in `Hex` or `RGB` format*
 
 ![Custom TitleBar Color](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/titlebar_color.png)
 
 ## 🖌️ Custom TitleBar Text Color
 
 ```python
 title_text_color.set(window, '#ff00ff') # sets the titlebar text color to magenta
+# title_text_color.reset(window) # resets the titlebar text color to default
 ```
 
-*You can pass any valid color in `Hex` or `RGB` format*
-
 ![Custom TitleBar Text Color](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/title_text_color.png)
 
+## 🖌️ Custom Border Color
+
+```python
+border_color.set(window, '#ff00ff') # sets the border color to magenta
+# border_color.reset(window) # resets the border color to default
+```
+
+![Custom Border Color](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/border_color.png)
+
 ## 💻 Window Management
 
 ### Center a window on the screen
 
 ```python
 window_frame.center(window)
 ```
@@ -245,22 +269,22 @@
 ![Circle Motion](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/circle_motion.gif)
 
 *The animation might appear a bit fasterer and rougher in the above preview gif than it is*
 
 ### Verical Shake
 
 ```python
-window_animation.vertical_shake(window, count=5, interval=5, apmlitude=20)
+window_animation.vertical_shake(window, count=5, interval=5, amplitude=20)
 # shakes the window vertically 5 times with 5ms interval and 10px distance
 ```
 
 ### Horizontal Shake
 
 ```python
-window_animation.horizontal_shake(window, count=5, interval=5, apmlitude=20)
+window_animation.horizontal_shake(window, count=5, interval=5, amplitude=20)
 # shakes the window horizontally 5 times with 5ms interval and 10px distance
 ```
 
 ## ✏️ Stylize text
 
 ```python
 title_text.stylize(window, style=1)
@@ -278,14 +302,21 @@
 >>> "𝔜𝔬𝔲𝔯 ℭ𝔲𝔰𝔱𝔬𝔪 𝔗𝔢𝔵𝔱"
 ```
 
 <br>
 
 ## 📜 hPyT Changelog
 
+### v1.3.0
+
+- Add support for setting custom border color
+- Add support for rainbow border color effect
+- Add support for resetting the titleBar color and titleText color
+- Fix an issue which caused the titleBar to appear black after the rainbow titleBar effect was stopped
+
 ### v1.2.1
 
 - Minor Bug Fixes
 
 ### v1.2.0
 
 - Add support for rainbow titlebar
```

### Comparing `hPyT-1.2.1/README.md` & `hpyt-1.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 # hPyT - Hack Python Titlebar
 
 A package to manipulate windows and titlebar of GUI applications made using python
 **Supports Both Windows 11 and 10**
 
-https://github.com/Zingzy/hPyT/assets/90309290/c61b3142-80d6-4c07-b8e3-65694faf945b
+https://github.com/Zingzy/hPyT/assets/90309290/f86df1c7-b75b-4477-974a-eb34cc117df3
 
-**You can download the above app from the [github releases](https://github.com/Zingzy/hPyT/releases/tag/v1.1.0/) to test out the package before installing/using it in your projects**
+**You can download the above app from the [github releases](https://github.com/Zingzy/hPyT/releases/tag/hPyT-preview/) to test out the package before installing/using it in your projects**
 
 <br>
 
 <details>
 
 <summary>📖 Table of Contents</summary>
 
 - [hPyT - Hack Python Titlebar](#hpyt---hack-python-titlebar)
 	- [📚 Supported Libraries](#-supported-libraries)
 	- [📦 Installing](#-installing)
 	- [📥 Importing](#-importing)
 	- [Hide/Unhide Title Bar](#hideunhide-title-bar)
 	- [🌈 Rainbow TitleBar](#-rainbow-titlebar)
+	- [🌈 Rainbow Border](#-rainbow-border)
 	- [Hide/Unhide both Maximize and Minimize Buttons (Completely Hides both buttons)](#hideunhide-both-maximize-and-minimize-buttons-completely-hides-both-buttons)
 	- [Hide/Unhide All Buttons or Stuffs](#hideunhide-all-buttons-or-stuffs)
 	- [Enable/Disable Maximize Button](#enabledisable-maximize-button)
 	- [Enable/Disable Minimize Button](#enabledisable-minimize-button)
 	- [Opacity](#opacity)
 	- [⚡ Flashing Window](#-flashing-window)
 	- [🎨 Custom TitleBar Color](#-custom-titlebar-color)
 	- [🖌️ Custom TitleBar Text Color](#️-custom-titlebar-text-color)
+	- [🖌️ Custom Border Color](#️-custom-border-color)
 	- [💻 Window Management](#-window-management)
 		- [Center a window on the screen](#center-a-window-on-the-screen)
 		- [Center a secondary window relative to the primary window](#center-a-secondary-window-relative-to-the-primary-window)
 		- [Other basic window management functions](#other-basic-window-management-functions)
 	- [✨ Window Animations](#-window-animations)
 		- [Circle Motion](#circle-motion)
 		- [Verical Shake](#verical-shake)
 		- [Horizontal Shake](#horizontal-shake)
 	- [✏️ Stylize text](#️-stylize-text)
 		- [Miscellaneous](#miscellaneous)
 	- [📜 hPyT Changelog](#-hpyt-changelog)
+		- [v1.3.0](#v130)
 		- [v1.2.1](#v121)
 		- [v1.2.0](#v120)
 		- [v1.1.3](#v113)
 		- [v1.1.2](#v112)
 		- [v1.1.1](#v111)
 		- [v1.1.0](#v110)
 </details>
@@ -55,15 +58,15 @@
 - PySide
 - WxPython
 - support for more libraries soon...
 
 ## 📦 Installing
 
 ```powershell
-pip install hPyT==1.2.1
+pip install hPyT==1.3.0
 ```
 
 ## 📥 Importing
 
 ```python
 from hPyT import *
 from customtkinter import * # you can use any other library from the above mentioned list
@@ -74,27 +77,37 @@
 ## Hide/Unhide Title Bar
 
 ```python
 title_bar.hide(window) # hides full titlebar
 # title_bar.unhide(window)
 ```
 
-![Hidden Title Bar](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/titlebar.png)
+![image](https://github.com/littlewhitecloud/hPyT/assets/71159641/03e533fe-c42a-4d84-b138-176a73ad7977)
 
 ## 🌈 Rainbow TitleBar
 
 ```python
 rainbow_title_bar.start(window, interval=5) # starts the rainbow titlebar
 # rainbow_title_bar.stop(window) # stops the rainbow titlebar
 ```
 
-*`interval` is the time in milliseconds in which the color would change*
+> [!NOTE]
+> *`interval` is the time in milliseconds in which the color would change*
 
 ![Rainbow TitleBar](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/rainbow_titlebar.gif)
 
+## 🌈 Rainbow Border
+
+```python
+rainbow_border.start(window, interval=4) # starts the rainbow border
+# rainbow_border.stop(window) # stops the rainbow border
+```
+
+![Rainbow Border](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/rainbow_border.gif)
+
 ## Hide/Unhide both Maximize and Minimize Buttons (Completely Hides both buttons)
 
 ```python
 maximize_minimize_button.hide(window) # hides both maximize and minimize button
 # maximize_minimize_button.unhide(window)
 ```
 
@@ -149,30 +162,40 @@
 
 ![Flashing Window](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/flashing.gif)
 
 ## 🎨 Custom TitleBar Color
 
 ```python
 title_bar_color.set(window, '#ff00ff') # sets the titlebar color to magenta
+# title_bar_color.reset(window) # resets the titlebar color to default
 ```
 
-*You can pass any valid color in `Hex` or `RGB` format*
+> [!NOTE]
+> *You can pass any valid color in `Hex` or `RGB` format*
 
 ![Custom TitleBar Color](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/titlebar_color.png)
 
 ## 🖌️ Custom TitleBar Text Color
 
 ```python
 title_text_color.set(window, '#ff00ff') # sets the titlebar text color to magenta
+# title_text_color.reset(window) # resets the titlebar text color to default
 ```
 
-*You can pass any valid color in `Hex` or `RGB` format*
-
 ![Custom TitleBar Text Color](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/title_text_color.png)
 
+## 🖌️ Custom Border Color
+
+```python
+border_color.set(window, '#ff00ff') # sets the border color to magenta
+# border_color.reset(window) # resets the border color to default
+```
+
+![Custom Border Color](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/border_color.png)
+
 ## 💻 Window Management
 
 ### Center a window on the screen
 
 ```python
 window_frame.center(window)
 ```
@@ -222,22 +245,22 @@
 ![Circle Motion](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/circle_motion.gif)
 
 *The animation might appear a bit fasterer and rougher in the above preview gif than it is*
 
 ### Verical Shake
 
 ```python
-window_animation.vertical_shake(window, count=5, interval=5, apmlitude=20)
+window_animation.vertical_shake(window, count=5, interval=5, amplitude=20)
 # shakes the window vertically 5 times with 5ms interval and 10px distance
 ```
 
 ### Horizontal Shake
 
 ```python
-window_animation.horizontal_shake(window, count=5, interval=5, apmlitude=20)
+window_animation.horizontal_shake(window, count=5, interval=5, amplitude=20)
 # shakes the window horizontally 5 times with 5ms interval and 10px distance
 ```
 
 ## ✏️ Stylize text
 
 ```python
 title_text.stylize(window, style=1)
@@ -255,14 +278,21 @@
 >>> "𝔜𝔬𝔲𝔯 ℭ𝔲𝔰𝔱𝔬𝔪 𝔗𝔢𝔵𝔱"
 ```
 
 <br>
 
 ## 📜 hPyT Changelog
 
+### v1.3.0
+
+- Add support for setting custom border color
+- Add support for rainbow border color effect
+- Add support for resetting the titleBar color and titleText color
+- Fix an issue which caused the titleBar to appear black after the rainbow titleBar effect was stopped
+
 ### v1.2.1
 
 - Minor Bug Fixes
 
 ### v1.2.0
 
 - Add support for rainbow titlebar
```

### Comparing `hPyT-1.2.1/hPyT/hPyT.py` & `hpyt-1.3.0/hPyT/hPyT.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,206 +1,282 @@
 try:
-    import threading
     import ctypes
     import math
+    import threading
+    from ctypes.wintypes import HWND, RECT, UINT
 except ImportError:
-    raise ImportError("hPtT import Error : No Windows Enviorment Found")
+    raise ImportError("hPyT import Error : No Windows Enviorment Found")
 
 set_window_pos = ctypes.windll.user32.SetWindowPos
 set_window_long = ctypes.windll.user32.SetWindowLongPtrW
-get_window_long = ctypes.windll.user32.GetWindowLongPtrW
+get_window_long = ctypes.windll.user32.GetWindowLongPtrA
 def_window_proc = ctypes.windll.user32.DefWindowProcW
+call_window_proc = ctypes.windll.user32.CallWindowProcW
+flash_window_ex = ctypes.windll.user32.FlashWindowEx
+
 
 GWL_STYLE = -16
+GWL_EXSTYLE = -20
+GWL_WNDPROC = -4
 
-WS_MINIMIZEBOX = 131072
-WS_MAXIMIZEBOX = 65536
+WS_MINIMIZEBOX = 0x00020000
+WS_MAXIMIZEBOX = 0x00010000
+WS_CAPTION = 0x00C00000
+WS_SYSMENU = 0x00080000
 
-WS_SYSMENU = 524288
+WS_EX_LAYERED = 524288
+
+WM_NCCALCSIZE = 0x0083
+WM_NCHITTEST = 0x0084
 
 SWP_NOZORDER = 4
 SWP_NOMOVE = 2
 SWP_NOSIZE = 1
 SWP_FRAMECHANGED = 32
 
-GWL_EXSTYLE = -20
-WS_EX_LAYERED = 524288
 LWA_ALPHA = 2
 
-WS_CAPTION = 12582912
-
 FLASHW_STOP = 0
 FLASHW_CAPTION = 1
 FLASHW_TRAY = 2
 FLASHW_ALL = 3
 FLASHW_TIMER = 4
 FLASHW_TIMERNOFG = 12
 
+
 class FLASHWINFO(ctypes.Structure):
     _fields_ = [("cbSize", ctypes.c_uint),
                 ("hwnd", ctypes.c_void_p),
                 ("dwFlags", ctypes.c_uint),
                 ("uCount", ctypes.c_uint),
                 ("dwTimeout", ctypes.c_uint)]
 
-flash_window_ex = ctypes.windll.user32.FlashWindowEx
+class PWINDOWPOS(ctypes.Structure):
+    _fields_ = [
+        ("hWnd", HWND),
+        ("hwndInsertAfter", HWND),
+        ("x", ctypes.c_int),
+        ("y", ctypes.c_int),
+        ("cx", ctypes.c_int),
+        ("cy", ctypes.c_int),
+        ("flags", UINT),
+    ]
+
+class NCCALCSIZE_PARAMS(ctypes.Structure):
+    _fields_ = [("rgrc", RECT * 3), ("lppos", ctypes.POINTER(PWINDOWPOS))]
 
 rnbtbs = []
+rnbbcs = []
 titles = {}
 
 class title_bar:
     @classmethod
-    def hide(cls, window):
+    def hide(cls, window) -> None:
+        def handle(hwnd: int, msg: int, wp: int, lp: int) -> int:
+            if msg == WM_NCCALCSIZE and wp:
+                lpncsp = NCCALCSIZE_PARAMS.from_address(lp)
+                lpncsp.rgrc[0].top -= 6
+
+            return call_window_proc(*map(ctypes.c_uint64, (globals()[old], hwnd, msg, wp, lp)))
+
+        old, new = "old_wndproc", "new_wndproc"
+        prototype = ctypes.WINFUNCTYPE(ctypes.c_uint64, ctypes.c_uint64, ctypes.c_uint64, ctypes.c_uint64, ctypes.c_uint64)
+
         hwnd = module_find(window)
+
+        globals()[old] = None
+        globals()[new] = prototype(handle)
+        globals()[old] = get_window_long(hwnd, GWL_WNDPROC)
+        set_window_long(hwnd, GWL_WNDPROC, globals()[new])
+        
         old_style = get_window_long(hwnd, GWL_STYLE)
         new_style = old_style & ~ WS_CAPTION
         set_window_long(hwnd, GWL_STYLE, new_style)
         set_window_pos(hwnd, 0, 0, 0, 0, 0, SWP_NOMOVE | SWP_NOSIZE | SWP_NOZORDER | SWP_FRAMECHANGED)
 
     @classmethod
-    def unhide(cls, window):
+    def unhide(cls, window) -> None:
         hwnd = module_find(window)
         old_style = get_window_long(hwnd, GWL_STYLE)
         new_style = old_style | WS_CAPTION
         set_window_long(hwnd, GWL_STYLE, new_style)
         set_window_pos(hwnd, 0, 0, 0, 0, 0, SWP_NOMOVE | SWP_NOSIZE | SWP_NOZORDER | SWP_FRAMECHANGED)
 
 class maximize_minimize_button():
     @classmethod
-    def hide(cls, window):
+    def hide(cls, window) -> None:
         hwnd = module_find(window)
         old_style = get_window_long(hwnd, GWL_STYLE)
         new_style = old_style & ~ WS_MAXIMIZEBOX & ~ WS_MINIMIZEBOX
         set_window_long(hwnd, GWL_STYLE, new_style)
         set_window_pos(hwnd, 0, 0, 0, 0, 0, SWP_NOMOVE | SWP_NOSIZE | SWP_NOZORDER | SWP_FRAMECHANGED)
     
     @classmethod
-    def unhide(cls, window):
+    def unhide(cls, window) -> None:
         hwnd = module_find(window)
         old_style = get_window_long(hwnd, GWL_STYLE)
         new_style = old_style | WS_MAXIMIZEBOX | WS_MINIMIZEBOX
         set_window_long(hwnd, GWL_STYLE, new_style)
         set_window_pos(hwnd, 0, 0, 0, 0, 0, SWP_NOMOVE | SWP_NOSIZE | SWP_NOZORDER | SWP_FRAMECHANGED)
 
 class maximize_button:
     @classmethod
-    def disable(cls, window):
+    def disable(cls, window) -> None:
         hwnd = module_find(window)
         old_style = get_window_long(hwnd, GWL_STYLE)
         new_style = old_style & ~WS_MAXIMIZEBOX
         set_window_long(hwnd, GWL_STYLE, new_style)
         set_window_pos(hwnd, 0, 0, 0, 0, 0, SWP_NOMOVE | SWP_NOSIZE | SWP_NOZORDER | SWP_FRAMECHANGED)
     
     @classmethod
-    def enable(cls, window):
+    def enable(cls, window) -> None:
         hwnd = module_find(window)
         old_style = get_window_long(hwnd, GWL_STYLE)
         new_style = old_style | WS_MAXIMIZEBOX
         set_window_long(hwnd, GWL_STYLE, new_style)
         set_window_pos(hwnd, 0, 0, 0, 0, 0, SWP_NOMOVE | SWP_NOSIZE | SWP_NOZORDER | SWP_FRAMECHANGED)
 
 class minimize_button:
     @classmethod
-    def disable(cls, window):
+    def disable(cls, window) -> None:
         hwnd = module_find(window)
         old_style = get_window_long(hwnd, GWL_STYLE)
         new_style = old_style & ~WS_MINIMIZEBOX
         set_window_long(hwnd, GWL_STYLE, new_style)
         set_window_pos(hwnd, 0, 0, 0, 0, 0, SWP_NOMOVE | SWP_NOSIZE | SWP_NOZORDER | SWP_FRAMECHANGED)
     
     @classmethod
-    def enable(cls, window):
+    def enable(cls, window) -> None:
         hwnd = module_find(window)
         old_style = get_window_long(hwnd, GWL_STYLE)
         new_style = old_style | WS_MINIMIZEBOX
         set_window_long(hwnd, GWL_STYLE, new_style)
         set_window_pos(hwnd, 0, 0, 0, 0, 0, SWP_NOMOVE | SWP_NOSIZE | SWP_NOZORDER | SWP_FRAMECHANGED)
 
 class all_stuffs():
     @classmethod
-    def hide(cls, window):
+    def hide(cls, window) -> None:
         hwnd = module_find(window)
         old_style = get_window_long(hwnd, GWL_STYLE)
         new_style = old_style & ~ WS_SYSMENU
         set_window_long(hwnd, GWL_STYLE, new_style)
         set_window_pos(hwnd, 0, 0, 0, 0, 0, SWP_NOMOVE | SWP_NOSIZE | SWP_NOZORDER | SWP_FRAMECHANGED)
+
     
     @classmethod
-    def unhide(cls, window):
+    def unhide(cls, window) -> None:
         hwnd = module_find(window)
         old_style = get_window_long(hwnd, GWL_STYLE)
         new_style = old_style | WS_SYSMENU
         set_window_long(hwnd, GWL_STYLE, new_style)
         set_window_pos(hwnd, 0, 0, 0, 0, 0, SWP_NOMOVE | SWP_NOSIZE | SWP_NOZORDER | SWP_FRAMECHANGED)
 
 class window_flash:
     @classmethod
-    def flash(cls, window, count=5, interval=1000):
+    def flash(cls, window, count=5, interval=1000) -> None:
         hwnd = module_find(window)
         info = FLASHWINFO(
             cbSize=ctypes.sizeof(FLASHWINFO),
             hwnd=hwnd,
             dwFlags=FLASHW_ALL | FLASHW_TIMER,
             uCount=count,
             dwTimeout=interval
         )
         flash_window_ex(ctypes.pointer(info))
 
     @classmethod
-    def stop(cls, window):
+    def stop(cls, window) -> None:
         hwnd = module_find(window)
         info = FLASHWINFO(
             cbSize=ctypes.sizeof(FLASHWINFO),
             hwnd=hwnd,
             dwFlags=FLASHW_STOP,
             uCount=0,
             dwTimeout=0
         )
         flash_window_ex(ctypes.pointer(info))
 
 class opacity():
     @classmethod
-    def set(cls, window, opacity):
+    def set(cls, window, opacity) -> None:
         hwnd = module_find(window)
         old_ex_style = get_window_long(hwnd, GWL_EXSTYLE)
         new_ex_style = old_ex_style | WS_EX_LAYERED
         set_window_long(hwnd, GWL_EXSTYLE, new_ex_style)
 
         # Opacity is a value between 0 (transparent) and 255 (opaque)
         # If the input is a float between 0.0 and 1.0, convert it to an integer between 0 and 255
         if isinstance(opacity, float) and 0.0 <= opacity <= 1.0:
             opacity = int(opacity * 255)
 
         ctypes.windll.user32.SetLayeredWindowAttributes(hwnd, 0, opacity, LWA_ALPHA)
 
 class title_bar_color:
     @classmethod
-    def set(cls, window, color):
+    def set(cls, window, color) -> None:
         color = convert_color(color)
         hwnd = module_find(window)
         old_ex_style = get_window_long(hwnd, GWL_EXSTYLE)
         new_ex_style = old_ex_style | WS_EX_LAYERED
         set_window_long(hwnd, GWL_EXSTYLE, new_ex_style)
         ctypes.windll.dwmapi.DwmSetWindowAttribute(hwnd, 35, ctypes.byref(ctypes.c_int(color)), 4)
         set_window_long(hwnd, GWL_EXSTYLE, old_ex_style)  # Reset the window style
 
+    @classmethod
+    def reset(cls, window) -> None:
+        hwnd = module_find(window)
+        old_ex_style = get_window_long(hwnd, GWL_EXSTYLE)
+        new_ex_style = old_ex_style | WS_EX_LAYERED
+        set_window_long(hwnd, GWL_EXSTYLE, new_ex_style)
+        ctypes.windll.dwmapi.DwmSetWindowAttribute(hwnd, 35, ctypes.byref(ctypes.c_int(-1)), 4)
+        set_window_long(hwnd, GWL_EXSTYLE, old_ex_style)
+
 class title_bar_text_color:
     @classmethod
-    def set(cls, window, color):
+    def set(cls, window, color) -> None:
         color = convert_color(color)
         hwnd = module_find(window)
         old_ex_style = get_window_long(hwnd, GWL_EXSTYLE)
         new_ex_style = old_ex_style | WS_EX_LAYERED
         set_window_long(hwnd, GWL_EXSTYLE, new_ex_style)
         ctypes.windll.dwmapi.DwmSetWindowAttribute(hwnd, 36, ctypes.byref(ctypes.c_int(color)), 4)
         set_window_long(hwnd, GWL_EXSTYLE, old_ex_style)  # Reset the window style
 
+    @classmethod
+    def reset(cls, window) -> None:
+        hwnd = module_find(window)
+        old_ex_style = get_window_long(hwnd, GWL_EXSTYLE)
+        new_ex_style = old_ex_style | WS_EX_LAYERED
+        set_window_long(hwnd, GWL_EXSTYLE, new_ex_style)
+        ctypes.windll.dwmapi.DwmSetWindowAttribute(hwnd, 36, ctypes.byref(ctypes.c_int(-1)), 4)
+        set_window_long(hwnd, GWL_EXSTYLE, old_ex_style)
+
+class border_color:
+    @classmethod
+    def set(cls, window, color) -> None:
+        color = convert_color(color)
+        hwnd = module_find(window)
+        old_ex_style = get_window_long(hwnd, GWL_EXSTYLE)
+        new_ex_style = old_ex_style | WS_EX_LAYERED
+        set_window_long(hwnd, GWL_EXSTYLE, new_ex_style)
+        ctypes.windll.dwmapi.DwmSetWindowAttribute(hwnd, 34, ctypes.byref(ctypes.c_int(color)), 4)
+        set_window_long(hwnd, GWL_EXSTYLE, old_ex_style)  # Reset the window style
+
+    @classmethod
+    def reset(cls, window) -> None:
+        hwnd = module_find(window)
+        old_ex_style = get_window_long(hwnd, GWL_EXSTYLE)
+        new_ex_style = old_ex_style | WS_EX_LAYERED
+        set_window_long(hwnd, GWL_EXSTYLE, new_ex_style)
+        ctypes.windll.dwmapi.DwmSetWindowAttribute(hwnd, 34, ctypes.byref(ctypes.c_int(-1)), 4)
+        set_window_long(hwnd, GWL_EXSTYLE, old_ex_style)
+
 class rainbow_title_bar:
     @classmethod
-    def start(cls, window, interval=3, color_stops=3):
+    def start(cls, window, interval=3, color_stops=3) -> None:
         def color_changer(hwnd, interval):
             r, g, b = 200, 0, 0
             while hwnd in rnbtbs:
                 color = (r << 16) | (g << 8) | b
 
                 ctypes.windll.dwmapi.DwmSetWindowAttribute(hwnd, 35, ctypes.byref(ctypes.c_int(color)), 4)
                 if r < 255 and g == 0 and b == 0:
@@ -215,39 +291,86 @@
                     g = max(0, g - color_stops)
                 elif b == 255 and r < 255 and g == 0:
                     r = min(255, r + color_stops)
                 elif b > 0 and r == 255 and g == 0:
                     b = max(0, b - color_stops)
                 ctypes.windll.kernel32.Sleep(interval)
             else:
-                ctypes.windll.dwmapi.DwmSetWindowAttribute(hwnd, 35, ctypes.byref(ctypes.c_int(0)), 4)
+                ctypes.windll.dwmapi.DwmSetWindowAttribute(hwnd, 35, ctypes.byref(ctypes.c_int(-1)), 4)
 
         hwnd = module_find(window)
         old_ex_style = get_window_long(hwnd, GWL_EXSTYLE)
         new_ex_style = old_ex_style | WS_EX_LAYERED
         set_window_long(hwnd, GWL_EXSTYLE, new_ex_style)
 
         rnbtbs.append(hwnd)
         thread = threading.Thread(target=color_changer, args=(hwnd, interval))
         thread.daemon = True
         thread.start()
 
         set_window_long(hwnd, GWL_EXSTYLE, old_ex_style)  # Reset the window style
 
     @classmethod
-    def stop(cls, window):
+    def stop(cls, window) -> None:
         hwnd = module_find(window)
         if hwnd in rnbtbs:
             rnbtbs.remove(hwnd)
         else:
             raise ValueError('Rainbow title bar is not running on this window.')
 
+class rainbow_border:
+    @classmethod
+    def start(cls, window, interval=3, color_stops=3) -> None:
+        def color_changer(hwnd, interval):
+            r, g, b = 200, 0, 0
+            while hwnd in rnbbcs:
+                color = (r << 16) | (g << 8) | b
+
+                ctypes.windll.dwmapi.DwmSetWindowAttribute(hwnd, 34, ctypes.byref(ctypes.c_int(color)), 4)
+                if r < 255 and g == 0 and b == 0:
+                    r = min(255, r + color_stops)
+                elif r == 255 and g < 255 and b == 0:
+                    g = min(255, g + color_stops)
+                elif r > 0 and g == 255 and b == 0:
+                    r = max(0, r - color_stops)
+                elif g == 255 and b < 255 and r == 0:
+                    b = min(255, b + color_stops)
+                elif g > 0 and b == 255 and r == 0:
+                    g = max(0, g - color_stops)
+                elif b == 255 and r < 255 and g == 0:
+                    r = min(255, r + color_stops)
+                elif b > 0 and r == 255 and g == 0:
+                    b = max(0, b - color_stops)
+                ctypes.windll.kernel32.Sleep(interval)
+            else:
+                ctypes.windll.dwmapi.DwmSetWindowAttribute(hwnd, 34, ctypes.byref(ctypes.c_int(-1)), 4)
+
+        hwnd = module_find(window)
+        old_ex_style = get_window_long(hwnd, GWL_EXSTYLE)
+        new_ex_style = old_ex_style | WS_EX_LAYERED
+        set_window_long(hwnd, GWL_EXSTYLE, new_ex_style)
+
+        rnbbcs.append(hwnd)
+        thread = threading.Thread(target=color_changer, args=(hwnd, interval))
+        thread.daemon = True
+        thread.start()
+
+        set_window_long(hwnd, GWL_EXSTYLE, old_ex_style)  # Reset the window style
+
+    @classmethod
+    def stop(cls, window) -> None:
+        hwnd = module_find(window)
+        if hwnd in rnbbcs:
+            rnbbcs.remove(hwnd)
+        else:
+            raise ValueError('Rainbow border is not running on this window.')
+
 class window_frame:
     @classmethod
-    def center(cls, window):
+    def center(cls, window) -> None:
         hwnd = module_find(window)
 
         # Get the window's current position and size
         rect = ctypes.wintypes.RECT()
         ctypes.windll.user32.GetWindowRect(hwnd, ctypes.byref(rect))
         window_width = rect.right - rect.left
         window_height = rect.bottom - rect.top
@@ -260,15 +383,15 @@
         new_x = (screen_width - window_width) // 2
         new_y = (screen_height - window_height) // 2
 
         # Set the window's new position
         ctypes.windll.user32.SetWindowPos(hwnd, 0, new_x, new_y, 0, 0, 0x0001)
 
     @classmethod
-    def center_relative(cls, window_parent, window_child):
+    def center_relative(cls, window_parent, window_child) -> None:
         hwnd_parent = module_find(window_parent)
         hwnd_child = module_find(window_child)
 
         # Get the parent window's current position and size
         rect_parent = ctypes.wintypes.RECT()
         ctypes.windll.user32.GetWindowRect(hwnd_parent, ctypes.byref(rect_parent))
         parent_width = rect_parent.right - rect_parent.left
@@ -284,41 +407,41 @@
         new_x = rect_parent.left + (parent_width - child_width) // 2
         new_y = rect_parent.top + (parent_height - child_height) // 2
 
         # Set the child window's new position
         ctypes.windll.user32.SetWindowPos(hwnd_child, 0, new_x, new_y, 0, 0, 0x0001)
 
     @classmethod
-    def move(cls, window, x, y):
+    def move(cls, window, x, y) -> None:
         hwnd = module_find(window)
         set_window_pos(hwnd, 0, x, y, 0, 0, 0x0001)
 
     @classmethod
-    def resize(cls, window, width, height):
+    def resize(cls, window, width, height) -> None:
         hwnd = module_find(window)
         set_window_pos(hwnd, 0, 0, 0, width, height, 0x0001)
 
     @classmethod
-    def minimize(cls, window):
+    def minimize(cls, window) -> None:
         hwnd = module_find(window)
         ctypes.windll.user32.ShowWindow(hwnd, 6)
 
     @classmethod
-    def maximize(cls, window):
+    def maximize(cls, window) -> None:
         hwnd = module_find(window)
         ctypes.windll.user32.ShowWindow(hwnd, 3)
 
     @classmethod
-    def restore(cls, window):
+    def restore(cls, window) -> None:
         hwnd = module_find(window)
         ctypes.windll.user32.ShowWindow(hwnd, 9)
 
 class window_animation:
     @classmethod
-    def circle_motion(cls, window, count=5, interval=5, radius=20):
+    def circle_motion(cls, window, count=5, interval=5, radius=20) -> None:
         def motion():
             hwnd = module_find(window)
             rect = ctypes.wintypes.RECT()
             ctypes.windll.user32.GetWindowRect(hwnd, ctypes.byref(rect))
             original_x = rect.left
             original_y = rect.top
             for angle in range(0, 360 * count, 5):  # move in a circle count times
@@ -329,15 +452,15 @@
                 ctypes.windll.kernel32.Sleep(interval)
 
         thread = threading.Thread(target=motion)
         thread.daemon = True
         thread.start()
 
     @classmethod
-    def vertical_shake(cls, window, count=5, interval=3, amplitude=20):
+    def vertical_shake(cls, window, count=5, interval=3, amplitude=20) -> None:
         def motion():
             hwnd = module_find(window)
             rect = ctypes.wintypes.RECT()
             ctypes.windll.user32.GetWindowRect(hwnd, ctypes.byref(rect))
             original_y = rect.top
             for offset in range(0, 360 * count, count):  # move up and down 5 times
                 rad = math.radians(offset)
@@ -346,15 +469,15 @@
                 ctypes.windll.kernel32.Sleep(interval)
 
         thread = threading.Thread(target=motion)
         thread.daemon = True
         thread.start()
 
     @classmethod
-    def horizontal_shake(cls, window, count=5, interval=3, amplitude=20):
+    def horizontal_shake(cls, window, count=5, interval=3, amplitude=20) -> None:
         def motion():
             hwnd = module_find(window)
             rect = ctypes.wintypes.RECT()
             ctypes.windll.user32.GetWindowRect(hwnd, ctypes.byref(rect))
             original_x = rect.left
             for offset in range(0, 360 * count, count):  # move left and right 5 times
                 rad = math.radians(offset)
@@ -364,36 +487,36 @@
 
         thread = threading.Thread(target=motion)
         thread.daemon = True
         thread.start()
 
 class title_text:
     @classmethod
-    def set(cls, window, title):
+    def set(cls, window, title) -> None:
         hwnd = module_find(window)
         ctypes.windll.user32.SetWindowTextW(hwnd, title)
 
     @classmethod
-    def stylize(cls, window, style=1):
+    def stylize(cls, window, style=1) -> None:
         hwnd = module_find(window)
         if hwnd not in titles:
             title = ctypes.create_unicode_buffer(1024)
             ctypes.windll.user32.GetWindowTextW(hwnd, title, 1024)
             titles[hwnd] = title.value
         title = stylize_text(titles[hwnd], style)
         ctypes.windll.user32.SetWindowTextW(hwnd, title)
 
     @classmethod
-    def reset(cls, window):
+    def reset(cls, window) -> None:
         hwnd = module_find(window)
         if hwnd in titles:
             ctypes.windll.user32.SetWindowTextW(hwnd, titles[hwnd])
             del titles[hwnd]
 
-def stylize_text(text, style):
+def stylize_text(text: str, style: int) -> str:
     normal = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ1234567890"
     styles = [
         "𝔞𝔟𝔠𝔡𝔢𝔣𝔤𝔥𝔦𝔧𝔨𝔩𝔪𝔫𝔬𝔭𝔮𝔯𝔰𝔱𝔲𝔳𝔴𝔵𝔶𝔷𝔄𝔅ℭ𝔇𝔈𝔉𝔊ℌℑ𝔍𝔎𝔏𝔐𝔑𝔒𝔓𝔔ℜ𝔖𝔗𝔘𝔙𝔚𝔛𝔜ℨ1234567890",
         "𝖆𝖇𝖈𝖉𝖊𝖋𝖌𝖍𝖎𝖏𝖐𝖑𝖒𝖓𝖔𝖕𝖖𝖗𝖘𝖙𝖚𝖛𝖜𝖝𝖞𝖟𝕬𝕭𝕮𝕯𝕰𝕱𝕲𝕳𝕴𝕵𝕶𝕷𝕸𝕹𝕺𝕻𝕼𝕽𝕾𝕿𝖀𝖁𝖂𝖃𝖄𝖅1234567890",
         "𝓪𝓫𝓬𝓭𝓮𝓯𝓰𝓱𝓲𝓳𝓴𝓵𝓶𝓷𝓸𝓹𝓺𝓻𝓼𝓽𝓾𝓿𝔀𝔁𝔂𝔃𝓐𝓑𝓒𝓓𝓔𝓕𝓖𝓗𝓘𝓙𝓚𝓛𝓜𝓝𝓞𝓟𝓠𝓡𝓢𝓣𝓤𝓥𝓦𝓧𝓨𝓩1234567890",
         "𝒶𝒷𝒸𝒹𝑒𝒻𝑔𝒽𝒾𝒿𝓀𝓁𝓂𝓃𝑜𝓅𝓆𝓇𝓈𝓉𝓊𝓋𝓌𝓍𝓎𝓏𝒜𝐵𝒞𝒟𝐸𝐹𝒢𝐻𝐼𝒥𝒦𝐿𝑀𝒩𝒪𝒫𝒬𝑅𝒮𝒯𝒰𝒱𝒲𝒳𝒴𝒵𝟣𝟤𝟥𝟦𝟧𝟨𝟩𝟪𝟫𝟢",
         "🅰🅱🅲🅳🅴🅵🅶🅷🅸🅹🅺🅻🅼🅽🅾🅿🆀🆁🆂🆃🆄🆅🆆🆇🆈🆉🅰🅱🅲🅳🅴🅵🅶🅷🅸🅹🅺🅻🅼🅽🅾🅿🆀🆁🆂🆃🆄🆅🆆🆇🆈🆉1234567890",
@@ -406,25 +529,25 @@
 
     if style < 1 or style > len(styles):
         raise ValueError("Invalid style number")
 
     translation_table = str.maketrans(normal, styles[style - 1])
     return text.translate(translation_table)
 
-def convert_color(color):
+def convert_color(color: tuple) -> int:
     if isinstance(color, tuple) and len(color) == 3:  # RGB format
         r, g, b = color
         return int(f"{b}{g}{r}", 16)
     elif isinstance(color, str) and color.startswith('#'):  # HEX format
         r, g, b = color[1:3], color[3:5], color[5:7]
         return int(f"{b}{g}{r}", 16)
     else:
         raise ValueError('Invalid color format. Expected RGB tuple or HEX string.')
 
-def module_find(window):
+def module_find(window) -> int:
     try:
         window.update() # for tk
         return ctypes.windll.user32.GetParent(window.winfo_id())
     except:
         pass
     try:
         return window.winId().__int__() # for pyQt and PySide
@@ -435,8 +558,8 @@
     except:
         pass
     try:
         gdk_window = window.get_window() # for PyGTK
         return gdk_window.get_xid()
     except:
         pass
-    return window    # others / notfound
+    return window    # others / notfound
```

### Comparing `hPyT-1.2.1/hPyT.egg-info/PKG-INFO` & `hpyt-1.3.0/hPyT.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hPyT
-Version: 1.2.1
+Version: 1.3.0
 Summary: Hack Python Titlebar - A package to manipulate windows and titlebar of GUI applications made using python.
 Home-page: https://github.com/zingzy/hPyT
 Author: zingzy
 License: MIT
 Keywords: Tkinter wxpython pyqt pyside GUI window controls decorations hide show titlebar
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,58 +13,62 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hPyT - Hack Python Titlebar
 
 A package to manipulate windows and titlebar of GUI applications made using python
 **Supports Both Windows 11 and 10**
 
-https://github.com/Zingzy/hPyT/assets/90309290/c61b3142-80d6-4c07-b8e3-65694faf945b
+https://github.com/Zingzy/hPyT/assets/90309290/f86df1c7-b75b-4477-974a-eb34cc117df3
 
-**You can download the above app from the [github releases](https://github.com/Zingzy/hPyT/releases/tag/v1.1.0/) to test out the package before installing/using it in your projects**
+**You can download the above app from the [github releases](https://github.com/Zingzy/hPyT/releases/tag/hPyT-preview/) to test out the package before installing/using it in your projects**
 
 <br>
 
 <details>
 
 <summary>📖 Table of Contents</summary>
 
 - [hPyT - Hack Python Titlebar](#hpyt---hack-python-titlebar)
 	- [📚 Supported Libraries](#-supported-libraries)
 	- [📦 Installing](#-installing)
 	- [📥 Importing](#-importing)
 	- [Hide/Unhide Title Bar](#hideunhide-title-bar)
 	- [🌈 Rainbow TitleBar](#-rainbow-titlebar)
+	- [🌈 Rainbow Border](#-rainbow-border)
 	- [Hide/Unhide both Maximize and Minimize Buttons (Completely Hides both buttons)](#hideunhide-both-maximize-and-minimize-buttons-completely-hides-both-buttons)
 	- [Hide/Unhide All Buttons or Stuffs](#hideunhide-all-buttons-or-stuffs)
 	- [Enable/Disable Maximize Button](#enabledisable-maximize-button)
 	- [Enable/Disable Minimize Button](#enabledisable-minimize-button)
 	- [Opacity](#opacity)
 	- [⚡ Flashing Window](#-flashing-window)
 	- [🎨 Custom TitleBar Color](#-custom-titlebar-color)
 	- [🖌️ Custom TitleBar Text Color](#️-custom-titlebar-text-color)
+	- [🖌️ Custom Border Color](#️-custom-border-color)
 	- [💻 Window Management](#-window-management)
 		- [Center a window on the screen](#center-a-window-on-the-screen)
 		- [Center a secondary window relative to the primary window](#center-a-secondary-window-relative-to-the-primary-window)
 		- [Other basic window management functions](#other-basic-window-management-functions)
 	- [✨ Window Animations](#-window-animations)
 		- [Circle Motion](#circle-motion)
 		- [Verical Shake](#verical-shake)
 		- [Horizontal Shake](#horizontal-shake)
 	- [✏️ Stylize text](#️-stylize-text)
 		- [Miscellaneous](#miscellaneous)
 	- [📜 hPyT Changelog](#-hpyt-changelog)
+		- [v1.3.0](#v130)
 		- [v1.2.1](#v121)
 		- [v1.2.0](#v120)
 		- [v1.1.3](#v113)
 		- [v1.1.2](#v112)
 		- [v1.1.1](#v111)
 		- [v1.1.0](#v110)
 </details>
@@ -78,15 +82,15 @@
 - PySide
 - WxPython
 - support for more libraries soon...
 
 ## 📦 Installing
 
 ```powershell
-pip install hPyT==1.2.1
+pip install hPyT==1.3.0
 ```
 
 ## 📥 Importing
 
 ```python
 from hPyT import *
 from customtkinter import * # you can use any other library from the above mentioned list
@@ -97,27 +101,37 @@
 ## Hide/Unhide Title Bar
 
 ```python
 title_bar.hide(window) # hides full titlebar
 # title_bar.unhide(window)
 ```
 
-![Hidden Title Bar](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/titlebar.png)
+![image](https://github.com/littlewhitecloud/hPyT/assets/71159641/03e533fe-c42a-4d84-b138-176a73ad7977)
 
 ## 🌈 Rainbow TitleBar
 
 ```python
 rainbow_title_bar.start(window, interval=5) # starts the rainbow titlebar
 # rainbow_title_bar.stop(window) # stops the rainbow titlebar
 ```
 
-*`interval` is the time in milliseconds in which the color would change*
+> [!NOTE]
+> *`interval` is the time in milliseconds in which the color would change*
 
 ![Rainbow TitleBar](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/rainbow_titlebar.gif)
 
+## 🌈 Rainbow Border
+
+```python
+rainbow_border.start(window, interval=4) # starts the rainbow border
+# rainbow_border.stop(window) # stops the rainbow border
+```
+
+![Rainbow Border](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/rainbow_border.gif)
+
 ## Hide/Unhide both Maximize and Minimize Buttons (Completely Hides both buttons)
 
 ```python
 maximize_minimize_button.hide(window) # hides both maximize and minimize button
 # maximize_minimize_button.unhide(window)
 ```
 
@@ -172,30 +186,40 @@
 
 ![Flashing Window](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/flashing.gif)
 
 ## 🎨 Custom TitleBar Color
 
 ```python
 title_bar_color.set(window, '#ff00ff') # sets the titlebar color to magenta
+# title_bar_color.reset(window) # resets the titlebar color to default
 ```
 
-*You can pass any valid color in `Hex` or `RGB` format*
+> [!NOTE]
+> *You can pass any valid color in `Hex` or `RGB` format*
 
 ![Custom TitleBar Color](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/titlebar_color.png)
 
 ## 🖌️ Custom TitleBar Text Color
 
 ```python
 title_text_color.set(window, '#ff00ff') # sets the titlebar text color to magenta
+# title_text_color.reset(window) # resets the titlebar text color to default
 ```
 
-*You can pass any valid color in `Hex` or `RGB` format*
-
 ![Custom TitleBar Text Color](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/title_text_color.png)
 
+## 🖌️ Custom Border Color
+
+```python
+border_color.set(window, '#ff00ff') # sets the border color to magenta
+# border_color.reset(window) # resets the border color to default
+```
+
+![Custom Border Color](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/border_color.png)
+
 ## 💻 Window Management
 
 ### Center a window on the screen
 
 ```python
 window_frame.center(window)
 ```
@@ -245,22 +269,22 @@
 ![Circle Motion](https://raw.githubusercontent.com/zingzy/hPyT/main/assets/circle_motion.gif)
 
 *The animation might appear a bit fasterer and rougher in the above preview gif than it is*
 
 ### Verical Shake
 
 ```python
-window_animation.vertical_shake(window, count=5, interval=5, apmlitude=20)
+window_animation.vertical_shake(window, count=5, interval=5, amplitude=20)
 # shakes the window vertically 5 times with 5ms interval and 10px distance
 ```
 
 ### Horizontal Shake
 
 ```python
-window_animation.horizontal_shake(window, count=5, interval=5, apmlitude=20)
+window_animation.horizontal_shake(window, count=5, interval=5, amplitude=20)
 # shakes the window horizontally 5 times with 5ms interval and 10px distance
 ```
 
 ## ✏️ Stylize text
 
 ```python
 title_text.stylize(window, style=1)
@@ -278,14 +302,21 @@
 >>> "𝔜𝔬𝔲𝔯 ℭ𝔲𝔰𝔱𝔬𝔪 𝔗𝔢𝔵𝔱"
 ```
 
 <br>
 
 ## 📜 hPyT Changelog
 
+### v1.3.0
+
+- Add support for setting custom border color
+- Add support for rainbow border color effect
+- Add support for resetting the titleBar color and titleText color
+- Fix an issue which caused the titleBar to appear black after the rainbow titleBar effect was stopped
+
 ### v1.2.1
 
 - Minor Bug Fixes
 
 ### v1.2.0
 
 - Add support for rainbow titlebar
```

### Comparing `hPyT-1.2.1/setup.py` & `hpyt-1.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='hPyT',
-    version='1.2.1',
+    version='1.3.0',
     description='Hack Python Titlebar - A package to manipulate windows and titlebar of GUI applications made using python.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='zingzy',
     url='https://github.com/zingzy/hPyT',
     license='MIT',
     packages=find_packages(),
@@ -21,11 +21,12 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11' ,
+        'Programming Language :: Python :: 3.12' ,
         "Operating System :: Microsoft :: Windows",
     ],
     keywords='Tkinter wxpython pyqt pyside GUI window controls decorations hide show titlebar',
 )
```


# Comparing `tmp/pgpyui-0.0.1.tar.gz` & `tmp/pgpyui-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgpyui-0.0.1.tar", last modified: Wed Apr 24 14:09:13 2024, max compression
+gzip compressed data, was "pgpyui-0.0.2.tar", last modified: Wed Apr 24 14:50:46 2024, max compression
```

## Comparing `pgpyui-0.0.1.tar` & `pgpyui-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 14:09:13.391296 pgpyui-0.0.1/
--rw-rw-rw-   0        0        0     2249 2024-04-24 14:09:13.391296 pgpyui-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1669 2024-04-24 13:59:43.000000 pgpyui-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 14:09:13.372306 pgpyui-0.0.1/pgpyui/
--rw-rw-rw-   0        0        0      149 2024-04-24 13:50:35.000000 pgpyui-0.0.1/pgpyui/__init__.py
--rw-rw-rw-   0        0        0     2296 2024-04-24 13:49:49.000000 pgpyui-0.0.1/pgpyui/button.py
--rw-rw-rw-   0        0        0     5498 2024-04-24 13:50:25.000000 pgpyui-0.0.1/pgpyui/textarea.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:09:13.390294 pgpyui-0.0.1/pgpyui.egg-info/
--rw-rw-rw-   0        0        0     2249 2024-04-24 14:09:13.000000 pgpyui-0.0.1/pgpyui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2024-04-24 14:09:13.000000 pgpyui-0.0.1/pgpyui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 14:09:13.000000 pgpyui-0.0.1/pgpyui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-24 14:09:13.000000 pgpyui-0.0.1/pgpyui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-24 14:09:13.000000 pgpyui-0.0.1/pgpyui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 14:09:13.393297 pgpyui-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      822 2024-04-24 14:09:08.000000 pgpyui-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:50:46.724336 pgpyui-0.0.2/
+-rw-rw-rw-   0        0        0     2289 2024-04-24 14:50:46.724336 pgpyui-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1709 2024-04-24 14:49:10.000000 pgpyui-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 14:50:46.701338 pgpyui-0.0.2/pgpyui/
+-rw-rw-rw-   0        0        0      149 2024-04-24 13:50:35.000000 pgpyui-0.0.2/pgpyui/__init__.py
+-rw-rw-rw-   0        0        0     2294 2024-04-24 14:47:53.000000 pgpyui-0.0.2/pgpyui/button.py
+-rw-rw-rw-   0        0        0     5496 2024-04-24 14:48:03.000000 pgpyui-0.0.2/pgpyui/textarea.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:50:46.723346 pgpyui-0.0.2/pgpyui.egg-info/
+-rw-rw-rw-   0        0        0     2289 2024-04-24 14:50:46.000000 pgpyui-0.0.2/pgpyui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2024-04-24 14:50:46.000000 pgpyui-0.0.2/pgpyui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 14:50:46.000000 pgpyui-0.0.2/pgpyui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-24 14:50:46.000000 pgpyui-0.0.2/pgpyui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 14:50:46.000000 pgpyui-0.0.2/pgpyui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 14:50:46.726336 pgpyui-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      822 2024-04-24 14:47:34.000000 pgpyui-0.0.2/setup.py
```

### Comparing `pgpyui-0.0.1/PKG-INFO` & `pgpyui-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgpyui
-Version: 0.0.1
+Version: 0.0.2
 Summary: The package is an add-on for Pygame to create a user interface on the screen.
 Home-page: https://pypi.org/project/pgpyui/
 Author: Memdved
 Author-email: mixail.vilyukov@icloud.com
 Project-URL: GitHub, https://github.com/Memdved
 Keywords: ui gui pgpyui pygame
 Classifier: Programming Language :: Python :: 3.10
@@ -13,39 +13,38 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests>=2.25.1
 
 # pgpyui
 
 pgpyui is an add-on module for pygame to create a user interface.
-It has a button and text area.
 
 ## Installation
 
 ```
 pip install pgpyui
 ```
 
 ## Usage
 
 ```python
-import pgpyui
+from pgpyui import button, textarea
 import pygame
 
 # Initialize pygame
 pygame.init()
 
 # Create a window
 window = pygame.display.set_mode((800, 600))
 
 # Create a button
-button = pgpyui.Button((100, 100), (200, 50), "Click me!", lambda: print("Button clicked!"))
+button = button.Button((100, 100), (200, 50), "Click me!", lambda: print("Button clicked!"))
 
 # Create a text area
-text_area = pgpyui.TextArea((100, 200), (200, 200), 20, 100)
+text_area = textarea.TextArea((100, 200), (200, 200), 20, 100)
 
 # Game loop
 running = True
 while running:
 # Handle events
     for event in pygame.event.get():
         if event.type == pygame.QUIT:
@@ -90,7 +89,11 @@
 * `max_symbols`: The maximum number of symbols that can be entered.
 * `is_enter`: Whether or not the enter key should be allowed.
 * `font`: The name of the font to use (optional).
 
 ## License
 
 MIT
+
+## Author mail
+
+mixail.vilyukov@icloud.com
```

### Comparing `pgpyui-0.0.1/README.md` & `pgpyui-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 # pgpyui
 
 pgpyui is an add-on module for pygame to create a user interface.
-It has a button and text area.
 
 ## Installation
 
 ```
 pip install pgpyui
 ```
 
 ## Usage
 
 ```python
-import pgpyui
+from pgpyui import button, textarea
 import pygame
 
 # Initialize pygame
 pygame.init()
 
 # Create a window
 window = pygame.display.set_mode((800, 600))
 
 # Create a button
-button = pgpyui.Button((100, 100), (200, 50), "Click me!", lambda: print("Button clicked!"))
+button = button.Button((100, 100), (200, 50), "Click me!", lambda: print("Button clicked!"))
 
 # Create a text area
-text_area = pgpyui.TextArea((100, 200), (200, 200), 20, 100)
+text_area = textarea.TextArea((100, 200), (200, 200), 20, 100)
 
 # Game loop
 running = True
 while running:
 # Handle events
     for event in pygame.event.get():
         if event.type == pygame.QUIT:
@@ -73,8 +72,12 @@
 * `font_size`: The size of the font.
 * `max_symbols`: The maximum number of symbols that can be entered.
 * `is_enter`: Whether or not the enter key should be allowed.
 * `font`: The name of the font to use (optional).
 
 ## License
 
-MIT
+MIT
+
+## Author mail
+
+mixail.vilyukov@icloud.com
```

### Comparing `pgpyui-0.0.1/pgpyui/button.py` & `pgpyui-0.0.2/pgpyui/button.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __init__ import *
+from pgpyui import *
 
 
 class Button:
     """
     A class to create a button.
 
     Displays a button.
```

### Comparing `pgpyui-0.0.1/pgpyui/textarea.py` & `pgpyui-0.0.2/pgpyui/textarea.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __init__ import *
+from pgpyui import *
 
 
 class TextArea:
     """
     A class for creating a Text Area.
 
     It is a multi-line control
```

### Comparing `pgpyui-0.0.1/pgpyui.egg-info/PKG-INFO` & `pgpyui-0.0.2/pgpyui.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgpyui
-Version: 0.0.1
+Version: 0.0.2
 Summary: The package is an add-on for Pygame to create a user interface on the screen.
 Home-page: https://pypi.org/project/pgpyui/
 Author: Memdved
 Author-email: mixail.vilyukov@icloud.com
 Project-URL: GitHub, https://github.com/Memdved
 Keywords: ui gui pgpyui pygame
 Classifier: Programming Language :: Python :: 3.10
@@ -13,39 +13,38 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests>=2.25.1
 
 # pgpyui
 
 pgpyui is an add-on module for pygame to create a user interface.
-It has a button and text area.
 
 ## Installation
 
 ```
 pip install pgpyui
 ```
 
 ## Usage
 
 ```python
-import pgpyui
+from pgpyui import button, textarea
 import pygame
 
 # Initialize pygame
 pygame.init()
 
 # Create a window
 window = pygame.display.set_mode((800, 600))
 
 # Create a button
-button = pgpyui.Button((100, 100), (200, 50), "Click me!", lambda: print("Button clicked!"))
+button = button.Button((100, 100), (200, 50), "Click me!", lambda: print("Button clicked!"))
 
 # Create a text area
-text_area = pgpyui.TextArea((100, 200), (200, 200), 20, 100)
+text_area = textarea.TextArea((100, 200), (200, 200), 20, 100)
 
 # Game loop
 running = True
 while running:
 # Handle events
     for event in pygame.event.get():
         if event.type == pygame.QUIT:
@@ -90,7 +89,11 @@
 * `max_symbols`: The maximum number of symbols that can be entered.
 * `is_enter`: Whether or not the enter key should be allowed.
 * `font`: The name of the font to use (optional).
 
 ## License
 
 MIT
+
+## Author mail
+
+mixail.vilyukov@icloud.com
```

### Comparing `pgpyui-0.0.1/setup.py` & `pgpyui-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 
 setup(
   name='pgpyui',
-  version='0.0.1',
+  version='0.0.2',
   author='Memdved',
   author_email='mixail.vilyukov@icloud.com',
   description='The package is an add-on for Pygame to create a user interface on the screen.',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://pypi.org/project/pgpyui/',
   packages=find_packages(),
```


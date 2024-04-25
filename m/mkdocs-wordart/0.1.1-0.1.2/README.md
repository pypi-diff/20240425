# Comparing `tmp/mkdocs_wordart-0.1.1.tar.gz` & `tmp/mkdocs_wordart-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_wordart-0.1.1.tar", last modified: Wed Apr 24 14:15:37 2024, max compression
+gzip compressed data, was "mkdocs_wordart-0.1.2.tar", last modified: Thu Apr 25 15:31:13 2024, max compression
```

## Comparing `mkdocs_wordart-0.1.1.tar` & `mkdocs_wordart-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:15:37.080925 mkdocs_wordart-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 14:15:27.000000 mkdocs_wordart-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-24 14:15:27.000000 mkdocs_wordart-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-24 14:15:37.080925 mkdocs_wordart-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-24 14:15:27.000000 mkdocs_wordart-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-24 14:15:27.000000 mkdocs_wordart-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:15:37.080925 mkdocs_wordart-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:15:37.076925 mkdocs_wordart-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:15:37.076925 mkdocs_wordart-0.1.1/src/mkdocs_wordart/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:15:37.076925 mkdocs_wordart-0.1.1/src/mkdocs_wordart/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   243780 2024-04-24 14:15:27.000000 mkdocs_wordart-0.1.1/src/mkdocs_wordart/assets/wordart.css
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-24 14:15:27.000000 mkdocs_wordart-0.1.1/src/mkdocs_wordart/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:15:37.080925 mkdocs_wordart-0.1.1/src/mkdocs_wordart/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-24 14:15:27.000000 mkdocs_wordart-0.1.1/src/mkdocs_wordart/templates/wordart.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:15:37.080925 mkdocs_wordart-0.1.1/src/mkdocs_wordart.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-24 14:15:37.000000 mkdocs_wordart-0.1.1/src/mkdocs_wordart.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-24 14:15:37.000000 mkdocs_wordart-0.1.1/src/mkdocs_wordart.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:15:37.000000 mkdocs_wordart-0.1.1/src/mkdocs_wordart.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-24 14:15:37.000000 mkdocs_wordart-0.1.1/src/mkdocs_wordart.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 14:15:37.000000 mkdocs_wordart-0.1.1/src/mkdocs_wordart.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 14:15:37.000000 mkdocs_wordart-0.1.1/src/mkdocs_wordart.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:31:13.534265 mkdocs_wordart-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-25 15:31:04.000000 mkdocs_wordart-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-25 15:31:04.000000 mkdocs_wordart-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-25 15:31:13.534265 mkdocs_wordart-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-25 15:31:04.000000 mkdocs_wordart-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-25 15:31:04.000000 mkdocs_wordart-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:31:13.534265 mkdocs_wordart-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:31:13.530265 mkdocs_wordart-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:31:13.530265 mkdocs_wordart-0.1.2/src/mkdocs_wordart/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:31:13.534265 mkdocs_wordart-0.1.2/src/mkdocs_wordart/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   215800 2024-04-25 15:31:04.000000 mkdocs_wordart-0.1.2/src/mkdocs_wordart/assets/wordart.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-25 15:31:04.000000 mkdocs_wordart-0.1.2/src/mkdocs_wordart/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:31:13.534265 mkdocs_wordart-0.1.2/src/mkdocs_wordart/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-25 15:31:04.000000 mkdocs_wordart-0.1.2/src/mkdocs_wordart/templates/wordart.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:31:13.534265 mkdocs_wordart-0.1.2/src/mkdocs_wordart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-25 15:31:13.000000 mkdocs_wordart-0.1.2/src/mkdocs_wordart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-25 15:31:13.000000 mkdocs_wordart-0.1.2/src/mkdocs_wordart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:31:13.000000 mkdocs_wordart-0.1.2/src/mkdocs_wordart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-25 15:31:13.000000 mkdocs_wordart-0.1.2/src/mkdocs_wordart.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 15:31:13.000000 mkdocs_wordart-0.1.2/src/mkdocs_wordart.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 15:31:13.000000 mkdocs_wordart-0.1.2/src/mkdocs_wordart.egg-info/top_level.txt
```

### Comparing `mkdocs_wordart-0.1.1/LICENSE` & `mkdocs_wordart-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_wordart-0.1.1/PKG-INFO` & `mkdocs_wordart-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-wordart
-Version: 0.1.1
+Version: 0.1.2
 Summary: A MkDocs plugin that makes wordart available again.
 Author-email: Useless DevLab <useless.devlab@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Useless DevLab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mkdocs_wordart-0.1.1/pyproject.toml` & `mkdocs_wordart-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mkdocs-wordart"
-version = "0.1.1"
+version = "0.1.2"
 description = "A MkDocs plugin that makes wordart available again."
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["mkdocs", "documentation", "wordart"]
 authors = [
   {name = "Useless DevLab", email = "useless.devlab@gmail.com"}
 ]
```

### Comparing `mkdocs_wordart-0.1.1/src/mkdocs_wordart/assets/wordart.css` & `mkdocs_wordart-0.1.2/src/mkdocs_wordart/assets/wordart.css`

 * *Files 18% similar despite different names*

```diff
@@ -1,801 +1,7 @@
-/* -------------------------------------
- ___ ___ ___ ___ _____
-| _ \ __/ __| __|_   _|
-|   / _|\__ \ _|  | |
-|_|_\___|___/___| |_|
-
--------------------------------------- */
-/* * {
-    border: 0;
-    padding: 0;
-    margin: 0;
-    box-sizing: border-box;
-    -moz-box-sizing: border-box;
-    -webkit-box-sizing: border-box;
-  } */
-  /* html,
-  body {
-    height: 100%;
-    font-family: MicrosoftSansSerif;
-    -webkit-font-smoothing: none;
-    -moz-osx-font-smoothing: none;
-    background: #3dff32;
-    background: url(data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiA/Pgo8c3ZnIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgd2lkdGg9IjEwMCUiIGhlaWdodD0iMTAwJSIgdmlld0JveD0iMCAwIDEgMSIgcHJlc2VydmVBc3BlY3RSYXRpbz0ibm9uZSI+CiAgPGxpbmVhckdyYWRpZW50IGlkPSJncmFkLXVjZ2ctZ2VuZXJhdGVkIiBncmFkaWVudFVuaXRzPSJ1c2VyU3BhY2VPblVzZSIgeDE9IjAlIiB5MT0iMCUiIHgyPSIxMDAlIiB5Mj0iMTAwJSI+CiAgICA8c3RvcCBvZmZzZXQ9IjAlIiBzdG9wLWNvbG9yPSIjM2RmZjMyIiBzdG9wLW9wYWNpdHk9IjEiLz4KICAgIDxzdG9wIG9mZnNldD0iNTAlIiBzdG9wLWNvbG9yPSIjMzBmNGZmIiBzdG9wLW9wYWNpdHk9IjEiLz4KICAgIDxzdG9wIG9mZnNldD0iMTAwJSIgc3RvcC1jb2xvcj0iI2ZmMDBmYSIgc3RvcC1vcGFjaXR5PSIxIi8+CiAgPC9saW5lYXJHcmFkaWVudD4KICA8cmVjdCB4PSIwIiB5PSIwIiB3aWR0aD0iMSIgaGVpZ2h0PSIxIiBmaWxsPSJ1cmwoI2dyYWQtdWNnZy1nZW5lcmF0ZWQpIiAvPgo8L3N2Zz4=);
-    background: -moz-linear-gradient(-45deg, #3dff32 0%, #30f4ff 50%, #ff00fa 100%);
-    background: -webkit-gradient(linear, left top, right bottom, color-stop(0%, #3dff32), color-stop(50%, #30f4ff), color-stop(100%, #ff00fa));
-    background: -webkit-linear-gradient(-45deg, #3dff32 0%, #30f4ff 50%, #ff00fa 100%);
-    background: -o-linear-gradient(-45deg, #3dff32 0%, #30f4ff 50%, #ff00fa 100%);
-    background: -ms-linear-gradient(-45deg, #3dff32 0%, #30f4ff 50%, #ff00fa 100%);
-    background: linear-gradient(135deg, #3dff32 0%, #30f4ff 50%, #ff00fa 100%);
-    filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#3dff32', endColorstr='#ff00fa', GradientType=1);
-    background-attachment: fixed;
-  } */
-  /* -------------------------------------
-   ___ __  __   _   ___ ___ ___
-  |_ _|  \/  | /_\ / __| __/ __|
-   | || |\/| |/ _ \ (_ | _|\__ \
-  |___|_|  |_/_/ \_\___|___|___/
-  
-  -------------------------------------- */
-  /* WINDOWS BG TILES */
-  /* GRADIENTS */
-  /* -------------------------------------
-   ___ ___  _  _ _____ ___
-  | __/ _ \| \| |_   _/ __|
-  | _| (_) | .` | | | \__ \
-  |_| \___/|_|\_| |_| |___/
-  
-  -------------------------------------- */
-  @font-face {
-    font-family: 'MicrosoftSansSerif';
-    src: url('fonts/MicrosoftSansSerif.eot?') format('eot'), url('fonts/MicrosoftSansSerif.woff') format('woff'), url('fonts/MicrosoftSansSerif.ttf') format('truetype'), url('fonts/MicrosoftSansSerif.svg#MicrosoftSansSerif') format('svg');
-  }
-  /* -------------------------------------
-   __  __ _____  _____ _  _ ___
-  |  \/  |_ _\ \/ /_ _| \| / __|
-  | |\/| || | >  < | || .` \__ \
-  |_|  |_|___/_/\_\___|_|\_|___/
-  
-  -------------------------------------- */
-  .noselect {
-    -webkit-touch-callout: none;
-    -webkit-user-select: none;
-    -khtml-user-select: none;
-    -moz-user-select: none;
-    -ms-user-select: none;
-    user-select: none;
-  }
-  .textBg {
-    background-clip: text;
-    -webkit-background-clip: text;
-    -webkit-text-fill-color: transparent;
-  }
-  .stacked {
-    transform: scaleY(0.75);
-    -webkit-transform: scaleY(0.75);
-    -moz-transform: scaleY(0.75);
-    -o-transform: scaleY(0.75);
-    -ms-transform: scaleY(0.75);
-    transform-origin: 0 50% 0;
-    display: inline-block;
-    text-align: center;
-    vertical-align: top;
-    line-height: 0.8em;
-    width: 1em;
-    word-wrap: break-word;
-    letter-spacing: 0.27em;
-  }
-  .stacked .text {
-    display: block;
-  }
-  .stacked .text:before {
-    display: block;
-    text-align: center;
-    color: transparent;
-    width: 100%;
-    word-wrap: break-word;
-    letter-spacing: 0.27em;
-  }
-  /* -------------------------------------
-  __      _____ _  _ ___ ___
-  \ \    / /_ _| \| / _ \ __|
-   \ \/\/ / | || .` \_, /__ \
-    \_/\_/ |___|_|\_|/_/|___/
-  
-  -------------------------------------- */
-  .wordart-icon {
-    -webkit-touch-callout: none;
-    -webkit-user-select: none;
-    -khtml-user-select: none;
-    -moz-user-select: none;
-    -ms-user-select: none;
-    user-select: none;
-    display: inline-block;
-    transform: rotateZ(20deg);
-    -webkit-transform: rotateZ(20deg);
-    -moz-transform: rotateZ(20deg);
-    -o-transform: rotateZ(20deg);
-    -ms-transform: rotateZ(20deg);
-    -webkit-font-smoothing: antialiased;
-    -moz-osx-font-smoothing: grayscale;
-  }
-  .wordart-icon .inner {
-    font-family: Times, 'Times New Roman', serif;
-    font-weight: bold;
-    transform-origin: 90% 90% 0;
-    background: #2a4afa;
-    background: url(data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiA/Pgo8c3ZnIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgd2lkdGg9IjEwMCUiIGhlaWdodD0iMTAwJSIgdmlld0JveD0iMCAwIDEgMSIgcHJlc2VydmVBc3BlY3RSYXRpbz0ibm9uZSI+CiAgPGxpbmVhckdyYWRpZW50IGlkPSJncmFkLXVjZ2ctZ2VuZXJhdGVkIiBncmFkaWVudFVuaXRzPSJ1c2VyU3BhY2VPblVzZSIgeDE9IjAlIiB5MT0iMCUiIHgyPSIwJSIgeTI9IjEwMCUiPgogICAgPHN0b3Agb2Zmc2V0PSIwJSIgc3RvcC1jb2xvcj0iIzJhNGFmYSIgc3RvcC1vcGFjaXR5PSIxIi8+CiAgICA8c3RvcCBvZmZzZXQ9IjEwMCUiIHN0b3AtY29sb3I9IiMzNTNmOTIiIHN0b3Atb3BhY2l0eT0iMSIvPgogIDwvbGluZWFyR3JhZGllbnQ+CiAgPHJlY3QgeD0iMCIgeT0iMCIgd2lkdGg9IjEiIGhlaWdodD0iMSIgZmlsbD0idXJsKCNncmFkLXVjZ2ctZ2VuZXJhdGVkKSIgLz4KPC9zdmc+);
-    background: -moz-linear-gradient(top, #2a4afa 0%, #353f92 100%);
-    background: -webkit-gradient(linear, left top, left bottom, color-stop(0%, #2a4afa), color-stop(100%, #353f92));
-    background: -webkit-linear-gradient(top, #2a4afa 0%, #353f92 100%);
-    background: -o-linear-gradient(top, #2a4afa 0%, #353f92 100%);
-    background: -ms-linear-gradient(top, #2a4afa 0%, #353f92 100%);
-    background: linear-gradient(to bottom, #2a4afa 0%, #353f92 100%);
-    filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#2a4afa', endColorstr='#353f92', GradientType=0);
-    background-clip: text;
-    -webkit-background-clip: text;
-    -webkit-text-fill-color: transparent;
-  }
-  .wordart-icon .inner:before {
-    position: absolute;
-    z-index: -1;
-    content: 'A';
-    text-shadow: 0.01em 0em 0 #949494, 0em -0.01em 0 #949494, 0.02em -0.01em 0 #949494, 0.01em -0.02em 0 #949494, 0.03em -0.02em 0 #949494, 0.02em -0.03em 0 #949494, 0.04em -0.03em 0 #949494, 0.03em -0.04em 0 #949494, 0.05em -0.04em 0 #949494, 0.04em -0.05em 0 #949494, 0.06em -0.05em 0 #949494, 0.05em -0.06em 0 #949494, 0.07em -0.06em 0 #949494, 0.06em -0.07em 0 #949494, 0.08em -0.07em 0 #949494, 0.07em -0.08em 0 #949494, 0.09em -0.08em 0 #949494, 0.08em -0.09em 0 #949494, 0.1em -0.09em 0 #949494, 0.09em -0.1em 0 #949494, 0.11em -0.1em 0 #949494, 0.1em -0.11em 0 #949494, 0.12em -0.11em 0 #949494, 0.11em -0.12em 0 #949494, 0.13em -0.12em 0 #949494, 0.12em -0.13em 0 #949494, 0.14em -0.13em 0 #949494, 0.13em -0.14em 0 #949494, 0.15em -0.14em 0 #949494, 0.14em -0.15em 0 #949494, 0.16em -0.15em 0 #393939, 0.15em -0.16em 0 #393939, 0.17em -0.16em 0 #393939, 0.16em -0.17em 0 #393939;
-  }
-  .window {
-    border-top: 2px solid #d7d7d7;
-    border-right: 2px solid #000;
-    border-bottom: 2px solid #000;
-    border-left: 2px solid #d7d7d7;
-    background: #b3b3b3;
-    padding: 4px;
-    font-size: 14px;
-    position: absolute;
-  }
-  .window:before {
-    position: absolute;
-    display: block;
-    content: '';
-    border-top: 2px solid #fff;
-    border-right: 2px solid #6d6d6d;
-    border-bottom: 2px solid #6d6d6d;
-    border-left: 2px solid #fff;
-    top: 0;
-    left: 0;
-    right: 0;
-    bottom: 0;
-  }
-  .window > .title {
-    background: #00006f;
-    background: url(data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiA/Pgo8c3ZnIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgd2lkdGg9IjEwMCUiIGhlaWdodD0iMTAwJSIgdmlld0JveD0iMCAwIDEgMSIgcHJlc2VydmVBc3BlY3RSYXRpbz0ibm9uZSI+CiAgPGxpbmVhckdyYWRpZW50IGlkPSJncmFkLXVjZ2ctZ2VuZXJhdGVkIiBncmFkaWVudFVuaXRzPSJ1c2VyU3BhY2VPblVzZSIgeDE9IjAlIiB5MT0iMCUiIHgyPSIxMDAlIiB5Mj0iMCUiPgogICAgPHN0b3Agb2Zmc2V0PSIwJSIgc3RvcC1jb2xvcj0iIzAwMDA2ZiIgc3RvcC1vcGFjaXR5PSIxIi8+CiAgICA8c3RvcCBvZmZzZXQ9IjEwMCUiIHN0b3AtY29sb3I9IiMwYTZjYzgiIHN0b3Atb3BhY2l0eT0iMSIvPgogIDwvbGluZWFyR3JhZGllbnQ+CiAgPHJlY3QgeD0iMCIgeT0iMCIgd2lkdGg9IjEiIGhlaWdodD0iMSIgZmlsbD0idXJsKCNncmFkLXVjZ2ctZ2VuZXJhdGVkKSIgLz4KPC9zdmc+);
-    background: -moz-linear-gradient(left, #00006f 0%, #0a6cc8 100%);
-    background: -webkit-gradient(linear, left top, right top, color-stop(0%, #00006f), color-stop(100%, #0a6cc8));
-    background: -webkit-linear-gradient(left, #00006f 0%, #0a6cc8 100%);
-    background: -o-linear-gradient(left, #00006f 0%, #0a6cc8 100%);
-    background: -ms-linear-gradient(left, #00006f 0%, #0a6cc8 100%);
-    background: linear-gradient(to right, #00006f 0%, #0a6cc8 100%);
-    filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#00006f', endColorstr='#0a6cc8', GradientType=1);
-    width: 100%;
-    height: 27px;
-    color: #fff;
-    text-indent: 4px;
-    padding-top: 4px;
-    font-size: 15px;
-    font-weight: bold;
-  }
-  .window .hk {
-    text-decoration: underline;
-  }
-  .window .button-box {
-    width: 100%;
-    padding: 24px 11px 0 11px;
-  }
-  .window .button-box.right {
-    text-align: right;
-  }
-  .window .button-box button {
-    margin-left: 10px;
-  }
-  .window button {
-    border-top: 2px solid #d7d7d7;
-    border-right: 2px solid #000;
-    border-bottom: 2px solid #000;
-    border-left: 2px solid #d7d7d7;
-    position: relative;
-    text-align: center;
-    font-family: MicrosoftSansSerif;
-    font-size: 14px;
-  }
-  .window button:before {
-    position: absolute;
-    display: block;
-    content: '';
-    border-top: 2px solid #fff;
-    border-right: 2px solid #6d6d6d;
-    border-bottom: 2px solid #6d6d6d;
-    border-left: 2px solid #fff;
-    top: 0;
-    left: 0;
-    right: 0;
-    bottom: 0;
-  }
-  .window button.ok,
-  .window button.cancel {
-    width: 114px;
-    height: 34px;
-  }
-  .window button:focus {
-    outline: 0;
-  }
-  .window button:active {
-    position: relative;
-    border-top: 2px solid #6d6d6d;
-    border-right: 2px solid #fff;
-    border-bottom: 2px solid #fff;
-    border-left: 2px solid #6d6d6d;
-    padding: 2px;
-  }
-  .window button:active:before {
-    position: absolute;
-    display: block;
-    content: '';
-    border-top: 2px solid #000;
-    border-right: 2px solid #d7d7d7;
-    border-bottom: 2px solid #d7d7d7;
-    border-left: 2px solid #000;
-    top: 0;
-    left: 0;
-    right: 0;
-    bottom: 0;
-  }
-  .dialog {
-    border-top: 2px solid #d7d7d7;
-    border-right: 2px solid #000;
-    border-bottom: 2px solid #000;
-    border-left: 2px solid #d7d7d7;
-    background: #b3b3b3;
-    padding: 4px;
-    font-size: 14px;
-    position: absolute;
-    width: 630px;
-    height: 540px;
-    display: none;
-    top: 40px;
-    left: 50%;
-    margin: 0 0 100px -315px;
-    z-index: 100;
-  }
-  .dialog:before {
-    position: absolute;
-    display: block;
-    content: '';
-    border-top: 2px solid #fff;
-    border-right: 2px solid #6d6d6d;
-    border-bottom: 2px solid #6d6d6d;
-    border-left: 2px solid #fff;
-    top: 0;
-    left: 0;
-    right: 0;
-    bottom: 0;
-  }
-  .dialog > .title {
-    background: #00006f;
-    background: url(data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiA/Pgo8c3ZnIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgd2lkdGg9IjEwMCUiIGhlaWdodD0iMTAwJSIgdmlld0JveD0iMCAwIDEgMSIgcHJlc2VydmVBc3BlY3RSYXRpbz0ibm9uZSI+CiAgPGxpbmVhckdyYWRpZW50IGlkPSJncmFkLXVjZ2ctZ2VuZXJhdGVkIiBncmFkaWVudFVuaXRzPSJ1c2VyU3BhY2VPblVzZSIgeDE9IjAlIiB5MT0iMCUiIHgyPSIxMDAlIiB5Mj0iMCUiPgogICAgPHN0b3Agb2Zmc2V0PSIwJSIgc3RvcC1jb2xvcj0iIzAwMDA2ZiIgc3RvcC1vcGFjaXR5PSIxIi8+CiAgICA8c3RvcCBvZmZzZXQ9IjEwMCUiIHN0b3AtY29sb3I9IiMwYTZjYzgiIHN0b3Atb3BhY2l0eT0iMSIvPgogIDwvbGluZWFyR3JhZGllbnQ+CiAgPHJlY3QgeD0iMCIgeT0iMCIgd2lkdGg9IjEiIGhlaWdodD0iMSIgZmlsbD0idXJsKCNncmFkLXVjZ2ctZ2VuZXJhdGVkKSIgLz4KPC9zdmc+);
-    background: -moz-linear-gradient(left, #00006f 0%, #0a6cc8 100%);
-    background: -webkit-gradient(linear, left top, right top, color-stop(0%, #00006f), color-stop(100%, #0a6cc8));
-    background: -webkit-linear-gradient(left, #00006f 0%, #0a6cc8 100%);
-    background: -o-linear-gradient(left, #00006f 0%, #0a6cc8 100%);
-    background: -ms-linear-gradient(left, #00006f 0%, #0a6cc8 100%);
-    background: linear-gradient(to right, #00006f 0%, #0a6cc8 100%);
-    filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#00006f', endColorstr='#0a6cc8', GradientType=1);
-    width: 100%;
-    height: 27px;
-    color: #fff;
-    text-indent: 4px;
-    padding-top: 4px;
-    font-size: 15px;
-    font-weight: bold;
-  }
-  .dialog .hk {
-    text-decoration: underline;
-  }
-  .dialog .button-box {
-    width: 100%;
-    padding: 24px 11px 0 11px;
-  }
-  .dialog .button-box.right {
-    text-align: right;
-  }
-  .dialog .button-box button {
-    margin-left: 10px;
-  }
-  .dialog button {
-    border-top: 2px solid #d7d7d7;
-    border-right: 2px solid #000;
-    border-bottom: 2px solid #000;
-    border-left: 2px solid #d7d7d7;
-    position: relative;
-    text-align: center;
-    font-family: MicrosoftSansSerif;
-    font-size: 14px;
-  }
-  .dialog button:before {
-    position: absolute;
-    display: block;
-    content: '';
-    border-top: 2px solid #fff;
-    border-right: 2px solid #6d6d6d;
-    border-bottom: 2px solid #6d6d6d;
-    border-left: 2px solid #fff;
-    top: 0;
-    left: 0;
-    right: 0;
-    bottom: 0;
-  }
-  .dialog button.ok,
-  .dialog button.cancel {
-    width: 114px;
-    height: 34px;
-  }
-  .dialog button:focus {
-    outline: 0;
-  }
-  .dialog button:active {
-    position: relative;
-    border-top: 2px solid #6d6d6d;
-    border-right: 2px solid #fff;
-    border-bottom: 2px solid #fff;
-    border-left: 2px solid #6d6d6d;
-    padding: 2px;
-  }
-  .dialog button:active:before {
-    position: absolute;
-    display: block;
-    content: '';
-    border-top: 2px solid #000;
-    border-right: 2px solid #d7d7d7;
-    border-bottom: 2px solid #d7d7d7;
-    border-left: 2px solid #000;
-    top: 0;
-    left: 0;
-    right: 0;
-    bottom: 0;
-  }
-  .alert {
-    border-top: 2px solid #d7d7d7;
-    border-right: 2px solid #000;
-    border-bottom: 2px solid #000;
-    border-left: 2px solid #d7d7d7;
-    background: #b3b3b3;
-    padding: 4px;
-    font-size: 14px;
-    position: absolute;
-    width: 500px;
-    height: 180px;
-    top: 50%;
-    left: 50%;
-    margin: -90px 0 0 -250px;
-    z-index: 200;
-  }
-  .alert:before {
-    position: absolute;
-    display: block;
-    content: '';
-    border-top: 2px solid #fff;
-    border-right: 2px solid #6d6d6d;
-    border-bottom: 2px solid #6d6d6d;
-    border-left: 2px solid #fff;
-    top: 0;
-    left: 0;
-    right: 0;
-    bottom: 0;
-  }
-  .alert > .title {
-    background: #00006f;
-    background: url(data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiA/Pgo8c3ZnIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgd2lkdGg9IjEwMCUiIGhlaWdodD0iMTAwJSIgdmlld0JveD0iMCAwIDEgMSIgcHJlc2VydmVBc3BlY3RSYXRpbz0ibm9uZSI+CiAgPGxpbmVhckdyYWRpZW50IGlkPSJncmFkLXVjZ2ctZ2VuZXJhdGVkIiBncmFkaWVudFVuaXRzPSJ1c2VyU3BhY2VPblVzZSIgeDE9IjAlIiB5MT0iMCUiIHgyPSIxMDAlIiB5Mj0iMCUiPgogICAgPHN0b3Agb2Zmc2V0PSIwJSIgc3RvcC1jb2xvcj0iIzAwMDA2ZiIgc3RvcC1vcGFjaXR5PSIxIi8+CiAgICA8c3RvcCBvZmZzZXQ9IjEwMCUiIHN0b3AtY29sb3I9IiMwYTZjYzgiIHN0b3Atb3BhY2l0eT0iMSIvPgogIDwvbGluZWFyR3JhZGllbnQ+CiAgPHJlY3QgeD0iMCIgeT0iMCIgd2lkdGg9IjEiIGhlaWdodD0iMSIgZmlsbD0idXJsKCNncmFkLXVjZ2ctZ2VuZXJhdGVkKSIgLz4KPC9zdmc+);
-    background: -moz-linear-gradient(left, #00006f 0%, #0a6cc8 100%);
-    background: -webkit-gradient(linear, left top, right top, color-stop(0%, #00006f), color-stop(100%, #0a6cc8));
-    background: -webkit-linear-gradient(left, #00006f 0%, #0a6cc8 100%);
-    background: -o-linear-gradient(left, #00006f 0%, #0a6cc8 100%);
-    background: -ms-linear-gradient(left, #00006f 0%, #0a6cc8 100%);
-    background: linear-gradient(to right, #00006f 0%, #0a6cc8 100%);
-    filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#00006f', endColorstr='#0a6cc8', GradientType=1);
-    width: 100%;
-    height: 27px;
-    color: #fff;
-    text-indent: 4px;
-    padding-top: 4px;
-    font-size: 15px;
-    font-weight: bold;
-  }
-  .alert .hk {
-    text-decoration: underline;
-  }
-  .alert .button-box {
-    width: 100%;
-    padding: 24px 11px 0 11px;
-  }
-  .alert .button-box.right {
-    text-align: right;
-  }
-  .alert .button-box button {
-    margin-left: 10px;
-  }
-  .alert button {
-    border-top: 2px solid #d7d7d7;
-    border-right: 2px solid #000;
-    border-bottom: 2px solid #000;
-    border-left: 2px solid #d7d7d7;
-    position: relative;
-    text-align: center;
-    font-family: MicrosoftSansSerif;
-    font-size: 14px;
-  }
-  .alert button:before {
-    position: absolute;
-    display: block;
-    content: '';
-    border-top: 2px solid #fff;
-    border-right: 2px solid #6d6d6d;
-    border-bottom: 2px solid #6d6d6d;
-    border-left: 2px solid #fff;
-    top: 0;
-    left: 0;
-    right: 0;
-    bottom: 0;
-  }
-  .alert button.ok,
-  .alert button.cancel {
-    width: 114px;
-    height: 34px;
-  }
-  .alert button:focus {
-    outline: 0;
-  }
-  .alert button:active {
-    position: relative;
-    border-top: 2px solid #6d6d6d;
-    border-right: 2px solid #fff;
-    border-bottom: 2px solid #fff;
-    border-left: 2px solid #6d6d6d;
-    padding: 2px;
-  }
-  .alert button:active:before {
-    position: absolute;
-    display: block;
-    content: '';
-    border-top: 2px solid #000;
-    border-right: 2px solid #d7d7d7;
-    border-bottom: 2px solid #d7d7d7;
-    border-left: 2px solid #000;
-    top: 0;
-    left: 0;
-    right: 0;
-    bottom: 0;
-  }
-  .alert p {
-    margin: 20px 0 0 20px;
-    display: inline-block;
-    vertical-align: top;
-  }
-  .alert .icon {
-    width: 50px;
-    height: 50px;
-    font-size: 50px;
-    margin-right: 15px;
-  }
-  .alert .icon.wordart {
-    -webkit-touch-callout: none;
-    -webkit-user-select: none;
-    -khtml-user-select: none;
-    -moz-user-select: none;
-    -ms-user-select: none;
-    user-select: none;
-    display: inline-block;
-    transform: rotateZ(20deg);
-    -webkit-transform: rotateZ(20deg);
-    -moz-transform: rotateZ(20deg);
-    -o-transform: rotateZ(20deg);
-    -ms-transform: rotateZ(20deg);
-    -webkit-font-smoothing: antialiased;
-    -moz-osx-font-smoothing: grayscale;
-  }
-  .alert .icon.wordart .inner {
-    font-family: Times, 'Times New Roman', serif;
-    font-weight: bold;
-    transform-origin: 90% 90% 0;
-    background: #2a4afa;
-    background: url(data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiA/Pgo8c3ZnIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgd2lkdGg9IjEwMCUiIGhlaWdodD0iMTAwJSIgdmlld0JveD0iMCAwIDEgMSIgcHJlc2VydmVBc3BlY3RSYXRpbz0ibm9uZSI+CiAgPGxpbmVhckdyYWRpZW50IGlkPSJncmFkLXVjZ2ctZ2VuZXJhdGVkIiBncmFkaWVudFVuaXRzPSJ1c2VyU3BhY2VPblVzZSIgeDE9IjAlIiB5MT0iMCUiIHgyPSIwJSIgeTI9IjEwMCUiPgogICAgPHN0b3Agb2Zmc2V0PSIwJSIgc3RvcC1jb2xvcj0iIzJhNGFmYSIgc3RvcC1vcGFjaXR5PSIxIi8+CiAgICA8c3RvcCBvZmZzZXQ9IjEwMCUiIHN0b3AtY29sb3I9IiMzNTNmOTIiIHN0b3Atb3BhY2l0eT0iMSIvPgogIDwvbGluZWFyR3JhZGllbnQ+CiAgPHJlY3QgeD0iMCIgeT0iMCIgd2lkdGg9IjEiIGhlaWdodD0iMSIgZmlsbD0idXJsKCNncmFkLXVjZ2ctZ2VuZXJhdGVkKSIgLz4KPC9zdmc+);
-    background: -moz-linear-gradient(top, #2a4afa 0%, #353f92 100%);
-    background: -webkit-gradient(linear, left top, left bottom, color-stop(0%, #2a4afa), color-stop(100%, #353f92));
-    background: -webkit-linear-gradient(top, #2a4afa 0%, #353f92 100%);
-    background: -o-linear-gradient(top, #2a4afa 0%, #353f92 100%);
-    background: -ms-linear-gradient(top, #2a4afa 0%, #353f92 100%);
-    background: linear-gradient(to bottom, #2a4afa 0%, #353f92 100%);
-    filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#2a4afa', endColorstr='#353f92', GradientType=0);
-    background-clip: text;
-    -webkit-background-clip: text;
-    -webkit-text-fill-color: transparent;
-  }
-  .alert .icon.wordart .inner:before {
-    position: absolute;
-    z-index: -1;
-    content: 'A';
-    text-shadow: 0.01em 0em 0 #949494, 0em -0.01em 0 #949494, 0.02em -0.01em 0 #949494, 0.01em -0.02em 0 #949494, 0.03em -0.02em 0 #949494, 0.02em -0.03em 0 #949494, 0.04em -0.03em 0 #949494, 0.03em -0.04em 0 #949494, 0.05em -0.04em 0 #949494, 0.04em -0.05em 0 #949494, 0.06em -0.05em 0 #949494, 0.05em -0.06em 0 #949494, 0.07em -0.06em 0 #949494, 0.06em -0.07em 0 #949494, 0.08em -0.07em 0 #949494, 0.07em -0.08em 0 #949494, 0.09em -0.08em 0 #949494, 0.08em -0.09em 0 #949494, 0.1em -0.09em 0 #949494, 0.09em -0.1em 0 #949494, 0.11em -0.1em 0 #949494, 0.1em -0.11em 0 #949494, 0.12em -0.11em 0 #949494, 0.11em -0.12em 0 #949494, 0.13em -0.12em 0 #949494, 0.12em -0.13em 0 #949494, 0.14em -0.13em 0 #949494, 0.13em -0.14em 0 #949494, 0.15em -0.14em 0 #949494, 0.14em -0.15em 0 #949494, 0.16em -0.15em 0 #393939, 0.15em -0.16em 0 #393939, 0.17em -0.16em 0 #393939, 0.16em -0.17em 0 #393939;
-  }
-  .bevel {
-    border-top: 2px solid #d7d7d7;
-    border-right: 2px solid #000;
-    border-bottom: 2px solid #000;
-    border-left: 2px solid #d7d7d7;
-  }
-  .bevel:before {
-    position: absolute;
-    display: block;
-    content: '';
-    border-top: 2px solid #fff;
-    border-right: 2px solid #6d6d6d;
-    border-bottom: 2px solid #6d6d6d;
-    border-left: 2px solid #fff;
-    top: 0;
-    left: 0;
-    right: 0;
-    bottom: 0;
-  }
-  .inset {
-    position: relative;
-    border-top: 2px solid #6d6d6d;
-    border-right: 2px solid #fff;
-    border-bottom: 2px solid #fff;
-    border-left: 2px solid #6d6d6d;
-    padding: 2px;
-  }
-  .inset:before {
-    position: absolute;
-    display: block;
-    content: '';
-    border-top: 2px solid #000;
-    border-right: 2px solid #d7d7d7;
-    border-bottom: 2px solid #d7d7d7;
-    border-left: 2px solid #000;
-    top: 0;
-    left: 0;
-    right: 0;
-    bottom: 0;
-  }
-  /* -------------------------------------
-    ___   _   _    _    ___ _____   __
-   / __| /_\ | |  | |  | __| _ \ \ / /
-  | (_ |/ _ \| |__| |__| _||   /\ V /
-   \___/_/ \_\____|____|___|_|_\ |_|
-  
-   -------------------------------------- */
-  .gallery {
-    z-index: 101;
-  }
-  .gallery > p {
-    margin: 22px 8px 10px 8px;
-  }
-  .gallery-thumbs {
-    margin-left: 11px;
-  }
-  .gallery-thumbs > li {
-    position: relative;
-    border-top: 2px solid #6d6d6d;
-    border-right: 2px solid #fff;
-    border-bottom: 2px solid #fff;
-    border-left: 2px solid #6d6d6d;
-    display: inline-block;
-    width: 96px;
-    height: 74px;
-    background: #fff;
-    padding: 2px;
-    text-align: center;
-    vertical-align: middle;
-    font-size: 22px;
-  }
-  .gallery-thumbs > li:before {
-    position: absolute;
-    display: block;
-    content: '';
-    border-top: 2px solid #000;
-    border-right: 2px solid #d7d7d7;
-    border-bottom: 2px solid #d7d7d7;
-    border-left: 2px solid #000;
-    top: 0;
-    left: 0;
-    right: 0;
-    bottom: 0;
-  }
-  .gallery-thumbs > li .wrapper {
-    position: relative;
-    top: 50%;
-    transform: translateY(-50%);
-    -webkit-transform: translateY(-50%);
-    -moz-transform: translateY(-50%);
-    -o-transform: translateY(-50%);
-    -ms-transform: translateY(-50%);
-  }
-  .gallery-thumbs > li.selected {
-    border: 2px solid #000;
-  }
-  .gallery-thumbs > li.selected:before {
-    border-color: #000;
-  }
-  .gallery-thumbs .stack {
-    padding-left: 15px;
-    font-size: 1.1em;
-    text-align: left;
-  }
-  .gallery-thumbs .stack .highlight {
-    text-align: center;
-    position: absolute;
-    top: 3px;
-    right: 3px;
-    width: 40px;
-    height: 25px;
-    border-left: 1px solid #acacac;
-    border-bottom: 1px solid #acacac;
-    font-size: 2em;
-    padding-left: 3px;
-  }
-  .gallery-thumbs .stack > .wordart {
-    margin-top: -10px;
-  }
-  /* -------------------------------------
-   ___ ___ ___ _____ ___  ___
-  | __|   \_ _|_   _/ _ \| _ \
-  | _|| |) | |  | || (_) |   /
-  |___|___/___| |_| \___/|_|_\
-  
-   -------------------------------------- */
-  .editor {
-    z-index: 102;
-  }
-  .editor label {
-    display: block;
-  }
-  .form-element {
-    display: block;
-    padding: 0 11px;
-  }
-  .text-box {
-    padding-top: 22px;
-  }
-  .text-box label {
-    margin-bottom: 8px;
-  }
-  .text-box span.inset {
-    display: block;
-    padding: 2px;
-  }
-  .text-box textarea {
-    font-size: 36px;
-    padding-left: 5px;
-    line-height: 1.4em;
-    position: relative;
-    border: 0;
-    outline: none;
-    height: 370px;
-    resize: none;
-    width: 100%;
-  }
-  /* -------------------------------------
-   ___ ___ ___ ___ _______
-  | _ \ __/ __|_ _|_  / __|
-  |   / _|\__ \| | / /| _|
-  |_|_\___|___/___/___|___|
-  
-  -------------------------------------- */
-  .stage .container {
-    padding: 11px;
-    height: 430px;
-  }
-  .stage .container .button-row {
-    margin-bottom: 11px;
-  }
-  .stage .container .button-row button {
-    width: 34px;
-    height: 34px;
-  }
-  .stage .container .button-row .create {
-    font-size: 22px;
-  }
-  .stage .container .window {
-    position: relative;
-    border-top: 2px solid #6d6d6d;
-    border-right: 2px solid #fff;
-    border-bottom: 2px solid #fff;
-    border-left: 2px solid #6d6d6d;
-    padding: 2px;
-    background: #fff;
-    width: 100%;
-    height: 100%;
-  }
-  .stage .container .window:before {
-    position: absolute;
-    display: block;
-    content: '';
-    border-top: 2px solid #000;
-    border-right: 2px solid #d7d7d7;
-    border-bottom: 2px solid #d7d7d7;
-    border-left: 2px solid #000;
-    top: 0;
-    left: 0;
-    right: 0;
-    bottom: 0;
-  }
-  .stage .container .stage {
-    position: relative;
-    width: 100%;
-    height: 100%;
-    overflow: scroll;
-  }
-  .stage .container .resizable {
-    position: absolute;
-    top: 0;
-    left: 0;
-    transform-origin: 0 0 0;
-  }
-  .stage .container .resizable.active {
-    border: 1px dashed #444;
-    cursor: move;
-  }
-  .stage .container .resizable.active .h {
-    width: 8px;
-    height: 8px;
-    position: absolute;
-    background: #000;
-  }
-  .stage .container .resizable.active .h.n {
-    top: -1px;
-  }
-  .stage .container .resizable.active .h.s {
-    bottom: -1px;
-  }
-  .stage .container .resizable.active .h.e {
-    right: -1px;
-  }
-  .stage .container .resizable.active .h.w {
-    left: -1px;
-  }
-  .stage .container .resizable.active .h.yc {
-    top: 50%;
-    margin-top: -4px;
-    cursor: ew-resize;
-  }
-  .stage .container .resizable.active .h.xc {
-    left: 50%;
-    margin-left: -4px;
-    cursor: ns-resize;
-  }
-  .stage .container .resizable.active .h.n.e,
-  .stage .container .resizable.active .h.s.w {
-    cursor: nesw-resize;
-  }
-  .stage .container .resizable.active .h.n.w,
-  .stage .container .resizable.active .h.s.e {
-    cursor: nwse-resize;
-  }
-  .stage .container .wrapper {
-    position: relative;
-    top: 50%;
-    transform: translateY(-50%);
-    -webkit-transform: translateY(-50%);
-    -moz-transform: translateY(-50%);
-    -o-transform: translateY(-50%);
-    -ms-transform: translateY(-50%);
-  }
-  .stage .container .wordart {
-    font-size: 60px;
-  }
-  .stage .container .wordart:not(.basic-stack):not(.brown-stack):not(.green-stack):not(.texture-stack):not(.stack-3d) {
-    white-space: nowrap;
-  }
   /* -------------------------------------
   __      _____  ___ ___   _   ___ _____
   \ \    / / _ \| _ \   \ /_\ | _ \_   _|
    \ \/\/ / (_) |   / |) / _ \|   / | |
     \_/\_/ \___/|_|_\___/_/ \_\_|_\ |_|
   
   -------------------------------------- */
@@ -1586,61 +792,7 @@
     color: #000;
   }
   .inverted-arc .text {
     font-family: Times, 'Times New Roman', serif;
     font-weight: bold;
     color: #000;
   }
-  .test {
-    font-size: 100px;
-  }
-  /* -------------------------------------
-   ___  ___
-  | _ )/ __|
-  | _ \ (_ |
-  |___/\___|
-  
-   -------------------------------------- */
-  .background {
-    width: 100%;
-    height: 100%;
-    position: relative;
-    overflow: hidden;
-  }
-  .background .wordart {
-    position: absolute;
-    top: -500px;
-    left: -500px;
-  }
-  .background .rotateY {
-    -webkit-animation: rotateY 2s infinite linear;
-  }
-  .background .rotateX {
-    -webkit-animation: rotateX 2s infinite linear;
-  }
-  .background .rotateZ {
-    -webkit-animation: rotateZ 2s infinite linear;
-  }
-  @-webkit-keyframes rotateY {
-    from {
-      -webkit-transform: rotateY(0deg);
-    }
-    to {
-      -webkit-transform: rotateY(360deg);
-    }
-  }
-  @-webkit-keyframes rotateX {
-    from {
-      -webkit-transform: rotateX(0deg);
-    }
-    to {
-      -webkit-transform: rotateX(360deg);
-    }
-  }
-  @-webkit-keyframes rotateZ {
-    from {
-      -webkit-transform: rotateZ(0deg);
-    }
-    to {
-      -webkit-transform: rotateZ(360deg);
-    }
-  }
```

### Comparing `mkdocs_wordart-0.1.1/src/mkdocs_wordart/plugin.py` & `mkdocs_wordart-0.1.2/src/mkdocs_wordart/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_wordart-0.1.1/src/mkdocs_wordart.egg-info/PKG-INFO` & `mkdocs_wordart-0.1.2/src/mkdocs_wordart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-wordart
-Version: 0.1.1
+Version: 0.1.2
 Summary: A MkDocs plugin that makes wordart available again.
 Author-email: Useless DevLab <useless.devlab@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Useless DevLab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```


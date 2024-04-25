# Comparing `tmp/XGEE-0.3.6.tar.gz` & `tmp/XGEE-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XGEE-0.3.6.tar", last modified: Tue Mar 19 20:30:32 2024, max compression
+gzip compressed data, was "XGEE-0.3.7.tar", last modified: Tue Apr 23 20:45:15 2024, max compression
```

## Comparing `XGEE-0.3.6.tar` & `XGEE-0.3.7.tar`

### file list

```diff
@@ -1,1054 +1,1055 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.674615 XGEE-0.3.6/
--rw-rw-rw-   0 root         (0) root         (0)     1111 2024-03-19 20:30:24.000000 XGEE-0.3.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3174 2024-03-19 20:30:32.674615 XGEE-0.3.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2398 2024-03-19 20:30:24.000000 XGEE-0.3.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.674615 XGEE-0.3.6/XGEE.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3174 2024-03-19 20:30:32.000000 XGEE-0.3.6/XGEE.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    43015 2024-03-19 20:30:32.000000 XGEE-0.3.6/XGEE.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-19 20:30:32.000000 XGEE-0.3.6/XGEE.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-03-19 20:30:32.000000 XGEE-0.3.6/XGEE.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       62 2024-03-19 20:30:32.000000 XGEE-0.3.6/XGEE.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-03-19 20:30:32.000000 XGEE-0.3.6/XGEE.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-19 20:30:32.675615 XGEE-0.3.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1945 2024-03-19 20:30:24.000000 XGEE-0.3.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.465613 XGEE-0.3.6/xgee/
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-03-19 20:30:24.000000 XGEE-0.3.6/xgee/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2024-03-19 20:30:24.000000 XGEE-0.3.6/xgee/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.466613 XGEE-0.3.6/xgee/core/
--rw-r--r--   0 root         (0) root         (0)       37 2024-03-19 20:30:27.000000 XGEE-0.3.6/xgee/core/.git
--rw-r--r--   0 root         (0) root         (0)      362 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/.gitmodules
--rw-r--r--   0 root         (0) root         (0)     1078 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/LICENSE
--rw-r--r--   0 root         (0) root         (0)      581 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.437613 XGEE-0.3.6/xgee/core/dep/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.467613 XGEE-0.3.6/xgee/core/dep/bluebird/
--rw-r--r--   0 root         (0) root         (0)   183390 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/bluebird/bluebird.js
--rw-r--r--   0 root         (0) root         (0)    81530 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/bluebird/bluebird.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.467613 XGEE-0.3.6/xgee/core/dep/font-awesome/
--rw-r--r--   0 root         (0) root         (0)     1548 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/LICENSE.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.471613 XGEE-0.3.6/xgee/core/dep/font-awesome/css/
--rw-r--r--   0 root         (0) root         (0)    73117 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/css/all.css
--rw-r--r--   0 root         (0) root         (0)    58935 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/css/all.min.css
--rw-r--r--   0 root         (0) root         (0)      732 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/css/brands.css
--rw-r--r--   0 root         (0) root         (0)      675 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/css/brands.min.css
--rw-r--r--   0 root         (0) root         (0)    71482 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/css/fontawesome.css
--rw-r--r--   0 root         (0) root         (0)    57503 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/css/fontawesome.min.css
--rw-r--r--   0 root         (0) root         (0)      734 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/css/regular.css
--rw-r--r--   0 root         (0) root         (0)      677 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/css/regular.min.css
--rw-r--r--   0 root         (0) root         (0)      727 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/css/solid.css
--rw-r--r--   0 root         (0) root         (0)      669 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/css/solid.min.css
--rw-r--r--   0 root         (0) root         (0)     8077 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/css/svg-with-js.css
--rw-r--r--   0 root         (0) root         (0)     6359 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/css/svg-with-js.min.css
--rw-r--r--   0 root         (0) root         (0)    41312 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/css/v4-shims.css
--rw-r--r--   0 root         (0) root         (0)    26702 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/css/v4-shims.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.479613 XGEE-0.3.6/xgee/core/dep/font-awesome/js/
--rw-r--r--   0 root         (0) root         (0)  1248390 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/js/all.js
--rw-r--r--   0 root         (0) root         (0)  1182553 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/js/all.min.js
--rw-r--r--   0 root         (0) root         (0)   445294 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/js/brands.js
--rw-r--r--   0 root         (0) root         (0)   438090 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/js/brands.min.js
--rw-r--r--   0 root         (0) root         (0)    33929 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/js/conflict-detection.js
--rw-r--r--   0 root         (0) root         (0)    13502 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/js/conflict-detection.min.js
--rw-r--r--   0 root         (0) root         (0)    79139 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/js/fontawesome.js
--rw-r--r--   0 root         (0) root         (0)    37191 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/js/fontawesome.min.js
--rw-r--r--   0 root         (0) root         (0)   107110 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/js/regular.js
--rw-r--r--   0 root         (0) root         (0)   103386 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/js/regular.min.js
--rw-r--r--   0 root         (0) root         (0)   617405 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/js/solid.js
--rw-r--r--   0 root         (0) root         (0)   604447 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/js/solid.min.js
--rw-r--r--   0 root         (0) root         (0)    17459 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/js/v4-shims.js
--rw-r--r--   0 root         (0) root         (0)    15055 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/js/v4-shims.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.485613 XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/
--rw-r--r--   0 root         (0) root         (0)   134878 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-brands-400.eot
--rw-r--r--   0 root         (0) root         (0)   729325 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-brands-400.svg
--rw-r--r--   0 root         (0) root         (0)   134572 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0 root         (0) root         (0)    90872 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-brands-400.woff
--rw-r--r--   0 root         (0) root         (0)    77444 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0 root         (0) root         (0)    34390 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-regular-400.eot
--rw-r--r--   0 root         (0) root         (0)   144322 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-regular-400.svg
--rw-r--r--   0 root         (0) root         (0)    34092 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0 root         (0) root         (0)    16800 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-regular-400.woff
--rw-r--r--   0 root         (0) root         (0)    13596 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0 root         (0) root         (0)   204866 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-solid-900.eot
--rw-r--r--   0 root         (0) root         (0)   910710 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-solid-900.svg
--rw-r--r--   0 root         (0) root         (0)   204580 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0 root         (0) root         (0)   104252 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-solid-900.woff
--rw-r--r--   0 root         (0) root         (0)    80328 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.488613 XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.488613 XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/font/
--rw-r--r--   0 root         (0) root         (0)     3528 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.eot
--rw-r--r--   0 root         (0) root         (0)     3320 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.ttf
--rw-r--r--   0 root         (0) root         (0)     2180 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.woff
--rw-r--r--   0 root         (0) root         (0)     1680 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.woff2
--rw-r--r--   0 root         (0) root         (0)     7278 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.css
--rw-r--r--   0 root         (0) root         (0)    91213 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.js
--rw-r--r--   0 root         (0) root         (0)     5991 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.css
--rw-r--r--   0 root         (0) root         (0)    14532 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.css.map
--rw-r--r--   0 root         (0) root         (0)    27807 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.js
--rw-r--r--   0 root         (0) root         (0)   131140 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.js.map
--rw-r--r--   0 root         (0) root         (0)    22405 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/jquery.ui.position.js
--rw-r--r--   0 root         (0) root         (0)     5855 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/jquery.ui.position.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.489613 XGEE-0.3.6/xgee/core/dep/jquery/
--rw-r--r--   0 root         (0) root         (0)     1097 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jquery/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    86927 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jquery/jquery-3.3.1.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.490613 XGEE-0.3.6/xgee/core/dep/jquery-ui/
--rw-r--r--   0 root         (0) root         (0)     1817 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jquery-ui/LICENSE.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.492613 XGEE-0.3.6/xgee/core/dep/jquery-ui/images/
--rw-r--r--   0 root         (0) root         (0)     7006 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jquery-ui/images/ui-icons_444444_256x240.png
--rw-r--r--   0 root         (0) root         (0)     7074 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jquery-ui/images/ui-icons_555555_256x240.png
--rw-r--r--   0 root         (0) root         (0)     4676 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jquery-ui/images/ui-icons_777620_256x240.png
--rw-r--r--   0 root         (0) root         (0)     7013 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jquery-ui/images/ui-icons_777777_256x240.png
--rw-r--r--   0 root         (0) root         (0)     4632 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jquery-ui/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 root         (0) root         (0)     6313 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jquery-ui/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 root         (0) root         (0)    32076 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jquery-ui/jquery-ui.min.css
--rw-r--r--   0 root         (0) root         (0)   253669 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jquery-ui/jquery-ui.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.495613 XGEE-0.3.6/xgee/core/dep/jsa/
--rw-r--r--   0 root         (0) root         (0)       55 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/jsa/.git
--rw-r--r--   0 root         (0) root         (0)       14 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/.gitignore
--rw-r--r--   0 root         (0) root         (0)     2327 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1137 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1291 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.498613 XGEE-0.3.6/xgee/core/dep/jsa/img/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.502613 XGEE-0.3.6/xgee/core/dep/jsa/img/black/
--rw-r--r--   0 root         (0) root         (0)     2092 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/black/bubble-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2083 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/black/bubble.svg
--rw-r--r--   0 root         (0) root         (0)     2214 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/black/close-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2196 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/black/close.svg
--rw-r--r--   0 root         (0) root         (0)     2097 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/black/folder.svg
--rw-r--r--   0 root         (0) root         (0)     2072 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/black/home.svg
--rw-r--r--   0 root         (0) root         (0)    12585 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/black/jsa.svg
--rw-r--r--   0 root         (0) root         (0)     2201 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/black/maximize-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2192 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/black/maximize.svg
--rw-r--r--   0 root         (0) root         (0)     2880 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/black/menu-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2862 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/black/menu.svg
--rw-r--r--   0 root         (0) root         (0)     2075 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/black/minimize-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2066 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/black/minimize.svg
--rw-r--r--   0 root         (0) root         (0)     2326 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/black/redo.svg
--rw-r--r--   0 root         (0) root         (0)     2374 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/black/settings.svg
--rw-r--r--   0 root         (0) root         (0)     2378 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/black/undo.svg
--rw-r--r--   0 root         (0) root         (0)     2343 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/black/view-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2334 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/black/view.svg
--rw-r--r--   0 root         (0) root         (0)     3032 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/close-hover.svg
--rw-r--r--   0 root         (0) root         (0)     3032 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/close.svg
--rw-r--r--   0 root         (0) root         (0)    12585 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/jsa.svg
--rw-r--r--   0 root         (0) root         (0)     3731 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/loading.svg
--rw-r--r--   0 root         (0) root         (0)     2443 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/maximize.svg
--rw-r--r--   0 root         (0) root         (0)     2437 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/minimize.svg
--rw-r--r--   0 root         (0) root         (0)     3173 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/resize-ne.svg
--rw-r--r--   0 root         (0) root         (0)     3172 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/resize-nw.svg
--rw-r--r--   0 root         (0) root         (0)     3173 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/resize-se.svg
--rw-r--r--   0 root         (0) root         (0)     3113 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/resize-sw.svg
--rw-r--r--   0 root         (0) root         (0)     3639 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/restore.svg
--rw-r--r--   0 root         (0) root         (0)     2637 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/tool-default.svg
--rw-r--r--   0 root         (0) root         (0)     2693 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/view-close.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.506613 XGEE-0.3.6/xgee/core/dep/jsa/img/white/
--rw-r--r--   0 root         (0) root         (0)     2083 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/white/bubble-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2074 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/white/bubble.svg
--rw-r--r--   0 root         (0) root         (0)     2205 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/white/close-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2196 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/white/close.svg
--rw-r--r--   0 root         (0) root         (0)     2097 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/white/folder.svg
--rw-r--r--   0 root         (0) root         (0)     2063 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/white/home.svg
--rw-r--r--   0 root         (0) root         (0)    12585 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/white/jsa.svg
--rw-r--r--   0 root         (0) root         (0)     2192 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/white/maximize-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2183 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/white/maximize.svg
--rw-r--r--   0 root         (0) root         (0)     2871 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/white/menu-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2853 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/white/menu.svg
--rw-r--r--   0 root         (0) root         (0)     2066 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/white/minimize-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2057 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/white/minimize.svg
--rw-r--r--   0 root         (0) root         (0)     2317 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/white/redo.svg
--rw-r--r--   0 root         (0) root         (0)     2365 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/white/settings.svg
--rw-r--r--   0 root         (0) root         (0)     2369 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/white/undo.svg
--rw-r--r--   0 root         (0) root         (0)     2334 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/white/view-hover.svg
--rw-r--r--   0 root         (0) root         (0)     2325 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/img/white/view.svg
--rw-r--r--   0 root         (0) root         (0)    46194 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/jsapplication.css
--rw-r--r--   0 root         (0) root         (0)   357922 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/jsapplication.js
--rw-r--r--   0 root         (0) root         (0)    15308 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/jsapplicationPlugins.js
--rw-r--r--   0 root         (0) root         (0)      402 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/package.json
--rw-r--r--   0 root         (0) root         (0)     1252 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/dep/jsa/webpack.config.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.506613 XGEE-0.3.6/xgee/core/dep/mxgraph/
--rw-r--r--   0 root         (0) root         (0)    10487 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.506613 XGEE-0.3.6/xgee/core/dep/mxgraph/css/
--rw-r--r--   0 root         (0) root         (0)     4325 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/css/common.css
--rw-r--r--   0 root         (0) root         (0)      486 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/css/explorer.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.510613 XGEE-0.3.6/xgee/core/dep/mxgraph/images/
--rw-r--r--   0 root         (0) root         (0)      137 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/images/button.gif
--rw-r--r--   0 root         (0) root         (0)       70 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/images/close.gif
--rw-r--r--   0 root         (0) root         (0)      877 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/images/collapsed.gif
--rw-r--r--   0 root         (0) root         (0)      907 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/images/error.gif
--rw-r--r--   0 root         (0) root         (0)      878 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/images/expanded.gif
--rw-r--r--   0 root         (0) root         (0)      843 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/images/maximize.gif
--rw-r--r--   0 root         (0) root         (0)       64 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/images/minimize.gif
--rw-r--r--   0 root         (0) root         (0)      845 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/images/normalize.gif
--rw-r--r--   0 root         (0) root         (0)       55 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/images/point.gif
--rw-r--r--   0 root         (0) root         (0)       74 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/images/resize.gif
--rw-r--r--   0 root         (0) root         (0)      146 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/images/separator.gif
--rw-r--r--   0 root         (0) root         (0)       56 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/images/submenu.gif
--rw-r--r--   0 root         (0) root         (0)       90 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/images/transparent.gif
--rw-r--r--   0 root         (0) root         (0)      276 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/images/warning.gif
--rw-r--r--   0 root         (0) root         (0)      425 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/images/warning.png
--rw-r--r--   0 root         (0) root         (0)      275 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/images/window-title.gif
--rw-r--r--   0 root         (0) root         (0)       75 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/images/window.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.511613 XGEE-0.3.6/xgee/core/dep/mxgraph/js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.512613 XGEE-0.3.6/xgee/core/dep/mxgraph/js/editor/
--rw-r--r--   0 root         (0) root         (0)     3232 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/editor/mxDefaultKeyHandler.js
--rw-r--r--   0 root         (0) root         (0)     9716 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/editor/mxDefaultPopupMenu.js
--rw-r--r--   0 root         (0) root         (0)    14610 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/editor/mxDefaultToolbar.js
--rw-r--r--   0 root         (0) root         (0)    74993 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/editor/mxEditor.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.516613 XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/
--rw-r--r--   0 root         (0) root         (0)     7282 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxCellHighlight.js
--rw-r--r--   0 root         (0) root         (0)     9337 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxCellMarker.js
--rw-r--r--   0 root         (0) root         (0)     2992 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxCellTracker.js
--rw-r--r--   0 root         (0) root         (0)    62381 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxConnectionHandler.js
--rw-r--r--   0 root         (0) root         (0)    13695 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxConstraintHandler.js
--rw-r--r--   0 root         (0) root         (0)    63081 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxEdgeHandler.js
--rw-r--r--   0 root         (0) root         (0)     9925 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxEdgeSegmentHandler.js
--rw-r--r--   0 root         (0) root         (0)     5944 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxElbowEdgeHandler.js
--rw-r--r--   0 root         (0) root         (0)    39448 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxGraphHandler.js
--rw-r--r--   0 root         (0) root         (0)     7701 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxHandle.js
--rw-r--r--   0 root         (0) root         (0)    10128 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxKeyHandler.js
--rw-r--r--   0 root         (0) root         (0)    11402 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxPanningHandler.js
--rw-r--r--   0 root         (0) root         (0)     5293 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxPopupMenuHandler.js
--rw-r--r--   0 root         (0) root         (0)     9837 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxRubberband.js
--rw-r--r--   0 root         (0) root         (0)     6478 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxSelectionCellsHandler.js
--rw-r--r--   0 root         (0) root         (0)     7419 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxTooltipHandler.js
--rw-r--r--   0 root         (0) root         (0)    52962 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxVertexHandler.js
--rw-r--r--   0 root         (0) root         (0)    12044 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/index.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.520614 XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/
--rw-r--r--   0 root         (0) root         (0)     4531 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxCellCodec.js
--rw-r--r--   0 root         (0) root         (0)     4207 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxChildChangeCodec.js
--rw-r--r--   0 root         (0) root         (0)    13541 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxCodec.js
--rw-r--r--   0 root         (0) root         (0)     2690 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxCodecRegistry.js
--rw-r--r--   0 root         (0) root         (0)     1986 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxDefaultKeyHandlerCodec.js
--rw-r--r--   0 root         (0) root         (0)     1226 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxDefaultPopupMenuCodec.js
--rw-r--r--   0 root         (0) root         (0)     9221 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxDefaultToolbarCodec.js
--rw-r--r--   0 root         (0) root         (0)     6163 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxEditorCodec.js
--rw-r--r--   0 root         (0) root         (0)     1798 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxGenericChangeCodec.js
--rw-r--r--   0 root         (0) root         (0)      621 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxGraphCodec.js
--rw-r--r--   0 root         (0) root         (0)     5022 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxGraphViewCodec.js
--rw-r--r--   0 root         (0) root         (0)     1705 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxModelCodec.js
--rw-r--r--   0 root         (0) root         (0)    30213 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxObjectCodec.js
--rw-r--r--   0 root         (0) root         (0)     1598 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxRootChangeCodec.js
--rw-r--r--   0 root         (0) root         (0)     4651 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxStylesheetCodec.js
--rw-r--r--   0 root         (0) root         (0)      818 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxTerminalChangeCodec.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.522613 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.523614 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.524613 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/model/
--rw-r--r--   0 root         (0) root         (0)     4029 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphAbstractHierarchyCell.js
--rw-r--r--   0 root         (0) root         (0)     3852 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyEdge.js
--rw-r--r--   0 root         (0) root         (0)    20322 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyModel.js
--rw-r--r--   0 root         (0) root         (0)     4915 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyNode.js
--rw-r--r--   0 root         (0) root         (0)    23605 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxSwimlaneModel.js
--rw-r--r--   0 root         (0) root         (0)    20146 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/mxHierarchicalLayout.js
--rw-r--r--   0 root         (0) root         (0)    22708 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/mxSwimlaneLayout.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.525613 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/
--rw-r--r--   0 root         (0) root         (0)    43070 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxCoordinateAssignment.js
--rw-r--r--   0 root         (0) root         (0)      726 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxHierarchicalLayoutStage.js
--rw-r--r--   0 root         (0) root         (0)    16867 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxMedianHybridCrossingReduction.js
--rw-r--r--   0 root         (0) root         (0)     3123 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxMinimumCycleRemover.js
--rw-r--r--   0 root         (0) root         (0)     2816 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxSwimlaneOrdering.js
--rw-r--r--   0 root         (0) root         (0)     4343 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/mxCircleLayout.js
--rw-r--r--   0 root         (0) root         (0)    22959 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/mxCompactTreeLayout.js
--rw-r--r--   0 root         (0) root         (0)     2496 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/mxCompositeLayout.js
--rw-r--r--   0 root         (0) root         (0)     3158 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/mxEdgeLabelLayout.js
--rw-r--r--   0 root         (0) root         (0)    14338 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/mxFastOrganicLayout.js
--rw-r--r--   0 root         (0) root         (0)    14251 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/mxGraphLayout.js
--rw-r--r--   0 root         (0) root         (0)     4851 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/mxParallelEdgeLayout.js
--rw-r--r--   0 root         (0) root         (0)     5537 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/mxPartitionLayout.js
--rw-r--r--   0 root         (0) root         (0)     8037 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/mxRadialTreeLayout.js
--rw-r--r--   0 root         (0) root         (0)    12740 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/mxStackLayout.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.526614 XGEE-0.3.6/xgee/core/dep/mxgraph/js/model/
--rw-r--r--   0 root         (0) root         (0)    15954 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/model/mxCell.js
--rw-r--r--   0 root         (0) root         (0)     2933 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/model/mxCellPath.js
--rw-r--r--   0 root         (0) root         (0)    12721 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/model/mxGeometry.js
--rw-r--r--   0 root         (0) root         (0)    62665 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/model/mxGraphModel.js
--rw-r--r--   0 root         (0) root         (0)    28988 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/mxClient.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.531613 XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/
--rw-r--r--   0 root         (0) root         (0)     2117 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxActor.js
--rw-r--r--   0 root         (0) root         (0)     3316 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxArrow.js
--rw-r--r--   0 root         (0) root         (0)    11601 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxArrowConnector.js
--rw-r--r--   0 root         (0) root         (0)     1506 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxCloud.js
--rw-r--r--   0 root         (0) root         (0)     4196 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxConnector.js
--rw-r--r--   0 root         (0) root         (0)     2694 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxCylinder.js
--rw-r--r--   0 root         (0) root         (0)     2823 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxDoubleEllipse.js
--rw-r--r--   0 root         (0) root         (0)     1159 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxEllipse.js
--rw-r--r--   0 root         (0) root         (0)      802 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxHexagon.js
--rw-r--r--   0 root         (0) root         (0)     6341 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxImageShape.js
--rw-r--r--   0 root         (0) root         (0)     6800 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxLabel.js
--rw-r--r--   0 root         (0) root         (0)     1139 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxLine.js
--rw-r--r--   0 root         (0) root         (0)     5400 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxMarker.js
--rw-r--r--   0 root         (0) root         (0)     2485 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxPolyline.js
--rw-r--r--   0 root         (0) root         (0)     3068 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxRectangleShape.js
--rw-r--r--   0 root         (0) root         (0)     1597 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxRhombus.js
--rw-r--r--   0 root         (0) root         (0)    38952 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxShape.js
--rw-r--r--   0 root         (0) root         (0)    26031 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxStencil.js
--rw-r--r--   0 root         (0) root         (0)     1053 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxStencilRegistry.js
--rw-r--r--   0 root         (0) root         (0)     9507 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxSwimlane.js
--rw-r--r--   0 root         (0) root         (0)    37084 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxText.js
--rw-r--r--   0 root         (0) root         (0)      828 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxTriangle.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.540614 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/
--rw-r--r--   0 root         (0) root         (0)    11723 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxAbstractCanvas2D.js
--rw-r--r--   0 root         (0) root         (0)     1895 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxAnimation.js
--rw-r--r--   0 root         (0) root         (0)     4430 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxAutoSaveManager.js
--rw-r--r--   0 root         (0) root         (0)     5354 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxClipboard.js
--rw-r--r--   0 root         (0) root         (0)    63826 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxConstants.js
--rw-r--r--   0 root         (0) root         (0)     2236 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxDictionary.js
--rw-r--r--   0 root         (0) root         (0)     3205 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxDivResizer.js
--rw-r--r--   0 root         (0) root         (0)    16885 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxDragSource.js
--rw-r--r--   0 root         (0) root         (0)     4460 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxEffects.js
--rw-r--r--   0 root         (0) root         (0)    27401 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxEvent.js
--rw-r--r--   0 root         (0) root         (0)     1941 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxEventObject.js
--rw-r--r--   0 root         (0) root         (0)     3778 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxEventSource.js
--rw-r--r--   0 root         (0) root         (0)     4041 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxForm.js
--rw-r--r--   0 root         (0) root         (0)    10378 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxGuide.js
--rw-r--r--   0 root         (0) root         (0)      670 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxImage.js
--rw-r--r--   0 root         (0) root         (0)     3380 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxImageBundle.js
--rw-r--r--   0 root         (0) root         (0)     3798 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxImageExport.js
--rw-r--r--   0 root         (0) root         (0)     8228 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxLog.js
--rw-r--r--   0 root         (0) root         (0)     5691 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxMorphing.js
--rw-r--r--   0 root         (0) root         (0)     4481 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxMouseEvent.js
--rw-r--r--   0 root         (0) root         (0)     1485 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxObjectIdentity.js
--rw-r--r--   0 root         (0) root         (0)     5082 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxPanningManager.js
--rw-r--r--   0 root         (0) root         (0)     1039 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxPoint.js
--rw-r--r--   0 root         (0) root         (0)    14045 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxPopupMenu.js
--rw-r--r--   0 root         (0) root         (0)     3693 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxRectangle.js
--rw-r--r--   0 root         (0) root         (0)    11080 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxResources.js
--rw-r--r--   0 root         (0) root         (0)    45946 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxSvgCanvas2D.js
--rw-r--r--   0 root         (0) root         (0)    12132 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxToolbar.js
--rw-r--r--   0 root         (0) root         (0)     5793 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxUndoManager.js
--rw-r--r--   0 root         (0) root         (0)     4535 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxUndoableEdit.js
--rw-r--r--   0 root         (0) root         (0)     2768 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxUrlConverter.js
--rw-r--r--   0 root         (0) root         (0)   106481 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxUtils.js
--rw-r--r--   0 root         (0) root         (0)    26243 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxVmlCanvas2D.js
--rw-r--r--   0 root         (0) root         (0)    27971 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxWindow.js
--rw-r--r--   0 root         (0) root         (0)    28763 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxXmlCanvas2D.js
--rw-r--r--   0 root         (0) root         (0)    10820 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxXmlRequest.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.545614 XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/
--rw-r--r--   0 root         (0) root         (0)    35624 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxCellEditor.js
--rw-r--r--   0 root         (0) root         (0)     6245 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxCellOverlay.js
--rw-r--r--   0 root         (0) root         (0)    44101 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxCellRenderer.js
--rw-r--r--   0 root         (0) root         (0)     9726 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxCellState.js
--rw-r--r--   0 root         (0) root         (0)     4286 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxCellStatePreview.js
--rw-r--r--   0 root         (0) root         (0)     1649 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxConnectionConstraint.js
--rw-r--r--   0 root         (0) root         (0)    42452 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxEdgeStyle.js
--rw-r--r--   0 root         (0) root         (0)   333205 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxGraph.js
--rw-r--r--   0 root         (0) root         (0)     9127 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxGraphSelectionModel.js
--rw-r--r--   0 root         (0) root         (0)    74549 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxGraphView.js
--rw-r--r--   0 root         (0) root         (0)    10941 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxLayoutManager.js
--rw-r--r--   0 root         (0) root         (0)     7440 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxMultiplicity.js
--rw-r--r--   0 root         (0) root         (0)    19683 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxOutline.js
--rw-r--r--   0 root         (0) root         (0)    20530 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxPerimeter.js
--rw-r--r--   0 root         (0) root         (0)    32135 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxPrintPreview.js
--rw-r--r--   0 root         (0) root         (0)     2022 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxStyleRegistry.js
--rw-r--r--   0 root         (0) root         (0)     6753 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxStylesheet.js
--rw-r--r--   0 root         (0) root         (0)     9336 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxSwimlaneManager.js
--rw-r--r--   0 root         (0) root         (0)     2955 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxTemporaryCellStates.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.546614 XGEE-0.3.6/xgee/core/dep/mxgraph/resources/
--rw-r--r--   0 root         (0) root         (0)       83 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/resources/editor.txt
--rw-r--r--   0 root         (0) root         (0)       96 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/resources/editor_de.txt
--rw-r--r--   0 root         (0) root         (0)       83 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/resources/editor_zh.txt
--rw-r--r--   0 root         (0) root         (0)      340 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/resources/graph.txt
--rw-r--r--   0 root         (0) root         (0)      375 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/resources/graph_de.txt
--rw-r--r--   0 root         (0) root         (0)      316 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/mxgraph/resources/graph_zh.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.547614 XGEE-0.3.6/xgee/core/dep/notifyjs/
--rw-r--r--   0 root         (0) root         (0)      290 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/notifyjs/LICENSE
--rw-r--r--   0 root         (0) root         (0)    13780 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/notifyjs/notify.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.547614 XGEE-0.3.6/xgee/core/dep/underscore/
--rw-r--r--   0 root         (0) root         (0)     1139 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/underscore/LICENSE
--rw-r--r--   0 root         (0) root         (0)    18069 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/dep/underscore/underscore-min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.457613 XGEE-0.3.6/xgee/core/plugins/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.547614 XGEE-0.3.6/xgee/core/plugins/autostart/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.548614 XGEE-0.3.6/xgee/core/plugins/autostart/js/
--rw-r--r--   0 root         (0) root         (0)      593 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/autostart/js/AppStartupEvent.js
--rw-r--r--   0 root         (0) root         (0)      823 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/autostart/js/AppStartupObserver.js
--rw-r--r--   0 root         (0) root         (0)     1138 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/autostart/js/Autostarter.js
--rw-r--r--   0 root         (0) root         (0)     3186 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/autostart/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.548614 XGEE-0.3.6/xgee/core/plugins/clipboard/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.550614 XGEE-0.3.6/xgee/core/plugins/clipboard/js/
--rw-r--r--   0 root         (0) root         (0)      969 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/clipboard/js/AppClipboard.js
--rw-r--r--   0 root         (0) root         (0)     1279 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/clipboard/js/Clipboard.js
--rw-r--r--   0 root         (0) root         (0)     6598 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/clipboard/js/ClipboardAPI.js
--rw-r--r--   0 root         (0) root         (0)      308 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/clipboard/js/ClipboardEvaluator.js
--rw-r--r--   0 root         (0) root         (0)      618 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/clipboard/js/ClipboardEventHandler.js
--rw-r--r--   0 root         (0) root         (0)     3342 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/clipboard/js/ClipboardManager.js
--rw-r--r--   0 root         (0) root         (0)     3665 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/clipboard/js/EcoreClipboardEvaluator.js
--rw-r--r--   0 root         (0) root         (0)     4999 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/clipboard/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.550614 XGEE-0.3.6/xgee/core/plugins/contextMenu/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.551614 XGEE-0.3.6/xgee/core/plugins/contextMenu/js/
--rw-r--r--   0 root         (0) root         (0)     3032 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/contextMenu/js/ContextMenu.js
--rw-r--r--   0 root         (0) root         (0)     1768 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/contextMenu/js/util.js
--rw-r--r--   0 root         (0) root         (0)     2762 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/contextMenu/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.550614 XGEE-0.3.6/xgee/core/plugins/contextMenu.ecore/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.550614 XGEE-0.3.6/xgee/core/plugins/contextMenu.ecore/css/
--rw-r--r--   0 root         (0) root         (0)      399 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/contextMenu.ecore/css/contextMenu.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.551614 XGEE-0.3.6/xgee/core/plugins/contextMenu.ecore/js/
--rw-r--r--   0 root         (0) root         (0)      361 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/contextMenu.ecore/js/Filter.js
--rw-r--r--   0 root         (0) root         (0)    13387 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/contextMenu.ecore/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.551614 XGEE-0.3.6/xgee/core/plugins/contextMenu.eoq/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.551614 XGEE-0.3.6/xgee/core/plugins/contextMenu.eoq/js/
--rw-r--r--   0 root         (0) root         (0)     4740 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/contextMenu.eoq/js/util.js
--rw-r--r--   0 root         (0) root         (0)     4218 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/contextMenu.eoq/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.552614 XGEE-0.3.6/xgee/core/plugins/ecore/
--rw-r--r--   0 root         (0) root         (0)    11515 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/LICENSE
--rw-r--r--   0 root         (0) root         (0)    93760 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/ecore.xmi.js
--rw-r--r--   0 root         (0) root         (0)      456 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.554614 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/
--rw-r--r--   0 root         (0) root         (0)       57 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/.gitignore
--rw-r--r--   0 root         (0) root         (0)      145 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/.travis.yml
--rw-r--r--   0 root         (0) root         (0)      366 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/AUTHORS
--rw-r--r--   0 root         (0) root         (0)      280 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     2011 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8381 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.557614 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/examples/
--rw-r--r--   0 root         (0) root         (0)   181013 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/examples/big-not-pretty.xml
--rw-r--r--   0 root         (0) root         (0)      790 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/examples/example.js
--rw-r--r--   0 root         (0) root         (0)     1539 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/examples/get-products.js
--rw-r--r--   0 root         (0) root         (0)      164 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/examples/hello-world.js
--rw-r--r--   0 root         (0) root         (0)      181 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/examples/not-pretty.xml
--rw-r--r--   0 root         (0) root         (0)     1506 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/examples/pretty-print.js
--rw-r--r--   0 root         (0) root         (0)    99650 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/examples/shopping.xml
--rw-r--r--   0 root         (0) root         (0)      138 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/examples/test.html
--rw-r--r--   0 root         (0) root         (0)    51402 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/examples/test.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.557614 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/lib/
--rw-r--r--   0 root         (0) root         (0)    43541 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/lib/sax.js
--rw-r--r--   0 root         (0) root         (0)    85352 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/package-lock.json
--rw-r--r--   0 root         (0) root         (0)      655 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.570614 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/
--rw-r--r--   0 root         (0) root         (0)      763 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/attribute-name.js
--rw-r--r--   0 root         (0) root         (0)     2426 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/attribute-no-space.js
--rw-r--r--   0 root         (0) root         (0)      719 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/attribute-unquoted.js
--rw-r--r--   0 root         (0) root         (0)     1478 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/bom.js
--rw-r--r--   0 root         (0) root         (0)     1047 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/buffer-overrun.js
--rw-r--r--   0 root         (0) root         (0)     1557 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/case.js
--rw-r--r--   0 root         (0) root         (0)      389 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/cdata-chunked.js
--rw-r--r--   0 root         (0) root         (0)      363 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/cdata-end-split.js
--rw-r--r--   0 root         (0) root         (0)      782 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/cdata-fake-end.js
--rw-r--r--   0 root         (0) root         (0)      514 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/cdata-multiple.js
--rw-r--r--   0 root         (0) root         (0)      362 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/cdata.js
--rw-r--r--   0 root         (0) root         (0)      247 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/cyrillic.js
--rw-r--r--   0 root         (0) root         (0)      383 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/duplicate-attribute.js
--rw-r--r--   0 root         (0) root         (0)      343 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/emoji.js
--rw-r--r--   0 root         (0) root         (0)      130 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/end_empty_stream.js
--rw-r--r--   0 root         (0) root         (0)      368 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/entities.js
--rw-r--r--   0 root         (0) root         (0)      372 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/entity-mega.js
--rw-r--r--   0 root         (0) root         (0)      238 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/entity-nan.js
--rw-r--r--   0 root         (0) root         (0)      329 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/flush.js
--rw-r--r--   0 root         (0) root         (0)     1311 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/index.js
--rw-r--r--   0 root         (0) root         (0)     1912 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/issue-23.js
--rw-r--r--   0 root         (0) root         (0)      691 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/issue-30.js
--rw-r--r--   0 root         (0) root         (0)      336 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/issue-35.js
--rw-r--r--   0 root         (0) root         (0)      398 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/issue-47.js
--rw-r--r--   0 root         (0) root         (0)     1155 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/issue-49.js
--rw-r--r--   0 root         (0) root         (0)      467 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/issue-84.js
--rw-r--r--   0 root         (0) root         (0)     1196 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/issue-86.js
--rw-r--r--   0 root         (0) root         (0)      240 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/not-string.js
--rw-r--r--   0 root         (0) root         (0)     1300 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/opentagstart.js
--rw-r--r--   0 root         (0) root         (0)      952 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/parser-position.js
--rw-r--r--   0 root         (0) root         (0)      637 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/script-close-better.js
--rw-r--r--   0 root         (0) root         (0)     1035 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/script.js
--rw-r--r--   0 root         (0) root         (0)     1072 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/self-closing-child-strict.js
--rw-r--r--   0 root         (0) root         (0)     1073 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/self-closing-child.js
--rw-r--r--   0 root         (0) root         (0)      904 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/self-closing-tag.js
--rw-r--r--   0 root         (0) root         (0)      217 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/stand-alone-comment.js
--rw-r--r--   0 root         (0) root         (0)      755 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/stray-ending.js
--rw-r--r--   0 root         (0) root         (0)      288 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/trailing-attribute-no-value.js
--rw-r--r--   0 root         (0) root         (0)      407 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/trailing-non-whitespace.js
--rw-r--r--   0 root         (0) root         (0)      387 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/unclosed-root.js
--rw-r--r--   0 root         (0) root         (0)      727 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/unquoted.js
--rw-r--r--   0 root         (0) root         (0)     1009 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/utf8-split.js
--rw-r--r--   0 root         (0) root         (0)     1846 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/xml-internal-entities.js
--rw-r--r--   0 root         (0) root         (0)      429 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/xml_entities.js
--rw-r--r--   0 root         (0) root         (0)      465 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/xmlns-as-tag-name.js
--rw-r--r--   0 root         (0) root         (0)     1668 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/xmlns-issue-41.js
--rw-r--r--   0 root         (0) root         (0)     5497 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/xmlns-rebinding.js
--rw-r--r--   0 root         (0) root         (0)     5577 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/xmlns-strict.js
--rw-r--r--   0 root         (0) root         (0)     1805 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/xmlns-unbound-element.js
--rw-r--r--   0 root         (0) root         (0)      947 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/xmlns-unbound.js
--rw-r--r--   0 root         (0) root         (0)     1070 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-ns.js
--rw-r--r--   0 root         (0) root         (0)      871 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-prefix-attribute.js
--rw-r--r--   0 root         (0) root         (0)      509 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-prefix.js
--rw-r--r--   0 root         (0) root         (0)     1096 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-redefine.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.440613 XGEE-0.3.6/xgee/core/plugins/ecoreDebuggerUi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.570614 XGEE-0.3.6/xgee/core/plugins/ecoreDebuggerUi/js/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecoreDebuggerUi/js/ecoreDebuggerUiController.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.571614 XGEE-0.3.6/xgee/core/plugins/ecoreSync/
--rw-r--r--   0 root         (0) root         (0)       69 2024-03-19 20:30:29.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/.git
--rw-r--r--   0 root         (0) root         (0)     1073 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.576614 XGEE-0.3.6/xgee/core/plugins/ecoreSync/changes/
--rw-r--r--   0 root         (0) root         (0)    10675 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/changes/esChanges.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.576614 XGEE-0.3.6/xgee/core/plugins/ecoreSync/dev/
--rw-r--r--   0 root         (0) root         (0)     5919 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/dev/esDebugging.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.576614 XGEE-0.3.6/xgee/core/plugins/ecoreSync/dev/lib/
--rw-r--r--   0 root         (0) root         (0)     4918 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/dev/lib/libesync.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.578614 XGEE-0.3.6/xgee/core/plugins/ecoreSync/domain/
--rw-r--r--   0 root         (0) root         (0)     1484 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/domain/esDomain.js
--rw-r--r--   0 root         (0) root         (0)      378 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/domain/esErrors.js
--rw-r--r--   0 root         (0) root         (0)     3129 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/domain/esLookup.js
--rw-r--r--   0 root         (0) root         (0)    13249 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/domain/esMetaSync.js
--rw-r--r--   0 root         (0) root         (0)    20548 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/domain/esObjectAccessors.js
--rw-r--r--   0 root         (0) root         (0)     1570 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/domain/esOperationHandler.js
--rw-r--r--   0 root         (0) root         (0)     1901 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/ecoreSync.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.578614 XGEE-0.3.6/xgee/core/plugins/ecoreSync/interfaces/
--rw-r--r--   0 root         (0) root         (0)     2956 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/interfaces/esInstance.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.579614 XGEE-0.3.6/xgee/core/plugins/ecoreSync/mdb/
--rw-r--r--   0 root         (0) root         (0)    10832 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/mdb/esMdbAccessor.js
--rw-r--r--   0 root         (0) root         (0)     9168 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/mdb/esMdbObserver.js
--rw-r--r--   0 root         (0) root         (0)     9420 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/mdb/esModelDatabase.js
--rw-r--r--   0 root         (0) root         (0)     2183 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/mdb/esSyncEvents.js
--rw-r--r--   0 root         (0) root         (0)     1834 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/mdb/esSyncStatus.js
--rw-r--r--   0 root         (0) root         (0)     1416 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.581614 XGEE-0.3.6/xgee/core/plugins/ecoreSync/queries/
--rw-r--r--   0 root         (0) root         (0)    20117 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/queries/esCmdRunner.js
--rw-r--r--   0 root         (0) root         (0)     1851 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/queries/esQueries.js
--rw-r--r--   0 root         (0) root         (0)    36223 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/queries/esQueryEvaluator.js
--rw-r--r--   0 root         (0) root         (0)    26527 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/queries/esQueryObserver.js
--rw-r--r--   0 root         (0) root         (0)     2491 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/queries/esQueryObserverState.js
--rw-r--r--   0 root         (0) root         (0)     4045 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/queries/esQueryUtils.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.581614 XGEE-0.3.6/xgee/core/plugins/ecoreSync/util/
--rw-r--r--   0 root         (0) root         (0)      966 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/util/auxiliaries.js
--rw-r--r--   0 root         (0) root         (0)       50 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/util/esLogging.js
--rw-r--r--   0 root         (0) root         (0)    14957 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/util/esUtils.js
--rw-r--r--   0 root         (0) root         (0)     1194 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync/util/uuid.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.571614 XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.571614 XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/css/
--rw-r--r--   0 root         (0) root         (0)     5694 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/css/EObjectCtrls.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.575614 XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/
--rw-r--r--   0 root         (0) root         (0)     3076 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-close-active.svg
--rw-r--r--   0 root         (0) root         (0)     3032 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-close.svg
--rw-r--r--   0 root         (0) root         (0)     2667 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-custom-active.svg
--rw-r--r--   0 root         (0) root         (0)     2651 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-custom.svg
--rw-r--r--   0 root         (0) root         (0)     4500 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-global-active.svg
--rw-r--r--   0 root         (0) root         (0)     4471 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-global.svg
--rw-r--r--   0 root         (0) root         (0)     2560 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-local-active.svg
--rw-r--r--   0 root         (0) root         (0)     2553 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-local.svg
--rw-r--r--   0 root         (0) root         (0)     3529 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-select-all-active.svg
--rw-r--r--   0 root         (0) root         (0)     3500 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-select-all.svg
--rw-r--r--   0 root         (0) root         (0)     5270 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-select-invert-active.svg
--rw-r--r--   0 root         (0) root         (0)     5138 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-select-invert.svg
--rw-r--r--   0 root         (0) root         (0)     2381 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-select-none-active.svg
--rw-r--r--   0 root         (0) root         (0)     2364 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-select-none.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.575614 XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/js/
--rw-r--r--   0 root         (0) root         (0)     8088 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrlFactory.js
--rw-r--r--   0 root         (0) root         (0)     5394 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrlUpdateHandler.js
--rw-r--r--   0 root         (0) root         (0)    48418 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrls.js
--rw-r--r--   0 root         (0) root         (0)      760 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.582614 XGEE-0.3.6/xgee/core/plugins/editor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.443613 XGEE-0.3.6/xgee/core/plugins/editor/controllers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.584614 XGEE-0.3.6/xgee/core/plugins/editor/controllers/graph/
--rw-r--r--   0 root         (0) root         (0)      970 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/controllers/graph/AnchorController.js
--rw-r--r--   0 root         (0) root         (0)      972 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/controllers/graph/ContainerController.js
--rw-r--r--   0 root         (0) root         (0)     2337 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/controllers/graph/EdgeController.js
--rw-r--r--   0 root         (0) root         (0)    15589 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/controllers/graph/GraphController.js
--rw-r--r--   0 root         (0) root         (0)     7060 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/controllers/graph/GraphControllerFactory.js
--rw-r--r--   0 root         (0) root         (0)      275 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/controllers/graph/GraphObjectController.js
--rw-r--r--   0 root         (0) root         (0)      976 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/controllers/graph/LabelController.js
--rw-r--r--   0 root         (0) root         (0)      978 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/controllers/graph/QueryController.js
--rw-r--r--   0 root         (0) root         (0)     5353 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/controllers/graph/VertexController.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.584614 XGEE-0.3.6/xgee/core/plugins/editor/controllers/palette/
--rw-r--r--   0 root         (0) root         (0)     1245 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/controllers/palette/PaletteController.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.584614 XGEE-0.3.6/xgee/core/plugins/editor/css/
--rw-r--r--   0 root         (0) root         (0)      547 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/css/loading.css
--rw-r--r--   0 root         (0) root         (0)      115 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/css/xgeeJsaIntegration.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.585614 XGEE-0.3.6/xgee/core/plugins/editor/extensions/
--rw-r--r--   0 root         (0) root         (0)     2473 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/extensions/EditorContextMenuProvider.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.585614 XGEE-0.3.6/xgee/core/plugins/editor/graph/
--rw-r--r--   0 root         (0) root         (0)     1383 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/graph/GraphResourceProvider.js
--rw-r--r--   0 root         (0) root         (0)     6693 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/graph/mxGraphIntegration.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.586614 XGEE-0.3.6/xgee/core/plugins/editor/interactions/
--rw-r--r--   0 root         (0) root         (0)     3785 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/interactions/DropReception.js
--rw-r--r--   0 root         (0) root         (0)     1042 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/interactions/GraphInteraction.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.586614 XGEE-0.3.6/xgee/core/plugins/editor/lib/
--rw-r--r--   0 root         (0) root         (0)    10080 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/lib/libapi.js
--rw-r--r--   0 root         (0) root         (0)     9750 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/lib/libaux.js
--rw-r--r--   0 root         (0) root         (0)    20059 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/lib/libjsa.js
--rw-r--r--   0 root         (0) root         (0)     1194 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/lib/uuid.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.587614 XGEE-0.3.6/xgee/core/plugins/editor/model/
--rw-r--r--   0 root         (0) root         (0)      339 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/PresentationModel.js
--rw-r--r--   0 root         (0) root         (0)    83708 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/editorModel.ecore
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.597614 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/
--rw-r--r--   0 root         (0) root         (0)     1866 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/Anchor.js
--rw-r--r--   0 root         (0) root         (0)     3246 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/AnchorManager.js
--rw-r--r--   0 root         (0) root         (0)      449 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/AnchorType.js
--rw-r--r--   0 root         (0) root         (0)     2305 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/Container.js
--rw-r--r--   0 root         (0) root         (0)     1896 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/ContainerManager.js
--rw-r--r--   0 root         (0) root         (0)      608 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/ContainerProvider.js
--rw-r--r--   0 root         (0) root         (0)     1760 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/ContainerType.js
--rw-r--r--   0 root         (0) root         (0)     1037 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/DeletableObject.js
--rw-r--r--   0 root         (0) root         (0)      266 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/EObjectOwner.js
--rw-r--r--   0 root         (0) root         (0)    10305 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/Edge.js
--rw-r--r--   0 root         (0) root         (0)     1264 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/EdgeContainer.js
--rw-r--r--   0 root         (0) root         (0)     6994 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/EdgeManager.js
--rw-r--r--   0 root         (0) root         (0)      383 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/EdgeType.js
--rw-r--r--   0 root         (0) root         (0)      566 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/EventProvider.js
--rw-r--r--   0 root         (0) root         (0)      346 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/FloatingLabel.js
--rw-r--r--   0 root         (0) root         (0)     1013 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/GraphEvent.js
--rw-r--r--   0 root         (0) root         (0)    27960 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/GraphLayoutManager.js
--rw-r--r--   0 root         (0) root         (0)     6623 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/GraphModel.js
--rw-r--r--   0 root         (0) root         (0)    12643 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/GraphModelFactory.js
--rw-r--r--   0 root         (0) root         (0)     4145 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/GraphModelManager.js
--rw-r--r--   0 root         (0) root         (0)      553 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/GraphObject.js
--rw-r--r--   0 root         (0) root         (0)     2097 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/GraphObjectManager.js
--rw-r--r--   0 root         (0) root         (0)      144 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/GraphObjectType.js
--rw-r--r--   0 root         (0) root         (0)     2200 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/Label.js
--rw-r--r--   0 root         (0) root         (0)     1990 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/LabelManager.js
--rw-r--r--   0 root         (0) root         (0)      478 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/LabelProvider.js
--rw-r--r--   0 root         (0) root         (0)     2061 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/LabelSegment.js
--rw-r--r--   0 root         (0) root         (0)     6090 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/LabelSegmentManager.js
--rw-r--r--   0 root         (0) root         (0)      419 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/LabelSegmentType.js
--rw-r--r--   0 root         (0) root         (0)      386 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/LabelType.js
--rw-r--r--   0 root         (0) root         (0)      932 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/LocatableObject.js
--rw-r--r--   0 root         (0) root         (0)      615 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/NestedLabel.js
--rw-r--r--   0 root         (0) root         (0)      464 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/RoutableObject.js
--rw-r--r--   0 root         (0) root         (0)     1527 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/SizableObject.js
--rw-r--r--   0 root         (0) root         (0)     2346 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/StaticVertex.js
--rw-r--r--   0 root         (0) root         (0)     7913 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/StaticVertexManager.js
--rw-r--r--   0 root         (0) root         (0)     1684 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/StaticVertexType.js
--rw-r--r--   0 root         (0) root         (0)      546 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/TransactionObject.js
--rw-r--r--   0 root         (0) root         (0)       84 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/TypedObject.js
--rw-r--r--   0 root         (0) root         (0)     3517 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/Vertex.js
--rw-r--r--   0 root         (0) root         (0)    12233 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/VertexContainer.js
--rw-r--r--   0 root         (0) root         (0)    12436 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/VertexManager.js
--rw-r--r--   0 root         (0) root         (0)     1682 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/graph/VertexType.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.598614 XGEE-0.3.6/xgee/core/plugins/editor/model/palette/
--rw-r--r--   0 root         (0) root         (0)     2655 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/palette/DragAndDropTool.js
--rw-r--r--   0 root         (0) root         (0)    16081 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/palette/EdgeRoutingTool.js
--rw-r--r--   0 root         (0) root         (0)     3656 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/palette/GraphTool.js
--rw-r--r--   0 root         (0) root         (0)     8885 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/palette/PaletteModel.js
--rw-r--r--   0 root         (0) root         (0)     3844 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/palette/SelectionTool.js
--rw-r--r--   0 root         (0) root         (0)     8885 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/model/palette/ToolGenerator.js
--rw-r--r--   0 root         (0) root         (0)     5667 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.599614 XGEE-0.3.6/xgee/core/plugins/editor/queries/
--rw-r--r--   0 root         (0) root         (0)     6432 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/queries/Query.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.600614 XGEE-0.3.6/xgee/core/plugins/editor/view/
--rw-r--r--   0 root         (0) root         (0)    55157 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/view/GraphView.js
--rw-r--r--   0 root         (0) root         (0)     1725 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/view/GraphViewMenu.js
--rw-r--r--   0 root         (0) root         (0)    22370 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/view/GraphViewPort.js
--rw-r--r--   0 root         (0) root         (0)     3483 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/view/PaletteView.js
--rw-r--r--   0 root         (0) root         (0)     5888 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/editor/view/ScreenshotExport.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.600614 XGEE-0.3.6/xgee/core/plugins/eoq.actions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.600614 XGEE-0.3.6/xgee/core/plugins/eoq.actions/css/
--rw-r--r--   0 root         (0) root         (0)     2193 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/eoq.actions/css/ActionsUi.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.601614 XGEE-0.3.6/xgee/core/plugins/eoq.actions/js/
--rw-r--r--   0 root         (0) root         (0)     5233 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/eoq.actions/js/ActionsController.js
--rw-r--r--   0 root         (0) root         (0)    14133 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/eoq.actions/js/ActionsCore.js
--rw-r--r--   0 root         (0) root         (0)    23053 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/eoq.actions/js/ActionsUi.js
--rw-r--r--   0 root         (0) root         (0)     1541 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/eoq.actions/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.603614 XGEE-0.3.6/xgee/core/plugins/eoq1/
--rw-r--r--   0 root         (0) root         (0)       64 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq1/.git
--rw-r--r--   0 root         (0) root         (0)     1160 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1077 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq1/README.md
--rw-r--r--   0 root         (0) root         (0)    11898 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq1/commandparser.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.604614 XGEE-0.3.6/xgee/core/plugins/eoq1/domains/
--rw-r--r--   0 root         (0) root         (0)     5897 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq1/domains/bufferingdomain.js
--rw-r--r--   0 root         (0) root         (0)      879 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq1/domains/domain.js
--rw-r--r--   0 root         (0) root         (0)     4364 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq1/domains/httppostdomain.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.604614 XGEE-0.3.6/xgee/core/plugins/eoq1/model/
--rw-r--r--   0 root         (0) root         (0)    37451 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq1/model/model.js
--rw-r--r--   0 root         (0) root         (0)      468 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq1/package.json
--rw-r--r--   0 root         (0) root         (0)      504 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq1/plugin.js
--rw-r--r--   0 root         (0) root         (0)       90 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq1/queryparser.js
--rw-r--r--   0 root         (0) root         (0)    11900 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq1/resultparser.js
--rw-r--r--   0 root         (0) root         (0)    12168 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq1/valueparser.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.605614 XGEE-0.3.6/xgee/core/plugins/eoq2/
--rw-r--r--   0 root         (0) root         (0)       64 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq2/.git
--rw-r--r--   0 root         (0) root         (0)     1160 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      925 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.606614 XGEE-0.3.6/xgee/core/plugins/eoq2/action/
--rw-r--r--   0 root         (0) root         (0)      579 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq2/action/call.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.606614 XGEE-0.3.6/xgee/core/plugins/eoq2/command/
--rw-r--r--   0 root         (0) root         (0)    12287 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq2/command/command.js
--rw-r--r--   0 root         (0) root         (0)     1365 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq2/command/result.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.606614 XGEE-0.3.6/xgee/core/plugins/eoq2/domain/
--rw-r--r--   0 root         (0) root         (0)      983 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq2/domain/domain.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.607614 XGEE-0.3.6/xgee/core/plugins/eoq2/domain/remote/
--rw-r--r--   0 root         (0) root         (0)     2267 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq2/domain/remote/httppostdomain.js
--rw-r--r--   0 root         (0) root         (0)     5812 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq2/domain/remote/websocketdomain.js
--rw-r--r--   0 root         (0) root         (0)     4806 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq2/eoq2.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.607614 XGEE-0.3.6/xgee/core/plugins/eoq2/event/
--rw-r--r--   0 root         (0) root         (0)     3879 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq2/event/event.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.607614 XGEE-0.3.6/xgee/core/plugins/eoq2/frame/
--rw-r--r--   0 root         (0) root         (0)      567 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq2/frame/frame.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.607614 XGEE-0.3.6/xgee/core/plugins/eoq2/legacy/
--rw-r--r--   0 root         (0) root         (0)    14240 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq2/legacy/legacy.js
--rw-r--r--   0 root         (0) root         (0)      440 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq2/package.json
--rw-r--r--   0 root         (0) root         (0)     2472 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq2/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.608614 XGEE-0.3.6/xgee/core/plugins/eoq2/query/
--rw-r--r--   0 root         (0) root         (0)    14393 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq2/query/query.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.608614 XGEE-0.3.6/xgee/core/plugins/eoq2/serialization/
--rw-r--r--   0 root         (0) root         (0)     1107 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq2/serialization/jsonserializer.js
--rw-r--r--   0 root         (0) root         (0)      725 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq2/serialization/serializer.js
--rw-r--r--   0 root         (0) root         (0)    40363 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq2/serialization/textserializer.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.609614 XGEE-0.3.6/xgee/core/plugins/eoq2/util/
--rw-r--r--   0 root         (0) root         (0)     2823 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/core/plugins/eoq2/util/logger.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.610614 XGEE-0.3.6/xgee/core/plugins/eventBroker/
--rw-r--r--   0 root         (0) root         (0)      506 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/eventBroker/BasicEvent.js
--rw-r--r--   0 root         (0) root         (0)      506 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/eventBroker/QueryDebugEvent.js
--rw-r--r--   0 root         (0) root         (0)      694 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/eventBroker/SelectionChangedEvent.js
--rw-r--r--   0 root         (0) root         (0)     3823 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/eventBroker/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.610614 XGEE-0.3.6/xgee/core/plugins/iconProvider/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.610614 XGEE-0.3.6/xgee/core/plugins/iconProvider/js/
--rw-r--r--   0 root         (0) root         (0)      387 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/iconProvider/js/IconProvider.js
--rw-r--r--   0 root         (0) root         (0)     2394 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/iconProvider/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.610614 XGEE-0.3.6/xgee/core/plugins/keyHandler/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.611614 XGEE-0.3.6/xgee/core/plugins/keyHandler/js/
--rw-r--r--   0 root         (0) root         (0)     1493 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/keyHandler/js/KeyHandler.js
--rw-r--r--   0 root         (0) root         (0)      391 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/keyHandler/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.611614 XGEE-0.3.6/xgee/core/plugins/keyHandler.ecore/
--rw-r--r--   0 root         (0) root         (0)      720 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/keyHandler.ecore/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.611614 XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.613614 XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.615614 XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/
--rw-r--r--   0 root         (0) root         (0)     3528 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.eot
--rw-r--r--   0 root         (0) root         (0)     3320 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.ttf
--rw-r--r--   0 root         (0) root         (0)     2180 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.woff
--rw-r--r--   0 root         (0) root         (0)     1680 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.woff2
--rw-r--r--   0 root         (0) root         (0)     7278 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.css
--rw-r--r--   0 root         (0) root         (0)    91213 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.js
--rw-r--r--   0 root         (0) root         (0)     5991 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.css
--rw-r--r--   0 root         (0) root         (0)    14532 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.css.map
--rw-r--r--   0 root         (0) root         (0)    27807 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.js
--rw-r--r--   0 root         (0) root         (0)   131140 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.js.map
--rw-r--r--   0 root         (0) root         (0)    22405 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.ui.position.js
--rw-r--r--   0 root         (0) root         (0)     5855 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.ui.position.min.js
--rw-r--r--   0 root         (0) root         (0)      669 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.615614 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.624614 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/
--rw-r--r--   0 root         (0) root         (0)      554 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EAnnotation.gif
--rw-r--r--   0 root         (0) root         (0)      123 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EAttribute.gif
--rw-r--r--   0 root         (0) root         (0)      206 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EClass.gif
--rw-r--r--   0 root         (0) root         (0)      199 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EDataType.gif
--rw-r--r--   0 root         (0) root         (0)      131 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EEnum.gif
--rw-r--r--   0 root         (0) root         (0)      109 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EEnumLiteral.gif
--rw-r--r--   0 root         (0) root         (0)      211 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EFactory.gif
--rw-r--r--   0 root         (0) root         (0)      102 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericElementType.gif
--rw-r--r--   0 root         (0) root         (0)      108 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericException.gif
--rw-r--r--   0 root         (0) root         (0)      139 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericSuperType.gif
--rw-r--r--   0 root         (0) root         (0)       99 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericType.gif
--rw-r--r--   0 root         (0) root         (0)      139 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericTypeArgument.gif
--rw-r--r--   0 root         (0) root         (0)      111 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericWildcard.gif
--rw-r--r--   0 root         (0) root         (0)      323 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EObject.gif
--rw-r--r--   0 root         (0) root         (0)       62 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceN.gif
--rw-r--r--   0 root         (0) root         (0)       71 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceNToM.gif
--rw-r--r--   0 root         (0) root         (0)       81 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceNToUnbounded.gif
--rw-r--r--   0 root         (0) root         (0)      131 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceNToUnspecified.gif
--rw-r--r--   0 root         (0) root         (0)       58 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceOne.gif
--rw-r--r--   0 root         (0) root         (0)       68 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceOneToN.gif
--rw-r--r--   0 root         (0) root         (0)       79 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceOneToUnbounded.gif
--rw-r--r--   0 root         (0) root         (0)      128 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceOneToUnspecified.gif
--rw-r--r--   0 root         (0) root         (0)       70 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceZero.gif
--rw-r--r--   0 root         (0) root         (0)       78 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceZeroToN.gif
--rw-r--r--   0 root         (0) root         (0)       77 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceZeroToOne.gif
--rw-r--r--   0 root         (0) root         (0)       83 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceZeroToUnbounded.gif
--rw-r--r--   0 root         (0) root         (0)      133 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceZeroToUnspecified.gif
--rw-r--r--   0 root         (0) root         (0)      141 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOperation.gif
--rw-r--r--   0 root         (0) root         (0)      207 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EPackage.gif
--rw-r--r--   0 root         (0) root         (0)      911 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EParameter.gif
--rw-r--r--   0 root         (0) root         (0)      183 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EReference.gif
--rw-r--r--   0 root         (0) root         (0)      213 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EStringToStringMapEntry.gif
--rw-r--r--   0 root         (0) root         (0)      211 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/ETypeParameter.gif
--rw-r--r--   0 root         (0) root         (0)      554 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eAnnotations.gif
--rw-r--r--   0 root         (0) root         (0)      206 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eClassifiers.gif
--rw-r--r--   0 root         (0) root         (0)      141 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eOperations.gif
--rw-r--r--   0 root         (0) root         (0)      207 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eSubpackages.gif
--rw-r--r--   0 root         (0) root         (0)      211 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eTypeParameters.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.624614 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/js/
--rw-r--r--   0 root         (0) root         (0)      577 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/js/TreeViewContextMenuProvider.js
--rw-r--r--   0 root         (0) root         (0)    29729 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.615614 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView.eoq/
--rw-r--r--   0 root         (0) root         (0)    16933 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView.eoq/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.625614 XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/
--rw-r--r--   0 root         (0) root         (0)     1078 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   128443 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/jquery.fancytree-all-deps.min.js
--rw-r--r--   0 root         (0) root         (0)   162267 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/jquery.fancytree-all-deps.min.js.map
--rw-r--r--   0 root         (0) root         (0)      562 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.627614 XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/skin-win8/
--rw-r--r--   0 root         (0) root         (0)     5513 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/skin-win8/icons-rtl.gif
--rw-r--r--   0 root         (0) root         (0)     5510 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/skin-win8/icons.gif
--rw-r--r--   0 root         (0) root         (0)     3234 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/skin-win8/loading.gif
--rw-r--r--   0 root         (0) root         (0)    24749 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/skin-win8/ui.fancytree.css
--rw-r--r--   0 root         (0) root         (0)     4818 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/skin-win8/ui.fancytree.less
--rw-r--r--   0 root         (0) root         (0)      852 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/skin-win8/vline-rtl.gif
--rw-r--r--   0 root         (0) root         (0)      852 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/skin-win8/vline.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.627614 XGEE-0.3.6/xgee/core/plugins/propertiesView/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.632614 XGEE-0.3.6/xgee/core/plugins/propertiesView/css/
--rw-r--r--   0 root         (0) root         (0)      961 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView/css/PropertiesView.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.632614 XGEE-0.3.6/xgee/core/plugins/propertiesView/doc/
--rw-r--r--   0 root         (0) root         (0)    38735 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView/doc/PropertiesView.pptx
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.633614 XGEE-0.3.6/xgee/core/plugins/propertiesView/js/
--rw-r--r--   0 root         (0) root         (0)     1641 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView/js/LoadOnDemandView.js
--rw-r--r--   0 root         (0) root         (0)      298 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView/js/PropertiesBubble.js
--rw-r--r--   0 root         (0) root         (0)      779 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView/js/PropertiesPaneProvider.js
--rw-r--r--   0 root         (0) root         (0)     7532 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView/js/PropertiesViewController.js
--rw-r--r--   0 root         (0) root         (0)     1795 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.627614 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.631614 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore/js/
--rw-r--r--   0 root         (0) root         (0)    10124 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore/js/EObjectPropertiesPane.js
--rw-r--r--   0 root         (0) root         (0)     1682 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore/js/EObjectPropertiesPaneProvider.js
--rw-r--r--   0 root         (0) root         (0)     1173 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.628614 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.custom/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.628614 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.custom/js/
--rw-r--r--   0 root         (0) root         (0)     7014 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPane.js
--rw-r--r--   0 root         (0) root         (0)     1163 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPaneConfig.js
--rw-r--r--   0 root         (0) root         (0)     2739 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPaneProvider.js
--rw-r--r--   0 root         (0) root         (0)      878 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.custom/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.629614 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.editors/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.629614 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.editors/css/
--rw-r--r--   0 root         (0) root         (0)      458 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.editors/css/EcoreEditorsPropertiesPane.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.629614 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.editors/js/
--rw-r--r--   0 root         (0) root         (0)     1565 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.editors/js/EcoreEditorsPropertiesPane.js
--rw-r--r--   0 root         (0) root         (0)     2170 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.editors/js/EcoreEditorsPropertiesPaneProvider.js
--rw-r--r--   0 root         (0) root         (0)     1297 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.editors/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.630614 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.modify/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.630614 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.modify/css/
--rw-r--r--   0 root         (0) root         (0)      458 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.modify/css/EcoreModifyPropertiesPane.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.630614 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.modify/js/
--rw-r--r--   0 root         (0) root         (0)     2571 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.modify/js/EcoreModifyPropertiesPane.js
--rw-r--r--   0 root         (0) root         (0)     2157 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.modify/js/EcoreModifyPropertiesPaneProvider.js
--rw-r--r--   0 root         (0) root         (0)     1287 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.modify/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.630614 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.workspace/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.631614 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.workspace/js/
--rw-r--r--   0 root         (0) root         (0)     1281 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.workspace/js/WorkspacePropertiesPaneConfig.js
--rw-r--r--   0 root         (0) root         (0)     1263 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.workspace/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.631614 XGEE-0.3.6/xgee/core/plugins/propertiesView.info/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.632614 XGEE-0.3.6/xgee/core/plugins/propertiesView.info/js/
--rw-r--r--   0 root         (0) root         (0)     3609 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView.info/js/InfoPropertiesPaneProvider.js
--rw-r--r--   0 root         (0) root         (0)      984 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/propertiesView.info/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.633614 XGEE-0.3.6/xgee/core/plugins/tool.goToView/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.634614 XGEE-0.3.6/xgee/core/plugins/tool.goToView/css/
--rw-r--r--   0 root         (0) root         (0)      126 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/tool.goToView/css/GoToViewTool.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.634614 XGEE-0.3.6/xgee/core/plugins/tool.goToView/img/
--rw-r--r--   0 root         (0) root         (0)     2842 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/tool.goToView/img/tool-go-to-view.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.634614 XGEE-0.3.6/xgee/core/plugins/tool.goToView/js/
--rw-r--r--   0 root         (0) root         (0)     2805 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/tool.goToView/js/GoToViewTool.js
--rw-r--r--   0 root         (0) root         (0)     1018 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/tool.goToView/js/GoToViewToolProvider.js
--rw-r--r--   0 root         (0) root         (0)     1262 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/tool.goToView/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.635614 XGEE-0.3.6/xgee/core/plugins/tool.notes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.635614 XGEE-0.3.6/xgee/core/plugins/tool.notes/css/
--rw-r--r--   0 root         (0) root         (0)     4415 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/tool.notes/css/NotesTool.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.636614 XGEE-0.3.6/xgee/core/plugins/tool.notes/img/
--rw-r--r--   0 root         (0) root         (0)     3331 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/tool.notes/img/notes-error.svg
--rw-r--r--   0 root         (0) root         (0)     2197 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/tool.notes/img/notes-info.svg
--rw-r--r--   0 root         (0) root         (0)     2085 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/tool.notes/img/notes-success.svg
--rw-r--r--   0 root         (0) root         (0)     3188 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/tool.notes/img/notes-warning.svg
--rw-r--r--   0 root         (0) root         (0)     2173 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/tool.notes/img/tool-notes.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.637614 XGEE-0.3.6/xgee/core/plugins/tool.notes/js/
--rw-r--r--   0 root         (0) root         (0)     6924 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/tool.notes/js/NotesTool.js
--rw-r--r--   0 root         (0) root         (0)      940 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/tool.notes/js/NotesToolProvider.js
--rw-r--r--   0 root         (0) root         (0)     1076 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/tool.notes/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.637614 XGEE-0.3.6/xgee/core/plugins/tools/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.637614 XGEE-0.3.6/xgee/core/plugins/tools/js/
--rw-r--r--   0 root         (0) root         (0)      364 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/tools/js/ToolProvider.js
--rw-r--r--   0 root         (0) root         (0)     1409 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/tools/js/ToolsController.js
--rw-r--r--   0 root         (0) root         (0)     1268 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/tools/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.637614 XGEE-0.3.6/xgee/core/plugins/view.dashboard/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.641614 XGEE-0.3.6/xgee/core/plugins/view.dashboard/css/
--rw-r--r--   0 root         (0) root         (0)      149 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/view.dashboard/css/DashboardView.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.641614 XGEE-0.3.6/xgee/core/plugins/view.dashboard/img/
--rw-r--r--   0 root         (0) root         (0)     2146 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/view.dashboard/img/view-dashboard.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.642614 XGEE-0.3.6/xgee/core/plugins/view.dashboard/js/
--rw-r--r--   0 root         (0) root         (0)      479 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/view.dashboard/js/DashProvider.js
--rw-r--r--   0 root         (0) root         (0)     3522 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/view.dashboard/js/DashboardViewProvider.js
--rw-r--r--   0 root         (0) root         (0)     2285 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/view.dashboard/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.638614 XGEE-0.3.6/xgee/core/plugins/view.dashboard.infoDash/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.638614 XGEE-0.3.6/xgee/core/plugins/view.dashboard.infoDash/js/
--rw-r--r--   0 root         (0) root         (0)     1123 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/view.dashboard.infoDash/js/InfoDashProvider.js
--rw-r--r--   0 root         (0) root         (0)     1659 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/view.dashboard.infoDash/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.638614 XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.638614 XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/css/
--rw-r--r--   0 root         (0) root         (0)     1506 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/css/StartModellingDash.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.640614 XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/img/
--rw-r--r--   0 root         (0) root         (0)     3787 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/img/delete.svg
--rw-r--r--   0 root         (0) root         (0)     2220 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/img/edit.svg
--rw-r--r--   0 root         (0) root         (0)     2936 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/img/new-object.svg
--rw-r--r--   0 root         (0) root         (0)     3277 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/img/new-subdir.svg
--rw-r--r--   0 root         (0) root         (0)     2181 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/img/object.svg
--rw-r--r--   0 root         (0) root         (0)     2403 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/img/parent.svg
--rw-r--r--   0 root         (0) root         (0)     2522 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/img/subdir.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.641614 XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/js/
--rw-r--r--   0 root         (0) root         (0)    24067 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDash.js
--rw-r--r--   0 root         (0) root         (0)     5322 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDashListEntry.js
--rw-r--r--   0 root         (0) root         (0)     2123 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDashProvider.js
--rw-r--r--   0 root         (0) root         (0)     2212 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.642614 XGEE-0.3.6/xgee/core/plugins/view.workspace/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.642614 XGEE-0.3.6/xgee/core/plugins/view.workspace/css/
--rw-r--r--   0 root         (0) root         (0)      176 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/view.workspace/css/WorkspaceView.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.642614 XGEE-0.3.6/xgee/core/plugins/view.workspace/img/
--rw-r--r--   0 root         (0) root         (0)     2511 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/view.workspace/img/view-workspace.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.643614 XGEE-0.3.6/xgee/core/plugins/view.workspace/js/
--rw-r--r--   0 root         (0) root         (0)     2417 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/view.workspace/js/WorkspaceViewProvider.js
--rw-r--r--   0 root         (0) root         (0)     1766 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/view.workspace/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.643614 XGEE-0.3.6/xgee/core/plugins/views/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.643614 XGEE-0.3.6/xgee/core/plugins/views/js/
--rw-r--r--   0 root         (0) root         (0)      435 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/views/js/ViewProvider.js
--rw-r--r--   0 root         (0) root         (0)     1886 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/views/js/ViewsController.js
--rw-r--r--   0 root         (0) root         (0)     1423 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/views/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.644614 XGEE-0.3.6/xgee/core/plugins/viewsMenu/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.644614 XGEE-0.3.6/xgee/core/plugins/viewsMenu/js/
--rw-r--r--   0 root         (0) root         (0)     5303 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/viewsMenu/js/ViewsMenuController.js
--rw-r--r--   0 root         (0) root         (0)     1290 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/viewsMenu/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.644614 XGEE-0.3.6/xgee/core/plugins/viewsTabbar/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.644614 XGEE-0.3.6/xgee/core/plugins/viewsTabbar/css/
--rw-r--r--   0 root         (0) root         (0)      856 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/viewsTabbar/css/ViewsTabbar.css
--rw-r--r--   0 root         (0) root         (0)     1919 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/plugins/viewsTabbar/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.457613 XGEE-0.3.6/xgee/core/res/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.646614 XGEE-0.3.6/xgee/core/res/css/
--rw-r--r--   0 root         (0) root         (0)      329 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/css/UIComponents.canvasSearch.css
--rw-r--r--   0 root         (0) root         (0)     1099 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/css/app.css
--rw-r--r--   0 root         (0) root         (0)      337 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/css/canvas.css
--rw-r--r--   0 root         (0) root         (0)      996 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/css/contextmenu.css
--rw-r--r--   0 root         (0) root         (0)       94 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/css/layout.css
--rw-r--r--   0 root         (0) root         (0)     4230 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/css/notes.css
--rw-r--r--   0 root         (0) root         (0)     1974 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/css/palette.css
--rw-r--r--   0 root         (0) root         (0)     7091 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/css/uiControls.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.649614 XGEE-0.3.6/xgee/core/res/img/
--rw-r--r--   0 root         (0) root         (0)     2989 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/img/edit.svg
--rw-r--r--   0 root         (0) root         (0)     3645 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/img/eye.svg
--rw-r--r--   0 root         (0) root         (0)     5763 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/img/globe.svg
--rw-r--r--   0 root         (0) root         (0)     3577 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/img/graph-view-oaam-allocations.svg
--rw-r--r--   0 root         (0) root         (0)     4433 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/img/graph-view-oaam-functions.svg
--rw-r--r--   0 root         (0) root         (0)     3096 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/img/graph-view-oaam-hardware.svg
--rw-r--r--   0 root         (0) root         (0)     2830 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/img/redo.svg
--rw-r--r--   0 root         (0) root         (0)     3529 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/img/tool-domain-status-down.svg
--rw-r--r--   0 root         (0) root         (0)     3152 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/img/tool-domain-status-error.svg
--rw-r--r--   0 root         (0) root         (0)     4286 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/img/tool-domain-status-up-down.svg
--rw-r--r--   0 root         (0) root         (0)     3535 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/img/tool-domain-status-up.svg
--rw-r--r--   0 root         (0) root         (0)     2803 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/img/tool-domain-status.svg
--rw-r--r--   0 root         (0) root         (0)     3449 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/img/tree.svg
--rw-r--r--   0 root         (0) root         (0)     2788 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/img/undo.svg
--rw-r--r--   0 root         (0) root         (0)     3010 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/img/view-editor.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.650614 XGEE-0.3.6/xgee/core/res/js/
--rw-r--r--   0 root         (0) root         (0)     3240 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/js/DomainStatistics.js
--rw-r--r--   0 root         (0) root         (0)    12997 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/js/app.js
--rw-r--r--   0 root         (0) root         (0)     5020 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/js/commands.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.651615 XGEE-0.3.6/xgee/core/res/js/connectors/
--rw-r--r--   0 root         (0) root         (0)     9049 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/js/connectors/connectors.graph.js
--rw-r--r--   0 root         (0) root         (0)     4190 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/js/connectors/connectors.selection.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.651615 XGEE-0.3.6/xgee/core/res/js/grids/
--rw-r--r--   0 root         (0) root         (0)      415 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/js/grids/points_grid.svg
--rw-r--r--   0 root         (0) root         (0)     3582 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/js/ports.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.651615 XGEE-0.3.6/xgee/core/res/js/ui/
--rw-r--r--   0 root         (0) root         (0)     4761 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/js/ui/DomainStatusTool.js
--rw-r--r--   0 root         (0) root         (0)     1437 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/js/ui/ui.colorProvider.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.652614 XGEE-0.3.6/xgee/core/res/js/workspace/
--rw-r--r--   0 root         (0) root         (0)     3669 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/js/workspace/workspace.jobs.js
--rw-r--r--   0 root         (0) root         (0)    18830 2024-03-19 20:30:28.000000 XGEE-0.3.6/xgee/core/res/js/workspace/workspace.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.652614 XGEE-0.3.6/xgee/eoqserver/
--rw-r--r--   0 root         (0) root         (0)    13048 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/eoqserver/PyEoq2WebServer.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 20:30:30.000000 XGEE-0.3.6/xgee/eoqserver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.653614 XGEE-0.3.6/xgee/eoqserver/eoq1/
--rw-r--r--   0 root         (0) root         (0)      182 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.654615 XGEE-0.3.6/xgee/eoqserver/eoq1/actions/
--rw-r--r--   0 root         (0) root         (0)      119 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq1/actions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2229 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq1/actions/actionutils.py
--rw-r--r--   0 root         (0) root         (0)    29323 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq1/actions/externalactionhandler.py
--rw-r--r--   0 root         (0) root         (0)     9347 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq1/commandparser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.655614 XGEE-0.3.6/xgee/eoqserver/eoq1/domains/
--rw-r--r--   0 root         (0) root         (0)      283 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq1/domains/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72154 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq1/domains/localdomain.py
--rw-r--r--   0 root         (0) root         (0)      979 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq1/domains/multiprocessingqueuedomainclient.py
--rw-r--r--   0 root         (0) root         (0)     1242 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq1/domains/multiprocessingqueuedomainhost.py
--rw-r--r--   0 root         (0) root         (0)     1268 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq1/domains/remotehttpdomain.py
--rw-r--r--   0 root         (0) root         (0)     2495 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq1/domains/simplepythondomainwrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.656614 XGEE-0.3.6/xgee/eoqserver/eoq1/error/
--rw-r--r--   0 root         (0) root         (0)      248 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq1/error/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2361 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq1/error/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.656614 XGEE-0.3.6/xgee/eoqserver/eoq1/model/
--rw-r--r--   0 root         (0) root         (0)     7459 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq1/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64472 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq1/model/model.py
--rw-r--r--   0 root         (0) root         (0)    22749 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq1/queryparser.py
--rw-r--r--   0 root         (0) root         (0)     8387 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq1/resultparser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.657615 XGEE-0.3.6/xgee/eoqserver/eoq1/utils/
--rw-r--r--   0 root         (0) root         (0)       63 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq1/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25693 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq1/utils/csvconnector.py
--rw-r--r--   0 root         (0) root         (0)    10694 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq1/valueparser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.657615 XGEE-0.3.6/xgee/eoqserver/eoq2/
--rw-r--r--   0 root         (0) root         (0)      117 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.658614 XGEE-0.3.6/xgee/eoqserver/eoq2/action/
--rw-r--r--   0 root         (0) root         (0)      142 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/action/__init__.py
--rw-r--r--   0 root         (0) root         (0)      856 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/action/action.py
--rw-r--r--   0 root         (0) root         (0)     2958 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/action/call.py
--rw-r--r--   0 root         (0) root         (0)      754 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/action/callhandler.py
--rw-r--r--   0 root         (0) root         (0)     1030 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/action/callmanager.py
--rw-r--r--   0 root         (0) root         (0)     8117 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/action/cmdrunnerbasedcallmanager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.659614 XGEE-0.3.6/xgee/eoqserver/eoq2/action/externalpy/
--rw-r--r--   0 root         (0) root         (0)       40 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/action/externalpy/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24055 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/action/externalpy/externalpyscripthandler.py
--rw-r--r--   0 root         (0) root         (0)     5080 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/action/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.660615 XGEE-0.3.6/xgee/eoqserver/eoq2/command/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/command/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9319 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/command/command.py
--rw-r--r--   0 root         (0) root         (0)    64224 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/command/commandrunner.py
--rw-r--r--   0 root         (0) root         (0)    43028 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/command/diff.py
--rw-r--r--   0 root         (0) root         (0)      854 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/command/result.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.661615 XGEE-0.3.6/xgee/eoqserver/eoq2/domain/
--rw-r--r--   0 root         (0) root         (0)       60 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/domain/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2055 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/domain/cmdrunnerbaseddomain.py
--rw-r--r--   0 root         (0) root         (0)      698 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/domain/domain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.661615 XGEE-0.3.6/xgee/eoqserver/eoq2/domain/local/
--rw-r--r--   0 root         (0) root         (0)       31 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/domain/local/__init__.py
--rw-r--r--   0 root         (0) root         (0)      699 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/domain/local/localmdbdomain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.662614 XGEE-0.3.6/xgee/eoqserver/eoq2/domain/multiprocessing/
--rw-r--r--   0 root         (0) root         (0)       86 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/domain/multiprocessing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1089 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingcallmanager.py
--rw-r--r--   0 root         (0) root         (0)     2668 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingdomainclient.py
--rw-r--r--   0 root         (0) root         (0)     3535 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingdomainhost.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.663615 XGEE-0.3.6/xgee/eoqserver/eoq2/domain/remote/
--rw-r--r--   0 root         (0) root         (0)       30 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/domain/remote/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6884 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/domain/remote/websocketdomain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.663615 XGEE-0.3.6/xgee/eoqserver/eoq2/event/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/event/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6359 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/event/event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.664615 XGEE-0.3.6/xgee/eoqserver/eoq2/frame/
--rw-r--r--   0 root         (0) root         (0)      127 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/frame/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1670 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/frame/domainframehandler.py
--rw-r--r--   0 root         (0) root         (0)      458 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/frame/frame.py
--rw-r--r--   0 root         (0) root         (0)      746 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/frame/framehandler.py
--rw-r--r--   0 root         (0) root         (0)     2186 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/frame/multiversionframehandler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.665614 XGEE-0.3.6/xgee/eoqserver/eoq2/legacy/
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/legacy/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12199 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/legacy/legacy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.666615 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/
--rw-r--r--   0 root         (0) root         (0)       99 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      471 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/mdb.py
--rw-r--r--   0 root         (0) root         (0)     2670 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/mdbaccessor.py
--rw-r--r--   0 root         (0) root         (0)      266 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/nocodec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.668614 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/
--rw-r--r--   0 root         (0) root         (0)      213 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.669615 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/constraintmodel/
--rw-r--r--   0 root         (0) root         (0)      867 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/constraintmodel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1631 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/constraintmodel/constraintmodel.py
--rw-r--r--   0 root         (0) root         (0)     1697 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/pyecoreidcodec.py
--rw-r--r--   0 root         (0) root         (0)     2389 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/pyecoremdb.py
--rw-r--r--   0 root         (0) root         (0)    36345 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/pyecoremdbaccessor.py
--rw-r--r--   0 root         (0) root         (0)      518 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresimpleobjectcodec.py
--rw-r--r--   0 root         (0) root         (0)     3823 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresinglefilemdb.py
--rw-r--r--   0 root         (0) root         (0)     5811 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresinglefilemdbprovider.py
--rw-r--r--   0 root         (0) root         (0)    80843 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/pyecoreworkspacemdbprovider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.669615 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/workspacemdbmodel/
--rw-r--r--   0 root         (0) root         (0)     1326 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/workspacemdbmodel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5277 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/workspacemdbmodel/workspacemdbmodel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.669615 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/xmlresourcemodel/
--rw-r--r--   0 root         (0) root         (0)     1092 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/xmlresourcemodel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3591 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/xmlresourcemodel/xmlresourcemodel.py
--rw-r--r--   0 root         (0) root         (0)      175 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/valuecodec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.670615 XGEE-0.3.6/xgee/eoqserver/eoq2/query/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/query/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12347 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/query/query.py
--rw-r--r--   0 root         (0) root         (0)    38368 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/query/queryrunner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.671615 XGEE-0.3.6/xgee/eoqserver/eoq2/serialization/
--rw-r--r--   0 root         (0) root         (0)      204 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/serialization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1203 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/serialization/jsonserializer.py
--rw-r--r--   0 root         (0) root         (0)     6755 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/serialization/jsserializer.py
--rw-r--r--   0 root         (0) root         (0)     5871 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/serialization/pyserializer.py
--rw-r--r--   0 root         (0) root         (0)      314 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/serialization/serializer.py
--rw-r--r--   0 root         (0) root         (0)    35630 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/serialization/textserializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.673615 XGEE-0.3.6/xgee/eoqserver/eoq2/util/
--rw-r--r--   0 root         (0) root         (0)      118 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2491 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/util/backup.py
--rw-r--r--   0 root         (0) root         (0)     4033 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/util/benchmark.py
--rw-r--r--   0 root         (0) root         (0)    13851 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/util/csvconnector.py
--rw-r--r--   0 root         (0) root         (0)     1272 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/util/error.py
--rw-r--r--   0 root         (0) root         (0)     4511 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/util/logger.py
--rw-r--r--   0 root         (0) root         (0)     2634 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/util/model.py
--rw-r--r--   0 root         (0) root         (0)     4037 2024-03-19 20:30:31.000000 XGEE-0.3.6/xgee/eoqserver/eoq2/util/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 20:30:32.673615 XGEE-0.3.6/xgee/meta/
--rw-rw-rw-   0 root         (0) root         (0)     7875 2024-03-19 20:30:24.000000 XGEE-0.3.6/xgee/meta/layout.ecore
--rw-rw-rw-   0 root         (0) root         (0)    11552 2024-03-19 20:30:24.000000 XGEE-0.3.6/xgee/xgee.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.761397 XGEE-0.3.7/
+-rw-rw-rw-   0 root         (0) root         (0)     1111 2024-04-23 20:45:08.000000 XGEE-0.3.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3174 2024-04-23 20:45:15.761397 XGEE-0.3.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2398 2024-04-23 20:45:08.000000 XGEE-0.3.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.761397 XGEE-0.3.7/XGEE.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3174 2024-04-23 20:45:15.000000 XGEE-0.3.7/XGEE.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    43053 2024-04-23 20:45:15.000000 XGEE-0.3.7/XGEE.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 20:45:15.000000 XGEE-0.3.7/XGEE.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-04-23 20:45:15.000000 XGEE-0.3.7/XGEE.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2024-04-23 20:45:15.000000 XGEE-0.3.7/XGEE.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-23 20:45:15.000000 XGEE-0.3.7/XGEE.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 20:45:15.761397 XGEE-0.3.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1945 2024-04-23 20:45:08.000000 XGEE-0.3.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.543399 XGEE-0.3.7/xgee/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-23 20:45:08.000000 XGEE-0.3.7/xgee/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2024-04-23 20:45:08.000000 XGEE-0.3.7/xgee/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.544399 XGEE-0.3.7/xgee/core/
+-rw-r--r--   0 root         (0) root         (0)       37 2024-04-23 20:45:10.000000 XGEE-0.3.7/xgee/core/.git
+-rw-r--r--   0 root         (0) root         (0)      362 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/.gitmodules
+-rw-r--r--   0 root         (0) root         (0)     1078 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      581 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.517399 XGEE-0.3.7/xgee/core/dep/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.545399 XGEE-0.3.7/xgee/core/dep/bluebird/
+-rw-r--r--   0 root         (0) root         (0)   183390 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/bluebird/bluebird.js
+-rw-r--r--   0 root         (0) root         (0)    81530 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/bluebird/bluebird.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.545399 XGEE-0.3.7/xgee/core/dep/font-awesome/
+-rw-r--r--   0 root         (0) root         (0)     1548 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.549399 XGEE-0.3.7/xgee/core/dep/font-awesome/css/
+-rw-r--r--   0 root         (0) root         (0)    73117 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/css/all.css
+-rw-r--r--   0 root         (0) root         (0)    58935 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/css/all.min.css
+-rw-r--r--   0 root         (0) root         (0)      732 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/css/brands.css
+-rw-r--r--   0 root         (0) root         (0)      675 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/css/brands.min.css
+-rw-r--r--   0 root         (0) root         (0)    71482 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/css/fontawesome.css
+-rw-r--r--   0 root         (0) root         (0)    57503 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/css/fontawesome.min.css
+-rw-r--r--   0 root         (0) root         (0)      734 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/css/regular.css
+-rw-r--r--   0 root         (0) root         (0)      677 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/css/regular.min.css
+-rw-r--r--   0 root         (0) root         (0)      727 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/css/solid.css
+-rw-r--r--   0 root         (0) root         (0)      669 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/css/solid.min.css
+-rw-r--r--   0 root         (0) root         (0)     8077 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/css/svg-with-js.css
+-rw-r--r--   0 root         (0) root         (0)     6359 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/css/svg-with-js.min.css
+-rw-r--r--   0 root         (0) root         (0)    41312 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/css/v4-shims.css
+-rw-r--r--   0 root         (0) root         (0)    26702 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/css/v4-shims.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.556398 XGEE-0.3.7/xgee/core/dep/font-awesome/js/
+-rw-r--r--   0 root         (0) root         (0)  1248390 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/js/all.js
+-rw-r--r--   0 root         (0) root         (0)  1182553 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/js/all.min.js
+-rw-r--r--   0 root         (0) root         (0)   445294 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/js/brands.js
+-rw-r--r--   0 root         (0) root         (0)   438090 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/js/brands.min.js
+-rw-r--r--   0 root         (0) root         (0)    33929 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/js/conflict-detection.js
+-rw-r--r--   0 root         (0) root         (0)    13502 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/js/conflict-detection.min.js
+-rw-r--r--   0 root         (0) root         (0)    79139 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/js/fontawesome.js
+-rw-r--r--   0 root         (0) root         (0)    37191 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/js/fontawesome.min.js
+-rw-r--r--   0 root         (0) root         (0)   107110 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/js/regular.js
+-rw-r--r--   0 root         (0) root         (0)   103386 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/js/regular.min.js
+-rw-r--r--   0 root         (0) root         (0)   617405 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/js/solid.js
+-rw-r--r--   0 root         (0) root         (0)   604447 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/js/solid.min.js
+-rw-r--r--   0 root         (0) root         (0)    17459 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/js/v4-shims.js
+-rw-r--r--   0 root         (0) root         (0)    15055 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/js/v4-shims.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.562399 XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/
+-rw-r--r--   0 root         (0) root         (0)   134878 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-brands-400.eot
+-rw-r--r--   0 root         (0) root         (0)   729325 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-brands-400.svg
+-rw-r--r--   0 root         (0) root         (0)   134572 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 root         (0) root         (0)    90872 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-brands-400.woff
+-rw-r--r--   0 root         (0) root         (0)    77444 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 root         (0) root         (0)    34390 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-regular-400.eot
+-rw-r--r--   0 root         (0) root         (0)   144322 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-regular-400.svg
+-rw-r--r--   0 root         (0) root         (0)    34092 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 root         (0) root         (0)    16800 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-regular-400.woff
+-rw-r--r--   0 root         (0) root         (0)    13596 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 root         (0) root         (0)   204866 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-solid-900.eot
+-rw-r--r--   0 root         (0) root         (0)   910710 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-solid-900.svg
+-rw-r--r--   0 root         (0) root         (0)   204580 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 root         (0) root         (0)   104252 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-solid-900.woff
+-rw-r--r--   0 root         (0) root         (0)    80328 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.565399 XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.566398 XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/font/
+-rw-r--r--   0 root         (0) root         (0)     3528 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.eot
+-rw-r--r--   0 root         (0) root         (0)     3320 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.ttf
+-rw-r--r--   0 root         (0) root         (0)     2180 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.woff
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.woff2
+-rw-r--r--   0 root         (0) root         (0)     7278 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.css
+-rw-r--r--   0 root         (0) root         (0)    91213 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.js
+-rw-r--r--   0 root         (0) root         (0)     5991 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.css
+-rw-r--r--   0 root         (0) root         (0)    14532 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.css.map
+-rw-r--r--   0 root         (0) root         (0)    27807 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.js
+-rw-r--r--   0 root         (0) root         (0)   131140 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.js.map
+-rw-r--r--   0 root         (0) root         (0)    22405 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/jquery.ui.position.js
+-rw-r--r--   0 root         (0) root         (0)     5855 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/jquery.ui.position.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.566398 XGEE-0.3.7/xgee/core/dep/jquery/
+-rw-r--r--   0 root         (0) root         (0)     1097 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jquery/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    86927 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jquery/jquery-3.3.1.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.567398 XGEE-0.3.7/xgee/core/dep/jquery-ui/
+-rw-r--r--   0 root         (0) root         (0)     1817 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jquery-ui/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.569398 XGEE-0.3.7/xgee/core/dep/jquery-ui/images/
+-rw-r--r--   0 root         (0) root         (0)     7006 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jquery-ui/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 root         (0) root         (0)     7074 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jquery-ui/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 root         (0) root         (0)     4676 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jquery-ui/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 root         (0) root         (0)     7013 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jquery-ui/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 root         (0) root         (0)     4632 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jquery-ui/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 root         (0) root         (0)     6313 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jquery-ui/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 root         (0) root         (0)    32076 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jquery-ui/jquery-ui.min.css
+-rw-r--r--   0 root         (0) root         (0)   253669 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jquery-ui/jquery-ui.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.571398 XGEE-0.3.7/xgee/core/dep/jsa/
+-rw-r--r--   0 root         (0) root         (0)       55 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/jsa/.git
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     2327 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1137 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1291 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.574398 XGEE-0.3.7/xgee/core/dep/jsa/img/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.577398 XGEE-0.3.7/xgee/core/dep/jsa/img/black/
+-rw-r--r--   0 root         (0) root         (0)     2092 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/black/bubble-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2083 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/black/bubble.svg
+-rw-r--r--   0 root         (0) root         (0)     2214 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/black/close-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2196 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/black/close.svg
+-rw-r--r--   0 root         (0) root         (0)     2097 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/black/folder.svg
+-rw-r--r--   0 root         (0) root         (0)     2072 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/black/home.svg
+-rw-r--r--   0 root         (0) root         (0)    12585 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/black/jsa.svg
+-rw-r--r--   0 root         (0) root         (0)     2201 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/black/maximize-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2192 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/black/maximize.svg
+-rw-r--r--   0 root         (0) root         (0)     2880 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/black/menu-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2862 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/black/menu.svg
+-rw-r--r--   0 root         (0) root         (0)     2075 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/black/minimize-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2066 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/black/minimize.svg
+-rw-r--r--   0 root         (0) root         (0)     2326 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/black/redo.svg
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/black/settings.svg
+-rw-r--r--   0 root         (0) root         (0)     2378 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/black/undo.svg
+-rw-r--r--   0 root         (0) root         (0)     2343 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/black/view-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2334 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/black/view.svg
+-rw-r--r--   0 root         (0) root         (0)     3032 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/close-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     3032 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/close.svg
+-rw-r--r--   0 root         (0) root         (0)    12585 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/jsa.svg
+-rw-r--r--   0 root         (0) root         (0)     3731 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/loading.svg
+-rw-r--r--   0 root         (0) root         (0)     2443 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/maximize.svg
+-rw-r--r--   0 root         (0) root         (0)     2437 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/minimize.svg
+-rw-r--r--   0 root         (0) root         (0)     3173 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/resize-ne.svg
+-rw-r--r--   0 root         (0) root         (0)     3172 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/resize-nw.svg
+-rw-r--r--   0 root         (0) root         (0)     3173 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/resize-se.svg
+-rw-r--r--   0 root         (0) root         (0)     3113 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/resize-sw.svg
+-rw-r--r--   0 root         (0) root         (0)     3639 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/restore.svg
+-rw-r--r--   0 root         (0) root         (0)     2637 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/tool-default.svg
+-rw-r--r--   0 root         (0) root         (0)     2693 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/view-close.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.581398 XGEE-0.3.7/xgee/core/dep/jsa/img/white/
+-rw-r--r--   0 root         (0) root         (0)     2083 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/white/bubble-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2074 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/white/bubble.svg
+-rw-r--r--   0 root         (0) root         (0)     2205 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/white/close-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2196 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/white/close.svg
+-rw-r--r--   0 root         (0) root         (0)     2097 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/white/folder.svg
+-rw-r--r--   0 root         (0) root         (0)     2063 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/white/home.svg
+-rw-r--r--   0 root         (0) root         (0)    12585 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/white/jsa.svg
+-rw-r--r--   0 root         (0) root         (0)     2192 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/white/maximize-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2183 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/white/maximize.svg
+-rw-r--r--   0 root         (0) root         (0)     2871 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/white/menu-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2853 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/white/menu.svg
+-rw-r--r--   0 root         (0) root         (0)     2066 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/white/minimize-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2057 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/white/minimize.svg
+-rw-r--r--   0 root         (0) root         (0)     2317 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/white/redo.svg
+-rw-r--r--   0 root         (0) root         (0)     2365 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/white/settings.svg
+-rw-r--r--   0 root         (0) root         (0)     2369 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/white/undo.svg
+-rw-r--r--   0 root         (0) root         (0)     2334 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/white/view-hover.svg
+-rw-r--r--   0 root         (0) root         (0)     2325 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/img/white/view.svg
+-rw-r--r--   0 root         (0) root         (0)    46194 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/jsapplication.css
+-rw-r--r--   0 root         (0) root         (0)   357922 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/jsapplication.js
+-rw-r--r--   0 root         (0) root         (0)    15308 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/jsapplicationPlugins.js
+-rw-r--r--   0 root         (0) root         (0)      402 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/package.json
+-rw-r--r--   0 root         (0) root         (0)     1252 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/dep/jsa/webpack.config.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.582398 XGEE-0.3.7/xgee/core/dep/mxgraph/
+-rw-r--r--   0 root         (0) root         (0)    10487 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.582398 XGEE-0.3.7/xgee/core/dep/mxgraph/css/
+-rw-r--r--   0 root         (0) root         (0)     4325 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/css/common.css
+-rw-r--r--   0 root         (0) root         (0)      486 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/css/explorer.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.586398 XGEE-0.3.7/xgee/core/dep/mxgraph/images/
+-rw-r--r--   0 root         (0) root         (0)      137 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/images/button.gif
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/images/close.gif
+-rw-r--r--   0 root         (0) root         (0)      877 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/images/collapsed.gif
+-rw-r--r--   0 root         (0) root         (0)      907 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/images/error.gif
+-rw-r--r--   0 root         (0) root         (0)      878 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/images/expanded.gif
+-rw-r--r--   0 root         (0) root         (0)      843 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/images/maximize.gif
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/images/minimize.gif
+-rw-r--r--   0 root         (0) root         (0)      845 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/images/normalize.gif
+-rw-r--r--   0 root         (0) root         (0)       55 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/images/point.gif
+-rw-r--r--   0 root         (0) root         (0)       74 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/images/resize.gif
+-rw-r--r--   0 root         (0) root         (0)      146 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/images/separator.gif
+-rw-r--r--   0 root         (0) root         (0)       56 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/images/submenu.gif
+-rw-r--r--   0 root         (0) root         (0)       90 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/images/transparent.gif
+-rw-r--r--   0 root         (0) root         (0)      276 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/images/warning.gif
+-rw-r--r--   0 root         (0) root         (0)      425 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/images/warning.png
+-rw-r--r--   0 root         (0) root         (0)      275 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/images/window-title.gif
+-rw-r--r--   0 root         (0) root         (0)       75 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/images/window.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.587398 XGEE-0.3.7/xgee/core/dep/mxgraph/js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.588398 XGEE-0.3.7/xgee/core/dep/mxgraph/js/editor/
+-rw-r--r--   0 root         (0) root         (0)     3232 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/editor/mxDefaultKeyHandler.js
+-rw-r--r--   0 root         (0) root         (0)     9716 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/editor/mxDefaultPopupMenu.js
+-rw-r--r--   0 root         (0) root         (0)    14610 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/editor/mxDefaultToolbar.js
+-rw-r--r--   0 root         (0) root         (0)    74993 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/editor/mxEditor.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.593398 XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/
+-rw-r--r--   0 root         (0) root         (0)     7282 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxCellHighlight.js
+-rw-r--r--   0 root         (0) root         (0)     9337 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxCellMarker.js
+-rw-r--r--   0 root         (0) root         (0)     2992 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxCellTracker.js
+-rw-r--r--   0 root         (0) root         (0)    62381 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxConnectionHandler.js
+-rw-r--r--   0 root         (0) root         (0)    13695 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxConstraintHandler.js
+-rw-r--r--   0 root         (0) root         (0)    63081 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxEdgeHandler.js
+-rw-r--r--   0 root         (0) root         (0)     9925 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxEdgeSegmentHandler.js
+-rw-r--r--   0 root         (0) root         (0)     5944 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxElbowEdgeHandler.js
+-rw-r--r--   0 root         (0) root         (0)    39448 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxGraphHandler.js
+-rw-r--r--   0 root         (0) root         (0)     7701 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxHandle.js
+-rw-r--r--   0 root         (0) root         (0)    10128 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxKeyHandler.js
+-rw-r--r--   0 root         (0) root         (0)    11402 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxPanningHandler.js
+-rw-r--r--   0 root         (0) root         (0)     5293 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxPopupMenuHandler.js
+-rw-r--r--   0 root         (0) root         (0)     9837 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxRubberband.js
+-rw-r--r--   0 root         (0) root         (0)     6478 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxSelectionCellsHandler.js
+-rw-r--r--   0 root         (0) root         (0)     7419 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxTooltipHandler.js
+-rw-r--r--   0 root         (0) root         (0)    52962 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxVertexHandler.js
+-rw-r--r--   0 root         (0) root         (0)    12044 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/index.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.596398 XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/
+-rw-r--r--   0 root         (0) root         (0)     4531 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxCellCodec.js
+-rw-r--r--   0 root         (0) root         (0)     4207 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxChildChangeCodec.js
+-rw-r--r--   0 root         (0) root         (0)    13541 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxCodec.js
+-rw-r--r--   0 root         (0) root         (0)     2690 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxCodecRegistry.js
+-rw-r--r--   0 root         (0) root         (0)     1986 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxDefaultKeyHandlerCodec.js
+-rw-r--r--   0 root         (0) root         (0)     1226 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxDefaultPopupMenuCodec.js
+-rw-r--r--   0 root         (0) root         (0)     9221 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxDefaultToolbarCodec.js
+-rw-r--r--   0 root         (0) root         (0)     6163 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxEditorCodec.js
+-rw-r--r--   0 root         (0) root         (0)     1798 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxGenericChangeCodec.js
+-rw-r--r--   0 root         (0) root         (0)      621 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxGraphCodec.js
+-rw-r--r--   0 root         (0) root         (0)     5022 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxGraphViewCodec.js
+-rw-r--r--   0 root         (0) root         (0)     1705 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxModelCodec.js
+-rw-r--r--   0 root         (0) root         (0)    30213 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxObjectCodec.js
+-rw-r--r--   0 root         (0) root         (0)     1598 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxRootChangeCodec.js
+-rw-r--r--   0 root         (0) root         (0)     4651 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxStylesheetCodec.js
+-rw-r--r--   0 root         (0) root         (0)      818 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxTerminalChangeCodec.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.598398 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.599398 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.600398 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/model/
+-rw-r--r--   0 root         (0) root         (0)     4029 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphAbstractHierarchyCell.js
+-rw-r--r--   0 root         (0) root         (0)     3852 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyEdge.js
+-rw-r--r--   0 root         (0) root         (0)    20322 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyModel.js
+-rw-r--r--   0 root         (0) root         (0)     4915 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyNode.js
+-rw-r--r--   0 root         (0) root         (0)    23605 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxSwimlaneModel.js
+-rw-r--r--   0 root         (0) root         (0)    20146 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/mxHierarchicalLayout.js
+-rw-r--r--   0 root         (0) root         (0)    22708 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/mxSwimlaneLayout.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.601398 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/
+-rw-r--r--   0 root         (0) root         (0)    43070 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxCoordinateAssignment.js
+-rw-r--r--   0 root         (0) root         (0)      726 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxHierarchicalLayoutStage.js
+-rw-r--r--   0 root         (0) root         (0)    16867 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxMedianHybridCrossingReduction.js
+-rw-r--r--   0 root         (0) root         (0)     3123 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxMinimumCycleRemover.js
+-rw-r--r--   0 root         (0) root         (0)     2816 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxSwimlaneOrdering.js
+-rw-r--r--   0 root         (0) root         (0)     4343 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/mxCircleLayout.js
+-rw-r--r--   0 root         (0) root         (0)    22959 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/mxCompactTreeLayout.js
+-rw-r--r--   0 root         (0) root         (0)     2496 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/mxCompositeLayout.js
+-rw-r--r--   0 root         (0) root         (0)     3158 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/mxEdgeLabelLayout.js
+-rw-r--r--   0 root         (0) root         (0)    14338 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/mxFastOrganicLayout.js
+-rw-r--r--   0 root         (0) root         (0)    14251 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/mxGraphLayout.js
+-rw-r--r--   0 root         (0) root         (0)     4851 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/mxParallelEdgeLayout.js
+-rw-r--r--   0 root         (0) root         (0)     5537 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/mxPartitionLayout.js
+-rw-r--r--   0 root         (0) root         (0)     8037 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/mxRadialTreeLayout.js
+-rw-r--r--   0 root         (0) root         (0)    12740 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/mxStackLayout.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.602398 XGEE-0.3.7/xgee/core/dep/mxgraph/js/model/
+-rw-r--r--   0 root         (0) root         (0)    15954 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/model/mxCell.js
+-rw-r--r--   0 root         (0) root         (0)     2933 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/model/mxCellPath.js
+-rw-r--r--   0 root         (0) root         (0)    12721 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/model/mxGeometry.js
+-rw-r--r--   0 root         (0) root         (0)    62665 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/model/mxGraphModel.js
+-rw-r--r--   0 root         (0) root         (0)    28988 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/mxClient.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.607398 XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/
+-rw-r--r--   0 root         (0) root         (0)     2117 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxActor.js
+-rw-r--r--   0 root         (0) root         (0)     3316 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxArrow.js
+-rw-r--r--   0 root         (0) root         (0)    11601 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxArrowConnector.js
+-rw-r--r--   0 root         (0) root         (0)     1506 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxCloud.js
+-rw-r--r--   0 root         (0) root         (0)     4196 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxConnector.js
+-rw-r--r--   0 root         (0) root         (0)     2694 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxCylinder.js
+-rw-r--r--   0 root         (0) root         (0)     2823 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxDoubleEllipse.js
+-rw-r--r--   0 root         (0) root         (0)     1159 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxEllipse.js
+-rw-r--r--   0 root         (0) root         (0)      802 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxHexagon.js
+-rw-r--r--   0 root         (0) root         (0)     6341 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxImageShape.js
+-rw-r--r--   0 root         (0) root         (0)     6800 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxLabel.js
+-rw-r--r--   0 root         (0) root         (0)     1139 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxLine.js
+-rw-r--r--   0 root         (0) root         (0)     5400 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxMarker.js
+-rw-r--r--   0 root         (0) root         (0)     2485 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxPolyline.js
+-rw-r--r--   0 root         (0) root         (0)     3068 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxRectangleShape.js
+-rw-r--r--   0 root         (0) root         (0)     1597 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxRhombus.js
+-rw-r--r--   0 root         (0) root         (0)    38952 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxShape.js
+-rw-r--r--   0 root         (0) root         (0)    26031 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxStencil.js
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxStencilRegistry.js
+-rw-r--r--   0 root         (0) root         (0)     9507 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxSwimlane.js
+-rw-r--r--   0 root         (0) root         (0)    37084 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxText.js
+-rw-r--r--   0 root         (0) root         (0)      828 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxTriangle.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.617398 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/
+-rw-r--r--   0 root         (0) root         (0)    11723 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxAbstractCanvas2D.js
+-rw-r--r--   0 root         (0) root         (0)     1895 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxAnimation.js
+-rw-r--r--   0 root         (0) root         (0)     4430 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxAutoSaveManager.js
+-rw-r--r--   0 root         (0) root         (0)     5354 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxClipboard.js
+-rw-r--r--   0 root         (0) root         (0)    63826 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxConstants.js
+-rw-r--r--   0 root         (0) root         (0)     2236 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxDictionary.js
+-rw-r--r--   0 root         (0) root         (0)     3205 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxDivResizer.js
+-rw-r--r--   0 root         (0) root         (0)    16885 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxDragSource.js
+-rw-r--r--   0 root         (0) root         (0)     4460 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxEffects.js
+-rw-r--r--   0 root         (0) root         (0)    27401 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxEvent.js
+-rw-r--r--   0 root         (0) root         (0)     1941 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxEventObject.js
+-rw-r--r--   0 root         (0) root         (0)     3778 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxEventSource.js
+-rw-r--r--   0 root         (0) root         (0)     4041 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxForm.js
+-rw-r--r--   0 root         (0) root         (0)    10378 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxGuide.js
+-rw-r--r--   0 root         (0) root         (0)      670 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxImage.js
+-rw-r--r--   0 root         (0) root         (0)     3380 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxImageBundle.js
+-rw-r--r--   0 root         (0) root         (0)     3798 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxImageExport.js
+-rw-r--r--   0 root         (0) root         (0)     8228 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxLog.js
+-rw-r--r--   0 root         (0) root         (0)     5691 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxMorphing.js
+-rw-r--r--   0 root         (0) root         (0)     4481 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxMouseEvent.js
+-rw-r--r--   0 root         (0) root         (0)     1485 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxObjectIdentity.js
+-rw-r--r--   0 root         (0) root         (0)     5082 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxPanningManager.js
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxPoint.js
+-rw-r--r--   0 root         (0) root         (0)    14045 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxPopupMenu.js
+-rw-r--r--   0 root         (0) root         (0)     3693 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxRectangle.js
+-rw-r--r--   0 root         (0) root         (0)    11080 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxResources.js
+-rw-r--r--   0 root         (0) root         (0)    45946 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxSvgCanvas2D.js
+-rw-r--r--   0 root         (0) root         (0)    12132 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxToolbar.js
+-rw-r--r--   0 root         (0) root         (0)     5793 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxUndoManager.js
+-rw-r--r--   0 root         (0) root         (0)     4535 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxUndoableEdit.js
+-rw-r--r--   0 root         (0) root         (0)     2768 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxUrlConverter.js
+-rw-r--r--   0 root         (0) root         (0)   106481 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxUtils.js
+-rw-r--r--   0 root         (0) root         (0)    26243 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxVmlCanvas2D.js
+-rw-r--r--   0 root         (0) root         (0)    27971 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxWindow.js
+-rw-r--r--   0 root         (0) root         (0)    28763 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxXmlCanvas2D.js
+-rw-r--r--   0 root         (0) root         (0)    10820 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxXmlRequest.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.623398 XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/
+-rw-r--r--   0 root         (0) root         (0)    35624 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxCellEditor.js
+-rw-r--r--   0 root         (0) root         (0)     6245 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxCellOverlay.js
+-rw-r--r--   0 root         (0) root         (0)    44101 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxCellRenderer.js
+-rw-r--r--   0 root         (0) root         (0)     9726 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxCellState.js
+-rw-r--r--   0 root         (0) root         (0)     4286 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxCellStatePreview.js
+-rw-r--r--   0 root         (0) root         (0)     1649 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxConnectionConstraint.js
+-rw-r--r--   0 root         (0) root         (0)    42452 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxEdgeStyle.js
+-rw-r--r--   0 root         (0) root         (0)   333205 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxGraph.js
+-rw-r--r--   0 root         (0) root         (0)     9127 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxGraphSelectionModel.js
+-rw-r--r--   0 root         (0) root         (0)    74549 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxGraphView.js
+-rw-r--r--   0 root         (0) root         (0)    10941 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxLayoutManager.js
+-rw-r--r--   0 root         (0) root         (0)     7440 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxMultiplicity.js
+-rw-r--r--   0 root         (0) root         (0)    19683 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxOutline.js
+-rw-r--r--   0 root         (0) root         (0)    20530 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxPerimeter.js
+-rw-r--r--   0 root         (0) root         (0)    32135 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxPrintPreview.js
+-rw-r--r--   0 root         (0) root         (0)     2022 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxStyleRegistry.js
+-rw-r--r--   0 root         (0) root         (0)     6753 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxStylesheet.js
+-rw-r--r--   0 root         (0) root         (0)     9336 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxSwimlaneManager.js
+-rw-r--r--   0 root         (0) root         (0)     2955 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxTemporaryCellStates.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.625398 XGEE-0.3.7/xgee/core/dep/mxgraph/resources/
+-rw-r--r--   0 root         (0) root         (0)       83 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/resources/editor.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/resources/editor_de.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/resources/editor_zh.txt
+-rw-r--r--   0 root         (0) root         (0)      340 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/resources/graph.txt
+-rw-r--r--   0 root         (0) root         (0)      375 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/resources/graph_de.txt
+-rw-r--r--   0 root         (0) root         (0)      316 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/mxgraph/resources/graph_zh.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.625398 XGEE-0.3.7/xgee/core/dep/notifyjs/
+-rw-r--r--   0 root         (0) root         (0)      290 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/notifyjs/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    13780 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/notifyjs/notify.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.626398 XGEE-0.3.7/xgee/core/dep/underscore/
+-rw-r--r--   0 root         (0) root         (0)     1139 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/underscore/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    18069 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/dep/underscore/underscore-min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.534399 XGEE-0.3.7/xgee/core/plugins/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.626398 XGEE-0.3.7/xgee/core/plugins/autostart/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.627398 XGEE-0.3.7/xgee/core/plugins/autostart/js/
+-rw-r--r--   0 root         (0) root         (0)      593 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/autostart/js/AppStartupEvent.js
+-rw-r--r--   0 root         (0) root         (0)      823 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/autostart/js/AppStartupObserver.js
+-rw-r--r--   0 root         (0) root         (0)     1138 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/autostart/js/Autostarter.js
+-rw-r--r--   0 root         (0) root         (0)     3186 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/autostart/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.627398 XGEE-0.3.7/xgee/core/plugins/clipboard/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.629398 XGEE-0.3.7/xgee/core/plugins/clipboard/js/
+-rw-r--r--   0 root         (0) root         (0)      969 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/clipboard/js/AppClipboard.js
+-rw-r--r--   0 root         (0) root         (0)     1279 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/clipboard/js/Clipboard.js
+-rw-r--r--   0 root         (0) root         (0)     6598 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/clipboard/js/ClipboardAPI.js
+-rw-r--r--   0 root         (0) root         (0)      308 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/clipboard/js/ClipboardEvaluator.js
+-rw-r--r--   0 root         (0) root         (0)      618 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/clipboard/js/ClipboardEventHandler.js
+-rw-r--r--   0 root         (0) root         (0)     3342 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/clipboard/js/ClipboardManager.js
+-rw-r--r--   0 root         (0) root         (0)     3665 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/clipboard/js/EcoreClipboardEvaluator.js
+-rw-r--r--   0 root         (0) root         (0)     4999 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/clipboard/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.629398 XGEE-0.3.7/xgee/core/plugins/contextMenu/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.630398 XGEE-0.3.7/xgee/core/plugins/contextMenu/js/
+-rw-r--r--   0 root         (0) root         (0)     3032 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/contextMenu/js/ContextMenu.js
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/contextMenu/js/util.js
+-rw-r--r--   0 root         (0) root         (0)     2762 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/contextMenu/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.629398 XGEE-0.3.7/xgee/core/plugins/contextMenu.ecore/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.629398 XGEE-0.3.7/xgee/core/plugins/contextMenu.ecore/css/
+-rw-r--r--   0 root         (0) root         (0)      399 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/contextMenu.ecore/css/contextMenu.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.629398 XGEE-0.3.7/xgee/core/plugins/contextMenu.ecore/js/
+-rw-r--r--   0 root         (0) root         (0)      361 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/contextMenu.ecore/js/Filter.js
+-rw-r--r--   0 root         (0) root         (0)    13387 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/contextMenu.ecore/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.630398 XGEE-0.3.7/xgee/core/plugins/contextMenu.eoq/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.630398 XGEE-0.3.7/xgee/core/plugins/contextMenu.eoq/js/
+-rw-r--r--   0 root         (0) root         (0)     4740 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/contextMenu.eoq/js/util.js
+-rw-r--r--   0 root         (0) root         (0)     4218 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/contextMenu.eoq/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.631398 XGEE-0.3.7/xgee/core/plugins/ecore/
+-rw-r--r--   0 root         (0) root         (0)    11515 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    93760 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/ecore.xmi.js
+-rw-r--r--   0 root         (0) root         (0)      456 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.633398 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/
+-rw-r--r--   0 root         (0) root         (0)       57 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      145 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/.travis.yml
+-rw-r--r--   0 root         (0) root         (0)      366 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)      280 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     2011 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8381 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.636398 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/examples/
+-rw-r--r--   0 root         (0) root         (0)   181013 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/examples/big-not-pretty.xml
+-rw-r--r--   0 root         (0) root         (0)      790 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/examples/example.js
+-rw-r--r--   0 root         (0) root         (0)     1539 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/examples/get-products.js
+-rw-r--r--   0 root         (0) root         (0)      164 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/examples/hello-world.js
+-rw-r--r--   0 root         (0) root         (0)      181 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/examples/not-pretty.xml
+-rw-r--r--   0 root         (0) root         (0)     1506 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/examples/pretty-print.js
+-rw-r--r--   0 root         (0) root         (0)    99650 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/examples/shopping.xml
+-rw-r--r--   0 root         (0) root         (0)      138 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/examples/test.html
+-rw-r--r--   0 root         (0) root         (0)    51402 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/examples/test.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.636398 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/lib/
+-rw-r--r--   0 root         (0) root         (0)    43541 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/lib/sax.js
+-rw-r--r--   0 root         (0) root         (0)    85352 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/package-lock.json
+-rw-r--r--   0 root         (0) root         (0)      655 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.649398 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/
+-rw-r--r--   0 root         (0) root         (0)      763 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/attribute-name.js
+-rw-r--r--   0 root         (0) root         (0)     2426 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/attribute-no-space.js
+-rw-r--r--   0 root         (0) root         (0)      719 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/attribute-unquoted.js
+-rw-r--r--   0 root         (0) root         (0)     1478 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/bom.js
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/buffer-overrun.js
+-rw-r--r--   0 root         (0) root         (0)     1557 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/case.js
+-rw-r--r--   0 root         (0) root         (0)      389 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/cdata-chunked.js
+-rw-r--r--   0 root         (0) root         (0)      363 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/cdata-end-split.js
+-rw-r--r--   0 root         (0) root         (0)      782 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/cdata-fake-end.js
+-rw-r--r--   0 root         (0) root         (0)      514 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/cdata-multiple.js
+-rw-r--r--   0 root         (0) root         (0)      362 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/cdata.js
+-rw-r--r--   0 root         (0) root         (0)      247 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/cyrillic.js
+-rw-r--r--   0 root         (0) root         (0)      383 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/duplicate-attribute.js
+-rw-r--r--   0 root         (0) root         (0)      343 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/emoji.js
+-rw-r--r--   0 root         (0) root         (0)      130 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/end_empty_stream.js
+-rw-r--r--   0 root         (0) root         (0)      368 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/entities.js
+-rw-r--r--   0 root         (0) root         (0)      372 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/entity-mega.js
+-rw-r--r--   0 root         (0) root         (0)      238 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/entity-nan.js
+-rw-r--r--   0 root         (0) root         (0)      329 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/flush.js
+-rw-r--r--   0 root         (0) root         (0)     1311 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/index.js
+-rw-r--r--   0 root         (0) root         (0)     1912 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/issue-23.js
+-rw-r--r--   0 root         (0) root         (0)      691 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/issue-30.js
+-rw-r--r--   0 root         (0) root         (0)      336 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/issue-35.js
+-rw-r--r--   0 root         (0) root         (0)      398 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/issue-47.js
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/issue-49.js
+-rw-r--r--   0 root         (0) root         (0)      467 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/issue-84.js
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/issue-86.js
+-rw-r--r--   0 root         (0) root         (0)      240 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/not-string.js
+-rw-r--r--   0 root         (0) root         (0)     1300 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/opentagstart.js
+-rw-r--r--   0 root         (0) root         (0)      952 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/parser-position.js
+-rw-r--r--   0 root         (0) root         (0)      637 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/script-close-better.js
+-rw-r--r--   0 root         (0) root         (0)     1035 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/script.js
+-rw-r--r--   0 root         (0) root         (0)     1072 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/self-closing-child-strict.js
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/self-closing-child.js
+-rw-r--r--   0 root         (0) root         (0)      904 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/self-closing-tag.js
+-rw-r--r--   0 root         (0) root         (0)      217 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/stand-alone-comment.js
+-rw-r--r--   0 root         (0) root         (0)      755 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/stray-ending.js
+-rw-r--r--   0 root         (0) root         (0)      288 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/trailing-attribute-no-value.js
+-rw-r--r--   0 root         (0) root         (0)      407 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/trailing-non-whitespace.js
+-rw-r--r--   0 root         (0) root         (0)      387 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/unclosed-root.js
+-rw-r--r--   0 root         (0) root         (0)      727 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/unquoted.js
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/utf8-split.js
+-rw-r--r--   0 root         (0) root         (0)     1846 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/xml-internal-entities.js
+-rw-r--r--   0 root         (0) root         (0)      429 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/xml_entities.js
+-rw-r--r--   0 root         (0) root         (0)      465 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/xmlns-as-tag-name.js
+-rw-r--r--   0 root         (0) root         (0)     1668 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/xmlns-issue-41.js
+-rw-r--r--   0 root         (0) root         (0)     5497 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/xmlns-rebinding.js
+-rw-r--r--   0 root         (0) root         (0)     5577 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/xmlns-strict.js
+-rw-r--r--   0 root         (0) root         (0)     1805 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/xmlns-unbound-element.js
+-rw-r--r--   0 root         (0) root         (0)      947 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/xmlns-unbound.js
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-ns.js
+-rw-r--r--   0 root         (0) root         (0)      871 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-prefix-attribute.js
+-rw-r--r--   0 root         (0) root         (0)      509 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-prefix.js
+-rw-r--r--   0 root         (0) root         (0)     1096 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-redefine.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.519399 XGEE-0.3.7/xgee/core/plugins/ecoreDebuggerUi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.650398 XGEE-0.3.7/xgee/core/plugins/ecoreDebuggerUi/js/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecoreDebuggerUi/js/ecoreDebuggerUiController.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.651398 XGEE-0.3.7/xgee/core/plugins/ecoreSync/
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-23 20:45:12.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/.git
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      709 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.656398 XGEE-0.3.7/xgee/core/plugins/ecoreSync/changes/
+-rw-r--r--   0 root         (0) root         (0)    10686 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/changes/esChanges.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.656398 XGEE-0.3.7/xgee/core/plugins/ecoreSync/dev/
+-rw-r--r--   0 root         (0) root         (0)     5919 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/dev/esDebugging.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.657398 XGEE-0.3.7/xgee/core/plugins/ecoreSync/dev/lib/
+-rw-r--r--   0 root         (0) root         (0)     4918 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/dev/lib/libesync.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.658398 XGEE-0.3.7/xgee/core/plugins/ecoreSync/domain/
+-rw-r--r--   0 root         (0) root         (0)     1484 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/domain/esDomain.js
+-rw-r--r--   0 root         (0) root         (0)      378 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/domain/esErrors.js
+-rw-r--r--   0 root         (0) root         (0)     3129 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/domain/esLookup.js
+-rw-r--r--   0 root         (0) root         (0)    13249 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/domain/esMetaSync.js
+-rw-r--r--   0 root         (0) root         (0)    20548 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/domain/esObjectAccessors.js
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/domain/esOperationHandler.js
+-rw-r--r--   0 root         (0) root         (0)     1901 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/ecoreSync.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.658398 XGEE-0.3.7/xgee/core/plugins/ecoreSync/interfaces/
+-rw-r--r--   0 root         (0) root         (0)     2956 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/interfaces/esInstance.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.660398 XGEE-0.3.7/xgee/core/plugins/ecoreSync/mdb/
+-rw-r--r--   0 root         (0) root         (0)    10832 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/mdb/esMdbAccessor.js
+-rw-r--r--   0 root         (0) root         (0)     9168 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/mdb/esMdbObserver.js
+-rw-r--r--   0 root         (0) root         (0)     9420 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/mdb/esModelDatabase.js
+-rw-r--r--   0 root         (0) root         (0)     2183 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/mdb/esSyncEvents.js
+-rw-r--r--   0 root         (0) root         (0)     1834 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/mdb/esSyncStatus.js
+-rw-r--r--   0 root         (0) root         (0)     1416 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.661398 XGEE-0.3.7/xgee/core/plugins/ecoreSync/queries/
+-rw-r--r--   0 root         (0) root         (0)    20117 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/queries/esCmdRunner.js
+-rw-r--r--   0 root         (0) root         (0)     1851 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/queries/esQueries.js
+-rw-r--r--   0 root         (0) root         (0)    36223 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/queries/esQueryEvaluator.js
+-rw-r--r--   0 root         (0) root         (0)    26527 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/queries/esQueryObserver.js
+-rw-r--r--   0 root         (0) root         (0)     2491 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/queries/esQueryObserverState.js
+-rw-r--r--   0 root         (0) root         (0)     4045 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/queries/esQueryUtils.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.662397 XGEE-0.3.7/xgee/core/plugins/ecoreSync/util/
+-rw-r--r--   0 root         (0) root         (0)      966 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/util/auxiliaries.js
+-rw-r--r--   0 root         (0) root         (0)       50 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/util/esLogging.js
+-rw-r--r--   0 root         (0) root         (0)    22109 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/util/esUtils.js
+-rw-r--r--   0 root         (0) root         (0)     1194 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync/util/uuid.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.651398 XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.651398 XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/css/
+-rw-r--r--   0 root         (0) root         (0)     5694 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/css/EObjectCtrls.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.655398 XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/
+-rw-r--r--   0 root         (0) root         (0)     3076 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-close-active.svg
+-rw-r--r--   0 root         (0) root         (0)     3032 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-close.svg
+-rw-r--r--   0 root         (0) root         (0)     2667 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-custom-active.svg
+-rw-r--r--   0 root         (0) root         (0)     2651 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-custom.svg
+-rw-r--r--   0 root         (0) root         (0)     4500 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-global-active.svg
+-rw-r--r--   0 root         (0) root         (0)     4471 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-global.svg
+-rw-r--r--   0 root         (0) root         (0)     2560 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-local-active.svg
+-rw-r--r--   0 root         (0) root         (0)     2553 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-local.svg
+-rw-r--r--   0 root         (0) root         (0)     3529 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-select-all-active.svg
+-rw-r--r--   0 root         (0) root         (0)     3500 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-select-all.svg
+-rw-r--r--   0 root         (0) root         (0)     5270 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-select-invert-active.svg
+-rw-r--r--   0 root         (0) root         (0)     5138 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-select-invert.svg
+-rw-r--r--   0 root         (0) root         (0)     2381 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-select-none-active.svg
+-rw-r--r--   0 root         (0) root         (0)     2364 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-select-none.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.656398 XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/js/
+-rw-r--r--   0 root         (0) root         (0)     8088 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrlFactory.js
+-rw-r--r--   0 root         (0) root         (0)     5394 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrlUpdateHandler.js
+-rw-r--r--   0 root         (0) root         (0)    48091 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrls.js
+-rw-r--r--   0 root         (0) root         (0)      760 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.662397 XGEE-0.3.7/xgee/core/plugins/editor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.521399 XGEE-0.3.7/xgee/core/plugins/editor/controllers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.665398 XGEE-0.3.7/xgee/core/plugins/editor/controllers/graph/
+-rw-r--r--   0 root         (0) root         (0)      970 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/controllers/graph/AnchorController.js
+-rw-r--r--   0 root         (0) root         (0)      972 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/controllers/graph/ContainerController.js
+-rw-r--r--   0 root         (0) root         (0)     2337 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/controllers/graph/EdgeController.js
+-rw-r--r--   0 root         (0) root         (0)    15710 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/controllers/graph/GraphController.js
+-rw-r--r--   0 root         (0) root         (0)     7060 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/controllers/graph/GraphControllerFactory.js
+-rw-r--r--   0 root         (0) root         (0)      275 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/controllers/graph/GraphObjectController.js
+-rw-r--r--   0 root         (0) root         (0)      976 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/controllers/graph/LabelController.js
+-rw-r--r--   0 root         (0) root         (0)      978 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/controllers/graph/QueryController.js
+-rw-r--r--   0 root         (0) root         (0)     5353 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/controllers/graph/VertexController.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.665398 XGEE-0.3.7/xgee/core/plugins/editor/controllers/palette/
+-rw-r--r--   0 root         (0) root         (0)     1245 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/controllers/palette/PaletteController.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.665398 XGEE-0.3.7/xgee/core/plugins/editor/css/
+-rw-r--r--   0 root         (0) root         (0)      547 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/css/loading.css
+-rw-r--r--   0 root         (0) root         (0)      115 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/css/xgeeJsaIntegration.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.666397 XGEE-0.3.7/xgee/core/plugins/editor/extensions/
+-rw-r--r--   0 root         (0) root         (0)     2473 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/extensions/EditorContextMenuProvider.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.666397 XGEE-0.3.7/xgee/core/plugins/editor/graph/
+-rw-r--r--   0 root         (0) root         (0)     1383 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/graph/GraphResourceProvider.js
+-rw-r--r--   0 root         (0) root         (0)     6693 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/graph/mxGraphIntegration.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.667397 XGEE-0.3.7/xgee/core/plugins/editor/interactions/
+-rw-r--r--   0 root         (0) root         (0)     3785 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/interactions/DropReception.js
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/interactions/GraphInteraction.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.668398 XGEE-0.3.7/xgee/core/plugins/editor/lib/
+-rw-r--r--   0 root         (0) root         (0)    10080 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/lib/libapi.js
+-rw-r--r--   0 root         (0) root         (0)     9750 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/lib/libaux.js
+-rw-r--r--   0 root         (0) root         (0)    20059 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/lib/libjsa.js
+-rw-r--r--   0 root         (0) root         (0)     1194 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/lib/uuid.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.668398 XGEE-0.3.7/xgee/core/plugins/editor/model/
+-rw-r--r--   0 root         (0) root         (0)      339 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/PresentationModel.js
+-rw-r--r--   0 root         (0) root         (0)    83708 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/editorModel.ecore
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.678397 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/
+-rw-r--r--   0 root         (0) root         (0)     1866 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/Anchor.js
+-rw-r--r--   0 root         (0) root         (0)     3246 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/AnchorManager.js
+-rw-r--r--   0 root         (0) root         (0)      449 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/AnchorType.js
+-rw-r--r--   0 root         (0) root         (0)     2305 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/Container.js
+-rw-r--r--   0 root         (0) root         (0)     1896 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/ContainerManager.js
+-rw-r--r--   0 root         (0) root         (0)      608 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/ContainerProvider.js
+-rw-r--r--   0 root         (0) root         (0)     1760 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/ContainerType.js
+-rw-r--r--   0 root         (0) root         (0)     1037 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/DeletableObject.js
+-rw-r--r--   0 root         (0) root         (0)      266 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/EObjectOwner.js
+-rw-r--r--   0 root         (0) root         (0)    10305 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/Edge.js
+-rw-r--r--   0 root         (0) root         (0)     1264 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/EdgeContainer.js
+-rw-r--r--   0 root         (0) root         (0)     7174 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/EdgeManager.js
+-rw-r--r--   0 root         (0) root         (0)      383 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/EdgeType.js
+-rw-r--r--   0 root         (0) root         (0)      566 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/EventProvider.js
+-rw-r--r--   0 root         (0) root         (0)      346 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/FloatingLabel.js
+-rw-r--r--   0 root         (0) root         (0)     1013 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/GraphEvent.js
+-rw-r--r--   0 root         (0) root         (0)    27960 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/GraphLayoutManager.js
+-rw-r--r--   0 root         (0) root         (0)     6623 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/GraphModel.js
+-rw-r--r--   0 root         (0) root         (0)    12792 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/GraphModelFactory.js
+-rw-r--r--   0 root         (0) root         (0)     4145 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/GraphModelManager.js
+-rw-r--r--   0 root         (0) root         (0)      553 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/GraphObject.js
+-rw-r--r--   0 root         (0) root         (0)     2252 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/GraphObjectManager.js
+-rw-r--r--   0 root         (0) root         (0)      144 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/GraphObjectType.js
+-rw-r--r--   0 root         (0) root         (0)     2200 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/Label.js
+-rw-r--r--   0 root         (0) root         (0)     1990 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/LabelManager.js
+-rw-r--r--   0 root         (0) root         (0)      478 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/LabelProvider.js
+-rw-r--r--   0 root         (0) root         (0)     2061 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/LabelSegment.js
+-rw-r--r--   0 root         (0) root         (0)     6090 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/LabelSegmentManager.js
+-rw-r--r--   0 root         (0) root         (0)      419 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/LabelSegmentType.js
+-rw-r--r--   0 root         (0) root         (0)      386 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/LabelType.js
+-rw-r--r--   0 root         (0) root         (0)      932 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/LocatableObject.js
+-rw-r--r--   0 root         (0) root         (0)      615 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/NestedLabel.js
+-rw-r--r--   0 root         (0) root         (0)      464 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/RoutableObject.js
+-rw-r--r--   0 root         (0) root         (0)     1527 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/SizableObject.js
+-rw-r--r--   0 root         (0) root         (0)     2346 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/StaticVertex.js
+-rw-r--r--   0 root         (0) root         (0)     7913 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/StaticVertexManager.js
+-rw-r--r--   0 root         (0) root         (0)     1684 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/StaticVertexType.js
+-rw-r--r--   0 root         (0) root         (0)      546 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/TransactionObject.js
+-rw-r--r--   0 root         (0) root         (0)       84 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/TypedObject.js
+-rw-r--r--   0 root         (0) root         (0)     3517 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/Vertex.js
+-rw-r--r--   0 root         (0) root         (0)    12233 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/VertexContainer.js
+-rw-r--r--   0 root         (0) root         (0)    14544 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/VertexManager.js
+-rw-r--r--   0 root         (0) root         (0)     1682 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/graph/VertexType.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.680397 XGEE-0.3.7/xgee/core/plugins/editor/model/palette/
+-rw-r--r--   0 root         (0) root         (0)     2655 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/palette/DragAndDropTool.js
+-rw-r--r--   0 root         (0) root         (0)    16081 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/palette/EdgeRoutingTool.js
+-rw-r--r--   0 root         (0) root         (0)     3656 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/palette/GraphTool.js
+-rw-r--r--   0 root         (0) root         (0)     8885 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/palette/PaletteModel.js
+-rw-r--r--   0 root         (0) root         (0)     3844 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/palette/SelectionTool.js
+-rw-r--r--   0 root         (0) root         (0)     8885 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/model/palette/ToolGenerator.js
+-rw-r--r--   0 root         (0) root         (0)     5667 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.680397 XGEE-0.3.7/xgee/core/plugins/editor/queries/
+-rw-r--r--   0 root         (0) root         (0)     6504 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/queries/Query.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.681397 XGEE-0.3.7/xgee/core/plugins/editor/view/
+-rw-r--r--   0 root         (0) root         (0)    55157 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/view/GraphView.js
+-rw-r--r--   0 root         (0) root         (0)     1725 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/view/GraphViewMenu.js
+-rw-r--r--   0 root         (0) root         (0)    22370 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/view/GraphViewPort.js
+-rw-r--r--   0 root         (0) root         (0)     3483 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/view/PaletteView.js
+-rw-r--r--   0 root         (0) root         (0)     5888 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/editor/view/ScreenshotExport.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.682397 XGEE-0.3.7/xgee/core/plugins/eoq.actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.682397 XGEE-0.3.7/xgee/core/plugins/eoq.actions/css/
+-rw-r--r--   0 root         (0) root         (0)     2193 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/eoq.actions/css/ActionsUi.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.683397 XGEE-0.3.7/xgee/core/plugins/eoq.actions/js/
+-rw-r--r--   0 root         (0) root         (0)     5233 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/eoq.actions/js/ActionsController.js
+-rw-r--r--   0 root         (0) root         (0)    14133 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/eoq.actions/js/ActionsCore.js
+-rw-r--r--   0 root         (0) root         (0)    23053 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/eoq.actions/js/ActionsUi.js
+-rw-r--r--   0 root         (0) root         (0)     1541 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/eoq.actions/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.685397 XGEE-0.3.7/xgee/core/plugins/eoq1/
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq1/.git
+-rw-r--r--   0 root         (0) root         (0)     1160 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1077 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq1/README.md
+-rw-r--r--   0 root         (0) root         (0)    11898 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq1/commandparser.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.686397 XGEE-0.3.7/xgee/core/plugins/eoq1/domains/
+-rw-r--r--   0 root         (0) root         (0)     5897 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq1/domains/bufferingdomain.js
+-rw-r--r--   0 root         (0) root         (0)      879 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq1/domains/domain.js
+-rw-r--r--   0 root         (0) root         (0)     4364 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq1/domains/httppostdomain.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.686397 XGEE-0.3.7/xgee/core/plugins/eoq1/model/
+-rw-r--r--   0 root         (0) root         (0)    37451 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq1/model/model.js
+-rw-r--r--   0 root         (0) root         (0)      468 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq1/package.json
+-rw-r--r--   0 root         (0) root         (0)      504 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq1/plugin.js
+-rw-r--r--   0 root         (0) root         (0)       90 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq1/queryparser.js
+-rw-r--r--   0 root         (0) root         (0)    11900 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq1/resultparser.js
+-rw-r--r--   0 root         (0) root         (0)    12168 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq1/valueparser.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.687397 XGEE-0.3.7/xgee/core/plugins/eoq2/
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq2/.git
+-rw-r--r--   0 root         (0) root         (0)     1160 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      925 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.688397 XGEE-0.3.7/xgee/core/plugins/eoq2/action/
+-rw-r--r--   0 root         (0) root         (0)      579 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq2/action/call.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.688397 XGEE-0.3.7/xgee/core/plugins/eoq2/command/
+-rw-r--r--   0 root         (0) root         (0)    12287 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq2/command/command.js
+-rw-r--r--   0 root         (0) root         (0)     1365 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq2/command/result.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.688397 XGEE-0.3.7/xgee/core/plugins/eoq2/domain/
+-rw-r--r--   0 root         (0) root         (0)      983 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq2/domain/domain.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.689397 XGEE-0.3.7/xgee/core/plugins/eoq2/domain/remote/
+-rw-r--r--   0 root         (0) root         (0)     2267 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq2/domain/remote/httppostdomain.js
+-rw-r--r--   0 root         (0) root         (0)     5812 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq2/domain/remote/websocketdomain.js
+-rw-r--r--   0 root         (0) root         (0)     4806 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq2/eoq2.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.689397 XGEE-0.3.7/xgee/core/plugins/eoq2/event/
+-rw-r--r--   0 root         (0) root         (0)     3879 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq2/event/event.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.689397 XGEE-0.3.7/xgee/core/plugins/eoq2/frame/
+-rw-r--r--   0 root         (0) root         (0)      567 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq2/frame/frame.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.690397 XGEE-0.3.7/xgee/core/plugins/eoq2/legacy/
+-rw-r--r--   0 root         (0) root         (0)    14240 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq2/legacy/legacy.js
+-rw-r--r--   0 root         (0) root         (0)      440 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq2/package.json
+-rw-r--r--   0 root         (0) root         (0)     2472 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq2/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.690397 XGEE-0.3.7/xgee/core/plugins/eoq2/query/
+-rw-r--r--   0 root         (0) root         (0)    14393 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq2/query/query.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.691397 XGEE-0.3.7/xgee/core/plugins/eoq2/serialization/
+-rw-r--r--   0 root         (0) root         (0)     1107 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq2/serialization/jsonserializer.js
+-rw-r--r--   0 root         (0) root         (0)      725 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq2/serialization/serializer.js
+-rw-r--r--   0 root         (0) root         (0)    40363 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq2/serialization/textserializer.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.691397 XGEE-0.3.7/xgee/core/plugins/eoq2/util/
+-rw-r--r--   0 root         (0) root         (0)     2823 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/core/plugins/eoq2/util/logger.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.693397 XGEE-0.3.7/xgee/core/plugins/eventBroker/
+-rw-r--r--   0 root         (0) root         (0)      506 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/eventBroker/BasicEvent.js
+-rw-r--r--   0 root         (0) root         (0)      506 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/eventBroker/QueryDebugEvent.js
+-rw-r--r--   0 root         (0) root         (0)      694 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/eventBroker/SelectionChangedEvent.js
+-rw-r--r--   0 root         (0) root         (0)     3823 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/eventBroker/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.693397 XGEE-0.3.7/xgee/core/plugins/iconProvider/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.693397 XGEE-0.3.7/xgee/core/plugins/iconProvider/js/
+-rw-r--r--   0 root         (0) root         (0)      387 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/iconProvider/js/IconProvider.js
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/iconProvider/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.693397 XGEE-0.3.7/xgee/core/plugins/keyHandler/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.694397 XGEE-0.3.7/xgee/core/plugins/keyHandler/js/
+-rw-r--r--   0 root         (0) root         (0)     1493 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/keyHandler/js/KeyHandler.js
+-rw-r--r--   0 root         (0) root         (0)      391 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/keyHandler/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.694397 XGEE-0.3.7/xgee/core/plugins/keyHandler.ecore/
+-rw-r--r--   0 root         (0) root         (0)      720 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/keyHandler.ecore/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.694397 XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.697397 XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.698397 XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/
+-rw-r--r--   0 root         (0) root         (0)     3528 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.eot
+-rw-r--r--   0 root         (0) root         (0)     3320 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.ttf
+-rw-r--r--   0 root         (0) root         (0)     2180 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.woff
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.woff2
+-rw-r--r--   0 root         (0) root         (0)     7278 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.css
+-rw-r--r--   0 root         (0) root         (0)    91213 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.js
+-rw-r--r--   0 root         (0) root         (0)     5991 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.css
+-rw-r--r--   0 root         (0) root         (0)    14532 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.css.map
+-rw-r--r--   0 root         (0) root         (0)    27807 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.js
+-rw-r--r--   0 root         (0) root         (0)   131140 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.js.map
+-rw-r--r--   0 root         (0) root         (0)    22405 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.ui.position.js
+-rw-r--r--   0 root         (0) root         (0)     5855 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.ui.position.min.js
+-rw-r--r--   0 root         (0) root         (0)      669 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.699397 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.709397 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/
+-rw-r--r--   0 root         (0) root         (0)      554 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EAnnotation.gif
+-rw-r--r--   0 root         (0) root         (0)      123 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EAttribute.gif
+-rw-r--r--   0 root         (0) root         (0)      206 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EClass.gif
+-rw-r--r--   0 root         (0) root         (0)      199 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EDataType.gif
+-rw-r--r--   0 root         (0) root         (0)      131 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EEnum.gif
+-rw-r--r--   0 root         (0) root         (0)      109 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EEnumLiteral.gif
+-rw-r--r--   0 root         (0) root         (0)      211 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EFactory.gif
+-rw-r--r--   0 root         (0) root         (0)      102 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericElementType.gif
+-rw-r--r--   0 root         (0) root         (0)      108 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericException.gif
+-rw-r--r--   0 root         (0) root         (0)      139 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericSuperType.gif
+-rw-r--r--   0 root         (0) root         (0)       99 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericType.gif
+-rw-r--r--   0 root         (0) root         (0)      139 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericTypeArgument.gif
+-rw-r--r--   0 root         (0) root         (0)      111 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EGenericWildcard.gif
+-rw-r--r--   0 root         (0) root         (0)      323 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EObject.gif
+-rw-r--r--   0 root         (0) root         (0)       62 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceN.gif
+-rw-r--r--   0 root         (0) root         (0)       71 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceNToM.gif
+-rw-r--r--   0 root         (0) root         (0)       81 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceNToUnbounded.gif
+-rw-r--r--   0 root         (0) root         (0)      131 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceNToUnspecified.gif
+-rw-r--r--   0 root         (0) root         (0)       58 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceOne.gif
+-rw-r--r--   0 root         (0) root         (0)       68 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceOneToN.gif
+-rw-r--r--   0 root         (0) root         (0)       79 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceOneToUnbounded.gif
+-rw-r--r--   0 root         (0) root         (0)      128 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceOneToUnspecified.gif
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceZero.gif
+-rw-r--r--   0 root         (0) root         (0)       78 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceZeroToN.gif
+-rw-r--r--   0 root         (0) root         (0)       77 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceZeroToOne.gif
+-rw-r--r--   0 root         (0) root         (0)       83 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceZeroToUnbounded.gif
+-rw-r--r--   0 root         (0) root         (0)      133 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOccurrenceZeroToUnspecified.gif
+-rw-r--r--   0 root         (0) root         (0)      141 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EOperation.gif
+-rw-r--r--   0 root         (0) root         (0)      207 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EPackage.gif
+-rw-r--r--   0 root         (0) root         (0)      911 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EParameter.gif
+-rw-r--r--   0 root         (0) root         (0)      183 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EReference.gif
+-rw-r--r--   0 root         (0) root         (0)      213 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EStringToStringMapEntry.gif
+-rw-r--r--   0 root         (0) root         (0)      211 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/ETypeParameter.gif
+-rw-r--r--   0 root         (0) root         (0)      554 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eAnnotations.gif
+-rw-r--r--   0 root         (0) root         (0)      206 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eClassifiers.gif
+-rw-r--r--   0 root         (0) root         (0)      141 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eOperations.gif
+-rw-r--r--   0 root         (0) root         (0)      207 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eSubpackages.gif
+-rw-r--r--   0 root         (0) root         (0)      211 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eTypeParameters.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.709397 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/js/
+-rw-r--r--   0 root         (0) root         (0)      577 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/js/TreeViewContextMenuProvider.js
+-rw-r--r--   0 root         (0) root         (0)    29729 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.699397 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView.eoq/
+-rw-r--r--   0 root         (0) root         (0)    16933 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView.eoq/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.711397 XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/
+-rw-r--r--   0 root         (0) root         (0)     1078 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   128443 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/jquery.fancytree-all-deps.min.js
+-rw-r--r--   0 root         (0) root         (0)   162267 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/jquery.fancytree-all-deps.min.js.map
+-rw-r--r--   0 root         (0) root         (0)      562 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.712397 XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/skin-win8/
+-rw-r--r--   0 root         (0) root         (0)     5513 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/skin-win8/icons-rtl.gif
+-rw-r--r--   0 root         (0) root         (0)     5510 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/skin-win8/icons.gif
+-rw-r--r--   0 root         (0) root         (0)     3234 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/skin-win8/loading.gif
+-rw-r--r--   0 root         (0) root         (0)    24749 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/skin-win8/ui.fancytree.css
+-rw-r--r--   0 root         (0) root         (0)     4818 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/skin-win8/ui.fancytree.less
+-rw-r--r--   0 root         (0) root         (0)      852 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/skin-win8/vline-rtl.gif
+-rw-r--r--   0 root         (0) root         (0)      852 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/skin-win8/vline.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.713397 XGEE-0.3.7/xgee/core/plugins/propertiesView/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.717397 XGEE-0.3.7/xgee/core/plugins/propertiesView/css/
+-rw-r--r--   0 root         (0) root         (0)      961 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView/css/PropertiesView.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.718397 XGEE-0.3.7/xgee/core/plugins/propertiesView/doc/
+-rw-r--r--   0 root         (0) root         (0)    38735 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView/doc/PropertiesView.pptx
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.719397 XGEE-0.3.7/xgee/core/plugins/propertiesView/js/
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView/js/LoadOnDemandView.js
+-rw-r--r--   0 root         (0) root         (0)      298 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView/js/PropertiesBubble.js
+-rw-r--r--   0 root         (0) root         (0)      779 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView/js/PropertiesPaneProvider.js
+-rw-r--r--   0 root         (0) root         (0)     7532 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView/js/PropertiesViewController.js
+-rw-r--r--   0 root         (0) root         (0)     1795 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.713397 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.717397 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore/js/
+-rw-r--r--   0 root         (0) root         (0)    10124 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore/js/EObjectPropertiesPane.js
+-rw-r--r--   0 root         (0) root         (0)     1682 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore/js/EObjectPropertiesPaneProvider.js
+-rw-r--r--   0 root         (0) root         (0)     1173 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.713397 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.custom/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.714397 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.custom/js/
+-rw-r--r--   0 root         (0) root         (0)     7014 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPane.js
+-rw-r--r--   0 root         (0) root         (0)     1163 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPaneConfig.js
+-rw-r--r--   0 root         (0) root         (0)     2739 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPaneProvider.js
+-rw-r--r--   0 root         (0) root         (0)      878 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.custom/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.714397 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.editors/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.714397 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.editors/css/
+-rw-r--r--   0 root         (0) root         (0)      458 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.editors/css/EcoreEditorsPropertiesPane.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.715397 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.editors/js/
+-rw-r--r--   0 root         (0) root         (0)     1565 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.editors/js/EcoreEditorsPropertiesPane.js
+-rw-r--r--   0 root         (0) root         (0)     2170 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.editors/js/EcoreEditorsPropertiesPaneProvider.js
+-rw-r--r--   0 root         (0) root         (0)     1297 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.editors/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.715397 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.modify/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.715397 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.modify/css/
+-rw-r--r--   0 root         (0) root         (0)      458 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.modify/css/EcoreModifyPropertiesPane.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.716397 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.modify/js/
+-rw-r--r--   0 root         (0) root         (0)     2571 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.modify/js/EcoreModifyPropertiesPane.js
+-rw-r--r--   0 root         (0) root         (0)     2157 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.modify/js/EcoreModifyPropertiesPaneProvider.js
+-rw-r--r--   0 root         (0) root         (0)     1287 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.modify/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.716397 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.workspace/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.716397 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.workspace/js/
+-rw-r--r--   0 root         (0) root         (0)     1281 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.workspace/js/WorkspacePropertiesPaneConfig.js
+-rw-r--r--   0 root         (0) root         (0)     1263 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.workspace/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.717397 XGEE-0.3.7/xgee/core/plugins/propertiesView.info/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.717397 XGEE-0.3.7/xgee/core/plugins/propertiesView.info/js/
+-rw-r--r--   0 root         (0) root         (0)     3609 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView.info/js/InfoPropertiesPaneProvider.js
+-rw-r--r--   0 root         (0) root         (0)      984 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/propertiesView.info/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.719397 XGEE-0.3.7/xgee/core/plugins/tool.goToView/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.719397 XGEE-0.3.7/xgee/core/plugins/tool.goToView/css/
+-rw-r--r--   0 root         (0) root         (0)      126 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/tool.goToView/css/GoToViewTool.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.719397 XGEE-0.3.7/xgee/core/plugins/tool.goToView/img/
+-rw-r--r--   0 root         (0) root         (0)     2842 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/tool.goToView/img/tool-go-to-view.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.720397 XGEE-0.3.7/xgee/core/plugins/tool.goToView/js/
+-rw-r--r--   0 root         (0) root         (0)     2805 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/tool.goToView/js/GoToViewTool.js
+-rw-r--r--   0 root         (0) root         (0)     1018 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/tool.goToView/js/GoToViewToolProvider.js
+-rw-r--r--   0 root         (0) root         (0)     1262 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/tool.goToView/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.720397 XGEE-0.3.7/xgee/core/plugins/tool.notes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.720397 XGEE-0.3.7/xgee/core/plugins/tool.notes/css/
+-rw-r--r--   0 root         (0) root         (0)     4415 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/tool.notes/css/NotesTool.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.722397 XGEE-0.3.7/xgee/core/plugins/tool.notes/img/
+-rw-r--r--   0 root         (0) root         (0)     3331 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/tool.notes/img/notes-error.svg
+-rw-r--r--   0 root         (0) root         (0)     2197 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/tool.notes/img/notes-info.svg
+-rw-r--r--   0 root         (0) root         (0)     2085 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/tool.notes/img/notes-success.svg
+-rw-r--r--   0 root         (0) root         (0)     3188 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/tool.notes/img/notes-warning.svg
+-rw-r--r--   0 root         (0) root         (0)     2173 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/tool.notes/img/tool-notes.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.722397 XGEE-0.3.7/xgee/core/plugins/tool.notes/js/
+-rw-r--r--   0 root         (0) root         (0)     6924 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/tool.notes/js/NotesTool.js
+-rw-r--r--   0 root         (0) root         (0)      940 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/tool.notes/js/NotesToolProvider.js
+-rw-r--r--   0 root         (0) root         (0)     1076 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/tool.notes/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.722397 XGEE-0.3.7/xgee/core/plugins/tools/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.723397 XGEE-0.3.7/xgee/core/plugins/tools/js/
+-rw-r--r--   0 root         (0) root         (0)      364 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/tools/js/ToolProvider.js
+-rw-r--r--   0 root         (0) root         (0)     1409 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/tools/js/ToolsController.js
+-rw-r--r--   0 root         (0) root         (0)     1268 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/tools/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.723397 XGEE-0.3.7/xgee/core/plugins/view.dashboard/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.726397 XGEE-0.3.7/xgee/core/plugins/view.dashboard/css/
+-rw-r--r--   0 root         (0) root         (0)      149 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/view.dashboard/css/DashboardView.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.727397 XGEE-0.3.7/xgee/core/plugins/view.dashboard/img/
+-rw-r--r--   0 root         (0) root         (0)     2146 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/view.dashboard/img/view-dashboard.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.727397 XGEE-0.3.7/xgee/core/plugins/view.dashboard/js/
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/view.dashboard/js/DashProvider.js
+-rw-r--r--   0 root         (0) root         (0)     3522 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/view.dashboard/js/DashboardViewProvider.js
+-rw-r--r--   0 root         (0) root         (0)     2285 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/view.dashboard/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.723397 XGEE-0.3.7/xgee/core/plugins/view.dashboard.infoDash/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.723397 XGEE-0.3.7/xgee/core/plugins/view.dashboard.infoDash/js/
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/view.dashboard.infoDash/js/InfoDashProvider.js
+-rw-r--r--   0 root         (0) root         (0)     1659 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/view.dashboard.infoDash/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.724397 XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.724397 XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/css/
+-rw-r--r--   0 root         (0) root         (0)     1506 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/css/StartModellingDash.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.725397 XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/img/
+-rw-r--r--   0 root         (0) root         (0)     3787 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/img/delete.svg
+-rw-r--r--   0 root         (0) root         (0)     2220 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/img/edit.svg
+-rw-r--r--   0 root         (0) root         (0)     2936 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/img/new-object.svg
+-rw-r--r--   0 root         (0) root         (0)     3277 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/img/new-subdir.svg
+-rw-r--r--   0 root         (0) root         (0)     2181 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/img/object.svg
+-rw-r--r--   0 root         (0) root         (0)     2403 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/img/parent.svg
+-rw-r--r--   0 root         (0) root         (0)     2522 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/img/subdir.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.726397 XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/js/
+-rw-r--r--   0 root         (0) root         (0)    24067 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDash.js
+-rw-r--r--   0 root         (0) root         (0)     5322 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDashListEntry.js
+-rw-r--r--   0 root         (0) root         (0)     2123 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDashProvider.js
+-rw-r--r--   0 root         (0) root         (0)     2212 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.727397 XGEE-0.3.7/xgee/core/plugins/view.workspace/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.728397 XGEE-0.3.7/xgee/core/plugins/view.workspace/css/
+-rw-r--r--   0 root         (0) root         (0)      176 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/view.workspace/css/WorkspaceView.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.728397 XGEE-0.3.7/xgee/core/plugins/view.workspace/img/
+-rw-r--r--   0 root         (0) root         (0)     2511 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/view.workspace/img/view-workspace.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.728397 XGEE-0.3.7/xgee/core/plugins/view.workspace/js/
+-rw-r--r--   0 root         (0) root         (0)     2417 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/view.workspace/js/WorkspaceViewProvider.js
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/view.workspace/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.728397 XGEE-0.3.7/xgee/core/plugins/views/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.729397 XGEE-0.3.7/xgee/core/plugins/views/js/
+-rw-r--r--   0 root         (0) root         (0)      435 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/views/js/ViewProvider.js
+-rw-r--r--   0 root         (0) root         (0)     1886 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/views/js/ViewsController.js
+-rw-r--r--   0 root         (0) root         (0)     1423 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/views/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.729397 XGEE-0.3.7/xgee/core/plugins/viewsMenu/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.729397 XGEE-0.3.7/xgee/core/plugins/viewsMenu/js/
+-rw-r--r--   0 root         (0) root         (0)     5303 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/viewsMenu/js/ViewsMenuController.js
+-rw-r--r--   0 root         (0) root         (0)     1290 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/viewsMenu/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.729397 XGEE-0.3.7/xgee/core/plugins/viewsTabbar/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.730397 XGEE-0.3.7/xgee/core/plugins/viewsTabbar/css/
+-rw-r--r--   0 root         (0) root         (0)      856 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/viewsTabbar/css/ViewsTabbar.css
+-rw-r--r--   0 root         (0) root         (0)     1919 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/plugins/viewsTabbar/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.535399 XGEE-0.3.7/xgee/core/res/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.732397 XGEE-0.3.7/xgee/core/res/css/
+-rw-r--r--   0 root         (0) root         (0)      329 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/css/UIComponents.canvasSearch.css
+-rw-r--r--   0 root         (0) root         (0)     1099 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/css/app.css
+-rw-r--r--   0 root         (0) root         (0)      337 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/css/canvas.css
+-rw-r--r--   0 root         (0) root         (0)      996 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/css/contextmenu.css
+-rw-r--r--   0 root         (0) root         (0)       94 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/css/layout.css
+-rw-r--r--   0 root         (0) root         (0)     4230 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/css/notes.css
+-rw-r--r--   0 root         (0) root         (0)     1974 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/css/palette.css
+-rw-r--r--   0 root         (0) root         (0)     7091 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/css/uiControls.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.735397 XGEE-0.3.7/xgee/core/res/img/
+-rw-r--r--   0 root         (0) root         (0)     2989 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/img/edit.svg
+-rw-r--r--   0 root         (0) root         (0)     3645 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/img/eye.svg
+-rw-r--r--   0 root         (0) root         (0)     5763 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/img/globe.svg
+-rw-r--r--   0 root         (0) root         (0)     3577 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/img/graph-view-oaam-allocations.svg
+-rw-r--r--   0 root         (0) root         (0)     4433 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/img/graph-view-oaam-functions.svg
+-rw-r--r--   0 root         (0) root         (0)     3096 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/img/graph-view-oaam-hardware.svg
+-rw-r--r--   0 root         (0) root         (0)     2830 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/img/redo.svg
+-rw-r--r--   0 root         (0) root         (0)     3529 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/img/tool-domain-status-down.svg
+-rw-r--r--   0 root         (0) root         (0)     3152 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/img/tool-domain-status-error.svg
+-rw-r--r--   0 root         (0) root         (0)     4286 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/img/tool-domain-status-up-down.svg
+-rw-r--r--   0 root         (0) root         (0)     3535 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/img/tool-domain-status-up.svg
+-rw-r--r--   0 root         (0) root         (0)     2803 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/img/tool-domain-status.svg
+-rw-r--r--   0 root         (0) root         (0)     3449 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/img/tree.svg
+-rw-r--r--   0 root         (0) root         (0)     2788 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/img/undo.svg
+-rw-r--r--   0 root         (0) root         (0)     3010 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/img/view-editor.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.737397 XGEE-0.3.7/xgee/core/res/js/
+-rw-r--r--   0 root         (0) root         (0)     3240 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/js/DomainStatistics.js
+-rw-r--r--   0 root         (0) root         (0)    12997 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/js/app.js
+-rw-r--r--   0 root         (0) root         (0)     5020 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/js/commands.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.737397 XGEE-0.3.7/xgee/core/res/js/connectors/
+-rw-r--r--   0 root         (0) root         (0)     9049 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/js/connectors/connectors.graph.js
+-rw-r--r--   0 root         (0) root         (0)     4190 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/js/connectors/connectors.selection.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.737397 XGEE-0.3.7/xgee/core/res/js/grids/
+-rw-r--r--   0 root         (0) root         (0)      415 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/js/grids/points_grid.svg
+-rw-r--r--   0 root         (0) root         (0)     3582 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/js/ports.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.738397 XGEE-0.3.7/xgee/core/res/js/ui/
+-rw-r--r--   0 root         (0) root         (0)     4761 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/js/ui/DomainStatusTool.js
+-rw-r--r--   0 root         (0) root         (0)     1437 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/js/ui/ui.colorProvider.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.738397 XGEE-0.3.7/xgee/core/res/js/workspace/
+-rw-r--r--   0 root         (0) root         (0)     3669 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/js/workspace/workspace.jobs.js
+-rw-r--r--   0 root         (0) root         (0)    18830 2024-04-23 20:45:11.000000 XGEE-0.3.7/xgee/core/res/js/workspace/workspace.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.739397 XGEE-0.3.7/xgee/eoqserver/
+-rw-r--r--   0 root         (0) root         (0)    13048 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/eoqserver/PyEoq2WebServer.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 20:45:13.000000 XGEE-0.3.7/xgee/eoqserver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.740397 XGEE-0.3.7/xgee/eoqserver/eoq1/
+-rw-r--r--   0 root         (0) root         (0)      182 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.741397 XGEE-0.3.7/xgee/eoqserver/eoq1/actions/
+-rw-r--r--   0 root         (0) root         (0)      119 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq1/actions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq1/actions/actionutils.py
+-rw-r--r--   0 root         (0) root         (0)    29323 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq1/actions/externalactionhandler.py
+-rw-r--r--   0 root         (0) root         (0)     9347 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq1/commandparser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.742397 XGEE-0.3.7/xgee/eoqserver/eoq1/domains/
+-rw-r--r--   0 root         (0) root         (0)      283 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq1/domains/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72154 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq1/domains/localdomain.py
+-rw-r--r--   0 root         (0) root         (0)      979 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq1/domains/multiprocessingqueuedomainclient.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq1/domains/multiprocessingqueuedomainhost.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq1/domains/remotehttpdomain.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq1/domains/simplepythondomainwrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.743397 XGEE-0.3.7/xgee/eoqserver/eoq1/error/
+-rw-r--r--   0 root         (0) root         (0)      248 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq1/error/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq1/error/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.743397 XGEE-0.3.7/xgee/eoqserver/eoq1/model/
+-rw-r--r--   0 root         (0) root         (0)     7459 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq1/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64472 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq1/model/model.py
+-rw-r--r--   0 root         (0) root         (0)    22749 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq1/queryparser.py
+-rw-r--r--   0 root         (0) root         (0)     8387 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq1/resultparser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.744397 XGEE-0.3.7/xgee/eoqserver/eoq1/utils/
+-rw-r--r--   0 root         (0) root         (0)       63 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq1/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25693 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq1/utils/csvconnector.py
+-rw-r--r--   0 root         (0) root         (0)    10694 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq1/valueparser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.744397 XGEE-0.3.7/xgee/eoqserver/eoq2/
+-rw-r--r--   0 root         (0) root         (0)      117 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.745397 XGEE-0.3.7/xgee/eoqserver/eoq2/action/
+-rw-r--r--   0 root         (0) root         (0)      142 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/action/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      856 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/action/action.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/action/call.py
+-rw-r--r--   0 root         (0) root         (0)      754 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/action/callhandler.py
+-rw-r--r--   0 root         (0) root         (0)     1030 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/action/callmanager.py
+-rw-r--r--   0 root         (0) root         (0)     8117 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/action/cmdrunnerbasedcallmanager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.746397 XGEE-0.3.7/xgee/eoqserver/eoq2/action/externalpy/
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/action/externalpy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24055 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/action/externalpy/externalpyscripthandler.py
+-rw-r--r--   0 root         (0) root         (0)     5080 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/action/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.747397 XGEE-0.3.7/xgee/eoqserver/eoq2/command/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/command/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9319 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/command/command.py
+-rw-r--r--   0 root         (0) root         (0)    64224 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/command/commandrunner.py
+-rw-r--r--   0 root         (0) root         (0)    43028 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/command/diff.py
+-rw-r--r--   0 root         (0) root         (0)      854 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/command/result.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.748397 XGEE-0.3.7/xgee/eoqserver/eoq2/domain/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/domain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/domain/cmdrunnerbaseddomain.py
+-rw-r--r--   0 root         (0) root         (0)      698 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/domain/domain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.748397 XGEE-0.3.7/xgee/eoqserver/eoq2/domain/local/
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/domain/local/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      699 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/domain/local/localmdbdomain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.749397 XGEE-0.3.7/xgee/eoqserver/eoq2/domain/multiprocessing/
+-rw-r--r--   0 root         (0) root         (0)       86 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/domain/multiprocessing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingcallmanager.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingdomainclient.py
+-rw-r--r--   0 root         (0) root         (0)     3535 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingdomainhost.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.750397 XGEE-0.3.7/xgee/eoqserver/eoq2/domain/remote/
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/domain/remote/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6884 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/domain/remote/websocketdomain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.750397 XGEE-0.3.7/xgee/eoqserver/eoq2/event/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/event/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6359 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/event/event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.751397 XGEE-0.3.7/xgee/eoqserver/eoq2/frame/
+-rw-r--r--   0 root         (0) root         (0)      127 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/frame/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/frame/domainframehandler.py
+-rw-r--r--   0 root         (0) root         (0)      458 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/frame/frame.py
+-rw-r--r--   0 root         (0) root         (0)      746 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/frame/framehandler.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/frame/multiversionframehandler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.752397 XGEE-0.3.7/xgee/eoqserver/eoq2/legacy/
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/legacy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12199 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/legacy/legacy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.753397 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/
+-rw-r--r--   0 root         (0) root         (0)       99 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      471 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/mdb.py
+-rw-r--r--   0 root         (0) root         (0)     2670 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/mdbaccessor.py
+-rw-r--r--   0 root         (0) root         (0)      266 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/nocodec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.755397 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/
+-rw-r--r--   0 root         (0) root         (0)      213 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.755397 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/constraintmodel/
+-rw-r--r--   0 root         (0) root         (0)      867 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/constraintmodel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1631 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/constraintmodel/constraintmodel.py
+-rw-r--r--   0 root         (0) root         (0)     1697 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/pyecoreidcodec.py
+-rw-r--r--   0 root         (0) root         (0)     2389 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/pyecoremdb.py
+-rw-r--r--   0 root         (0) root         (0)    36345 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/pyecoremdbaccessor.py
+-rw-r--r--   0 root         (0) root         (0)      518 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresimpleobjectcodec.py
+-rw-r--r--   0 root         (0) root         (0)     3823 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresinglefilemdb.py
+-rw-r--r--   0 root         (0) root         (0)     5811 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresinglefilemdbprovider.py
+-rw-r--r--   0 root         (0) root         (0)    80843 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/pyecoreworkspacemdbprovider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.756397 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/workspacemdbmodel/
+-rw-r--r--   0 root         (0) root         (0)     1326 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/workspacemdbmodel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5277 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/workspacemdbmodel/workspacemdbmodel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.756397 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/xmlresourcemodel/
+-rw-r--r--   0 root         (0) root         (0)     1092 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/xmlresourcemodel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3591 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/xmlresourcemodel/xmlresourcemodel.py
+-rw-r--r--   0 root         (0) root         (0)      175 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/valuecodec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.757397 XGEE-0.3.7/xgee/eoqserver/eoq2/query/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/query/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12347 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/query/query.py
+-rw-r--r--   0 root         (0) root         (0)    38368 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/query/queryrunner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.758396 XGEE-0.3.7/xgee/eoqserver/eoq2/serialization/
+-rw-r--r--   0 root         (0) root         (0)      204 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/serialization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/serialization/jsonserializer.py
+-rw-r--r--   0 root         (0) root         (0)     6755 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/serialization/jsserializer.py
+-rw-r--r--   0 root         (0) root         (0)     5871 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/serialization/pyserializer.py
+-rw-r--r--   0 root         (0) root         (0)      314 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/serialization/serializer.py
+-rw-r--r--   0 root         (0) root         (0)    35630 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/serialization/textserializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.760397 XGEE-0.3.7/xgee/eoqserver/eoq2/util/
+-rw-r--r--   0 root         (0) root         (0)      118 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2491 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/util/backup.py
+-rw-r--r--   0 root         (0) root         (0)     4033 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/util/benchmark.py
+-rw-r--r--   0 root         (0) root         (0)    13851 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/util/csvconnector.py
+-rw-r--r--   0 root         (0) root         (0)     1272 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/util/error.py
+-rw-r--r--   0 root         (0) root         (0)     4511 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/util/logger.py
+-rw-r--r--   0 root         (0) root         (0)     2634 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/util/model.py
+-rw-r--r--   0 root         (0) root         (0)     4037 2024-04-23 20:45:14.000000 XGEE-0.3.7/xgee/eoqserver/eoq2/util/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 20:45:15.760397 XGEE-0.3.7/xgee/meta/
+-rw-rw-rw-   0 root         (0) root         (0)     7875 2024-04-23 20:45:08.000000 XGEE-0.3.7/xgee/meta/layout.ecore
+-rw-rw-rw-   0 root         (0) root         (0)    11552 2024-04-23 20:45:08.000000 XGEE-0.3.7/xgee/xgee.py
```

### Comparing `XGEE-0.3.6/LICENSE` & `XGEE-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/PKG-INFO` & `XGEE-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XGEE
-Version: 0.3.6
+Version: 0.3.7
 Summary: eXtensible Graphical EMOF Editor - a framework for graphical editing single page web-applications
 Home-page: https://gitlab.com/xgee/py/xgee
 Author: Matthias Brunner
 Author-email: matthias.brunner@ils.uni-stuttgart.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `XGEE-0.3.6/README.md` & `XGEE-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/XGEE.egg-info/PKG-INFO` & `XGEE-0.3.7/XGEE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XGEE
-Version: 0.3.6
+Version: 0.3.7
 Summary: eXtensible Graphical EMOF Editor - a framework for graphical editing single page web-applications
 Home-page: https://gitlab.com/xgee/py/xgee
 Author: Matthias Brunner
 Author-email: matthias.brunner@ils.uni-stuttgart.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `XGEE-0.3.6/XGEE.egg-info/SOURCES.txt` & `XGEE-0.3.7/XGEE.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -409,14 +409,15 @@
 xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-ns.js
 xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-prefix-attribute.js
 xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-prefix.js
 xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-redefine.js
 xgee/core/plugins/ecoreDebuggerUi/js/ecoreDebuggerUiController.js
 xgee/core/plugins/ecoreSync/.git
 xgee/core/plugins/ecoreSync/LICENSE
+xgee/core/plugins/ecoreSync/README.md
 xgee/core/plugins/ecoreSync/ecoreSync.js
 xgee/core/plugins/ecoreSync/plugin.js
 xgee/core/plugins/ecoreSync.ui/plugin.js
 xgee/core/plugins/ecoreSync.ui/css/EObjectCtrls.css
 xgee/core/plugins/ecoreSync.ui/img/select-list-close-active.svg
 xgee/core/plugins/ecoreSync.ui/img/select-list-close.svg
 xgee/core/plugins/ecoreSync.ui/img/select-list-scope-custom-active.svg
```

### Comparing `XGEE-0.3.6/setup.py` & `XGEE-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/LICENSE` & `XGEE-0.3.7/xgee/core/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/README.md` & `XGEE-0.3.7/xgee/core/README.md`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/bluebird/bluebird.js` & `XGEE-0.3.7/xgee/core/dep/bluebird/bluebird.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/bluebird/bluebird.min.js` & `XGEE-0.3.7/xgee/core/dep/bluebird/bluebird.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/LICENSE.txt` & `XGEE-0.3.7/xgee/core/dep/font-awesome/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/css/all.css` & `XGEE-0.3.7/xgee/core/dep/font-awesome/css/all.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/css/all.min.css` & `XGEE-0.3.7/xgee/core/dep/font-awesome/css/all.min.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/css/brands.css` & `XGEE-0.3.7/xgee/core/dep/font-awesome/css/brands.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/css/brands.min.css` & `XGEE-0.3.7/xgee/core/dep/font-awesome/css/brands.min.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/css/fontawesome.css` & `XGEE-0.3.7/xgee/core/dep/font-awesome/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/css/fontawesome.min.css` & `XGEE-0.3.7/xgee/core/dep/font-awesome/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/css/regular.css` & `XGEE-0.3.7/xgee/core/dep/font-awesome/css/regular.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/css/regular.min.css` & `XGEE-0.3.7/xgee/core/dep/font-awesome/css/regular.min.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/css/solid.css` & `XGEE-0.3.7/xgee/core/dep/font-awesome/css/solid.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/css/solid.min.css` & `XGEE-0.3.7/xgee/core/dep/font-awesome/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/css/svg-with-js.css` & `XGEE-0.3.7/xgee/core/dep/font-awesome/css/svg-with-js.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/css/svg-with-js.min.css` & `XGEE-0.3.7/xgee/core/dep/font-awesome/css/svg-with-js.min.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/css/v4-shims.css` & `XGEE-0.3.7/xgee/core/dep/font-awesome/css/v4-shims.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/css/v4-shims.min.css` & `XGEE-0.3.7/xgee/core/dep/font-awesome/css/v4-shims.min.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/js/all.js` & `XGEE-0.3.7/xgee/core/dep/font-awesome/js/all.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/js/all.min.js` & `XGEE-0.3.7/xgee/core/dep/font-awesome/js/all.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/js/brands.js` & `XGEE-0.3.7/xgee/core/dep/font-awesome/js/brands.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/js/brands.min.js` & `XGEE-0.3.7/xgee/core/dep/font-awesome/js/brands.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/js/conflict-detection.js` & `XGEE-0.3.7/xgee/core/dep/font-awesome/js/conflict-detection.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/js/conflict-detection.min.js` & `XGEE-0.3.7/xgee/core/dep/font-awesome/js/conflict-detection.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/js/fontawesome.js` & `XGEE-0.3.7/xgee/core/dep/font-awesome/js/fontawesome.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/js/fontawesome.min.js` & `XGEE-0.3.7/xgee/core/dep/font-awesome/js/fontawesome.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/js/regular.js` & `XGEE-0.3.7/xgee/core/dep/font-awesome/js/regular.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/js/regular.min.js` & `XGEE-0.3.7/xgee/core/dep/font-awesome/js/regular.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/js/solid.js` & `XGEE-0.3.7/xgee/core/dep/font-awesome/js/solid.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/js/solid.min.js` & `XGEE-0.3.7/xgee/core/dep/font-awesome/js/solid.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/js/v4-shims.js` & `XGEE-0.3.7/xgee/core/dep/font-awesome/js/v4-shims.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/js/v4-shims.min.js` & `XGEE-0.3.7/xgee/core/dep/font-awesome/js/v4-shims.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-brands-400.eot` & `XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-brands-400.svg` & `XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-brands-400.ttf` & `XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-brands-400.woff` & `XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-brands-400.woff2` & `XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-regular-400.eot` & `XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-regular-400.svg` & `XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-regular-400.ttf` & `XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-regular-400.woff` & `XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-regular-400.woff2` & `XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-solid-900.eot` & `XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-solid-900.svg` & `XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-solid-900.ttf` & `XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-solid-900.woff` & `XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/font-awesome/webfonts/fa-solid-900.woff2` & `XGEE-0.3.7/xgee/core/dep/font-awesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/LICENSE` & `XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.eot` & `XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.eot`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.ttf` & `XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.ttf`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.woff` & `XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.woff`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.woff2` & `XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/font/context-menu-icons.woff2`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.css` & `XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.js` & `XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.css` & `XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.css.map` & `XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.css.map`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.js` & `XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.js.map` & `XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/jquery.contextMenu.min.js.map`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/jquery.ui.position.js` & `XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/jquery.ui.position.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jQuery-contextMenu-2.8/jquery.ui.position.min.js` & `XGEE-0.3.7/xgee/core/dep/jQuery-contextMenu-2.8/jquery.ui.position.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jquery/LICENSE.txt` & `XGEE-0.3.7/xgee/core/dep/jquery/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jquery/jquery-3.3.1.min.js` & `XGEE-0.3.7/xgee/core/dep/jquery/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jquery-ui/LICENSE.txt` & `XGEE-0.3.7/xgee/core/dep/jquery-ui/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jquery-ui/images/ui-icons_444444_256x240.png` & `XGEE-0.3.7/xgee/core/dep/jquery-ui/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jquery-ui/images/ui-icons_555555_256x240.png` & `XGEE-0.3.7/xgee/core/dep/jquery-ui/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jquery-ui/images/ui-icons_777620_256x240.png` & `XGEE-0.3.7/xgee/core/dep/jquery-ui/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jquery-ui/images/ui-icons_777777_256x240.png` & `XGEE-0.3.7/xgee/core/dep/jquery-ui/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jquery-ui/images/ui-icons_cc0000_256x240.png` & `XGEE-0.3.7/xgee/core/dep/jquery-ui/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jquery-ui/images/ui-icons_ffffff_256x240.png` & `XGEE-0.3.7/xgee/core/dep/jquery-ui/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jquery-ui/jquery-ui.min.css` & `XGEE-0.3.7/xgee/core/dep/jquery-ui/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jquery-ui/jquery-ui.min.js` & `XGEE-0.3.7/xgee/core/dep/jquery-ui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/CHANGELOG.md` & `XGEE-0.3.7/xgee/core/dep/jsa/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/LICENSE` & `XGEE-0.3.7/xgee/core/dep/jsa/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/README.md` & `XGEE-0.3.7/xgee/core/dep/jsa/README.md`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/black/bubble-hover.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/black/bubble-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/black/bubble.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/black/bubble.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/black/close-hover.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/black/close-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/black/close.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/black/close.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/black/folder.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/black/folder.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/black/home.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/black/home.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/black/jsa.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/black/jsa.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/black/maximize-hover.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/black/maximize-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/black/maximize.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/black/maximize.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/black/menu-hover.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/black/menu-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/black/menu.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/black/menu.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/black/minimize-hover.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/black/minimize-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/black/minimize.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/black/minimize.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/black/redo.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/black/redo.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/black/settings.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/black/settings.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/black/undo.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/black/undo.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/black/view-hover.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/black/view-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/black/view.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/black/view.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/close-hover.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/close-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/close.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/close.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/jsa.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/jsa.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/loading.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/loading.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/maximize.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/maximize.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/minimize.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/minimize.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/resize-ne.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/resize-ne.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/resize-nw.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/resize-nw.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/resize-se.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/resize-se.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/resize-sw.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/resize-sw.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/restore.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/restore.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/tool-default.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/tool-default.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/view-close.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/view-close.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/white/bubble-hover.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/white/bubble-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/white/bubble.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/white/bubble.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/white/close-hover.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/white/close-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/white/close.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/white/close.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/white/folder.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/white/folder.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/white/home.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/white/home.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/white/jsa.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/white/jsa.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/white/maximize-hover.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/white/maximize-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/white/maximize.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/white/maximize.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/white/menu-hover.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/white/menu-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/white/menu.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/white/menu.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/white/minimize-hover.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/white/minimize-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/white/minimize.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/white/minimize.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/white/redo.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/white/redo.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/white/settings.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/white/settings.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/white/undo.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/white/undo.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/white/view-hover.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/white/view-hover.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/img/white/view.svg` & `XGEE-0.3.7/xgee/core/dep/jsa/img/white/view.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/jsapplication.css` & `XGEE-0.3.7/xgee/core/dep/jsa/jsapplication.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/jsapplication.js` & `XGEE-0.3.7/xgee/core/dep/jsa/jsapplication.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/jsapplicationPlugins.js` & `XGEE-0.3.7/xgee/core/dep/jsa/jsapplicationPlugins.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/jsa/webpack.config.js` & `XGEE-0.3.7/xgee/core/dep/jsa/webpack.config.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/LICENSE` & `XGEE-0.3.7/xgee/core/dep/mxgraph/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/css/common.css` & `XGEE-0.3.7/xgee/core/dep/mxgraph/css/common.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/images/collapsed.gif` & `XGEE-0.3.7/xgee/core/dep/mxgraph/images/collapsed.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/images/error.gif` & `XGEE-0.3.7/xgee/core/dep/mxgraph/images/error.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/images/expanded.gif` & `XGEE-0.3.7/xgee/core/dep/mxgraph/images/expanded.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/images/maximize.gif` & `XGEE-0.3.7/xgee/core/dep/mxgraph/images/maximize.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/images/normalize.gif` & `XGEE-0.3.7/xgee/core/dep/mxgraph/images/normalize.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/editor/mxDefaultKeyHandler.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/editor/mxDefaultKeyHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/editor/mxDefaultPopupMenu.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/editor/mxDefaultPopupMenu.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/editor/mxDefaultToolbar.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/editor/mxDefaultToolbar.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/editor/mxEditor.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/editor/mxEditor.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxCellHighlight.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxCellHighlight.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxCellMarker.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxCellMarker.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxCellTracker.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxCellTracker.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxConnectionHandler.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxConnectionHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxConstraintHandler.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxConstraintHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxEdgeHandler.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxEdgeHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxEdgeSegmentHandler.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxEdgeSegmentHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxElbowEdgeHandler.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxElbowEdgeHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxGraphHandler.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxGraphHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxHandle.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxHandle.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxKeyHandler.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxKeyHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxPanningHandler.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxPanningHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxPopupMenuHandler.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxPopupMenuHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxRubberband.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxRubberband.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxSelectionCellsHandler.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxSelectionCellsHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxTooltipHandler.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxTooltipHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/handler/mxVertexHandler.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/handler/mxVertexHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/index.txt` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/index.txt`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxCellCodec.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxCellCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxChildChangeCodec.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxChildChangeCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxCodec.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxCodecRegistry.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxCodecRegistry.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxDefaultKeyHandlerCodec.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxDefaultKeyHandlerCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxDefaultPopupMenuCodec.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxDefaultPopupMenuCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxDefaultToolbarCodec.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxDefaultToolbarCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxEditorCodec.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxEditorCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxGenericChangeCodec.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxGenericChangeCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxGraphCodec.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxGraphCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxGraphViewCodec.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxGraphViewCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxModelCodec.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxModelCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxObjectCodec.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxObjectCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxRootChangeCodec.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxRootChangeCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxStylesheetCodec.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxStylesheetCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/io/mxTerminalChangeCodec.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/io/mxTerminalChangeCodec.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphAbstractHierarchyCell.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphAbstractHierarchyCell.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyEdge.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyEdge.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyModel.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyModel.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyNode.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxGraphHierarchyNode.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxSwimlaneModel.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/model/mxSwimlaneModel.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/mxHierarchicalLayout.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/mxHierarchicalLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/mxSwimlaneLayout.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/mxSwimlaneLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxCoordinateAssignment.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxCoordinateAssignment.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxHierarchicalLayoutStage.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxHierarchicalLayoutStage.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxMedianHybridCrossingReduction.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxMedianHybridCrossingReduction.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxMinimumCycleRemover.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxMinimumCycleRemover.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxSwimlaneOrdering.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/hierarchical/stage/mxSwimlaneOrdering.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/mxCircleLayout.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/mxCircleLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/mxCompactTreeLayout.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/mxCompactTreeLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/mxCompositeLayout.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/mxCompositeLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/mxEdgeLabelLayout.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/mxEdgeLabelLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/mxFastOrganicLayout.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/mxFastOrganicLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/mxGraphLayout.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/mxGraphLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/mxParallelEdgeLayout.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/mxParallelEdgeLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/mxPartitionLayout.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/mxPartitionLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/mxRadialTreeLayout.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/mxRadialTreeLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/layout/mxStackLayout.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/layout/mxStackLayout.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/model/mxCell.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/model/mxCell.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/model/mxCellPath.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/model/mxCellPath.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/model/mxGeometry.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/model/mxGeometry.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/model/mxGraphModel.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/model/mxGraphModel.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/mxClient.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/mxClient.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxActor.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxActor.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxArrow.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxArrow.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxArrowConnector.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxArrowConnector.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxCloud.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxCloud.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxConnector.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxConnector.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxCylinder.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxCylinder.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxDoubleEllipse.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxDoubleEllipse.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxEllipse.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxEllipse.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxHexagon.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxHexagon.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxImageShape.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxImageShape.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxLabel.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxLabel.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxLine.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxLine.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxMarker.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxMarker.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxPolyline.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxPolyline.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxRectangleShape.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxRectangleShape.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxRhombus.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxRhombus.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxShape.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxShape.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxStencil.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxStencil.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxStencilRegistry.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxStencilRegistry.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxSwimlane.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxSwimlane.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxText.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxText.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/shape/mxTriangle.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/shape/mxTriangle.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxAbstractCanvas2D.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxAbstractCanvas2D.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxAnimation.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxAnimation.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxAutoSaveManager.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxAutoSaveManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxClipboard.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxClipboard.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxConstants.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxConstants.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxDictionary.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxDictionary.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxDivResizer.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxDivResizer.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxDragSource.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxDragSource.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxEffects.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxEffects.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxEvent.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxEvent.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxEventObject.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxEventObject.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxEventSource.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxEventSource.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxForm.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxForm.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxGuide.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxGuide.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxImage.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxImage.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxImageBundle.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxImageBundle.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxImageExport.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxImageExport.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxLog.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxLog.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxMorphing.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxMorphing.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxMouseEvent.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxMouseEvent.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxObjectIdentity.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxObjectIdentity.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxPanningManager.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxPanningManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxPoint.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxPoint.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxPopupMenu.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxPopupMenu.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxRectangle.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxRectangle.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxResources.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxResources.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxSvgCanvas2D.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxSvgCanvas2D.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxToolbar.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxToolbar.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxUndoManager.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxUndoManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxUndoableEdit.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxUndoableEdit.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxUrlConverter.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxUrlConverter.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxUtils.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxUtils.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxVmlCanvas2D.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxVmlCanvas2D.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxWindow.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxWindow.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxXmlCanvas2D.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxXmlCanvas2D.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/util/mxXmlRequest.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/util/mxXmlRequest.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxCellEditor.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxCellEditor.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxCellOverlay.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxCellOverlay.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxCellRenderer.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxCellRenderer.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxCellState.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxCellState.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxCellStatePreview.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxCellStatePreview.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxConnectionConstraint.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxConnectionConstraint.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxEdgeStyle.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxEdgeStyle.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxGraph.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxGraph.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxGraphSelectionModel.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxGraphSelectionModel.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxGraphView.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxGraphView.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxLayoutManager.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxLayoutManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxMultiplicity.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxMultiplicity.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxOutline.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxOutline.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxPerimeter.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxPerimeter.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxPrintPreview.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxPrintPreview.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxStyleRegistry.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxStyleRegistry.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxStylesheet.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxStylesheet.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxSwimlaneManager.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxSwimlaneManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/mxgraph/js/view/mxTemporaryCellStates.js` & `XGEE-0.3.7/xgee/core/dep/mxgraph/js/view/mxTemporaryCellStates.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/notifyjs/notify.min.js` & `XGEE-0.3.7/xgee/core/dep/notifyjs/notify.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/underscore/LICENSE` & `XGEE-0.3.7/xgee/core/dep/underscore/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/dep/underscore/underscore-min.js` & `XGEE-0.3.7/xgee/core/dep/underscore/underscore-min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/autostart/js/AppStartupEvent.js` & `XGEE-0.3.7/xgee/core/plugins/autostart/js/AppStartupEvent.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/autostart/js/AppStartupObserver.js` & `XGEE-0.3.7/xgee/core/plugins/autostart/js/AppStartupObserver.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/autostart/js/Autostarter.js` & `XGEE-0.3.7/xgee/core/plugins/autostart/js/Autostarter.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/autostart/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/autostart/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/clipboard/js/AppClipboard.js` & `XGEE-0.3.7/xgee/core/plugins/clipboard/js/AppClipboard.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/clipboard/js/Clipboard.js` & `XGEE-0.3.7/xgee/core/plugins/clipboard/js/Clipboard.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/clipboard/js/ClipboardAPI.js` & `XGEE-0.3.7/xgee/core/plugins/clipboard/js/ClipboardAPI.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/clipboard/js/ClipboardEventHandler.js` & `XGEE-0.3.7/xgee/core/plugins/clipboard/js/ClipboardEventHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/clipboard/js/ClipboardManager.js` & `XGEE-0.3.7/xgee/core/plugins/clipboard/js/ClipboardManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/clipboard/js/EcoreClipboardEvaluator.js` & `XGEE-0.3.7/xgee/core/plugins/clipboard/js/EcoreClipboardEvaluator.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/clipboard/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/clipboard/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/contextMenu/js/ContextMenu.js` & `XGEE-0.3.7/xgee/core/plugins/contextMenu/js/ContextMenu.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/contextMenu/js/util.js` & `XGEE-0.3.7/xgee/core/plugins/contextMenu/js/util.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/contextMenu/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/contextMenu/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/contextMenu.ecore/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/contextMenu.ecore/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/contextMenu.eoq/js/util.js` & `XGEE-0.3.7/xgee/core/plugins/contextMenu.eoq/js/util.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/contextMenu.eoq/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/contextMenu.eoq/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/LICENSE` & `XGEE-0.3.7/xgee/core/plugins/ecore/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/ecore.xmi.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/ecore.xmi.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/LICENSE` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/README.md` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/README.md`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/examples/big-not-pretty.xml` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/examples/big-not-pretty.xml`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/examples/example.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/examples/example.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/examples/get-products.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/examples/get-products.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/examples/pretty-print.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/examples/pretty-print.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/examples/shopping.xml` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/examples/shopping.xml`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/examples/test.xml` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/examples/test.xml`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/lib/sax.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/lib/sax.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/package-lock.json` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/package-lock.json`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/package.json` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/package.json`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/attribute-name.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/attribute-name.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/attribute-no-space.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/attribute-no-space.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/attribute-unquoted.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/attribute-unquoted.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/bom.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/bom.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/buffer-overrun.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/buffer-overrun.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/case.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/case.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/cdata-fake-end.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/cdata-fake-end.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/cdata-multiple.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/cdata-multiple.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/index.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/index.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/issue-23.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/issue-23.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/issue-30.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/issue-30.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/issue-49.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/issue-49.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/issue-86.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/issue-86.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/opentagstart.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/opentagstart.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/parser-position.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/parser-position.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/script-close-better.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/script-close-better.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/script.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/script.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/self-closing-child-strict.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/self-closing-child-strict.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/self-closing-child.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/self-closing-child.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/self-closing-tag.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/self-closing-tag.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/stray-ending.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/stray-ending.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/unquoted.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/unquoted.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/utf8-split.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/utf8-split.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/xml-internal-entities.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/xml-internal-entities.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/xmlns-issue-41.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/xmlns-issue-41.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/xmlns-rebinding.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/xmlns-rebinding.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/xmlns-strict.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/xmlns-strict.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/xmlns-unbound-element.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/xmlns-unbound-element.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/xmlns-unbound.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/xmlns-unbound.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-ns.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-ns.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-prefix-attribute.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-prefix-attribute.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-redefine.js` & `XGEE-0.3.7/xgee/core/plugins/ecore/sax-js-master/test/xmlns-xml-default-redefine.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/LICENSE` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/changes/esChanges.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/changes/esChanges.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -277,12 +277,12 @@
     }
 
     markChangeIdAsLocal(changeId) {
         this.localChanges.add(changeId);
     }
 
     syncToChangeId(changeId) {
-        return Promise.reject('placeholder for future use');
+        return Promise.reject(new Error('placeholder for future use'));
     }
 
 
 }
```

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/dev/esDebugging.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/dev/esDebugging.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/dev/lib/libesync.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/dev/lib/libesync.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/domain/esDomain.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/domain/esDomain.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/domain/esLookup.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/domain/esLookup.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/domain/esMetaSync.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/domain/esMetaSync.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/domain/esObjectAccessors.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/domain/esObjectAccessors.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/domain/esOperationHandler.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/domain/esOperationHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/ecoreSync.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/ecoreSync.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/interfaces/esInstance.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/interfaces/esInstance.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/mdb/esMdbAccessor.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/mdb/esMdbAccessor.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/mdb/esMdbObserver.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/mdb/esMdbObserver.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/mdb/esModelDatabase.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/mdb/esModelDatabase.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/mdb/esSyncEvents.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/mdb/esSyncEvents.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/mdb/esSyncStatus.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/mdb/esSyncStatus.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/queries/esCmdRunner.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/queries/esCmdRunner.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -96,17 +96,17 @@
         }
 
         return res
     }
 
     async StartTransaction() {
         await this.mdbAccessor.Lock()
-        if ($DEBUG) console.debug("Local transaction id=" + tid + " started")
         this.latestTransactionId += 1
         var tid = this.latestTransactionId
+        if ($DEBUG) console.debug("Local transaction id=" + tid + " started")
         this.tempHistoryForTransaction[tid] = []
         return tid
     }
 
     async EndTransaction(res, tid) {
         await this.mdbAccessor.Release()
         if ($DEBUG) console.debug("Local transaction id=" + tid + " complete")
```

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/queries/esQueries.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/queries/esQueries.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/queries/esQueryEvaluator.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/queries/esQueryEvaluator.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/queries/esQueryObserver.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/queries/esQueryObserver.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/queries/esQueryObserverState.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/queries/esQueryObserverState.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/queries/esQueryUtils.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/queries/esQueryUtils.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/util/auxiliaries.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/util/auxiliaries.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/util/esUtils.js` & `XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView.eoq/plugin.js`

 * *Files 27% similar despite different names*

#### js-beautify {}

```diff
@@ -1,450 +1,444 @@
-class EsUtilities {
-    constructor(esDomain) {
-        this._esDomain = esDomain;
-        this.builtInClasses = []
-    }
+export function init(pluginAPI) {
 
-    init() {
-        this.builtInClasses = this.getBuiltInClasses();
-    }
+    var WorkspaceView = function(iconPath) {
+        var self = this;
+        this.iconPath = iconPath;
+        this.apply = function(data) {
+            var view = {};
+            if (data.type == 'eObject') {
+                switch (data.value.eClass.get("name")) {
+                    case 'Workspace':
+                        view = {
+                            title: 'Workspace',
+                            folder: true,
+                            eObject: data.value,
+                            modifiers: data.modifiers,
+                            lazy: true
+                        };
+                        break;
+                    case 'Directory':
+                        view = {
+                            title: data.value.get("name"),
+                            folder: true,
+                            eObject: data.value,
+                            modifiers: data.modifiers,
+                            lazy: true
+                        };
+                        break;
+                    case 'ModelResource':
+                        view = {
+                            title: data.value.get("name"),
+                            eObject: data.value,
+                            modifiers: data.modifiers,
+                            lazy: true
+                        };
+                        break;
+                }
+            }
+            return view;
+        };
 
-    getBuiltInClasses() {
-        return Object.values(this._esDomain.getEcore()).filter((val) => {
-            return val.eClass ? true : false
-        })
-    }
+        this.canDisplay = function(data) {
+            if (data.type != 'eObject') {
+                return false;
+            } else {
+                var displayableClasses = [{
+                    name: 'Workspace',
+                    nsURI: "http://www.eoq.de/workspacemdbmodel/v1.0"
+                }, {
+                    name: 'Directory',
+                    nsURI: "http://www.eoq.de/workspacemdbmodel/v1.0"
+                }, {
+                    name: 'ModelResource',
+                    nsURI: "http://www.eoq.de/workspacemdbmodel/v1.0"
+                }];
+                if (data.value) {
+                    if (displayableClasses.find(function(e) {
+                            return e.name == data.value.eClass.get("name") && e.nsURI == data.value.eClass.eContainer.get("nsURI")
+                        })) {
+                        return true;
+                    }
+                } else {
+                    console.error(data)
+                }
 
-    async isEClassInitialized(eClass) {
-        var oid = this._esDomain.rlookup(eClass);
-        if (oid != null) {
-            return this._esDomain.initEClass(oid, true);
+            }
         }
     }
 
-    isContained(eContainer, featureName, eObject) {
-        var res = false;
-        if (eContainer.get(featureName).array().includes(eObject)) {
-            res = true;
+    var WorkspaceController = function(ecoreSync) {
+        var ecoreSync = ecoreSync;
+        var self = this;
+        this.onUpdate = function(parentEObject, eObject, callbackFcn) {
+            eObject.on('add:subdirectories', function() {
+                self.load(parentEObject, eObject).then(function(loadedData) {
+                    callbackFcn(loadedData);
+                })
+            });
+            eObject.on('add:resources', function() {
+                self.load(parentEObject, eObject).then(function(loadedData) {
+                    callbackFcn(loadedData);
+                })
+            })
+            eObject.on('remove:subdirectories', function() {
+                self.load(parentEObject, eObject).then(function(loadedData) {
+                    callbackFcn(loadedData);
+                })
+            });
+            eObject.on('remove:resources', function() {
+                self.load(parentEObject, eObject).then(function(loadedData) {
+                    callbackFcn(loadedData);
+                })
+            })
         }
-        return res;
-    }
 
-    isLocalEcoreElement(name) {
-        let res = false;
-        if (name == 'EInteger') name = 'EInt'
-        var keys = Object.keys(this._esDomain.getEcore());
-        if (keys.includes(name)) {
-            res = true;
+        this.onChange = function(data, callbackFcn) {
+            if (data.type = 'eObject') {
+                data.value.on('change', function() {
+                    callbackFcn(data.value)
+                });
+            }
         }
-        return res;
-    }
 
-    getLocalEcoreElement(name) {
-        let res = null;
-        if (name == 'EInteger') name = 'EInt'
-        var keys = Object.keys(this._esDomain.getEcore());
-        if (keys.includes(name)) {
-            res = this._esDomain.getEcore()[name]
+        this.canLoad = function(data) {
+            return data.node.data.eObject.eClass.eContainer.get("nsURI") == 'http://www.eoq.de/workspacemdbmodel/v1.0' && data.node.data.eObject.eClass.get('name') == 'Workspace';
         }
-        return res;
-    }
 
-    checkType(eType, value) {
-        //ecoreSync integrated type checking
-        var res = false;
-        var typeName = ''
-
-        switch (eType.eClass.get('name')) {
-            case "EDataType":
-                typeName = eType.get('name')
-                break;
-            case "EEnum":
-                typeName = 'EEnum'
-                break;
-            default:
-                typeName = 'unsupported'
-                break;
-        }
+        this.load = function(parentEObject, eObject) {
+            var load = [];
+            switch (eObject.eClass.get("name")) {
+                default:
+                    load = ecoreSync.utils.isEClassInitialized(eObject.eClass).then(function() {
+                        var subdirectories = ecoreSync.get(eObject, "subdirectories").then(function(results) {
+                            return Promise.all(results.map(function(e) {
+                                return ecoreSync.get(e, "name");
+                            })).then(function() {
+                                return Promise.resolve(results.map(function(e) {
+                                    return {
+                                        type: 'eObject',
+                                        value: e,
+                                        modifiers: {}
+                                    }
+                                }));
+                            });
+                        });
+
+                        var resources = ecoreSync.get(eObject, "resources").then(function(results) {
+                            return Promise.all(results.map(function(e) {
+                                return ecoreSync.get(e, "name");
+                            })).then(function() {
+                                return Promise.resolve(results.map(function(e) {
+                                    return {
+                                        type: 'eObject',
+                                        value: e,
+                                        modifiers: {}
+                                    }
+                                }));
+                            });
+                        });
+
+                        return Promise.all([subdirectories, resources]).then(function(values) {
+                            var contents = values[0];
+                            contents = contents.concat(values[1]);
+                            return Promise.resolve(contents);
+                        });
+
+                    });
+            }
+
+            return load;
+        };
+    };
 
-        switch (typeName) {
-            case "EChar":
-                if (typeof value == 'string' && value.length == 1) res = true;
-                break;
-            case "EString":
-                if (typeof value == 'string') res = true;
-                break;
-            case "EInt":
-                if (Number.isInteger(value) && value != null) res = true;
-                break;
-            case "EByte":
-                if (Number.isInteger(value) && value != null) res = true;
-                break;
-            case "EFloat":
-                if (typeof value == 'number' && value != null) res = true;
-                break;
-            case "EDouble":
-                if (typeof value == 'number' && value != null) res = true;
-                break;
-            case "EBoolean":
-                if (typeof value == 'boolean') res = true;
-                break;
-            case "EEnum":
-                if (typeof value == 'string') res = true; //because EOQ expects it like this
-                break;
-            case "EInteger": //ecorejs compatibility support
-                if (Number.isInteger(value) && value != null) res = true;
-                break;
-            default:
-                res = true; //seems to be custom type, we won't bother with that
-                break;
-        }
-        return res;
-    }
+    var DirectoryController = function(ecoreSync) {
+        var ecoreSync = ecoreSync;
+        var self = this;
+        this.onUpdate = function(parentEObject, eObject, callbackFcn) {
+            eObject.on('add:subdirectories', function() {
+
+                self.load(parentEObject, eObject).then(function(loadedData) {
+                    callbackFcn(loadedData);
+                })
+            });
+            eObject.on('add:resources', function() {
 
-    valueToQuery(eType, value) {
-        var res = null;
+                self.load(parentEObject, eObject).then(function(loadedData) {
+                    callbackFcn(loadedData);
+                })
+            })
+            eObject.on('remove:subdirectories', function() {
+
+                self.load(parentEObject, eObject).then(function(loadedData) {
+                    callbackFcn(loadedData);
+                })
+            });
+            eObject.on('remove:resources', function() {
 
-        if (this.checkType(eType, value)) {
+                self.load(parentEObject, eObject).then(function(loadedData) {
+                    callbackFcn(loadedData);
+                })
+            })
+        }
 
-            var typeName = ''
-            switch (eType.eClass.get('name')) {
-                case "EDataType":
-                    typeName = eType.get('name')
-                    break;
-                case "EEnum":
-                    typeName = 'EEnum'
-                    break;
-                default:
-                    typeName = 'unsupported'
-                    break;
+        this.onChange = function(data, callbackFcn) {
+            if (data.type = 'eObject') {
+                data.value.on('change', function() {
+                    callbackFcn(data.value)
+                });
             }
+        }
 
-            switch (typeName) {
-                case "EChar":
-                    res = value;
-                    break;
-                case "EString":
-                    res = String(value);
-                    break;
-                case "EInt":
-                    res = value;
-                    break;
-                case "EByte":
-                    res = value;
-                    break;
-                case "EFloat":
-                    res = value;
-                    if (Number.isInteger(value)) res += 1e-5;
-                    break;
-                case "EDouble":
-                    res = value;
-                    if (Number.isInteger(value)) res += 1e-5;
-                    break;
-                case "EBoolean":
-                    res = value;
-                    break;
-                case "EEnum":
-                    res = value;
-                    break;
-                case "EInteger": //ecorejs compatibility support
-                    res = value;
-                    break;
-                default:
-                    if (value != null) {
-                        let oid = this._esDomain.rlookup(value);
-                        if (oid != null) {
-                            res = QRY.Obj(oid);
-                        } else {
-                            throw 'unknown datatype conversion'
-                        }
-                    } else {
-                        res = value //no conversion of null value
-                    }
-                    break;
-            }
-        } else {
-            throw 'supplied value was of incompatible type'
+        this.canLoad = function(data) {
+            return data.node.data.eObject.eClass.eContainer.get("nsURI") == 'http://www.eoq.de/workspacemdbmodel/v1.0' && data.node.data.eObject.eClass.get('name') == 'Directory';
         }
-        return res;
-    }
 
-    isBuiltInClass(eClass) {
-        let res = this.builtInClasses.find((clazz) => {
-            return clazz == eClass
-        }) ? true : false
-        return res
-    }
+        this.load = function(parentEObject, eObject) {
+            var load = [];
+            switch (eObject.eClass.get("name")) {
+                default:
+                    load = ecoreSync.utils.isEClassInitialized(eObject.eClass).then(function() {
 
-    isObjectURL(url) {
-        var res = false;
-        if (typeof url == 'string') {
-            if (url.includes('eoq://') && url.includes('/#')) {
-                res = true;
-            }
-        }
-        return res;
-    }
+                        var subdirectories = ecoreSync.get(eObject, "subdirectories").then(function(results) {
+                            return Promise.all(results.map(function(e) {
+                                return ecoreSync.get(e, "name");
+                            })).then(function() {
+                                return Promise.resolve(results.map(function(e) {
+                                    return {
+                                        type: 'eObject',
+                                        value: e,
+                                        modifiers: {}
+                                    }
+                                }));
+                            });
+                        });
 
-    getObjectURL(eObject) {
-        var oid = this._esDomain.rlookup(eObject);
-        if (oid == null) throw 'the supplied eObject is unknown to ecoreSync'
-        return (this._esDomain.eoq2domain.url + '/#' + oid).replace('ws://', 'eoq://').replace('ws/eoq.do/', '');
-    }
+                        var resources = ecoreSync.get(eObject, "resources").then(function(results) {
+                            return Promise.all(results.map(function(e) {
+                                return ecoreSync.get(e, "name");
+                            })).then(function() {
+                                return Promise.resolve(results.map(function(e) {
+                                    return {
+                                        type: 'eObject',
+                                        value: e,
+                                        modifiers: {}
+                                    }
+                                }));
+                            });
+                        });
+
+                        return Promise.all([subdirectories, resources]).then(function(values) {
 
-    async getObjectByURL(url) {
-        var res = null;
-        if (this.isObjectURL(url)) {
-            let domainHost = url.substr(url.indexOf('eoq://') + 6, url.indexOf('/#') - (url.indexOf('eoq://') + 6));
-            if (this._esDomain.eoq2domain.url.includes(domainHost)) {
-                let objId = Number.parseInt(url.substr(url.indexOf('/#') + 2));
-                res = this._esDomain.getObject(objId);
+                                var contents = values[0];
+                                contents = contents.concat(values[1]);
+                                return Promise.resolve(contents);
+                            },
+                            function(msg) {
+                                console.error('failed to load')
+                            });
+
+                    });
             }
-            return res;
-        }
-    }
 
-    async getResource(eObject) {
-        //gets the  EOQ resource containing the supplied eObject
-        let oid = this._esDomain.rlookup(eObject);
-        if (oid == null) throw 'the supplied eObject is unknown to ecoreSync'
-        let cmd = CMD.Get(QRY.Obj(oid).Met("ALLPARENTS").Sel(new eoq2.Qry().Met("CLASSNAME").Equ("ModelResource")).Trm(new eoq2.Met('SIZE').Equ(0), null).Idx(0));
-        let mdlResource = await this._esDomain.remoteExec(cmd, true);
-        return mdlResource;
-    }
+            return load;
+        };
 
-    async getModelRoot(eObject) {
-        //gets the  EOQ resource containing the supplied eObject
-        let oid = this._esDomain.rlookup(eObject);
-        if (oid == null) throw 'the supplied eObject is unknown to ecoreSync'
-        let cmd = CMD.Get(QRY.Obj(oid).Met("ALLPARENTS").Sel(new eoq2.Qry().Met("CLASSNAME").Equ("ModelResource")).Trm(new eoq2.Met('SIZE').Equ(0), null).Idx(0).Pth('contents').Trm(new eoq2.Met('SIZE').Equ(0), null).Idx(0));
-        let mdlRoot = await this._esDomain.remoteExec(cmd, true);
-        return mdlRoot;
-    }
 
-    async getContainer(eObject) {
-        //gets the eContainer of the supplied object
-        var res = null;
-        if (eObject.eContainer) {
-            res = eObject.eContainer;
-        } else {
-            let oid = this._esDomain.rlookup(eObject);
-            if (!oid) throw 'the supplied eObject is unknown to ecoreSync'
-            let cmd = CMD.Get(QRY.Obj(oid).Met("PARENT"));
-            res = await this._esDomain.remoteExec(cmd, true);
+    };
+
+
+
+    var ResourceController = function(ecoreSync) {
+        var ecoreSync = ecoreSync;
+        this.canLoad = function(data) {
+            return data.node.data.eObject.eClass.eContainer.get("nsURI") == 'http://www.eoq.de/workspacemdbmodel/v1.0' && data.node.data.eObject.eClass.get('name') == 'ModelResource';
         }
-        return res;
-    }
 
-    async getObjectShortPath(eObject) {
-        //TODO: Update with new EOQ commands?
-        var res = '';
-        let oid = this._esDomain.rlookup(eObject);
-        if (!oid) throw 'the supplied eObject is unknown to ecoreSync'
-
-        let cmd = new eoq2.Cmp().Get(new eoq2.Qry().Obj(oid).Met("ALLPARENTS"))
-            .Get(new eoq2.Qry().His(-1).Pth("name"));
-
-        let val = await this._esDomain.eoq2domain.Do(cmd)
-        let pathSegments = [];
-        for (let j = 0; j < val[0].length; j++) {
-            let segmentName = val[1][j];
-            let segmentId = val[0][j].v;
-            pathSegments.push(segmentName ? segmentName : '#' + segmentId);
+        this.onUpdate = function() {
+            //ResourceController does not provide updates     
         }
-        res = pathSegments.join('/')
 
-        return res;
-    }
+        this.onChange = function() {
+            //ResourceController does not provide changes       
+        }
 
-    async getObjectStringPath(eObject) {
-        //TODO: Update with new EOQ commands?
-        var res = '';
-        let oid = this._esDomain.rlookup(eObject);
-        if (!oid) throw 'the supplied eObject is unknown to ecoreSync'
-
-        if (oid != 0) {
-            //return the path to the object
-            let cmd = CMD.Cmp()
-                .Get(QRY.Obj(oid).Met("INDEX"))
-                .Get(QRY.Obj(oid).Met("CONTAININGFEATURE"))
-                .Get(QRY.His(-1).Pth("name"))
-                .Get(QRY.His(-2).Pth("upperBound"))
-                .Get(QRY.Obj(oid).Met("ALLPARENTS").Idx([1, -1, 1]))
-                .Get(QRY.His(-1).Met("INDEX"))
-                .Get(QRY.His(-2).Met("CONTAININGFEATURE"))
-                .Get(QRY.His(-1).Pth("name"))
-                .Get(QRY.His(-2).Pth("upperBound"))
-
-            let val = await this._esDomain.eoq2domain.Do(cmd)
-            var pathSegments = [];
-            //do the container segments first
-            var n = val[4].length;
-            for (var i = 0; i < n; i++) {
-                var index = val[5][i];
-                var featureName = val[7][i];
-                var upperBound = val[8][i];
-                var segmentStr = featureName;
-                if (upperBound != 1) {
-                    segmentStr += '.' + index;
-                }
-                pathSegments.push(segmentStr);
-            }
-            //the last segment need special care 
-            {
-                var index = val[0];
-                var featureName = val[2];
-                var upperBound = val[3];
-                var segmentStr = featureName;
-                if (upperBound != 1) {
-                    segmentStr += '.' + index;
-                }
-                pathSegments.push(segmentStr);
+        this.load = function(parentEObject, eObject) {
+            var load = [];
+            switch (eObject.eClass.get("name")) {
+                default:
+                    load = ecoreSync.utils.isEClassInitialized(eObject.eClass).then(function() {
+
+                        return ecoreSync.get(eObject, "contents").then(function(contents) {
+                            return ecoreSync.utils.isEClassInitialized(contents[0].eClass).then(function() {
+                                return Promise.resolve([{
+                                    type: 'eObject',
+                                    value: contents[0],
+                                    modifiers: {
+                                        eOwner: eObject
+                                    }
+                                }]);
+                            });
+
+
+                        });
+
+
+                    });
             }
-            res = pathSegments.join('/');
-        }
 
-        return res;
-    }
+            return load;
+        };
+    };
 
-    async getAllContents(eObject, filter = null) {
+
+    var WorkspaceContextMenu = function(ecoreSync) {
         var self = this;
-        var results = [];
-        let oid = this._esDomain.rlookup(eObject);
-        if (!oid) {
-            throw 'cannot get contents: the supplied eObject is unknown to this ecoreSync instance'
-        }
-        if (filter != null) {
-            if (filter(eObject)) {
-                results.push(eObject);
-            }
-        }
-        await this.isEClassInitialized(eObject.eClass)
-        var containments = eObject.eClass.get("eAllContainments");
-        let cmd = new eoq2.Cmp();
-
-        containments.forEach(function(cnt) {
-            cmd.Get(new eoq2.Obj(oid).Pth(cnt.get("name")));
-        })
-
-        var res = await this._esDomain.exec(cmd);
-        res.forEach(function(cnts) {
-            if (Array.isArray(cnts)) {
-                results = results.concat(cnts);
+        this.ecoreSync = ecoreSync;
+        this.orderPriority = 1;
+        this.canDisplayMenuFor = function(data) {
+            if (!data.eObject) {
+                return false;
             } else {
-                if (cnts) {
-                    results.push(cnts);
+                var nsURI = "http://www.eoq.de/workspacemdbmodel/v1.0";
+                switch (data.eObject.eClass.get("name")) {
+                    case 'EReference':
+                        return data.eObject.eContainer.eContainer.get("nsURI").includes(nsURI);
+                    case 'EAttribute':
+                        return data.eObject.eContainer.eContainer.get("nsURI").includes(nsURI);
+                    default:
+                        return data.eObject.eClass.eContainer.get("nsURI").includes(nsURI);
+
                 }
-            }
-        });
 
-        var subContents = [];
-        results.forEach(function(obj) {
-            if (obj) {
-                subContents.push(self.getAllContents(obj));
             }
-        })
-        subContents = await Promise.all(subContents);
-        subContents.forEach(function(sc) {
-            results = results.concat(sc);
-        })
-
-        if (filter == null) {
-            return results;
-        } else {
-            return results.filter(filter);
-        }
-    }
+        };
 
-    getObserverState(observerToken) {
-        var res = [];
-        if (this._esDomain.qryObservers.has(observerToken)) {
-            var observer = this._esDomain.qryObservers.get(observerToken);
-            var state = observer.observerState;
-            return {
-                results: state.getResults(),
-                deltaPlus: state.getDeltaPlus(),
-                deltaMinus: state.getDeltaMinus()
-            };
-        }
-        return res;
-    }
+        this.display = function(node) {
+            var data = node.data;
+
+
+            let dirCreatableItems = {
+                "subdir-create": {
+                    name: 'Directory',
+                    icon: 'directory',
+                    callback: async function() {
+
+
+                        var subDirNames = await ecoreSync.exec(new eoq2.Get(new eoq2.Obj(data.eObject.get("_#EOQ")).Pth('subdirectories').Pth('name')));
+
+                        var dirBaseName = "newSubdir";
+                        var currentDirName = dirBaseName;
+                        var collisions = 0;
+                        var nameFound = false;
+                        while (!nameFound) {
+                            var nameTaken = false;
+
+                            for (let n in subDirNames) {
+                                if (subDirNames[n] == currentDirName) {
+                                    nameTaken = true;
+                                    break;
+                                }
+                            }
+
+                            if (nameTaken) {
+                                currentDirName = dirBaseName + (collisions + 1);
+                                collisions += 1;
+                            } else {
+                                nameFound = true;
+                            }
+                        }
+
+                        var cmd = new eoq2.Cmp();
+                        cmd.Crn('http://www.eoq.de/workspacemdbmodel/v1.0', 'Directory');
+                        cmd.Set(new eoq2.His(-1), 'name', currentDirName);
+                        cmd.Add(new eoq2.Obj(data.eObject.get("_#EOQ")), 'subdirectories', new eoq2.His(0));
+                        ecoreSync.exec(cmd)
 
-    async decode(obj) {
-        var self = this;
-        var res = null;
-        if (Array.isArray(obj)) {
-            try {
-                res = await awaitAll(obj.map(function(e) {
-                    return self.decode(e);
-                }));
-            } catch (e) {
-                throw 'ecoreSync: Failed while decoding array ' + e
-            }
-        } else {
-            if (obj != null) {
-                if (obj.qry == "OBJ") {
-                    try {
-                        if (!Number.isInteger(obj.v)) throw 'ecoreSync: Invalid input format during decode: object id is invalid'
-                        res = await this._esDomain.getObject(obj.v);
-                    } catch (e) {
-                        throw ('ecoreSync: Failed to get object during decoding ' + e);
                     }
-                } else {
-                    res = obj;
                 }
-            }
-        }
-        return res;
-    }
+            };
 
-    encode(obj) {
-        var self = this;
-        if (Array.isArray(obj)) {
-            return obj.map(function(e) {
-                return self.encode(e);
-            });
-        }
-        var res = null;
-        if (obj != null) {
+            var eoqMenu = {
+                callback: function(key, options) {
+                    //TODO: menu actions
+                    if (key == "delete") {
+                        var dialog = new jsa.MsgBox({
+                            content: 'Do you really want to delete ' + data.eObject.get("name") + '? This action can not be undone.',
+                            buttons: {
+                                yes: {
+                                    name: 'Yes',
+                                    startEnabled: true,
+                                    data: this,
+                                    onClickCallback: function(event) {
+                                        //MB: why is there another layer above ecoreSync?
+                                        pluginAPI.getGlobal('app').commandManager.Execute(new ERemoveCommand(ecoreSync, data.eObject.eContainer, data.eObject.eContainingFeature.get("name"), data.eObject));
+                                        dialog.Dissolve();
+                                    }
+                                },
+                                no: {
+                                    name: 'No',
+                                    startEnabled: true,
+                                    data: this,
+                                    onClickCallback: function(event) {
+                                        dialog.Dissolve();
+                                    }
+                                }
+                            }
+                        });
+                        pluginAPI.getGlobal('app').AddChild(dialog);
+
+                        /*
+                        ecoreSync.remove(data.eObject.eContainer,data.eObject.eContainingFeature.get("name"),data.eObject).then(function(){
+                            if ($DEBUG) console.debug('eObject successfully removed from reference')
+                        })     
+                        */
+                    }
 
-            switch (obj.constructor.name) {
-                case "EObject":
-                    let oid = this._esDomain.rlookup(obj);
-                    if (oid == null) throw 'cannot encode: the supplied eObject of type ' + obj.eClass.get('name') + ' is unknown to this ecoreSync instance'
-                    res = {
-                        qry: "OBJ",
-                        v: oid
+                    if (key == "rename") {
+                        node.editStart();
                     }
-                    break;
-                default:
-                    res = obj
-                    break;
-            }
-        }
-        return res
-    }
 
 
-    async awaitAll(obj) {
-        // aux function to await all promises in an array structure
-        var res = obj;
-        if (Array.isArray(obj)) {
-            res = [];
-            for (let i in obj) {
-                res.push(awaitAll(obj[i]))
-            }
-            res = await Promise.all(res);
-        } else {
-            res = await obj
-        }
-        return res;
-    }
-}
 
-export default class EsUtils {
 
-    initializer() {
-        this.utils = new EsUtilities(this);
+                },
+                items: {}
+            };
+
+
+            if (data.eObject.eClass.get("name") == "Directory" || data.eObject.eClass.get("name") == "Workspace") {
+                eoqMenu.items['create'] = {
+                    name: 'Create',
+                    icon: 'add',
+                    action: false,
+                    items: dirCreatableItems
+                };
+            }
+            if (data.eObject.eClass.get("name") != "Workspace") {
+                eoqMenu.items['delete'] = {
+                    name: "Delete",
+                    icon: "delete"
+                };
+            }
+
+            return eoqMenu;
+
+        };
     }
 
-}
+
+    pluginAPI.implement("plugin.ecoreTreeView.views", WorkspaceView);
+    pluginAPI.implement("plugin.ecoreTreeView.controllers", WorkspaceController);
+    pluginAPI.implement("plugin.ecoreTreeView.controllers", DirectoryController);
+    pluginAPI.implement("plugin.ecoreTreeView.controllers", ResourceController);
+    pluginAPI.implement('plugin.ecoreTreeView.menus', WorkspaceContextMenu);
+    return Promise.resolve();
+
+};
+
+export var meta = {
+    "id": "plugin.ecoreTreeView.eoq",
+    description: "EOQ Plugin for Ecore Tree View",
+    "author": "Matthias Brunner",
+    "version": "0.0.1",
+    "requires": ['plugin.ecoreTreeView']
+};
```

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync/util/uuid.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync/util/uuid.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/css/EObjectCtrls.css` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/css/EObjectCtrls.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-close-active.svg` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-close-active.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-close.svg` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-close.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-custom-active.svg` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-custom-active.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-custom.svg` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-custom.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-global-active.svg` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-global-active.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-global.svg` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-global.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-local-active.svg` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-local-active.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-local.svg` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-scope-local.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-select-all-active.svg` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-select-all-active.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-select-all.svg` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-select-all.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-select-invert-active.svg` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-select-invert-active.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-select-invert.svg` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-select-invert.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-select-none-active.svg` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-select-none-active.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/img/select-list-select-none.svg` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/img/select-list-select-none.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrlFactory.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrlFactory.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrlUpdateHandler.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrlUpdateHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrls.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/js/EObjectCtrls.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -191,19 +191,14 @@
     /* ESTRINGCTRL */
     function EStringCtrl(params = {}, createDom = true) {
         EAttributeTextCtrlA.call(this, params, false);
 
         //parameters
         this.validateFunction = function(valueStr) {
             return true; // validation deactivated to allow paths with slashes
-            // Validation was possibly to prevent code injection. However, this is not possible since the value is not evaluated as code.
-            if (/['"#\$\[\]\/\\]/.test(valueStr)) {
-                throw new Error('Illegal value: String should not contain \',",#,$,[,],\\ or /!');
-            }
-            return true;
         } //Shall throw an Error if validation fails
 
         jsa.CopyParams(this, params);
 
         if (createDom) {
             this.CreateDom();
         }
```

### Comparing `XGEE-0.3.6/xgee/core/plugins/ecoreSync.ui/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/ecoreSync.ui/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/controllers/graph/AnchorController.js` & `XGEE-0.3.7/xgee/core/plugins/editor/controllers/graph/AnchorController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/controllers/graph/ContainerController.js` & `XGEE-0.3.7/xgee/core/plugins/editor/controllers/graph/ContainerController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/controllers/graph/EdgeController.js` & `XGEE-0.3.7/xgee/core/plugins/editor/controllers/graph/EdgeController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/controllers/graph/GraphController.js` & `XGEE-0.3.7/xgee/core/plugins/editor/controllers/graph/GraphController.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -115,16 +115,20 @@
     }
 
 
     async init(paletteController) {
         this.paletteController = paletteController
         this.controllerEvents["initBegin"].raise();
         var t0 = performance.now();
-        var self = this
-        await this.model.init()
+        var self = this;
+        try {
+            await this.model.init();
+        } catch (error) {
+            console.error("Error initializing model:", error);
+        }
         await this.view.reset();
 
         var initContainer = async function(c) {
             self.view.addContainerToGraph(c);
             await c.arrange();
             for (let subVertex of c.vertices) {
                 await initVertex(subVertex);
```

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/controllers/graph/GraphControllerFactory.js` & `XGEE-0.3.7/xgee/core/plugins/editor/controllers/graph/GraphControllerFactory.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/controllers/graph/LabelController.js` & `XGEE-0.3.7/xgee/core/plugins/editor/controllers/graph/LabelController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/controllers/graph/QueryController.js` & `XGEE-0.3.7/xgee/core/plugins/editor/controllers/graph/QueryController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/controllers/graph/VertexController.js` & `XGEE-0.3.7/xgee/core/plugins/editor/controllers/graph/VertexController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/controllers/palette/PaletteController.js` & `XGEE-0.3.7/xgee/core/plugins/editor/controllers/palette/PaletteController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/css/loading.css` & `XGEE-0.3.7/xgee/core/plugins/editor/css/loading.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/extensions/EditorContextMenuProvider.js` & `XGEE-0.3.7/xgee/core/plugins/editor/extensions/EditorContextMenuProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/graph/GraphResourceProvider.js` & `XGEE-0.3.7/xgee/core/plugins/editor/graph/GraphResourceProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/graph/mxGraphIntegration.js` & `XGEE-0.3.7/xgee/core/plugins/editor/graph/mxGraphIntegration.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/interactions/DropReception.js` & `XGEE-0.3.7/xgee/core/plugins/editor/interactions/DropReception.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/interactions/GraphInteraction.js` & `XGEE-0.3.7/xgee/core/plugins/editor/interactions/GraphInteraction.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/lib/libapi.js` & `XGEE-0.3.7/xgee/core/plugins/editor/lib/libapi.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/lib/libaux.js` & `XGEE-0.3.7/xgee/core/plugins/editor/lib/libaux.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/lib/libjsa.js` & `XGEE-0.3.7/xgee/core/plugins/editor/lib/libjsa.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/lib/uuid.js` & `XGEE-0.3.7/xgee/core/plugins/editor/lib/uuid.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/editorModel.ecore` & `XGEE-0.3.7/xgee/core/plugins/editor/model/editorModel.ecore`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/Anchor.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/Anchor.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/AnchorManager.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/AnchorManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/Container.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/Container.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/ContainerManager.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/ContainerManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/ContainerProvider.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/ContainerProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/ContainerType.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/ContainerType.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/DeletableObject.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/DeletableObject.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/Edge.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/Edge.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/EdgeContainer.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/EdgeContainer.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/EdgeManager.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/EdgeManager.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -154,14 +154,18 @@
             if(!edge) edge=self.graphModelFactory.createEdge(self.model,self.type,eObject)
             return edge 
         })
     }*/
 
     async _postProcessResults(results, container = null) {
         var self = this;
+        // check results against null
+        if (!results) {
+            console.warn('No results supplied for edge. Please contact the developer and include a log or open a Gitlab issue.')
+        }
         if (!Array.isArray(results)) {
             results = [results]
         }
         if (!container) {
             return results.map(function(eObject) {
                 return self.graphModelFactory.createEdge(self.model, self.type, eObject);
             });
```

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/EventProvider.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/EventProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/GraphEvent.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/GraphEvent.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/GraphLayoutManager.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/GraphLayoutManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/GraphModel.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/GraphModel.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/GraphModelFactory.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/GraphModelFactory.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -241,14 +241,18 @@
     createStaticVertexType(ecoreSync, model) {
         var staticVertexType = new StaticVertexType(ecoreSync, model)
         staticVertexType.shape = this.resourceProvider.LoadResource(model.get("shape").get("filepath"))
         return staticVertexType;
     }
 
     createVertex(graphModel, type, eObject) {
+        // check for eObject
+        if (!eObject) {
+            throw new Error(`Trying to create a vertex with eObject = null. Every vertex needs an eObject.`)
+        }
         var vertex = new Vertex(graphModel)
         vertex.eObject = eObject;
         vertex.type = type;
         vertex.init();
         return vertex
     }
```

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/GraphModelManager.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/GraphModelManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/GraphObject.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/GraphObject.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/GraphObjectManager.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/GraphObjectManager.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -10,18 +10,19 @@
     }
 
     async load(valueSet) {
         try {
             var vSet = Object.assign({}, valueSet);
             var query = this.type.query.build(vSet);
             var cmd = new eoq2.Get(query);
-            var results = await this.ecoreSync.exec(cmd, false)
+            var results = await this.ecoreSync.exec(cmd, false) // no result checking here, because it is done in the _postProcessResults method (at least for vertices)  
             var res = await this._postProcessResults(results);
-        } catch (e) {
-            throw (this.constructor.name + ' failed to load:' + e)
+        } catch (error) {
+            error.message = this.constructor.name + ' failed to load: ' + error.message
+            throw error
         }
         return res;
     }
 
     async observe(valueSet, callback) {
         var vSet = Object.assign({}, valueSet);
         var self = this;
```

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/Label.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/Label.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/LabelManager.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/LabelManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/LabelSegment.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/LabelSegment.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/LabelSegmentManager.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/LabelSegmentManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/LocatableObject.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/LocatableObject.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/NestedLabel.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/NestedLabel.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/SizableObject.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/SizableObject.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/StaticVertex.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/StaticVertex.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/StaticVertexManager.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/StaticVertexManager.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/StaticVertexType.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/StaticVertexType.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/TransactionObject.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/TransactionObject.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/Vertex.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/Vertex.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/VertexContainer.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/VertexContainer.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/VertexManager.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/VertexManager.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
     constructor(...args) {
         super(...args)
     }
 
     async load(valueSet) {
 
         var self = this;
-        var results = await super.load(valueSet);
+        var results = await super.load(valueSet); // no result checking here, because it is done in the super.load method, which calls the _postProcessResults method (at least for vertices)
         var valueSets = await this.type.query.makeValueSets(valueSet, results.map(function(e) {
             return e.getEObject()
         }));
 
         var pendingVSets = valueSets.map(function(vSet) {
             //for each loaded vertex, apply the submanagers load routine
             let loadingSubManagers = [];
@@ -63,15 +63,15 @@
 
 
         return results;
     }
 
     async observe(valueSet, callback, container) {
         var self = this;
-        if (!container) throw ' no container supplied '
+        if (!container) throw new Error(' no container supplied ')
 
 
         var ObserverCallback = async function(results, addedVertices, removedVertices) {
 
 
             for (let i = 0; i < removedVertices.length; i++) {
                 let vertex = removedVertices[i];
@@ -282,25 +282,44 @@
 
             })
         })
 
         callback(results, deltaPlus, deltaMinus);
     }
 
+
+    /**
+     * Processes the results and creates vertices for the given results.
+     * @param {Array<EObject>|EObject} results - The results from a query of the GraphManager to be processed. It can be an array of eObjects or a single eObject.
+     * @param {Object} [container=null] - The container object. Used by observers. The container is e.g. the vertex that contains the observed vertices.
+     * @returns {Array} - An array of vertices created from the results. If a vertex could not be created, an empty array is returned for that result.
+     */
     async _postProcessResults(results, container = null) {
         var self = this;
+
+        // Handling of getting 'null' as a result
+        if (!results) {
+            let container_id = container ? container.type.model.values.id : null
+            let container_name = container ? container.type.model.values.name : null
+            console.warn(`Problem in editorModel with id: ${self.type.model.values.id} and name: ${self.type.model.values.name}. Input: results: ${results}, container id: ${container_id}, container name: ${container_name}. The queryStr: ${self.type.model.values.queryStr} resulted with 'null' as a result. Cannot create a vertex for 'null'.\nThe queryStr: ${self.type.model.values.queryStr} likely wants to query a single value feature (SET). XGEE is optimized for features with a multiplicity of '*' (ADD). If you still want to display it as a vertex, turn it into a list by adding a '&TRM((=%),[])' to the queryStr.\nFor your better experience, I will skip this vertex for now and continue rendering. However you are now entering untested territory. It is highly recommended to use TRM and follow the docu at: https://docs.xgee.de/tutorial/xgee_example_app.html.`)
+            return []; // return an empty array to signal that the vertex could not be created and allow further processing. Empty list means so execution of .map, so no valueSets will be created. 
+        }
+
         if (!Array.isArray(results)) {
             results = [results]
         }
+
+        // default behavior
         if (!container) {
             return results.map(function(eObject) {
                 return self.graphModelFactory.createVertex(self.model, self.type, eObject);
             });
         }
 
+        // container behavior (used by observers)
         return results.map(function(eObject) {
             let vertex = container.getVertexByEObject(eObject)
             if (!vertex) {
                 vertex = self.graphModelFactory.createVertex(self.model, self.type, eObject)
             } else {
                 if (vertex.type != self.type) {
                     vertex = self.graphModelFactory.createVertex(self.model, self.type, eObject)
```

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/graph/VertexType.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/graph/VertexType.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/palette/DragAndDropTool.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/palette/DragAndDropTool.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/palette/EdgeRoutingTool.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/palette/EdgeRoutingTool.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/palette/GraphTool.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/palette/GraphTool.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/palette/PaletteModel.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/palette/PaletteModel.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/palette/SelectionTool.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/palette/SelectionTool.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/model/palette/ToolGenerator.js` & `XGEE-0.3.7/xgee/core/plugins/editor/model/palette/ToolGenerator.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/editor/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/queries/Query.js` & `XGEE-0.3.7/xgee/core/plugins/editor/queries/Query.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -107,14 +107,15 @@
      * @returns {Array|dictionary} Returns an array of valueSets if multiple eObjects were supplied, otherwise a single valueSet dictionary is returned.
      */
     async makeValueSets(valueSet, results) {
         var self = this;
         if (Array.isArray(results)) {
             let vSets = [];
             var fillVSet = async (vSet, eObject) => {
+                if (!eObject) throw new Error('no eObject was supplied')
                 vSet["MODELROOT"] = await this.ecoreSync.utils.getModelRoot(eObject)
                 vSet["RESOURCE"] = await this.ecoreSync.utils.getResource(eObject)
                 return vSet;
             };
             for (let i = 0; i < results.length; i++) {
                 let vSet = Object.assign({}, valueSet);
                 if (self.alias) {
```

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/view/GraphView.js` & `XGEE-0.3.7/xgee/core/plugins/editor/view/GraphView.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/view/GraphViewMenu.js` & `XGEE-0.3.7/xgee/core/plugins/editor/view/GraphViewMenu.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/view/GraphViewPort.js` & `XGEE-0.3.7/xgee/core/plugins/editor/view/GraphViewPort.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/view/PaletteView.js` & `XGEE-0.3.7/xgee/core/plugins/editor/view/PaletteView.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/editor/view/ScreenshotExport.js` & `XGEE-0.3.7/xgee/core/plugins/editor/view/ScreenshotExport.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq.actions/css/ActionsUi.css` & `XGEE-0.3.7/xgee/core/plugins/eoq.actions/css/ActionsUi.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq.actions/js/ActionsController.js` & `XGEE-0.3.7/xgee/core/plugins/eoq.actions/js/ActionsController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq.actions/js/ActionsCore.js` & `XGEE-0.3.7/xgee/core/plugins/eoq.actions/js/ActionsCore.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq.actions/js/ActionsUi.js` & `XGEE-0.3.7/xgee/core/plugins/eoq.actions/js/ActionsUi.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq.actions/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/eoq.actions/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq1/LICENSE` & `XGEE-0.3.7/xgee/core/plugins/eoq1/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq1/README.md` & `XGEE-0.3.7/xgee/core/plugins/eoq1/README.md`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq1/commandparser.js` & `XGEE-0.3.7/xgee/core/plugins/eoq1/commandparser.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq1/domains/bufferingdomain.js` & `XGEE-0.3.7/xgee/core/plugins/eoq1/domains/bufferingdomain.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq1/domains/domain.js` & `XGEE-0.3.7/xgee/core/plugins/eoq1/domains/domain.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq1/domains/httppostdomain.js` & `XGEE-0.3.7/xgee/core/plugins/eoq1/domains/httppostdomain.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq1/model/model.js` & `XGEE-0.3.7/xgee/core/plugins/eoq1/model/model.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq1/resultparser.js` & `XGEE-0.3.7/xgee/core/plugins/eoq1/resultparser.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq1/valueparser.js` & `XGEE-0.3.7/xgee/core/plugins/eoq1/valueparser.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq2/LICENSE` & `XGEE-0.3.7/xgee/core/plugins/eoq2/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq2/README.md` & `XGEE-0.3.7/xgee/core/plugins/eoq2/README.md`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq2/action/call.js` & `XGEE-0.3.7/xgee/core/plugins/eoq2/action/call.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq2/command/command.js` & `XGEE-0.3.7/xgee/core/plugins/eoq2/command/command.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq2/command/result.js` & `XGEE-0.3.7/xgee/core/plugins/eoq2/command/result.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq2/domain/domain.js` & `XGEE-0.3.7/xgee/core/plugins/eoq2/domain/domain.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq2/domain/remote/httppostdomain.js` & `XGEE-0.3.7/xgee/core/plugins/eoq2/domain/remote/httppostdomain.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq2/domain/remote/websocketdomain.js` & `XGEE-0.3.7/xgee/core/plugins/eoq2/domain/remote/websocketdomain.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq2/eoq2.js` & `XGEE-0.3.7/xgee/core/plugins/eoq2/eoq2.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq2/event/event.js` & `XGEE-0.3.7/xgee/core/plugins/eoq2/event/event.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq2/frame/frame.js` & `XGEE-0.3.7/xgee/core/plugins/eoq2/frame/frame.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq2/legacy/legacy.js` & `XGEE-0.3.7/xgee/core/plugins/eoq2/legacy/legacy.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq2/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/eoq2/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq2/query/query.js` & `XGEE-0.3.7/xgee/core/plugins/eoq2/query/query.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq2/serialization/jsonserializer.js` & `XGEE-0.3.7/xgee/core/plugins/eoq2/serialization/jsonserializer.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq2/serialization/serializer.js` & `XGEE-0.3.7/xgee/core/plugins/eoq2/serialization/serializer.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq2/serialization/textserializer.js` & `XGEE-0.3.7/xgee/core/plugins/eoq2/serialization/textserializer.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eoq2/util/logger.js` & `XGEE-0.3.7/xgee/core/plugins/eoq2/util/logger.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eventBroker/SelectionChangedEvent.js` & `XGEE-0.3.7/xgee/core/plugins/eventBroker/SelectionChangedEvent.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/eventBroker/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/eventBroker/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/iconProvider/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/iconProvider/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/keyHandler/js/KeyHandler.js` & `XGEE-0.3.7/xgee/core/plugins/keyHandler/js/KeyHandler.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/keyHandler.ecore/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/keyHandler.ecore/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/LICENSE` & `XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/LICENSE`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.eot` & `XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.eot`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.ttf` & `XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.ttf`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.woff` & `XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.woff`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.woff2` & `XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/font/context-menu-icons.woff2`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.css` & `XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.js` & `XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.css` & `XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.css.map` & `XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.css.map`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.js` & `XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.js.map` & `XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.contextMenu.min.js.map`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.ui.position.js` & `XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.ui.position.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.ui.position.min.js` & `XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/jQuery-contextMenu-2.8/jquery.ui.position.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.contextMenu/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/plugin.contextMenu/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EAnnotation.gif` & `XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EAnnotation.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EParameter.gif` & `XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/EParameter.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eAnnotations.gif` & `XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/ecore-icons/eAnnotations.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/js/TreeViewContextMenuProvider.js` & `XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/js/TreeViewContextMenuProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/plugin.ecoreTreeView/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.ecoreTreeView.eoq/plugin.js` & `XGEE-0.3.7/xgee/core/res/js/workspace/workspace.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -1,444 +1,455 @@
-export function init(pluginAPI) {
+// Workspace Provider
+// Enables support for workspaces on the remote server 
+// (C) 2019 Matthias Brunner
+
+var WorkspaceProvider = function(ecoreSync) {
+    var self = this;
+    this.ecoreSync = ecoreSync;
+    this.name = "workspace";
 
-    var WorkspaceView = function(iconPath) {
-        var self = this;
-        this.iconPath = iconPath;
-        this.apply = function(data) {
-            var view = {};
-            if (data.type == 'eObject') {
-                switch (data.value.eClass.get("name")) {
-                    case 'Workspace':
-                        view = {
-                            title: 'Workspace',
-                            folder: true,
-                            eObject: data.value,
-                            modifiers: data.modifiers,
-                            lazy: true
-                        };
-                        break;
-                    case 'Directory':
-                        view = {
-                            title: data.value.get("name"),
-                            folder: true,
-                            eObject: data.value,
-                            modifiers: data.modifiers,
-                            lazy: true
-                        };
-                        break;
-                    case 'ModelResource':
-                        view = {
-                            title: data.value.get("name"),
-                            eObject: data.value,
-                            modifiers: data.modifiers,
-                            lazy: true
-                        };
-                        break;
-                }
-            }
-            return view;
-        };
 
-        this.canDisplay = function(data) {
-            if (data.type != 'eObject') {
-                return false;
-            } else {
-                var displayableClasses = [{
-                    name: 'Workspace',
-                    nsURI: "http://www.eoq.de/workspacemdbmodel/v1.0"
-                }, {
-                    name: 'Directory',
-                    nsURI: "http://www.eoq.de/workspacemdbmodel/v1.0"
-                }, {
-                    name: 'ModelResource',
-                    nsURI: "http://www.eoq.de/workspacemdbmodel/v1.0"
-                }];
-                if (data.value) {
-                    if (displayableClasses.find(function(e) {
-                            return e.name == data.value.eClass.get("name") && e.nsURI == data.value.eClass.eContainer.get("nsURI")
-                        })) {
-                        return true;
-                    }
-                } else {
-                    console.error(data)
-                }
+    this.delay = function(until = 100) {
+        return new Promise(function(resolve, reject) {
+            setTimeout(resolve, until);
+        });
+    };
 
-            }
-        }
-    }
+    var Resource = function(workspace, objectId) {
+        //API to access resources
 
-    var WorkspaceController = function(ecoreSync) {
-        var ecoreSync = ecoreSync;
         var self = this;
-        this.onUpdate = function(parentEObject, eObject, callbackFcn) {
-            eObject.on('add:subdirectories', function() {
-                self.load(parentEObject, eObject).then(function(loadedData) {
-                    callbackFcn(loadedData);
-                })
-            });
-            eObject.on('add:resources', function() {
-                self.load(parentEObject, eObject).then(function(loadedData) {
-                    callbackFcn(loadedData);
-                })
-            })
-            eObject.on('remove:subdirectories', function() {
-                self.load(parentEObject, eObject).then(function(loadedData) {
-                    callbackFcn(loadedData);
-                })
-            });
-            eObject.on('remove:resources', function() {
-                self.load(parentEObject, eObject).then(function(loadedData) {
-                    callbackFcn(loadedData);
-                })
-            })
+        this.workspace = workspace;
+        this.objectId = objectId; //the resource object Id (workspace model)
+        this.rootObjectId = objectId; //the root object Id (resource)
+        this.name = "";
+        this.isResource = true;
+        this.isWorkspaceObject = true;
+        this.isLoaded = false;
+        this.isDirty = false;
+        this.eObject = null; //the resource eObject (workspace model)
+        this.rootObject = null; // the root object of the resource (resource)
+        this.__listeners = [];
+        this.__update = new rateLimitedFunctionCall(function() {
+            self.fireOnUpdate();
+        }, 10);
+        this.isInitialized = function() {
+            //A resource is initialized (!=loaded) if its name and its EObject (not the root object) is present
+            return new Promise(function(resolve, reject) {
+                self.getEObject().then(function() {
+                    self.getName().then(function() {
+                        resolve();
+                    });
+                });
+            });
         }
+        this.getEObject = function() {
+            //Gets the resources EObject
+            var setupListeners = function(eObject) {
+                eObject.on('change', function(change) {
+                    self.update();
+                });
+            };
+            return new Promise(function(resolve, reject) {
+                self.workspace.ecoreSync.getObjectById(self.objectId).then(function(eObject) {
+                    self.eObject = ecoreSync.getProxiedObject(eObject);
+                    setupListeners(eObject.noproxy);
+                    resolve(self.eObject);
+                });
+            });
+        };
+        this.getName = function() {
+            //Gets the resource's file name
 
-        this.onChange = function(data, callbackFcn) {
-            if (data.type = 'eObject') {
-                data.value.on('change', function() {
-                    callbackFcn(data.value)
+            return new Promise(function(resolve, reject) {
+                self.workspace.ecoreSync.isAttributeInitialized(self.eObject, "name").then(function() {
+                    resolve();
                 });
+            });
+        };
+        this.update = function() {
+            //Updates the resources state variables
+            self.isDirty = self.eObject.get("isDirty");
+            self.name = self.eObject.get("name");
+            self.fireOnUpdate();
+        };
+        this.getRootObject = function() {
+            //This function gets the resource's root object, the actual model root. If the root object is requested,
+            //the resource is also loaded on the remote server. 
+            //Note: This resource object also contains another eObject (see getEObject()) referring to its workspace model object.
+            return new Promise(function(resolve, reject) {
+                if (!self.isLoaded) {
+                    self.load().then(function() {
+                        resolve(self.rootObject);
+                    });
+                } else {
+                    resolve(self.rootObject);
+                }
+            });
+        };
+        this.load = function() {
+            //Loads the resource on the remote server and stores the root object (and id) in the workspace model
+            return new Promise(function(resolve, reject) {
+                if (!self.isLoaded) {
+                    self.workspace.ecoreSync.loadResource(self.objectId, function(rootObjectId) {
+                        self.isLoaded = true;
+                        self.rootObjectId = rootObjectId;
+                        self.rootObject = ecoreSync.getProxiedObject(self.workspace.ecoreSync.index.getById(rootObjectId));
+                        self.workspace.ecoreSync.isClassInitialized(self.rootObject.eClass).then(resolve());
+                    });
+                } else {
+                    resolve();
+                }
+            });
+        };
+        this.save = function() {
+            //Saves the resource on the remote server
+            if (self.isLoaded) {
+                let query = "CALL 'save-resource' [#" + objectId + "]";
+                let onSuccess = function() {
+                    $app.notesManager.PutNote("Saved.", "success");
+                };
+                let onFailure = function() {
+                    $app.notesManager.PutNote("Saving failed.", "error");
+                };
+                self.workspace.ecoreSync.domain.DoFromStr(query, onSuccess, onFailure);
             }
         }
-
-        this.canLoad = function(data) {
-            return data.node.data.eObject.eClass.eContainer.get("nsURI") == 'http://www.eoq.de/workspacemdbmodel/v1.0' && data.node.data.eObject.eClass.get('name') == 'Workspace';
-        }
-
-        this.load = function(parentEObject, eObject) {
-            var load = [];
-            switch (eObject.eClass.get("name")) {
-                default:
-                    load = ecoreSync.utils.isEClassInitialized(eObject.eClass).then(function() {
-                        var subdirectories = ecoreSync.get(eObject, "subdirectories").then(function(results) {
-                            return Promise.all(results.map(function(e) {
-                                return ecoreSync.get(e, "name");
-                            })).then(function() {
-                                return Promise.resolve(results.map(function(e) {
-                                    return {
-                                        type: 'eObject',
-                                        value: e,
-                                        modifiers: {}
-                                    }
-                                }));
-                            });
-                        });
-
-                        var resources = ecoreSync.get(eObject, "resources").then(function(results) {
-                            return Promise.all(results.map(function(e) {
-                                return ecoreSync.get(e, "name");
-                            })).then(function() {
-                                return Promise.resolve(results.map(function(e) {
-                                    return {
-                                        type: 'eObject',
-                                        value: e,
-                                        modifiers: {}
-                                    }
-                                }));
-                            });
-                        });
-
-                        return Promise.all([subdirectories, resources]).then(function(values) {
-                            var contents = values[0];
-                            contents = contents.concat(values[1]);
-                            return Promise.resolve(contents);
-                        });
-
-                    });
+        this.onUpdate = function(cb) {
+            //Registers a callback function (cb) to fire in the case of an update (onUpdate event)
+            if (self.__listeners.indexOf(cb) == -1) {
+                self.__listeners.push(cb);
             }
-
-            return load;
         };
+        this.fireOnUpdate = function() {
+            //fires the onUpdate event
+            for (let i in self.__listeners) {
+                setTimeout(self.__listeners[i], 1);
+            }
+        }
     };
 
-    var DirectoryController = function(ecoreSync) {
-        var ecoreSync = ecoreSync;
+    var Directory = function(workspace, objectId, isRoot = false, name = "") {
         var self = this;
-        this.onUpdate = function(parentEObject, eObject, callbackFcn) {
-            eObject.on('add:subdirectories', function() {
-
-                self.load(parentEObject, eObject).then(function(loadedData) {
-                    callbackFcn(loadedData);
-                })
-            });
-            eObject.on('add:resources', function() {
-
-                self.load(parentEObject, eObject).then(function(loadedData) {
-                    callbackFcn(loadedData);
-                })
-            })
-            eObject.on('remove:subdirectories', function() {
-
-                self.load(parentEObject, eObject).then(function(loadedData) {
-                    callbackFcn(loadedData);
-                })
-            });
-            eObject.on('remove:resources', function() {
-
-                self.load(parentEObject, eObject).then(function(loadedData) {
-                    callbackFcn(loadedData);
-                })
-            })
-        }
-
-        this.onChange = function(data, callbackFcn) {
-            if (data.type = 'eObject') {
-                data.value.on('change', function() {
-                    callbackFcn(data.value)
-                });
-            }
-        }
+        this.workspace = workspace;
+        this.objectId = objectId;
+        this.eObject = null;
+        this.__eObjectListeners = false;
+        this.name = name;
+        this.resources = [];
+        this.directories = [];
+        this.metamodels = [];
+        this.isRoot = isRoot;
+        this.isDirectory = true;
+        this.isWorkspaceObject = true;
+        this.__listeners = [];
+        this.__initialized = false;
+        this.pendingUpdate = Promise.resolve();
+        this.__update = new rateLimitedFunctionCall(function() {
+            self.pendingUpdate.then(function() {
+                self.updateContents().then(self.fireOnUpdate);
+            });
+        }, 10);
+        this.update = function() {
+            self.__update.runRateLimited();
+        };
+        this.getEObject = function() {
+            console.trace();
+            var setupListeners = function() {
+                return new Promise(function(resolve, reject) {
 
-        this.canLoad = function(data) {
-            return data.node.data.eObject.eClass.eContainer.get("nsURI") == 'http://www.eoq.de/workspacemdbmodel/v1.0' && data.node.data.eObject.eClass.get('name') == 'Directory';
-        }
 
-        this.load = function(parentEObject, eObject) {
-            var load = [];
-            switch (eObject.eClass.get("name")) {
-                default:
-                    load = ecoreSync.utils.isEClassInitialized(eObject.eClass).then(function() {
-
-                        var subdirectories = ecoreSync.get(eObject, "subdirectories").then(function(results) {
-                            return Promise.all(results.map(function(e) {
-                                return ecoreSync.get(e, "name");
-                            })).then(function() {
-                                return Promise.resolve(results.map(function(e) {
-                                    return {
-                                        type: 'eObject',
-                                        value: e,
-                                        modifiers: {}
-                                    }
-                                }));
-                            });
+                    //Sets up eObject listeners to react to object changes
+
+                    if (!self.__eObjectListeners) {
+                        //Listen to properties changes
+                        self.eObject.noproxy.on('change', function(change) {
+                            self.update();
                         });
 
-                        var resources = ecoreSync.get(eObject, "resources").then(function(results) {
-                            return Promise.all(results.map(function(e) {
-                                return ecoreSync.get(e, "name");
-                            })).then(function() {
-                                return Promise.resolve(results.map(function(e) {
-                                    return {
-                                        type: 'eObject',
-                                        value: e,
-                                        modifiers: {}
-                                    }
-                                }));
+                        //Listen to references add/remove
+                        let observedFeatures = [];
+                        if (self.isRoot) {
+                            observedFeatures = ['subdirectories', 'resources' /*,'metamodels'*/ ];
+                        } else {
+                            observedFeatures = ['subdirectories', 'resources'];
+                        }
+                        for (let i in observedFeatures) {
+                            self.eObject.noproxy.on('add:' + observedFeatures[i], function(change) {
+                                self.update();
                             });
-                        });
-
-                        return Promise.all([subdirectories, resources]).then(function(values) {
-
-                                var contents = values[0];
-                                contents = contents.concat(values[1]);
-                                return Promise.resolve(contents);
-                            },
-                            function(msg) {
-                                console.error('failed to load')
+                            self.eObject.noproxy.on('remove:' + observedFeatures[i], function(change) {
+                                self.update();
                             });
+                            self.eObject.get(observedFeatures[i]);
+                        }
+                        self.__eObjectListeners = true;
+                    }
 
-                    });
-            }
+                    resolve();
+                });
+            };
 
-            return load;
+            return new Promise(function(resolve, reject) {
+                self.workspace.ecoreSync.getObjectById(self.objectId).then(function(eObject) {
+                    self.eObject = self.workspace.ecoreSync.getProxiedObject(eObject);
+                    self.workspace.ecoreSync.isClassInitialized(self.eObject.eClass).then(
+                        function() {
+                            setupListeners().then(resolve(self.eObject));
+                            resolve();
+                        }
+                    );
+                });
+            });
+        };
+        this.__addResource = function(id) {
+            let resource = self.resources.find(function(e) {
+                return e.objectId == id;
+            });
+            if (!resource) {
+                resource = new Resource(self.workspace, id);
+                let resourceInitialized = resource.isInitialized();
+                resourceInitialized.then(function() {
+                    self.resources.push(resource);
+                });
+                return resourceInitialized;
+            } else {
+                return Promise.resolve();
+            }
         };
 
+        this.__addDirectory = function(id) {
+            let dir = self.directories.find(function(e) {
+                return e.objectId == id;
+            });
+            if (!dir) {
+                dir = new Directory(self.workspace, id);
+                let dirInitialized = dir.isInitialized()
+                dirInitialized.then(function() {
+                    self.directories.push(dir);
+                });
+                return dirInitialized;
+            } else {
+                return Promise.resolve();
+            }
+        };
+        this.__addMetamodel = function(id) {
+            let metamodel = self.metamodels.find(function(e) {
+                return e.objectId == id;
+            });
+            if (!metamodel) {
+                metamodel = new Metamodel(self.workspace, id);
+                self.metamodels.push(metamodel);
+            }
+            return Promise.resolve();
+        }
 
-    };
-
+        this.updateContents = function() {
 
+            var contentUpdate = function() {
+                return new Promise(
+                    function(resolve, reject) {
+
+                        var featuresInitialized = [];
+                        featuresInitialized.push(self.workspace.ecoreSync.isReferenceInitialized(self.eObject, "subdirectories"));
+                        featuresInitialized.push(self.workspace.ecoreSync.isReferenceInitialized(self.eObject, "resources"));
+                        if (self.isRoot) {
+                            //featuresInitialized.push(self.workspace.ecoreSync.isReferenceInitialized(self.eObject,"metamodels"));
+                        } else {
+                            featuresInitialized.push(self.workspace.ecoreSync.isAttributeInitialized(self.eObject, "name"));
+                        }
 
-    var ResourceController = function(ecoreSync) {
-        var ecoreSync = ecoreSync;
-        this.canLoad = function(data) {
-            return data.node.data.eObject.eClass.eContainer.get("nsURI") == 'http://www.eoq.de/workspacemdbmodel/v1.0' && data.node.data.eObject.eClass.get('name') == 'ModelResource';
-        }
+                        Promise.all(featuresInitialized).then(function() {
 
-        this.onUpdate = function() {
-            //ResourceController does not provide updates     
-        }
+                            var objectsInitialized = [];
 
-        this.onChange = function() {
-            //ResourceController does not provide changes       
-        }
+                            //update the workspace
+                            let dirs = self.eObject.get("subdirectories").array();
+                            for (let i in dirs) {
+                                objectsInitialized.push(self.__addDirectory(dirs[i].get("_#EOQ")));
+                            }
+                            let resources = self.eObject.get("resources").array();
+                            for (let i in resources) {
+                                objectsInitialized.push(self.__addResource(resources[i].get("_#EOQ")));
+                            }
+                            if (self.isRoot) {
+                                //only the root directory provides meta models
+                                // let metas=self.eObject.get("metamodels").array();
+                                // for(let i in metas)
+                                // {
+                                //     objectsInitialized.push(self.__addMetamodel(metas[i].get("_#EOQ")));
+                                // }
+                                //$.notify("metas "+metas.length);
+                            } else {
+                                self.name = self.eObject.get("name");
+                            }
 
-        this.load = function(parentEObject, eObject) {
-            var load = [];
-            switch (eObject.eClass.get("name")) {
-                default:
-                    load = ecoreSync.utils.isEClassInitialized(eObject.eClass).then(function() {
-
-                        return ecoreSync.get(eObject, "contents").then(function(contents) {
-                            return ecoreSync.utils.isEClassInitialized(contents[0].eClass).then(function() {
-                                return Promise.resolve([{
-                                    type: 'eObject',
-                                    value: contents[0],
-                                    modifiers: {
-                                        eOwner: eObject
-                                    }
-                                }]);
+                            Promise.all(objectsInitialized).then(function() {
+                                self.__initialized = true;
+                                resolve();
                             });
 
-
                         });
-
-
                     });
-            }
+            };
 
-            return load;
+            return new Promise(function(resolve, reject) {
+                self.pendingUpdate = new Promise(function(updateComplete, updateFailed) {
+                    contentUpdate().then(function() {
+                        updateComplete();
+                    }).catch(function(reason) {
+                        alert(' An error occured: ' + reason);
+                        console.trace();
+                    })
+                });
+                self.pendingUpdate.then(function() {
+                    self.fireOnUpdate();
+                    resolve()
+                });
+            });
         };
-    };
-
 
-    var WorkspaceContextMenu = function(ecoreSync) {
-        var self = this;
-        this.ecoreSync = ecoreSync;
-        this.orderPriority = 1;
-        this.canDisplayMenuFor = function(data) {
-            if (!data.eObject) {
-                return false;
+        this.getContents = function() {
+            let contents = [];
+            contents = contents.concat(self.directories);
+            contents = contents.concat(self.resources);
+            //contents=contents.concat(self.metamodels);
+            return contents;
+        };
+        this.onUpdate = function(cb, remove = false) {
+            if (!remove) {
+                if (self.__listeners.indexOf(cb) == -1) {
+                    self.__listeners.push(cb);
+                }
             } else {
-                var nsURI = "http://www.eoq.de/workspacemdbmodel/v1.0";
-                switch (data.eObject.eClass.get("name")) {
-                    case 'EReference':
-                        return data.eObject.eContainer.eContainer.get("nsURI").includes(nsURI);
-                    case 'EAttribute':
-                        return data.eObject.eContainer.eContainer.get("nsURI").includes(nsURI);
-                    default:
-                        return data.eObject.eClass.eContainer.get("nsURI").includes(nsURI);
-
+                let rcb = self.__listeners.find(function(e) {
+                    return e == cb;
+                });
+                if (rcb) {
+                    self.__listeners.splice(self.__listeners.indexOf(rcb), 1);
                 }
-
             }
         };
+        this.fireOnUpdate = function() {
+            for (let i in self.__listeners) {
+                setTimeout(self.__listeners[i], 1);
+            }
+        };
+        this.isInitialized = function() {
 
-        this.display = function(node) {
-            var data = node.data;
+            //A directory is initialized if all subordinate objects and its name and eObject are initialized
 
+            return new Promise(function(resolve, reject) {
+                console.warn("Directory initializing " + self.name);
+                self.getEObject()
+                    .then(function(eObject) {
+                        return self.updateContents();
+                    })
+                    .then(function() {
+                        resolve();
+                    });
+            });
+        };
 
-            let dirCreatableItems = {
-                "subdir-create": {
-                    name: 'Directory',
-                    icon: 'directory',
-                    callback: async function() {
-
-
-                        var subDirNames = await ecoreSync.exec(new eoq2.Get(new eoq2.Obj(data.eObject.get("_#EOQ")).Pth('subdirectories').Pth('name')));
-
-                        var dirBaseName = "newSubdir";
-                        var currentDirName = dirBaseName;
-                        var collisions = 0;
-                        var nameFound = false;
-                        while (!nameFound) {
-                            var nameTaken = false;
-
-                            for (let n in subDirNames) {
-                                if (subDirNames[n] == currentDirName) {
-                                    nameTaken = true;
-                                    break;
-                                }
-                            }
+    };
 
-                            if (nameTaken) {
-                                currentDirName = dirBaseName + (collisions + 1);
-                                collisions += 1;
-                            } else {
-                                nameFound = true;
-                            }
-                        }
+    //setup workspace directory
+    this.workspaceDirectory = new Directory(this, 0, true, "Workspace");
 
-                        var cmd = new eoq2.Cmp();
-                        cmd.Crn('http://www.eoq.de/workspacemdbmodel/v1.0', 'Directory');
-                        cmd.Set(new eoq2.His(-1), 'name', currentDirName);
-                        cmd.Add(new eoq2.Obj(data.eObject.get("_#EOQ")), 'subdirectories', new eoq2.His(0));
-                        ecoreSync.exec(cmd)
+    var Metamodel = function(workspace, objectId) {
+        var self = this;
+        this.workspace = workspace;
+        this.objectId = objectId;
+        this.name = "";
+        this.isMetamodel = true;
+        this.isWorkspaceObject = true;
+    };
 
-                    }
+    var ModelObject = function(workspace, eObject, featureObj = null) {
+        var self = this;
+        this.__listeners = [];
+        this.workspace = workspace;
+        this.eObject = eObject;
+        this.featureObj = featureObj
+        this.feature = featureObj ? featureObj.get('name') : null;
+        this.isModelObject = true;
+        this.isWorkspaceObject = true;
+        this.__update = new rateLimitedFunctionCall(function() {
+            self.fireOnUpdate();
+        }, 10);
+        this.onUpdate = function(cb) {
+            if (self.__listeners.indexOf(cb) == -1) {
+                self.__listeners.push(cb);
+            }
+        };
+        this.fireOnUpdate = function() {
+            for (let i in self.__listeners) {
+                setTimeout(self.__listeners[i], 1);
+            }
+        }
+        if (eObject) {
+            if (self.feature == null) {
+                self.eObject.noproxy.on('change', function(change) {
+                    self.__update.runRateLimited();
+                });
+            } else {
+                //BA: changed
+                //let featureName = self.feature.get('name');
+                if (self.featureObj.get('upperBound') == 1) {
+                    self.eObject.noproxy.on('change:' + self.feature, function(change) {
+                        self.__update.runRateLimited();
+                    });
+                } else {
+                    self.eObject.noproxy.on('add:' + self.feature, function(change) {
+                        self.__update.runRateLimited();
+                    });
+                    self.eObject.noproxy.on('remove:' + self.feature, function(change) {
+                        self.__update.runRateLimited();
+                    });
                 }
-            };
-
-            var eoqMenu = {
-                callback: function(key, options) {
-                    //TODO: menu actions
-                    if (key == "delete") {
-                        var dialog = new jsa.MsgBox({
-                            content: 'Do you really want to delete ' + data.eObject.get("name") + '? This action can not be undone.',
-                            buttons: {
-                                yes: {
-                                    name: 'Yes',
-                                    startEnabled: true,
-                                    data: this,
-                                    onClickCallback: function(event) {
-                                        //MB: why is there another layer above ecoreSync?
-                                        pluginAPI.getGlobal('app').commandManager.Execute(new ERemoveCommand(ecoreSync, data.eObject.eContainer, data.eObject.eContainingFeature.get("name"), data.eObject));
-                                        dialog.Dissolve();
-                                    }
-                                },
-                                no: {
-                                    name: 'No',
-                                    startEnabled: true,
-                                    data: this,
-                                    onClickCallback: function(event) {
-                                        dialog.Dissolve();
-                                    }
-                                }
-                            }
-                        });
-                        pluginAPI.getGlobal('app').AddChild(dialog);
-
-                        /*
-                        ecoreSync.remove(data.eObject.eContainer,data.eObject.eContainingFeature.get("name"),data.eObject).then(function(){
-                            if ($DEBUG) console.debug('eObject successfully removed from reference')
-                        })     
-                        */
-                    }
-
-                    if (key == "rename") {
-                        node.editStart();
-                    }
-
-
-
-
-                },
-                items: {}
-            };
+            }
+        }
+    };
 
 
-            if (data.eObject.eClass.get("name") == "Directory" || data.eObject.eClass.get("name") == "Workspace") {
-                eoqMenu.items['create'] = {
-                    name: 'Create',
-                    icon: 'add',
-                    action: false,
-                    items: dirCreatableItems
-                };
+    this.getType = function(object) {
+        if (object) {
+            if (object == self) {
+                return "WORKSPACE";
             }
-            if (data.eObject.eClass.get("name") != "Workspace") {
-                eoqMenu.items['delete'] = {
-                    name: "Delete",
-                    icon: "delete"
-                };
+
+            if (object.hasOwnProperty("isWorkspaceObject")) {
+                if (object.isResource) {
+                    return "RESOURCE";
+                }
+                if (object.isDirectory) {
+                    return "DIRECTORY";
+                }
+                if (object.isMetamodel) {
+                    return "METAMODEL";
+                }
+                if (object.isModelObject) {
+                    return "MODELOBJECT";
+                }
             }
+        }
+    };
 
-            return eoqMenu;
+    this.createModelObject = function(eObject, feature) {
+        var modelObject = new ModelObject(self, eObject, feature);
+        return modelObject;
+    }
 
-        };
+    this.getContents = function() {
+        return this.workspaceDirectory.getContents();
     }
 
+    this.isInitialized = function() {
+        //Proxy for workspace directory initialization
+        return self.workspaceDirectory.isInitialized();
+    }
+
+    this.onUpdate = function(cb) {
+        this.workspaceDirectory.onUpdate(cb);
+    }
 
-    pluginAPI.implement("plugin.ecoreTreeView.views", WorkspaceView);
-    pluginAPI.implement("plugin.ecoreTreeView.controllers", WorkspaceController);
-    pluginAPI.implement("plugin.ecoreTreeView.controllers", DirectoryController);
-    pluginAPI.implement("plugin.ecoreTreeView.controllers", ResourceController);
-    pluginAPI.implement('plugin.ecoreTreeView.menus', WorkspaceContextMenu);
-    return Promise.resolve();
-
-};
-
-export var meta = {
-    "id": "plugin.ecoreTreeView.eoq",
-    description: "EOQ Plugin for Ecore Tree View",
-    "author": "Matthias Brunner",
-    "version": "0.0.1",
-    "requires": ['plugin.ecoreTreeView']
-};
+}
```

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/LICENSE.txt` & `XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/jquery.fancytree-all-deps.min.js` & `XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/jquery.fancytree-all-deps.min.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/jquery.fancytree-all-deps.min.js.map` & `XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/jquery.fancytree-all-deps.min.js.map`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/skin-win8/icons-rtl.gif` & `XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/skin-win8/icons-rtl.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/skin-win8/icons.gif` & `XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/skin-win8/icons.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/skin-win8/loading.gif` & `XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/skin-win8/loading.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/skin-win8/ui.fancytree.css` & `XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/skin-win8/ui.fancytree.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/skin-win8/ui.fancytree.less` & `XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/skin-win8/ui.fancytree.less`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/skin-win8/vline-rtl.gif` & `XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/skin-win8/vline-rtl.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/plugin.fancyTree/skin-win8/vline.gif` & `XGEE-0.3.7/xgee/core/plugins/plugin.fancyTree/skin-win8/vline.gif`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/propertiesView/css/PropertiesView.css` & `XGEE-0.3.7/xgee/core/plugins/propertiesView/css/PropertiesView.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/propertiesView/doc/PropertiesView.pptx` & `XGEE-0.3.7/xgee/core/plugins/propertiesView/doc/PropertiesView.pptx`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/propertiesView/js/LoadOnDemandView.js` & `XGEE-0.3.7/xgee/core/plugins/propertiesView/js/LoadOnDemandView.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/propertiesView/js/PropertiesPaneProvider.js` & `XGEE-0.3.7/xgee/core/plugins/propertiesView/js/PropertiesPaneProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/propertiesView/js/PropertiesViewController.js` & `XGEE-0.3.7/xgee/core/plugins/propertiesView/js/PropertiesViewController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/propertiesView/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/propertiesView/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore/js/EObjectPropertiesPane.js` & `XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore/js/EObjectPropertiesPane.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore/js/EObjectPropertiesPaneProvider.js` & `XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore/js/EObjectPropertiesPaneProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPane.js` & `XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPane.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPaneConfig.js` & `XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPaneConfig.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPaneProvider.js` & `XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.custom/js/CustomPropertiesPaneProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.custom/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.custom/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.editors/js/EcoreEditorsPropertiesPane.js` & `XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.editors/js/EcoreEditorsPropertiesPane.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.editors/js/EcoreEditorsPropertiesPaneProvider.js` & `XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.editors/js/EcoreEditorsPropertiesPaneProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.editors/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.editors/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.modify/js/EcoreModifyPropertiesPane.js` & `XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.modify/js/EcoreModifyPropertiesPane.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.modify/js/EcoreModifyPropertiesPaneProvider.js` & `XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.modify/js/EcoreModifyPropertiesPaneProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.modify/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.modify/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.workspace/js/WorkspacePropertiesPaneConfig.js` & `XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.workspace/js/WorkspacePropertiesPaneConfig.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/propertiesView.ecore.workspace/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/propertiesView.ecore.workspace/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/propertiesView.info/js/InfoPropertiesPaneProvider.js` & `XGEE-0.3.7/xgee/core/plugins/propertiesView.info/js/InfoPropertiesPaneProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/propertiesView.info/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/propertiesView.info/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/tool.goToView/img/tool-go-to-view.svg` & `XGEE-0.3.7/xgee/core/plugins/tool.goToView/img/tool-go-to-view.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/tool.goToView/js/GoToViewTool.js` & `XGEE-0.3.7/xgee/core/plugins/tool.goToView/js/GoToViewTool.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/tool.goToView/js/GoToViewToolProvider.js` & `XGEE-0.3.7/xgee/core/plugins/tool.goToView/js/GoToViewToolProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/tool.goToView/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/tool.goToView/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/tool.notes/css/NotesTool.css` & `XGEE-0.3.7/xgee/core/plugins/tool.notes/css/NotesTool.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/tool.notes/img/notes-error.svg` & `XGEE-0.3.7/xgee/core/plugins/tool.notes/img/notes-error.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/tool.notes/img/notes-info.svg` & `XGEE-0.3.7/xgee/core/plugins/tool.notes/img/notes-info.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/tool.notes/img/notes-success.svg` & `XGEE-0.3.7/xgee/core/plugins/tool.notes/img/notes-success.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/tool.notes/img/notes-warning.svg` & `XGEE-0.3.7/xgee/core/plugins/tool.notes/img/notes-warning.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/tool.notes/img/tool-notes.svg` & `XGEE-0.3.7/xgee/core/plugins/tool.notes/img/tool-notes.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/tool.notes/js/NotesTool.js` & `XGEE-0.3.7/xgee/core/plugins/tool.notes/js/NotesTool.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/tool.notes/js/NotesToolProvider.js` & `XGEE-0.3.7/xgee/core/plugins/tool.notes/js/NotesToolProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/tool.notes/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/tool.notes/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/tools/js/ToolsController.js` & `XGEE-0.3.7/xgee/core/plugins/tools/js/ToolsController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/tools/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/tools/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/view.dashboard/img/view-dashboard.svg` & `XGEE-0.3.7/xgee/core/plugins/view.dashboard/img/view-dashboard.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/view.dashboard/js/DashboardViewProvider.js` & `XGEE-0.3.7/xgee/core/plugins/view.dashboard/js/DashboardViewProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/view.dashboard/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/view.dashboard/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/view.dashboard.infoDash/js/InfoDashProvider.js` & `XGEE-0.3.7/xgee/core/plugins/view.dashboard.infoDash/js/InfoDashProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/view.dashboard.infoDash/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/view.dashboard.infoDash/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/css/StartModellingDash.css` & `XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/css/StartModellingDash.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/img/delete.svg` & `XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/img/delete.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/img/edit.svg` & `XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/img/edit.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/img/new-object.svg` & `XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/img/new-object.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/img/new-subdir.svg` & `XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/img/new-subdir.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/img/object.svg` & `XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/img/object.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/img/parent.svg` & `XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/img/parent.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/img/subdir.svg` & `XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/img/subdir.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDash.js` & `XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDash.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDashListEntry.js` & `XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDashListEntry.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDashProvider.js` & `XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/js/StartModellingDashProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/view.dashboard.startModellingDash/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/view.dashboard.startModellingDash/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/view.workspace/img/view-workspace.svg` & `XGEE-0.3.7/xgee/core/plugins/view.workspace/img/view-workspace.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/view.workspace/js/WorkspaceViewProvider.js` & `XGEE-0.3.7/xgee/core/plugins/view.workspace/js/WorkspaceViewProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/view.workspace/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/view.workspace/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/views/js/ViewsController.js` & `XGEE-0.3.7/xgee/core/plugins/views/js/ViewsController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/views/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/views/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/viewsMenu/js/ViewsMenuController.js` & `XGEE-0.3.7/xgee/core/plugins/viewsMenu/js/ViewsMenuController.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/viewsMenu/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/viewsMenu/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/viewsTabbar/css/ViewsTabbar.css` & `XGEE-0.3.7/xgee/core/plugins/viewsTabbar/css/ViewsTabbar.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/plugins/viewsTabbar/plugin.js` & `XGEE-0.3.7/xgee/core/plugins/viewsTabbar/plugin.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/css/app.css` & `XGEE-0.3.7/xgee/core/res/css/app.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/css/contextmenu.css` & `XGEE-0.3.7/xgee/core/res/css/contextmenu.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/css/notes.css` & `XGEE-0.3.7/xgee/core/res/css/notes.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/css/palette.css` & `XGEE-0.3.7/xgee/core/res/css/palette.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/css/uiControls.css` & `XGEE-0.3.7/xgee/core/res/css/uiControls.css`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/img/edit.svg` & `XGEE-0.3.7/xgee/core/res/img/edit.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/img/eye.svg` & `XGEE-0.3.7/xgee/core/res/img/eye.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/img/globe.svg` & `XGEE-0.3.7/xgee/core/res/img/globe.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/img/graph-view-oaam-allocations.svg` & `XGEE-0.3.7/xgee/core/res/img/graph-view-oaam-allocations.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/img/graph-view-oaam-functions.svg` & `XGEE-0.3.7/xgee/core/res/img/graph-view-oaam-functions.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/img/graph-view-oaam-hardware.svg` & `XGEE-0.3.7/xgee/core/res/img/graph-view-oaam-hardware.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/img/redo.svg` & `XGEE-0.3.7/xgee/core/res/img/redo.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/img/tool-domain-status-down.svg` & `XGEE-0.3.7/xgee/core/res/img/tool-domain-status-down.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/img/tool-domain-status-error.svg` & `XGEE-0.3.7/xgee/core/res/img/tool-domain-status-error.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/img/tool-domain-status-up-down.svg` & `XGEE-0.3.7/xgee/core/res/img/tool-domain-status-up-down.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/img/tool-domain-status-up.svg` & `XGEE-0.3.7/xgee/core/res/img/tool-domain-status-up.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/img/tool-domain-status.svg` & `XGEE-0.3.7/xgee/core/res/img/tool-domain-status.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/img/tree.svg` & `XGEE-0.3.7/xgee/core/res/img/tree.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/img/undo.svg` & `XGEE-0.3.7/xgee/core/res/img/undo.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/img/view-editor.svg` & `XGEE-0.3.7/xgee/core/res/img/view-editor.svg`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/js/DomainStatistics.js` & `XGEE-0.3.7/xgee/core/res/js/DomainStatistics.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/js/app.js` & `XGEE-0.3.7/xgee/core/res/js/app.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/js/commands.js` & `XGEE-0.3.7/xgee/core/res/js/commands.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/js/connectors/connectors.graph.js` & `XGEE-0.3.7/xgee/core/res/js/connectors/connectors.graph.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/js/connectors/connectors.selection.js` & `XGEE-0.3.7/xgee/core/res/js/connectors/connectors.selection.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/js/ports.js` & `XGEE-0.3.7/xgee/core/res/js/ports.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/js/ui/DomainStatusTool.js` & `XGEE-0.3.7/xgee/core/res/js/ui/DomainStatusTool.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/js/ui/ui.colorProvider.js` & `XGEE-0.3.7/xgee/core/res/js/ui/ui.colorProvider.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/core/res/js/workspace/workspace.jobs.js` & `XGEE-0.3.7/xgee/core/res/js/workspace/workspace.jobs.js`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/PyEoq2WebServer.py` & `XGEE-0.3.7/xgee/eoqserver/PyEoq2WebServer.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq1/actions/actionutils.py` & `XGEE-0.3.7/xgee/eoqserver/eoq1/actions/actionutils.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq1/actions/externalactionhandler.py` & `XGEE-0.3.7/xgee/eoqserver/eoq1/actions/externalactionhandler.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq1/commandparser.py` & `XGEE-0.3.7/xgee/eoqserver/eoq1/commandparser.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq1/domains/localdomain.py` & `XGEE-0.3.7/xgee/eoqserver/eoq1/domains/localdomain.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq1/domains/multiprocessingqueuedomainclient.py` & `XGEE-0.3.7/xgee/eoqserver/eoq1/domains/multiprocessingqueuedomainclient.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq1/domains/multiprocessingqueuedomainhost.py` & `XGEE-0.3.7/xgee/eoqserver/eoq1/domains/multiprocessingqueuedomainhost.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq1/domains/remotehttpdomain.py` & `XGEE-0.3.7/xgee/eoqserver/eoq1/domains/remotehttpdomain.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq1/domains/simplepythondomainwrapper.py` & `XGEE-0.3.7/xgee/eoqserver/eoq1/domains/simplepythondomainwrapper.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq1/error/error.py` & `XGEE-0.3.7/xgee/eoqserver/eoq1/error/error.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq1/model/__init__.py` & `XGEE-0.3.7/xgee/eoqserver/eoq1/model/__init__.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq1/model/model.py` & `XGEE-0.3.7/xgee/eoqserver/eoq1/model/model.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq1/queryparser.py` & `XGEE-0.3.7/xgee/eoqserver/eoq1/queryparser.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq1/resultparser.py` & `XGEE-0.3.7/xgee/eoqserver/eoq1/resultparser.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq1/utils/csvconnector.py` & `XGEE-0.3.7/xgee/eoqserver/eoq1/utils/csvconnector.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq1/valueparser.py` & `XGEE-0.3.7/xgee/eoqserver/eoq1/valueparser.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/action/action.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/action/action.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/action/call.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/action/call.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/action/callhandler.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/action/callhandler.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/action/callmanager.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/action/callmanager.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/action/cmdrunnerbasedcallmanager.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/action/cmdrunnerbasedcallmanager.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/action/externalpy/externalpyscripthandler.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/action/externalpy/externalpyscripthandler.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/action/util.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/action/util.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/command/command.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/command/command.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/command/commandrunner.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/command/commandrunner.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/command/diff.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/command/diff.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/command/result.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/command/result.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/domain/cmdrunnerbaseddomain.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/domain/cmdrunnerbaseddomain.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/domain/domain.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/domain/domain.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/domain/local/localmdbdomain.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/domain/local/localmdbdomain.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingcallmanager.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingcallmanager.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingdomainclient.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingdomainclient.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingdomainhost.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/domain/multiprocessing/multiprocessingdomainhost.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/domain/remote/websocketdomain.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/domain/remote/websocketdomain.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/event/event.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/event/event.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/frame/domainframehandler.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/frame/domainframehandler.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/frame/framehandler.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/frame/framehandler.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/frame/multiversionframehandler.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/frame/multiversionframehandler.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/legacy/legacy.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/legacy/legacy.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/mdbaccessor.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/mdbaccessor.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/constraintmodel/__init__.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/constraintmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/constraintmodel/constraintmodel.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/constraintmodel/constraintmodel.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/pyecoreidcodec.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/pyecoreidcodec.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/pyecoremdb.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/pyecoremdb.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/pyecoremdbaccessor.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/pyecoremdbaccessor.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresimpleobjectcodec.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresimpleobjectcodec.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresinglefilemdb.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresinglefilemdb.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresinglefilemdbprovider.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/pyecoresinglefilemdbprovider.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/pyecoreworkspacemdbprovider.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/pyecoreworkspacemdbprovider.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/workspacemdbmodel/__init__.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/workspacemdbmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/workspacemdbmodel/workspacemdbmodel.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/workspacemdbmodel/workspacemdbmodel.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/xmlresourcemodel/__init__.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/xmlresourcemodel/__init__.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/mdb/pyecore/xmlresourcemodel/xmlresourcemodel.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/mdb/pyecore/xmlresourcemodel/xmlresourcemodel.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/query/query.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/query/query.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/query/queryrunner.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/query/queryrunner.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/serialization/jsonserializer.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/serialization/jsonserializer.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/serialization/jsserializer.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/serialization/jsserializer.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/serialization/pyserializer.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/serialization/pyserializer.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/serialization/textserializer.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/serialization/textserializer.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/util/backup.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/util/backup.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/util/benchmark.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/util/benchmark.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/util/csvconnector.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/util/csvconnector.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/util/error.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/util/error.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/util/logger.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/util/logger.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/util/model.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/util/model.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/eoqserver/eoq2/util/util.py` & `XGEE-0.3.7/xgee/eoqserver/eoq2/util/util.py`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/meta/layout.ecore` & `XGEE-0.3.7/xgee/meta/layout.ecore`

 * *Files identical despite different names*

### Comparing `XGEE-0.3.6/xgee/xgee.py` & `XGEE-0.3.7/xgee/xgee.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 try:
     from yaml import CLoader as Loader, CDumper as Dumper
 except ImportError:
     from yaml import Loader, Dumper
 
 import __main__
 
-__version__ = '0.3.6'
+__version__ = '0.3.7'
 
 DEFAULT_PATH='./'
 DEFAULT_HOST=socket.gethostname()
 localpath=str(Path().resolve())
 FRAMEWORK_RUN_FLAG=True
 apps=[]
```


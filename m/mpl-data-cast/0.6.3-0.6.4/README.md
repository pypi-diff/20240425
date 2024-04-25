# Comparing `tmp/mpl_data_cast-0.6.3.tar.gz` & `tmp/mpl_data_cast-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl_data_cast-0.6.3.tar", last modified: Wed Apr 17 12:08:47 2024, max compression
+gzip compressed data, was "mpl_data_cast-0.6.4.tar", last modified: Thu Apr 25 06:45:14 2024, max compression
```

## Comparing `mpl_data_cast-0.6.3.tar` & `mpl_data_cast-0.6.4.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.584481 mpl_data_cast-0.6.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.568480 mpl_data_cast-0.6.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.572480 mpl_data_cast-0.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/.github/workflows/deploy_github.yml
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-17 12:08:47.584481 mpl_data_cast-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.572480 mpl_data_cast-0.6.3/build-recipes/
--rw-r--r--   0 runner    (1001) docker     (127)   108901 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/MPLDataCast.icns
--rw-r--r--   0 runner    (1001) docker     (127)   353118 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/MPLDataCast.ico
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/MPLDataCastLauncher.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/MPLDataCastLauncherCLI.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/hook-mpl_data_cast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/macos_MPLDataCast.spec
--rwxr-xr-x   0 runner    (1001) docker     (127)     1981 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/macos_build_app.sh
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/macos_build_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/win_MPLDataCast.spec
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/win_build_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/win_make_iss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/build-recipes/win_mpl-data-cast.iss_dummy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.576480 mpl_data_cast-0.6.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-17 12:08:39.000000 mpl_data_cast-0.6.3/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.576480 mpl_data_cast-0.6.3/docs/artwork/
--rw-r--r--   0 runner    (1001) docker     (127)    13309 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/artwork/mpldc_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15233 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/artwork/mpldc_splash.png
--rw-r--r--   0 runner    (1001) docker     (127)    14802 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/artwork/mpldc_splash.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.576480 mpl_data_cast-0.6.3/docs/scrots/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/scrots/make_scrots_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/scrots/ui_main.png
--rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/scrots/ui_preferences.png
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/sec_cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/sec_gui.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/docs/sec_intro.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.576480 mpl_data_cast-0.6.3/mpl_data_cast/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 12:08:47.000000 mpl_data_cast-0.6.3/mpl_data_cast/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.576480 mpl_data_cast-0.6.3/mpl_data_cast/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.580480 mpl_data_cast-0.6.3/mpl_data_cast/gui/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.580480 mpl_data_cast-0.6.3/mpl_data_cast/gui/img/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/img/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28754 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/img/mpldc_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    10542 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/main.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/preferences.ui
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/splash.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/widget_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/widget_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/widget_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/gui/widget_tree.ui
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.580480 mpl_data_cast-0.6.3/mpl_data_cast/mod_recipes/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/mod_recipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/mod_recipes/rcp_catchall.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/mod_recipes/rcp_oah.py
--rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/mod_recipes/rcp_qlsi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/mod_recipes/rcp_rtdc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11902 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/recipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/mpl_data_cast/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.580480 mpl_data_cast-0.6.3/mpl_data_cast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-17 12:08:47.000000 mpl_data_cast-0.6.3/mpl_data_cast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-17 12:08:47.000000 mpl_data_cast-0.6.3/mpl_data_cast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 12:08:47.000000 mpl_data_cast-0.6.3/mpl_data_cast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-17 12:08:47.000000 mpl_data_cast-0.6.3/mpl_data_cast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-17 12:08:47.000000 mpl_data_cast-0.6.3/mpl_data_cast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 12:08:47.000000 mpl_data_cast-0.6.3/mpl_data_cast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-17 12:08:47.584481 mpl_data_cast-0.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.580480 mpl_data_cast-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/tests/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:08:47.580480 mpl_data_cast-0.6.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)   116686 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/tests/data/rcp_rtdc_mask-contour_2018.zip
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/tests/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/tests/test_gui_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/tests/test_gui_rtdc.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/tests/test_rcp_catchall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/tests/test_rcp_rtdc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-17 12:08:40.000000 mpl_data_cast-0.6.3/tests/test_recipe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:45:14.754800 mpl_data_cast-0.6.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:45:14.738800 mpl_data_cast-0.6.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:45:14.742800 mpl_data_cast-0.6.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/.github/workflows/deploy_github.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-25 06:45:14.754800 mpl_data_cast-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:45:14.742800 mpl_data_cast-0.6.4/build-recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)   108901 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/build-recipes/MPLDataCast.icns
+-rw-r--r--   0 runner    (1001) docker     (127)   353118 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/build-recipes/MPLDataCast.ico
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/build-recipes/MPLDataCastLauncher.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/build-recipes/MPLDataCastLauncherCLI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/build-recipes/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/build-recipes/hook-mpl_data_cast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/build-recipes/macos_MPLDataCast.spec
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1981 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/build-recipes/macos_build_app.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/build-recipes/macos_build_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/build-recipes/win_MPLDataCast.spec
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/build-recipes/win_build_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/build-recipes/win_make_iss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/build-recipes/win_mpl-data-cast.iss_dummy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:45:14.746800 mpl_data_cast-0.6.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:45:14.746800 mpl_data_cast-0.6.4/docs/artwork/
+-rw-r--r--   0 runner    (1001) docker     (127)    13309 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/docs/artwork/mpldc_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15233 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/docs/artwork/mpldc_splash.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14802 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/docs/artwork/mpldc_splash.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:45:14.746800 mpl_data_cast-0.6.4/docs/scrots/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/docs/scrots/make_scrots_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/docs/scrots/ui_main.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/docs/scrots/ui_preferences.png
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/docs/sec_cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/docs/sec_gui.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/docs/sec_intro.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:45:14.746800 mpl_data_cast-0.6.4/mpl_data_cast/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 06:45:14.000000 mpl_data_cast-0.6.4/mpl_data_cast/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:45:14.746800 mpl_data_cast-0.6.4/mpl_data_cast/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:45:14.750800 mpl_data_cast-0.6.4/mpl_data_cast/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/gui/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:45:14.750800 mpl_data_cast-0.6.4/mpl_data_cast/gui/img/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/gui/img/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28754 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/gui/img/mpldc_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10542 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/gui/main.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/gui/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/gui/preferences.ui
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/gui/splash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/gui/widget_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/gui/widget_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/gui/widget_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/gui/widget_tree.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:45:14.750800 mpl_data_cast-0.6.4/mpl_data_cast/mod_recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/mod_recipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/mod_recipes/rcp_catchall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/mod_recipes/rcp_oah.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/mod_recipes/rcp_qlsi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/mod_recipes/rcp_rtdc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11902 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/mpl_data_cast/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:45:14.754800 mpl_data_cast-0.6.4/mpl_data_cast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-25 06:45:14.000000 mpl_data_cast-0.6.4/mpl_data_cast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-25 06:45:14.000000 mpl_data_cast-0.6.4/mpl_data_cast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 06:45:14.000000 mpl_data_cast-0.6.4/mpl_data_cast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-25 06:45:14.000000 mpl_data_cast-0.6.4/mpl_data_cast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-25 06:45:14.000000 mpl_data_cast-0.6.4/mpl_data_cast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 06:45:14.000000 mpl_data_cast-0.6.4/mpl_data_cast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-25 06:45:14.754800 mpl_data_cast-0.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:45:14.750800 mpl_data_cast-0.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/tests/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:45:14.754800 mpl_data_cast-0.6.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   116686 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/tests/data/rcp_rtdc_mask-contour_2018.zip
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/tests/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/tests/test_gui_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/tests/test_gui_rtdc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/tests/test_rcp_catchall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/tests/test_rcp_rtdc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-25 06:45:11.000000 mpl_data_cast-0.6.4/tests/test_recipe.py
```

### Comparing `mpl_data_cast-0.6.3/.github/workflows/check.yml` & `mpl_data_cast-0.6.4/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/.github/workflows/deploy_github.yml` & `mpl_data_cast-0.6.4/.github/workflows/deploy_github.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 name: Deploy to GitHub Releases
 
 on:
   push:
     tags:
       - '*'
 
+env:
+  PYINSTALLER_COMPILE_BOOTLOADER: 1
+
 jobs:
   build:
     name: Create Release
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
```

### Comparing `mpl_data_cast-0.6.3/.github/workflows/deploy_pypi.yml` & `mpl_data_cast-0.6.4/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/.gitignore` & `mpl_data_cast-0.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/CHANGELOG` & `mpl_data_cast-0.6.4/CHANGELOG`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+0.6.4
+ - setup: compile PyInstaller bootloader for every release
 0.6.3
  - fix: cleanup temporary directories on startup (#29)
  - fix: avoid possible name clashes when storing logs in DC output file
  - enh: warn user when source and target directory are identical (#28)
 0.6.2
  - setup: bump dclab from 0.55.7 to 0.57.0
 0.6.1
```

### Comparing `mpl_data_cast-0.6.3/LICENSE` & `mpl_data_cast-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/PKG-INFO` & `mpl_data_cast-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl_data_cast
-Version: 0.6.3
+Version: 0.6.4
 Summary: convert and transfer data to network shares
 Author: Benedikt Hartmann, Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: GPL v3
 Project-URL: source, https://github.com/GuckLab/MPL-Data-Cast
 Project-URL: tracker, https://github.com/GuckLab/MPL-Data-Cast/issues
 Project-URL: documentation, https://mpl-data-cast.readthedocs.io
```

### Comparing `mpl_data_cast-0.6.3/README.rst` & `mpl_data_cast-0.6.4/README.rst`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/build-recipes/MPLDataCast.icns` & `mpl_data_cast-0.6.4/build-recipes/MPLDataCast.icns`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/build-recipes/MPLDataCast.ico` & `mpl_data_cast-0.6.4/build-recipes/MPLDataCast.ico`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/build-recipes/Readme.md` & `mpl_data_cast-0.6.4/build-recipes/Readme.md`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/build-recipes/hook-mpl_data_cast.py` & `mpl_data_cast-0.6.4/build-recipes/hook-mpl_data_cast.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/build-recipes/macos_MPLDataCast.spec` & `mpl_data_cast-0.6.4/build-recipes/macos_MPLDataCast.spec`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/build-recipes/macos_build_app.sh` & `mpl_data_cast-0.6.4/build-recipes/macos_build_app.sh`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/build-recipes/win_MPLDataCast.spec` & `mpl_data_cast-0.6.4/build-recipes/win_MPLDataCast.spec`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/build-recipes/win_make_iss.py` & `mpl_data_cast-0.6.4/build-recipes/win_make_iss.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/build-recipes/win_mpl-data-cast.iss_dummy` & `mpl_data_cast-0.6.4/build-recipes/win_mpl-data-cast.iss_dummy`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/docs/artwork/mpldc_icon.svg` & `mpl_data_cast-0.6.4/docs/artwork/mpldc_icon.svg`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/docs/artwork/mpldc_splash.png` & `mpl_data_cast-0.6.4/docs/artwork/mpldc_splash.png`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/docs/artwork/mpldc_splash.svg` & `mpl_data_cast-0.6.4/docs/artwork/mpldc_splash.svg`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/docs/conf.py` & `mpl_data_cast-0.6.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/docs/scrots/ui_main.png` & `mpl_data_cast-0.6.4/docs/scrots/ui_main.png`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/docs/scrots/ui_preferences.png` & `mpl_data_cast-0.6.4/docs/scrots/ui_preferences.png`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/docs/sec_gui.rst` & `mpl_data_cast-0.6.4/docs/sec_gui.rst`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/docs/sec_intro.rst` & `mpl_data_cast-0.6.4/docs/sec_intro.rst`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/mpl_data_cast/cli/cli.py` & `mpl_data_cast-0.6.4/mpl_data_cast/cli/cli.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/mpl_data_cast/gui/__main__.py` & `mpl_data_cast-0.6.4/mpl_data_cast/gui/__main__.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/mpl_data_cast/gui/img/mpldc_icon.png` & `mpl_data_cast-0.6.4/mpl_data_cast/gui/img/mpldc_icon.png`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/mpl_data_cast/gui/main.py` & `mpl_data_cast-0.6.4/mpl_data_cast/gui/main.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/mpl_data_cast/gui/main.ui` & `mpl_data_cast-0.6.4/mpl_data_cast/gui/main.ui`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/mpl_data_cast/gui/preferences.py` & `mpl_data_cast-0.6.4/mpl_data_cast/gui/preferences.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/mpl_data_cast/gui/preferences.ui` & `mpl_data_cast-0.6.4/mpl_data_cast/gui/preferences.ui`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/mpl_data_cast/gui/widget_tree.py` & `mpl_data_cast-0.6.4/mpl_data_cast/gui/widget_tree.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/mpl_data_cast/gui/widget_tree.ui` & `mpl_data_cast-0.6.4/mpl_data_cast/gui/widget_tree.ui`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/mpl_data_cast/helper.py` & `mpl_data_cast-0.6.4/mpl_data_cast/helper.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/mpl_data_cast/mod_recipes/rcp_catchall.py` & `mpl_data_cast-0.6.4/mpl_data_cast/mod_recipes/rcp_catchall.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/mpl_data_cast/mod_recipes/rcp_oah.py` & `mpl_data_cast-0.6.4/mpl_data_cast/mod_recipes/rcp_oah.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/mpl_data_cast/mod_recipes/rcp_qlsi.py` & `mpl_data_cast-0.6.4/mpl_data_cast/mod_recipes/rcp_qlsi.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/mpl_data_cast/mod_recipes/rcp_rtdc.py` & `mpl_data_cast-0.6.4/mpl_data_cast/mod_recipes/rcp_rtdc.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/mpl_data_cast/recipe.py` & `mpl_data_cast-0.6.4/mpl_data_cast/recipe.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/mpl_data_cast/util.py` & `mpl_data_cast-0.6.4/mpl_data_cast/util.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/mpl_data_cast.egg-info/PKG-INFO` & `mpl_data_cast-0.6.4/mpl_data_cast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl_data_cast
-Version: 0.6.3
+Version: 0.6.4
 Summary: convert and transfer data to network shares
 Author: Benedikt Hartmann, Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: GPL v3
 Project-URL: source, https://github.com/GuckLab/MPL-Data-Cast
 Project-URL: tracker, https://github.com/GuckLab/MPL-Data-Cast/issues
 Project-URL: documentation, https://mpl-data-cast.readthedocs.io
```

### Comparing `mpl_data_cast-0.6.3/mpl_data_cast.egg-info/SOURCES.txt` & `mpl_data_cast-0.6.4/mpl_data_cast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/pyproject.toml` & `mpl_data_cast-0.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/tests/data/rcp_rtdc_mask-contour_2018.zip` & `mpl_data_cast-0.6.4/tests/data/rcp_rtdc_mask-contour_2018.zip`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/tests/test_gui_basic.py` & `mpl_data_cast-0.6.4/tests/test_gui_basic.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/tests/test_gui_rtdc.py` & `mpl_data_cast-0.6.4/tests/test_gui_rtdc.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/tests/test_rcp_catchall.py` & `mpl_data_cast-0.6.4/tests/test_rcp_catchall.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/tests/test_rcp_rtdc.py` & `mpl_data_cast-0.6.4/tests/test_rcp_rtdc.py`

 * *Files identical despite different names*

### Comparing `mpl_data_cast-0.6.3/tests/test_recipe.py` & `mpl_data_cast-0.6.4/tests/test_recipe.py`

 * *Files identical despite different names*


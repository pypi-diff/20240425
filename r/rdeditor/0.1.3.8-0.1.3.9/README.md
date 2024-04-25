# Comparing `tmp/rdeditor-0.1.3.8.tar.gz` & `tmp/rdeditor-0.1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdeditor-0.1.3.8.tar", last modified: Fri Apr 12 12:51:30 2024, max compression
+gzip compressed data, was "rdeditor-0.1.3.9.tar", last modified: Thu Apr 25 08:03:59 2024, max compression
```

## Comparing `rdeditor-0.1.3.8.tar` & `rdeditor-0.1.3.9.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:51:30.470513 rdeditor-0.1.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:51:30.446513 rdeditor-0.1.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:51:30.446513 rdeditor-0.1.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/.github/workflows/actions.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/CITATION.bib
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/DEVELOPER.md
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-12 12:51:30.470513 rdeditor-0.1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:51:30.446513 rdeditor-0.1.3.8/Screenshots/
--rw-r--r--   0 runner    (1001) docker     (127)    52961 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/Screenshots/Main_window.png
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/Screenshots/Side_bar.png
--rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/Screenshots/Top_Menu.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:51:30.450513 rdeditor-0.1.3.8/rdeditor/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/Mendelev_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-12 12:51:30.000000 rdeditor-0.1.3.8/rdeditor/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:51:30.446513 rdeditor-0.1.3.8/rdeditor/icon_themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:51:30.450513 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:51:30.458513 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/Change_E_Z.png
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/Change_E_Z.svg
--rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/Change_R_S.png
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/about.png
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/appicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/calc.png
--rw-r--r--   0 runner    (1001) docker     (127)    20137 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/exit.png
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/grid.png
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Broom.png
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Bulleted List.png
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Cancel.png
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Carbon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Cursor.png
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Decrease Font.png
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Delete.png
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Double.png
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Edit.png
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Exit.png
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Hydrogen.png
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Increase Font.png
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Info.png
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Left.png
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Line.png
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Minus.png
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Molecule.png
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Open.png
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Oxygen.png
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Physics.png
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Pinch.png
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Redo.png
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Replace Atom.png
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Reset.png
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Right.png
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Save as.png
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Save.png
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Scatter Plot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Shutdown.png
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Single.png
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Trash.png
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Triple.png
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Undo.png
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-copy-96.png
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-paste-100.png
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/molblock.png
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/next.png
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/open.png
--rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/plot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/prev.png
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/ptable.png
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/ptable.svg
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/dark/index.theme
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:51:30.458513 rdeditor-0.1.3.8/rdeditor/icon_themes/light/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:51:30.470513 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/
--rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/Change_E_Z.png
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/Change_E_Z.svg
--rw-r--r--   0 runner    (1001) docker     (127)    16252 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/Change_R_S.png
--rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/about.png
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/appicon copy.png
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/appicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/appicon.svg.png
--rw-r--r--   0 runner    (1001) docker     (127)     7764 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/calc.png
--rw-r--r--   0 runner    (1001) docker     (127)    20176 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/exit.png
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/grid.png
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Broom.png
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Bulleted List.png
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Cancel.png
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Carbon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Cursor.png
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Decrease Font.png
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Delete.png
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Double.png
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Edit.png
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Exit.png
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Hydrogen.png
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Increase Font.png
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Info.png
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Left.png
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Line.png
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Minus.png
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Molecule.png
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Open.png
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Oxygen.png
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Physics.png
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Pinch.png
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Redo.png
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Replace Atom.png
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Reset.png
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Right.png
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Save as.png
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Save.png
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Scatter Plot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Shutdown.png
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Single.png
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Trash.png
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Triple.png
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Undo.png
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-copy-96.png
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-paste-100.png
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/molblock.png
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/next.png
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/open.png
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/plot.png
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/prev.png
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/ptable.png
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/ptable.svg
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/icon_themes/light/index.theme
--rw-r--r--   0 runner    (1001) docker     (127)    17024 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/molEditWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/molViewWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/ptable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/ptable_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    28183 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/rdeditor/rdEditor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:51:30.470513 rdeditor-0.1.3.8/rdeditor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-12 12:51:30.000000 rdeditor-0.1.3.8/rdeditor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-12 12:51:30.000000 rdeditor-0.1.3.8/rdeditor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:51:30.000000 rdeditor-0.1.3.8/rdeditor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 12:51:30.000000 rdeditor-0.1.3.8/rdeditor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:51:30.000000 rdeditor-0.1.3.8/rdeditor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-12 12:51:30.000000 rdeditor-0.1.3.8/rdeditor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 12:51:30.000000 rdeditor-0.1.3.8/rdeditor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 12:51:30.470513 rdeditor-0.1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-12 12:51:21.000000 rdeditor-0.1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:59.375580 rdeditor-0.1.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:59.347580 rdeditor-0.1.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:59.351580 rdeditor-0.1.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/.github/workflows/actions.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/CITATION.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/DEVELOPER.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-25 08:03:59.375580 rdeditor-0.1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:59.351580 rdeditor-0.1.3.9/Screenshots/
+-rw-r--r--   0 runner    (1001) docker     (127)    52961 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/Screenshots/Main_window.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/Screenshots/Side_bar.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/Screenshots/Top_Menu.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:59.351580 rdeditor-0.1.3.9/rdeditor/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/Mendelev_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-25 08:03:59.000000 rdeditor-0.1.3.9/rdeditor/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:59.347580 rdeditor-0.1.3.9/rdeditor/icon_themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:59.355580 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:59.363580 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/Change_E_Z.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/Change_E_Z.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/Change_R_S.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/about.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/appicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/calc.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20137 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/exit.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/grid.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Broom.png
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Bulleted List.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Cancel.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Carbon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Cursor.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Decrease Font.png
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Delete.png
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Double.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Edit.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Exit.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Hydrogen.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Increase Font.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Info.png
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Left.png
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Line.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Molecule.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Open.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Oxygen.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Physics.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Pinch.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Redo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Replace Atom.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Reset.png
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Right.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Save as.png
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Save.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Scatter Plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Shutdown.png
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Single.png
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Trash.png
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Triple.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Undo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-copy-96.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-paste-100.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/molblock.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/next.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/open.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/prev.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/ptable.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/ptable.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/dark/index.theme
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:59.363580 rdeditor-0.1.3.9/rdeditor/icon_themes/light/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:59.375580 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/
+-rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/Change_E_Z.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/Change_E_Z.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    16252 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/Change_R_S.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/about.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/appicon copy.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/appicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/appicon.svg.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7764 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/calc.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20176 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/exit.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/grid.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Broom.png
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Bulleted List.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Cancel.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Carbon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Cursor.png
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Decrease Font.png
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Delete.png
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Double.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Edit.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Exit.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Hydrogen.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Increase Font.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Info.png
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Left.png
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Line.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Molecule.png
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Open.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Oxygen.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Physics.png
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Pinch.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Redo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Replace Atom.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Reset.png
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Right.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Save as.png
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Save.png
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Scatter Plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Shutdown.png
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Single.png
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Trash.png
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Triple.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Undo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-copy-96.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-paste-100.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/molblock.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/next.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/open.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/prev.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/ptable.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/ptable.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/icon_themes/light/index.theme
+-rw-r--r--   0 runner    (1001) docker     (127)    17024 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/molEditWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/molViewWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/ptable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/ptable_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28148 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/rdeditor/rdEditor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:03:59.375580 rdeditor-0.1.3.9/rdeditor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-25 08:03:59.000000 rdeditor-0.1.3.9/rdeditor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-25 08:03:59.000000 rdeditor-0.1.3.9/rdeditor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:03:59.000000 rdeditor-0.1.3.9/rdeditor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 08:03:59.000000 rdeditor-0.1.3.9/rdeditor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:03:59.000000 rdeditor-0.1.3.9/rdeditor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-25 08:03:59.000000 rdeditor-0.1.3.9/rdeditor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 08:03:59.000000 rdeditor-0.1.3.9/rdeditor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 08:03:59.375580 rdeditor-0.1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-25 08:03:52.000000 rdeditor-0.1.3.9/setup.py
```

### Comparing `rdeditor-0.1.3.8/.github/workflows/actions.yml` & `rdeditor-0.1.3.9/.github/workflows/actions.yml`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/.gitignore` & `rdeditor-0.1.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/CITATION.bib` & `rdeditor-0.1.3.9/CITATION.bib`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/DEVELOPER.md` & `rdeditor-0.1.3.9/DEVELOPER.md`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/LICENSE` & `rdeditor-0.1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/PKG-INFO` & `rdeditor-0.1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdeditor
-Version: 0.1.3.8
+Version: 0.1.3.9
 Summary: An RDKit based molecule editor using PySide
 Home-page: http://github.com/ebjerrum/rdeditor
 Author: Esben Jannik Bjerrum
 Author-email: esbenjannik@rocketmail.com
 License: LGPL
 Keywords: RDKit molecule editor pyside
 Requires-Python: >=3.8
```

### Comparing `rdeditor-0.1.3.8/README.md` & `rdeditor-0.1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/Screenshots/Main_window.png` & `rdeditor-0.1.3.9/Screenshots/Main_window.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/Screenshots/Side_bar.png` & `rdeditor-0.1.3.9/Screenshots/Side_bar.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/Screenshots/Top_Menu.png` & `rdeditor-0.1.3.9/Screenshots/Top_Menu.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/Change_E_Z.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/Change_E_Z.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/Change_E_Z.svg` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/Change_E_Z.svg`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/Change_R_S.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/Change_R_S.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/about.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/about.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/appicon.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/appicon.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/calc.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/calc.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/exit.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/exit.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/grid.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/grid.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Broom.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Broom.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Bulleted List.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Bulleted List.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Cancel.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Cancel.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Carbon.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Carbon.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Cursor.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Cursor.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Decrease Font.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Decrease Font.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Delete.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Delete.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Double.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Double.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Edit.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Edit.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Exit.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Exit.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Hydrogen.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Hydrogen.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Increase Font.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Increase Font.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Info.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Info.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Left.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Left.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Line.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Line.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Minus.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Minus.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Molecule.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Molecule.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Open.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Open.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Oxygen.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Oxygen.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Physics.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Physics.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Pinch.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Pinch.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Plus.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Plus.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Redo.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Redo.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Replace Atom.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Replace Atom.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Reset.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Reset.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Right.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Right.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Save as.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Save as.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Save.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Save.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Scatter Plot.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Scatter Plot.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Shutdown.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Shutdown.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Single.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Single.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Trash.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Trash.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Triple.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Triple.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-Undo.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-Undo.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-copy-96.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-copy-96.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/icons8-paste-100.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/icons8-paste-100.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/molblock.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/molblock.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/next.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/next.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/open.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/open.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/plot.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/plot.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/prev.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/prev.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/ptable.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/ptable.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/dark/application/ptable.svg` & `rdeditor-0.1.3.9/rdeditor/icon_themes/dark/application/ptable.svg`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/Change_E_Z.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/Change_E_Z.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/Change_E_Z.svg` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/Change_E_Z.svg`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/Change_R_S.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/Change_R_S.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/about.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/about.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/appicon copy.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/appicon copy.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/appicon.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/appicon.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/appicon.svg.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/appicon.svg.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/calc.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/calc.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/exit.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/exit.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/grid.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/grid.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Broom.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Broom.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Bulleted List.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Bulleted List.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Cancel.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Cancel.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Carbon.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Carbon.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Cursor.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Cursor.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Decrease Font.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Decrease Font.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Delete.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Delete.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Edit.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Edit.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Exit.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Exit.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Hydrogen.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Hydrogen.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Increase Font.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Increase Font.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Info.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Info.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Left.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Left.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Minus.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Minus.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Molecule.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Molecule.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Open.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Open.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Oxygen.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Oxygen.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Physics.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Physics.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Pinch.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Pinch.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Plus.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Plus.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Redo.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Redo.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Replace Atom.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Replace Atom.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Reset.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Reset.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Right.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Right.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Save as.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Save as.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Save.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Save.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Scatter Plot.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Scatter Plot.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Shutdown.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Shutdown.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Trash.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Trash.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Triple.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Triple.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-Undo.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-Undo.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-copy-96.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-copy-96.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/icons8-paste-100.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/icons8-paste-100.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/molblock.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/molblock.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/next.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/next.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/open.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/open.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/plot.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/plot.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/prev.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/prev.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/ptable.png` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/ptable.png`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/icon_themes/light/application/ptable.svg` & `rdeditor-0.1.3.9/rdeditor/icon_themes/light/application/ptable.svg`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/molEditWidget.py` & `rdeditor-0.1.3.9/rdeditor/molEditWidget.py`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/molViewWidget.py` & `rdeditor-0.1.3.9/rdeditor/molViewWidget.py`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/ptable.py` & `rdeditor-0.1.3.9/rdeditor/ptable.py`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/ptable_widget.py` & `rdeditor-0.1.3.9/rdeditor/ptable_widget.py`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/rdeditor/rdEditor.py` & `rdeditor-0.1.3.9/rdeditor/rdEditor.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,15 +354,15 @@
             self.ptable.close()
             exit(0)  # TODO, how to exit qapplication from within class instance?
         else:
             self.editor.logger.debug("Abort closing")
 
     # Function to show Diaglog box with provided Title and Message
     def msgApp(self, title, msg):
-        userInfo = QMessageBox.question(self, title, msg, QMessageBox.Yes or QMessageBox.No)
+        userInfo = QMessageBox.question(self, title, msg)
         if userInfo == QMessageBox.Yes:
             return "Y"
         if userInfo == QMessageBox.No:
             return "N"
         self.close()
 
     def aboutHelp(self):
```

### Comparing `rdeditor-0.1.3.8/rdeditor.egg-info/PKG-INFO` & `rdeditor-0.1.3.9/rdeditor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdeditor
-Version: 0.1.3.8
+Version: 0.1.3.9
 Summary: An RDKit based molecule editor using PySide
 Home-page: http://github.com/ebjerrum/rdeditor
 Author: Esben Jannik Bjerrum
 Author-email: esbenjannik@rocketmail.com
 License: LGPL
 Keywords: RDKit molecule editor pyside
 Requires-Python: >=3.8
```

### Comparing `rdeditor-0.1.3.8/rdeditor.egg-info/SOURCES.txt` & `rdeditor-0.1.3.9/rdeditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rdeditor-0.1.3.8/setup.py` & `rdeditor-0.1.3.9/setup.py`

 * *Files identical despite different names*


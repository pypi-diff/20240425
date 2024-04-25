# Comparing `tmp/Dpowers-0.1.5rc1.tar.gz` & `tmp/Dpowers-0.1.5rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dpowers-0.1.5rc1.tar", last modified: Sat Mar 11 18:45:12 2023, max compression
+gzip compressed data, was "Dpowers-0.1.5rc2.tar", last modified: Sun Jan  7 20:33:43 2024, max compression
```

## Comparing `Dpowers-0.1.5rc1.tar` & `Dpowers-0.1.5rc2.tar`

### file list

```diff
@@ -1,202 +1,202 @@
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.914154 Dpowers-0.1.5rc1/
--rw-rw-r--   0 d         (1000) d         (1000)      112 2021-02-11 22:26:21.000000 Dpowers-0.1.5rc1/.gitignore
--rw-rw-r--   0 d         (1000) d         (1000)    35149 2020-03-01 00:41:51.000000 Dpowers-0.1.5rc1/COPYING
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.898154 Dpowers-0.1.5rc1/Dlib/
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.902154 Dpowers-0.1.5rc1/Dlib/Dhelpers/
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.902154 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/
--rw-rw-r--   0 d         (1000) d         (1000)     5861 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/__init__.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.906154 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/
--rw-rw-r--   0 d         (1000) d         (1000)      689 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)     3663 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/al.json
--rw-rw-r--   0 d         (1000) d         (1000)     2519 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/am.json
--rw-rw-r--   0 d         (1000) d         (1000)     2301 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/apl.json
--rw-rw-r--   0 d         (1000) d         (1000)     3922 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/at.json
--rw-rw-r--   0 d         (1000) d         (1000)     2026 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/au.json
--rw-rw-r--   0 d         (1000) d         (1000)     1414 2021-04-05 21:23:17.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/base.json
--rw-rw-r--   0 d         (1000) d         (1000)     3775 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/be.json
--rw-rw-r--   0 d         (1000) d         (1000)     4145 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/bt.json
--rw-rw-r--   0 d         (1000) d         (1000)     2477 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/by.json
--rw-rw-r--   0 d         (1000) d         (1000)     2721 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/cd.json
--rw-rw-r--   0 d         (1000) d         (1000)     3778 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ch.json
--rw-rw-r--   0 d         (1000) d         (1000)     2026 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/cm.json
--rw-rw-r--   0 d         (1000) d         (1000)     2026 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/cn.json
--rw-rw-r--   0 d         (1000) d         (1000)     3922 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/de.json
--rw-rw-r--   0 d         (1000) d         (1000)     3881 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/dk.json
--rw-rw-r--   0 d         (1000) d         (1000)     3688 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ee.json
--rw-rw-r--   0 d         (1000) d         (1000)     2474 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/epo.json
--rw-rw-r--   0 d         (1000) d         (1000)     3671 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/es.json
--rw-rw-r--   0 d         (1000) d         (1000)     3891 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/fo.json
--rw-rw-r--   0 d         (1000) d         (1000)     3706 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/fr.json
--rw-rw-r--   0 d         (1000) d         (1000)     2758 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ge.json
--rw-rw-r--   0 d         (1000) d         (1000)     2062 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/gh.json
--rw-rw-r--   0 d         (1000) d         (1000)     2346 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/gn.json
--rw-rw-r--   0 d         (1000) d         (1000)     3848 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/hu.json
--rw-rw-r--   0 d         (1000) d         (1000)     3745 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ie.json
--rw-rw-r--   0 d         (1000) d         (1000)     3799 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/is.json
--rw-rw-r--   0 d         (1000) d         (1000)     3777 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/it.json
--rw-rw-r--   0 d         (1000) d         (1000)     2435 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/kg.json
--rw-rw-r--   0 d         (1000) d         (1000)     2553 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/kz.json
--rw-rw-r--   0 d         (1000) d         (1000)     2216 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/la.json
--rw-rw-r--   0 d         (1000) d         (1000)     3675 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/latam.json
--rw-rw-r--   0 d         (1000) d         (1000)     3660 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/latin.json
--rw-rw-r--   0 d         (1000) d         (1000)     3738 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/lt.json
--rw-rw-r--   0 d         (1000) d         (1000)     3612 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/lv.json
--rw-rw-r--   0 d         (1000) d         (1000)     3727 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mao.json
--rw-rw-r--   0 d         (1000) d         (1000)     2733 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/md.json
--rw-rw-r--   0 d         (1000) d         (1000)     2411 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mk.json
--rw-rw-r--   0 d         (1000) d         (1000)     3721 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ml.json
--rw-rw-r--   0 d         (1000) d         (1000)     3601 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mm.json
--rw-rw-r--   0 d         (1000) d         (1000)     3195 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mn.json
--rw-rw-r--   0 d         (1000) d         (1000)     3769 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mt.json
--rw-rw-r--   0 d         (1000) d         (1000)     2346 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mv.json
--rw-rw-r--   0 d         (1000) d         (1000)     2596 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/my.json
--rw-rw-r--   0 d         (1000) d         (1000)     2062 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ng.json
--rw-rw-r--   0 d         (1000) d         (1000)     3768 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/nl.json
--rw-rw-r--   0 d         (1000) d         (1000)     2293 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/np.json
--rw-rw-r--   0 d         (1000) d         (1000)     3879 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/pl.json
--rw-rw-r--   0 d         (1000) d         (1000)     3789 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/pt.json
--rw-rw-r--   0 d         (1000) d         (1000)     2733 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ro.json
--rw-rw-r--   0 d         (1000) d         (1000)     3947 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/se.json
--rw-rw-r--   0 d         (1000) d         (1000)     3741 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/sn.json
--rw-rw-r--   0 d         (1000) d         (1000)     3002 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/tg.json
--rw-rw-r--   0 d         (1000) d         (1000)     2440 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/th.json
--rw-rw-r--   0 d         (1000) d         (1000)     2644 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/tj.json
--rw-rw-r--   0 d         (1000) d         (1000)     2314 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/tm.json
--rw-rw-r--   0 d         (1000) d         (1000)     3697 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/tr.json
--rw-rw-r--   0 d         (1000) d         (1000)     2026 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/us.json
--rw-rw-r--   0 d         (1000) d         (1000)     2278 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/vn.json
--rw-rw-r--   0 d         (1000) d         (1000)     3679 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/za.json
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.906154 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/other_layouts/
--rw-rw-r--   0 d         (1000) d         (1000)      689 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/other_layouts/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)     1414 2021-04-05 21:15:47.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/other_layouts/evdev.json
--rw-rw-r--   0 d         (1000) d         (1000)     1570 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/SingleInstance.py
--rw-rw-r--   0 d         (1000) d         (1000)      764 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/__init__.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.906154 Dpowers-0.1.5rc1/Dlib/Dhelpers/adaptor/
--rw-rw-r--   0 d         (1000) d         (1000)      784 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/adaptor/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)    30795 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/adaptor/adaptor_classes.py
--rw-rw-r--   0 d         (1000) d         (1000)     7670 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/adaptor/backend_class.py
--rw-rw-r--   0 d         (1000) d         (1000)    11857 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/adaptor/dependency_testing.py
--rw-rw-r--   0 d         (1000) d         (1000)     2135 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/adaptor/sphinx_directives.py
--rw-rw-r--   0 d         (1000) d         (1000)     1234 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/all.py
--rw-rw-r--   0 d         (1000) d         (1000)     6299 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/arghandling.py
--rw-rw-r--   0 d         (1000) d         (1000)    13301 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/baseclasses.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.906154 Dpowers-0.1.5rc1/Dlib/Dhelpers/builtin_manipulation/
--rw-rw-r--   0 d         (1000) d         (1000)     1079 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/builtin_manipulation/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)     4454 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/builtin_manipulation/customprint.py
--rw-rw-r--   0 d         (1000) d         (1000)     1741 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/builtin_manipulation/debug.py
--rw-rw-r--   0 d         (1000) d         (1000)     2543 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/builtin_manipulation/error_warning.py
--rw-rw-r--   0 d         (1000) d         (1000)     2856 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/container.py
--rw-rw-r--   0 d         (1000) d         (1000)     1417 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/counting.py
--rw-rw-r--   0 d         (1000) d         (1000)     1096 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/crypt.py
--rw-rw-r--   0 d         (1000) d         (1000)     2400 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/decorators.py
--rw-rw-r--   0 d         (1000) d         (1000)     8444 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/external.py
--rw-rw-r--   0 d         (1000) d         (1000)     8965 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/file_iteration.py
--rw-rw-r--   0 d         (1000) d         (1000)     1852 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/importtools.py
--rw-rw-r--   0 d         (1000) d         (1000)    11899 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/launcher.py
--rw-rw-r--   0 d         (1000) d         (1000)     2133 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/linux_checks.py
--rw-rw-r--   0 d         (1000) d         (1000)    15951 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/named.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.906154 Dpowers-0.1.5rc1/Dlib/Dhelpers/old/
--rw-rw-r--   0 d         (1000) d         (1000)      689 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/old/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)       95 2020-03-01 04:08:04.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/old/explain.txt
--rw-rw-r--   0 d         (1000) d         (1000)     8325 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/old/portable.py
--rw-rw-r--   0 d         (1000) d         (1000)     3733 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/old/this_script.py
--rw-rw-r--   0 d         (1000) d         (1000)     4730 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/platform.py
--rw-rw-r--   0 d         (1000) d         (1000)     1767 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/psutil_fix.py
--rw-rw-r--   0 d         (1000) d         (1000)     5225 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/sphinx.py
--rw-rw-r--   0 d         (1000) d         (1000)     2597 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dhelpers/strhandling.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.910154 Dpowers-0.1.5rc1/Dlib/Dpowers/
--rw-rw-r--   0 d         (1000) d         (1000)     9806 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/Dfuncs.py
--rw-rw-r--   0 d         (1000) d         (1000)     3773 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)      883 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/autoadapt.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.910154 Dpowers-0.1.5rc1/Dlib/Dpowers/clipboardpower/
--rw-rw-r--   0 d         (1000) d         (1000)     3269 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/clipboardpower/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)     1172 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/clipboardpower/adapt_xclip_bash.py
--rw-rw-r--   0 d         (1000) d         (1000)     1131 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/clipboardpower/adapt_xsel_bash.py
--rw-rw-r--   0 d         (1000) d         (1000)     2327 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/default_backends.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.910154 Dpowers-0.1.5rc1/Dlib/Dpowers/dialogpower/
--rw-rw-r--   0 d         (1000) d         (1000)     2568 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/dialogpower/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)     2358 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/dialogpower/adapt_tkinter.py
--rw-rw-r--   0 d         (1000) d         (1000)     5227 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/dialogpower/adapt_zenity_bash.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.910154 Dpowers-0.1.5rc1/Dlib/Dpowers/editing/
--rw-rw-r--   0 d         (1000) d         (1000)     1134 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/editing/__init__.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.910154 Dpowers-0.1.5rc1/Dlib/Dpowers/editing/imagepower/
--rw-rw-r--   0 d         (1000) d         (1000)     2379 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/editing/imagepower/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)      991 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/editing/imagepower/adapt_pil.py
--rw-rw-r--   0 d         (1000) d         (1000)     2366 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/editing/imagepower/adapt_wand.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.910154 Dpowers-0.1.5rc1/Dlib/Dpowers/editing/mp3power/
--rw-rw-r--   0 d         (1000) d         (1000)     1133 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/editing/mp3power/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)     1316 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/editing/mp3power/adapt_eyed3.py
--rw-rw-r--   0 d         (1000) d         (1000)    19215 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/editing/ressource_classes.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.910154 Dpowers-0.1.5rc1/Dlib/Dpowers/events/
--rw-rw-r--   0 d         (1000) d         (1000)      258 2021-10-02 22:19:32.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/events/TODO
--rw-rw-r--   0 d         (1000) d         (1000)     3005 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/events/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)    13599 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/events/event_classes.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.910154 Dpowers-0.1.5rc1/Dlib/Dpowers/events/hookpower/
--rw-rw-r--   0 d         (1000) d         (1000)     4502 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/events/hookpower/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)     6185 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/events/hookpower/adapt_evdev.py
--rw-rw-r--   0 d         (1000) d         (1000)     3592 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/events/hookpower/adapt_pynput.py
--rw-rw-r--   0 d         (1000) d         (1000)    19621 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/events/hookpower/baseclasses.py
--rw-rw-r--   0 d         (1000) d         (1000)     4209 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/events/keybutton_classes.py
--rw-rw-r--   0 d         (1000) d         (1000)    11287 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/events/keybutton_names.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.910154 Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/
--rw-rw-r--   0 d         (1000) d         (1000)      766 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)    17601 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/event_sender.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.910154 Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/keybpower/
--rw-rw-r--   0 d         (1000) d         (1000)    12943 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/keybpower/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)     1394 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/keybpower/adapt_evdev.py
--rw-rw-r--   0 d         (1000) d         (1000)     1628 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/keybpower/adapt_pynput.py
--rw-rw-r--   0 d         (1000) d         (1000)     3680 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/keybpower/adapt_xdotool_bash.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.914154 Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/mousepower/
--rw-rw-r--   0 d         (1000) d         (1000)     4259 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/mousepower/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)     1307 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/mousepower/adapt_evdev.py
--rw-rw-r--   0 d         (1000) d         (1000)     1222 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/mousepower/adapt_pynput.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.914154 Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/senderpower/
--rw-rw-r--   0 d         (1000) d         (1000)     1522 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/senderpower/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)     2214 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/senderpower/adapt_evdev.py
--rw-rw-r--   0 d         (1000) d         (1000)    11673 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/events/trigman.py
--rw-rw-r--   0 d         (1000) d         (1000)     9768 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/events/waiter.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.914154 Dpowers-0.1.5rc1/Dlib/Dpowers/iconpower/
--rw-rw-r--   0 d         (1000) d         (1000)     4005 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/iconpower/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)     1725 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/iconpower/adapt_pystray.py
--rw-rw-r--   0 d         (1000) d         (1000)     2045 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/iconpower/adapt_yad_bash.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.914154 Dpowers-0.1.5rc1/Dlib/Dpowers/iconpower/icons/
--rw-r--r--   0 d         (1000) d         (1000)    14520 2017-07-12 20:52:15.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/iconpower/icons/Dicon.png
--rw-r--r--   0 d         (1000) d         (1000)    18068 2019-12-20 23:04:48.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/iconpower/icons/Dicon.svg
--rw-rw-r--   0 d         (1000) d         (1000)      689 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/iconpower/icons/__init__.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.914154 Dpowers-0.1.5rc1/Dlib/Dpowers/notificationpower/
--rw-rw-r--   0 d         (1000) d         (1000)     1504 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/notificationpower/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)     1083 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/notificationpower/adapt_notify_send_bash.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.914154 Dpowers-0.1.5rc1/Dlib/Dpowers/sound/
--rw-rw-r--   0 d         (1000) d         (1000)      762 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/sound/__init__.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.914154 Dpowers-0.1.5rc1/Dlib/Dpowers/sound/ttspower/
--rw-rw-r--   0 d         (1000) d         (1000)     1207 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/sound/ttspower/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)     1039 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/sound/ttspower/adapt_ttsx3.py
--rw-rw-r--   0 d         (1000) d         (1000)     3847 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/winapps.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.914154 Dpowers-0.1.5rc1/Dlib/Dpowers/windowpower/
--rw-rw-r--   0 d         (1000) d         (1000)     4182 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/windowpower/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)     6974 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/windowpower/adapt_xtools_bash.py
--rw-rw-r--   0 d         (1000) d         (1000)    21450 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/Dpowers/windowpower/windowobjects.py
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.910154 Dpowers-0.1.5rc1/Dlib/Dpowers.egg-info/
--rw-rw-r--   0 d         (1000) d         (1000)     1156 2023-03-11 18:45:12.000000 Dpowers-0.1.5rc1/Dlib/Dpowers.egg-info/PKG-INFO
--rw-rw-r--   0 d         (1000) d         (1000)     7724 2023-03-11 18:45:12.000000 Dpowers-0.1.5rc1/Dlib/Dpowers.egg-info/SOURCES.txt
--rw-rw-r--   0 d         (1000) d         (1000)        1 2023-03-11 18:45:12.000000 Dpowers-0.1.5rc1/Dlib/Dpowers.egg-info/dependency_links.txt
--rw-rw-r--   0 d         (1000) d         (1000)       19 2023-03-11 18:45:12.000000 Dpowers-0.1.5rc1/Dlib/Dpowers.egg-info/requires.txt
--rw-rw-r--   0 d         (1000) d         (1000)        8 2023-03-11 18:45:12.000000 Dpowers-0.1.5rc1/Dlib/Dpowers.egg-info/top_level.txt
--rw-rw-r--   0 d         (1000) d         (1000)      689 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/Dlib/__init__.py
--rw-rw-r--   0 d         (1000) d         (1000)     1156 2023-03-11 18:45:12.914154 Dpowers-0.1.5rc1/PKG-INFO
--rw-rw-r--   0 d         (1000) d         (1000)      616 2021-09-01 20:54:23.000000 Dpowers-0.1.5rc1/README.md
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.914154 Dpowers-0.1.5rc1/docs/
--rwxrwxr-x   0 d         (1000) d         (1000)      641 2021-02-27 03:20:25.000000 Dpowers-0.1.5rc1/docs/Makefile
--rw-rw-r--   0 d         (1000) d         (1000)     4051 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/docs/conf.py
--rw-rw-r--   0 d         (1000) d         (1000)      607 2021-08-19 20:13:51.000000 Dpowers-0.1.5rc1/docs/index.rst
--rw-rw-r--   0 d         (1000) d         (1000)     1430 2021-09-01 20:54:23.000000 Dpowers-0.1.5rc1/docs/intro.rst
--rwxrwxr-x   0 d         (1000) d         (1000)      760 2022-03-18 20:48:42.000000 Dpowers-0.1.5rc1/docs/make.bat
--rw-rw-r--   0 d         (1000) d         (1000)     3360 2021-10-02 15:48:38.000000 Dpowers-0.1.5rc1/docs/preperation.rst
--rw-rw-r--   0 d         (1000) d         (1000)     5092 2021-09-01 20:54:23.000000 Dpowers-0.1.5rc1/docs/quickstart.rst
-drwxrwxr-x   0 d         (1000) d         (1000)        0 2023-03-11 18:45:12.914154 Dpowers-0.1.5rc1/docs/reference/
--rw-rw-r--   0 d         (1000) d         (1000)      619 2021-09-01 20:54:23.000000 Dpowers-0.1.5rc1/docs/reference/power.rst
--rw-rw-r--   0 d         (1000) d         (1000)     1565 2021-09-01 20:54:23.000000 Dpowers-0.1.5rc1/docs/reference/powerclasses.rst
--rw-rw-r--   0 d         (1000) d         (1000)       16 2021-10-02 22:11:02.000000 Dpowers-0.1.5rc1/docs/requirements.txt
--rw-rw-r--   0 d         (1000) d         (1000)      658 2023-03-10 20:42:51.000000 Dpowers-0.1.5rc1/licenseheader.txt
--rw-rw-r--   0 d         (1000) d         (1000)       38 2023-03-11 18:45:12.914154 Dpowers-0.1.5rc1/setup.cfg
--rw-rw-r--   0 d         (1000) d         (1000)     3421 2023-03-11 18:45:11.000000 Dpowers-0.1.5rc1/setup.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.390105 Dpowers-0.1.5rc2/
+-rw-rw-r--   0 d         (1000) d         (1000)      112 2021-02-11 22:26:21.000000 Dpowers-0.1.5rc2/.gitignore
+-rw-rw-r--   0 d         (1000) d         (1000)    35149 2020-03-01 00:41:51.000000 Dpowers-0.1.5rc2/COPYING
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.358105 Dpowers-0.1.5rc2/Dlib/
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.358105 Dpowers-0.1.5rc2/Dlib/Dhelpers/
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.362105 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/
+-rw-rw-r--   0 d         (1000) d         (1000)     5861 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/__init__.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.370105 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/
+-rw-rw-r--   0 d         (1000) d         (1000)      689 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     3663 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/al.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2519 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/am.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2301 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/apl.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3922 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/at.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2026 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/au.json
+-rw-rw-r--   0 d         (1000) d         (1000)     1414 2021-04-05 21:23:17.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/base.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3775 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/be.json
+-rw-rw-r--   0 d         (1000) d         (1000)     4145 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/bt.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2477 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/by.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2721 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/cd.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3778 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ch.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2026 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/cm.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2026 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/cn.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3922 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/de.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3881 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/dk.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3688 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ee.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2474 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/epo.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3671 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/es.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3891 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/fo.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3706 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/fr.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2758 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ge.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2062 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/gh.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2346 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/gn.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3848 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/hu.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3745 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ie.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3799 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/is.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3777 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/it.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2435 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/kg.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2553 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/kz.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2216 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/la.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3675 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/latam.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3660 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/latin.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3738 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/lt.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3612 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/lv.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3727 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mao.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2733 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/md.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2411 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mk.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3721 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ml.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3601 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mm.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3195 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mn.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3769 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mt.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2346 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mv.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2596 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/my.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2062 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ng.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3768 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/nl.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2293 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/np.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3879 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/pl.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3789 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/pt.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2733 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ro.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3947 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/se.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3741 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/sn.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3002 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/tg.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2440 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/th.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2644 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/tj.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2314 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/tm.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3697 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/tr.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2026 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/us.json
+-rw-rw-r--   0 d         (1000) d         (1000)     2278 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/vn.json
+-rw-rw-r--   0 d         (1000) d         (1000)     3679 2020-01-03 23:48:54.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/za.json
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.370105 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/other_layouts/
+-rw-rw-r--   0 d         (1000) d         (1000)      689 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/other_layouts/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1414 2021-04-05 21:15:47.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/other_layouts/evdev.json
+-rw-rw-r--   0 d         (1000) d         (1000)     1570 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/SingleInstance.py
+-rw-rw-r--   0 d         (1000) d         (1000)      764 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/__init__.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.374105 Dpowers-0.1.5rc2/Dlib/Dhelpers/adaptor/
+-rw-rw-r--   0 d         (1000) d         (1000)      784 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/adaptor/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)    30795 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/adaptor/adaptor_classes.py
+-rw-rw-r--   0 d         (1000) d         (1000)     7670 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/adaptor/backend_class.py
+-rw-rw-r--   0 d         (1000) d         (1000)    11857 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/adaptor/dependency_testing.py
+-rw-rw-r--   0 d         (1000) d         (1000)     2135 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/adaptor/sphinx_directives.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1234 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/all.py
+-rw-rw-r--   0 d         (1000) d         (1000)     6299 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/arghandling.py
+-rw-rw-r--   0 d         (1000) d         (1000)    13301 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/baseclasses.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.374105 Dpowers-0.1.5rc2/Dlib/Dhelpers/builtin_manipulation/
+-rw-rw-r--   0 d         (1000) d         (1000)     1079 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/builtin_manipulation/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     4454 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/builtin_manipulation/customprint.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1741 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/builtin_manipulation/debug.py
+-rw-rw-r--   0 d         (1000) d         (1000)     2543 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/builtin_manipulation/error_warning.py
+-rw-rw-r--   0 d         (1000) d         (1000)     2856 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/container.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1417 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/counting.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1096 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/crypt.py
+-rw-rw-r--   0 d         (1000) d         (1000)     2400 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/decorators.py
+-rw-rw-r--   0 d         (1000) d         (1000)     8444 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/external.py
+-rw-rw-r--   0 d         (1000) d         (1000)    11801 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/file_iteration.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1852 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/importtools.py
+-rw-rw-r--   0 d         (1000) d         (1000)    11899 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/launcher.py
+-rw-rw-r--   0 d         (1000) d         (1000)     2133 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/linux_checks.py
+-rw-rw-r--   0 d         (1000) d         (1000)    15951 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/named.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.374105 Dpowers-0.1.5rc2/Dlib/Dhelpers/old/
+-rw-rw-r--   0 d         (1000) d         (1000)      689 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/old/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)       95 2020-03-01 04:08:04.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/old/explain.txt
+-rw-rw-r--   0 d         (1000) d         (1000)     8325 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/old/portable.py
+-rw-rw-r--   0 d         (1000) d         (1000)     3733 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/old/this_script.py
+-rw-rw-r--   0 d         (1000) d         (1000)     4730 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/platform.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1767 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/psutil_fix.py
+-rw-rw-r--   0 d         (1000) d         (1000)     5225 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/sphinx.py
+-rw-rw-r--   0 d         (1000) d         (1000)     2597 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dhelpers/strhandling.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.374105 Dpowers-0.1.5rc2/Dlib/Dpowers/
+-rw-rw-r--   0 d         (1000) d         (1000)     9806 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/Dfuncs.py
+-rw-rw-r--   0 d         (1000) d         (1000)     3773 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)      883 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/autoadapt.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.374105 Dpowers-0.1.5rc2/Dlib/Dpowers/clipboardpower/
+-rw-rw-r--   0 d         (1000) d         (1000)     3269 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/clipboardpower/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1172 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/clipboardpower/adapt_xclip_bash.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1131 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/clipboardpower/adapt_xsel_bash.py
+-rw-rw-r--   0 d         (1000) d         (1000)     2327 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/default_backends.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.374105 Dpowers-0.1.5rc2/Dlib/Dpowers/dialogpower/
+-rw-rw-r--   0 d         (1000) d         (1000)     2568 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/dialogpower/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     2358 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/dialogpower/adapt_tkinter.py
+-rw-rw-r--   0 d         (1000) d         (1000)     5227 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/dialogpower/adapt_zenity_bash.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.374105 Dpowers-0.1.5rc2/Dlib/Dpowers/editing/
+-rw-rw-r--   0 d         (1000) d         (1000)     1134 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/editing/__init__.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.374105 Dpowers-0.1.5rc2/Dlib/Dpowers/editing/imagepower/
+-rw-rw-r--   0 d         (1000) d         (1000)     2379 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/editing/imagepower/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)      991 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/editing/imagepower/adapt_pil.py
+-rw-rw-r--   0 d         (1000) d         (1000)     2366 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/editing/imagepower/adapt_wand.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.374105 Dpowers-0.1.5rc2/Dlib/Dpowers/editing/mp3power/
+-rw-rw-r--   0 d         (1000) d         (1000)     1133 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/editing/mp3power/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1316 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/editing/mp3power/adapt_eyed3.py
+-rw-rw-r--   0 d         (1000) d         (1000)    19215 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/editing/ressource_classes.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.378105 Dpowers-0.1.5rc2/Dlib/Dpowers/events/
+-rw-rw-r--   0 d         (1000) d         (1000)      258 2021-10-02 22:19:32.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/events/TODO
+-rw-rw-r--   0 d         (1000) d         (1000)     3005 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/events/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)    13599 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/events/event_classes.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.378105 Dpowers-0.1.5rc2/Dlib/Dpowers/events/hookpower/
+-rw-rw-r--   0 d         (1000) d         (1000)     4502 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/events/hookpower/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     6185 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/events/hookpower/adapt_evdev.py
+-rw-rw-r--   0 d         (1000) d         (1000)     3592 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/events/hookpower/adapt_pynput.py
+-rw-rw-r--   0 d         (1000) d         (1000)    19621 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/events/hookpower/baseclasses.py
+-rw-rw-r--   0 d         (1000) d         (1000)     4209 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/events/keybutton_classes.py
+-rw-rw-r--   0 d         (1000) d         (1000)    11287 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/events/keybutton_names.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.378105 Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/
+-rw-rw-r--   0 d         (1000) d         (1000)      766 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)    17601 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/event_sender.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.378105 Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/keybpower/
+-rw-rw-r--   0 d         (1000) d         (1000)    12943 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/keybpower/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1394 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/keybpower/adapt_evdev.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1628 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/keybpower/adapt_pynput.py
+-rw-rw-r--   0 d         (1000) d         (1000)     3680 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/keybpower/adapt_xdotool_bash.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.378105 Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/mousepower/
+-rw-rw-r--   0 d         (1000) d         (1000)     4259 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/mousepower/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1307 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/mousepower/adapt_evdev.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1222 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/mousepower/adapt_pynput.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.378105 Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/senderpower/
+-rw-rw-r--   0 d         (1000) d         (1000)     1522 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/senderpower/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     2214 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/senderpower/adapt_evdev.py
+-rw-rw-r--   0 d         (1000) d         (1000)    11673 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/events/trigman.py
+-rw-rw-r--   0 d         (1000) d         (1000)     9768 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/events/waiter.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.378105 Dpowers-0.1.5rc2/Dlib/Dpowers/iconpower/
+-rw-rw-r--   0 d         (1000) d         (1000)     3866 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/iconpower/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1725 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/iconpower/adapt_pystray.py
+-rw-rw-r--   0 d         (1000) d         (1000)     2045 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/iconpower/adapt_yad_bash.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.382105 Dpowers-0.1.5rc2/Dlib/Dpowers/iconpower/icons/
+-rw-r--r--   0 d         (1000) d         (1000)    14520 2017-07-12 20:52:15.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/iconpower/icons/Dicon.png
+-rw-r--r--   0 d         (1000) d         (1000)    18068 2019-12-20 23:04:48.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/iconpower/icons/Dicon.svg
+-rw-rw-r--   0 d         (1000) d         (1000)      689 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/iconpower/icons/__init__.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.382105 Dpowers-0.1.5rc2/Dlib/Dpowers/notificationpower/
+-rw-rw-r--   0 d         (1000) d         (1000)     1504 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/notificationpower/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1083 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/notificationpower/adapt_notify_send_bash.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.382105 Dpowers-0.1.5rc2/Dlib/Dpowers/sound/
+-rw-rw-r--   0 d         (1000) d         (1000)      762 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/sound/__init__.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.382105 Dpowers-0.1.5rc2/Dlib/Dpowers/sound/ttspower/
+-rw-rw-r--   0 d         (1000) d         (1000)     1207 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/sound/ttspower/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1039 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/sound/ttspower/adapt_ttsx3.py
+-rw-rw-r--   0 d         (1000) d         (1000)     3847 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/winapps.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.386105 Dpowers-0.1.5rc2/Dlib/Dpowers/windowpower/
+-rw-rw-r--   0 d         (1000) d         (1000)     4201 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/windowpower/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     6974 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/windowpower/adapt_xtools_bash.py
+-rw-rw-r--   0 d         (1000) d         (1000)    21450 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/Dpowers/windowpower/windowobjects.py
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.374105 Dpowers-0.1.5rc2/Dlib/Dpowers.egg-info/
+-rw-rw-r--   0 d         (1000) d         (1000)     1156 2024-01-07 20:33:43.000000 Dpowers-0.1.5rc2/Dlib/Dpowers.egg-info/PKG-INFO
+-rw-rw-r--   0 d         (1000) d         (1000)     7724 2024-01-07 20:33:43.000000 Dpowers-0.1.5rc2/Dlib/Dpowers.egg-info/SOURCES.txt
+-rw-rw-r--   0 d         (1000) d         (1000)        1 2024-01-07 20:33:43.000000 Dpowers-0.1.5rc2/Dlib/Dpowers.egg-info/dependency_links.txt
+-rw-rw-r--   0 d         (1000) d         (1000)       19 2024-01-07 20:33:43.000000 Dpowers-0.1.5rc2/Dlib/Dpowers.egg-info/requires.txt
+-rw-rw-r--   0 d         (1000) d         (1000)        8 2024-01-07 20:33:43.000000 Dpowers-0.1.5rc2/Dlib/Dpowers.egg-info/top_level.txt
+-rw-rw-r--   0 d         (1000) d         (1000)      689 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/Dlib/__init__.py
+-rw-rw-r--   0 d         (1000) d         (1000)     1156 2024-01-07 20:33:43.390105 Dpowers-0.1.5rc2/PKG-INFO
+-rw-rw-r--   0 d         (1000) d         (1000)      616 2021-09-01 20:54:23.000000 Dpowers-0.1.5rc2/README.md
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.386105 Dpowers-0.1.5rc2/docs/
+-rwxrwxr-x   0 d         (1000) d         (1000)      641 2021-02-27 03:20:25.000000 Dpowers-0.1.5rc2/docs/Makefile
+-rw-rw-r--   0 d         (1000) d         (1000)     4051 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/docs/conf.py
+-rw-rw-r--   0 d         (1000) d         (1000)      607 2021-08-19 20:13:51.000000 Dpowers-0.1.5rc2/docs/index.rst
+-rw-rw-r--   0 d         (1000) d         (1000)     1430 2021-09-01 20:54:23.000000 Dpowers-0.1.5rc2/docs/intro.rst
+-rwxrwxr-x   0 d         (1000) d         (1000)      760 2022-03-18 20:48:42.000000 Dpowers-0.1.5rc2/docs/make.bat
+-rw-rw-r--   0 d         (1000) d         (1000)     3360 2021-10-02 15:48:38.000000 Dpowers-0.1.5rc2/docs/preperation.rst
+-rw-rw-r--   0 d         (1000) d         (1000)     5092 2021-09-01 20:54:23.000000 Dpowers-0.1.5rc2/docs/quickstart.rst
+drwxrwxr-x   0 d         (1000) d         (1000)        0 2024-01-07 20:33:43.386105 Dpowers-0.1.5rc2/docs/reference/
+-rw-rw-r--   0 d         (1000) d         (1000)      619 2021-09-01 20:54:23.000000 Dpowers-0.1.5rc2/docs/reference/power.rst
+-rw-rw-r--   0 d         (1000) d         (1000)     1565 2021-09-01 20:54:23.000000 Dpowers-0.1.5rc2/docs/reference/powerclasses.rst
+-rw-rw-r--   0 d         (1000) d         (1000)       16 2021-10-02 22:11:02.000000 Dpowers-0.1.5rc2/docs/requirements.txt
+-rw-rw-r--   0 d         (1000) d         (1000)      658 2023-03-10 20:42:51.000000 Dpowers-0.1.5rc2/licenseheader.txt
+-rw-rw-r--   0 d         (1000) d         (1000)       38 2024-01-07 20:33:43.390105 Dpowers-0.1.5rc2/setup.cfg
+-rw-rw-r--   0 d         (1000) d         (1000)     3421 2024-01-07 20:33:41.000000 Dpowers-0.1.5rc2/setup.py
```

### Comparing `Dpowers-0.1.5rc1/COPYING` & `Dpowers-0.1.5rc2/COPYING`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/__init__.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/__init__.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/al.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/al.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/am.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/am.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/apl.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/apl.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/at.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/at.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/au.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/au.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/base.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/base.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/be.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/be.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/bt.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/bt.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/by.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/by.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/cd.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/cd.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ch.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ch.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/cm.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/cm.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/cn.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/cn.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/de.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/de.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/dk.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/dk.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ee.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ee.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/epo.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/epo.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/es.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/es.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/fo.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/fo.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/fr.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/fr.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ge.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ge.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/gh.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/gh.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/gn.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/gn.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/hu.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/hu.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ie.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ie.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/is.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/is.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/it.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/it.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/kg.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/kg.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/kz.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/kz.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/la.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/la.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/latam.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/latam.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/latin.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/latin.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/lt.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/lt.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/lv.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/lv.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mao.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mao.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/md.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/md.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mk.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mk.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ml.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ml.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mm.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mm.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mn.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mn.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mt.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mt.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mv.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/mv.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/my.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/my.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ng.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ng.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/nl.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/nl.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/np.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/np.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/pl.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/pl.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/pt.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/pt.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ro.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/ro.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/se.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/se.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/sn.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/sn.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/tg.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/tg.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/th.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/th.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/tj.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/tj.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/tm.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/tm.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/tr.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/tr.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/us.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/us.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/vn.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/vn.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/za.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/layouts_imported_from_xkb/za.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/other_layouts/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/other_layouts/__init__.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/KeyboardLayouts/other_layouts/evdev.json` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/KeyboardLayouts/other_layouts/evdev.json`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/SingleInstance.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/SingleInstance.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 #we don't want to import anything automatically
 
 
-__version__ = "0.1.5rc1"
+__version__ = "0.1.5rc2"
```

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/adaptor/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/adaptor/__init__.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/adaptor/adaptor_classes.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/adaptor/adaptor_classes.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/adaptor/backend_class.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/adaptor/backend_class.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/adaptor/dependency_testing.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/adaptor/dependency_testing.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/adaptor/sphinx_directives.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/adaptor/sphinx_directives.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/all.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/all.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/arghandling.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/arghandling.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/baseclasses.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/baseclasses.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/builtin_manipulation/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/builtin_manipulation/__init__.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/builtin_manipulation/customprint.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/builtin_manipulation/customprint.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/builtin_manipulation/debug.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/builtin_manipulation/debug.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/builtin_manipulation/error_warning.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/builtin_manipulation/error_warning.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/container.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/container.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/counting.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/counting.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/crypt.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/crypt.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/decorators.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/decorators.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/external.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/external.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/file_iteration.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/file_iteration.py`

 * *Files 16% similar despite different names*

```diff
@@ -138,19 +138,22 @@
         filelist_cls.creator = self
         self.Filelist = filelist_cls
         self.basepath = basepath
         self.destpath = destpath
         self.filelist_objs = {}
         self.file_paths = {}
         self.imported_lists = None
+        self.filelist_combinations = list()
+        self._custom_file_func = NotImplemented
         
     @property
     def destpath(self):
         if not self._destpath and self.basepath:
-            return os.path.join(self.basepath, "__playlists")
+            parent = os.path.split(self.basepath)[0]
+            return os.path.join(parent, "__Playlists")
         return self._destpath
         
     @destpath.setter
     def destpath(self, val):
         self._destpath = val
         
     
@@ -215,16 +218,22 @@
         if assemble: self.assemble_lists(*names, **kwargs)
         print("Creating playlists:")
         os.makedirs(self.destpath, exist_ok=True)
         for name, file_path_list in self.file_paths.items():
             self._write_filelist(name,file_path_list, self.destpath)
             
             
-    def _write_filelist(self, name, file_path_list, path):
-        fpath = os.path.join(path, name + self.filelist_extension)
+    def _write_filelist(self, name, file_path_list, path, overwrite=True):
+        fpath_base = os.path.join(path, name)
+        fpath = fpath_base + self.filelist_extension
+        if overwrite is False:
+            num = 0
+            while os.path.isfile(fpath):
+                num += 1
+                fpath = fpath_base + "__" + str(num) + self.filelist_extension
         with open(fpath, "w") as new:
             new.write(self.file_start + "\n")
             for file in file_path_list: new.write(file + "\n")
         print(f"{name}: {len(file_path_list)} songs in {fpath}")
 
 
 
@@ -236,22 +245,85 @@
             name, ext = os.path.splitext(file)
             if ext not in allowed_ext: continue
             with open(os.path.join(destpath,file), "r") as opened:
                 for line in opened.readlines():
                     self.imported_lists[name].append(line.strip())
         return self.imported_lists
     
-    def create_combination(self, *file_list_names, insert=None,
-            from_imported=False):
-        lists = self.imported_lists if from_imported else self.file_paths
-        for name in file_list_names:
-            if isinstance(name,self.Filelist): name=name.name
-            l = lists[name]
-            yield random.choice(l)
-            if insert: yield insert
-    
-    @functools.wraps(create_combination)
-    def write_combination(self, *args, **kwargs):
-        filelist = tuple(self.create_combination(*args,**kwargs))
-        comb_path=os.path.join(self.destpath, "combinations")
-        os.makedirs(comb_path, exist_ok=True)
-        self._write_filelist("test_combination", filelist, comb_path)
+    def define_combination(self, *args, **kwargs):
+        c = FilelistCombination(self, *args,**kwargs)
+        self.filelist_combinations.append(c)
+        return c
+    
+    def write_combinations(self, *args,**kwargs):
+        for c in self.filelist_combinations: c.write(*args,**kwargs)
+        
+    def get_custom_file(self, name_or_number):
+        if self._custom_file_func is NotImplemented: raise NotImplementedError
+        file = self._custom_file_func(self, name_or_number)
+        if not os.path.isfile(file): raise FileNotFoundError(file)
+        return file
+    
+    def custom_file_finder(self, func):
+        """A decorator to define the function returning files for
+        get_custom_file()"""
+        self._custom_file_func = func
+        return func
+
+class FilelistCombination:
+    
+    def __init__(self, playlist_creator, name, file_list_names,*, insert=None,
+            from_imported=False, destpath=None):
+        self.name = name
+        self.creator = playlist_creator
+        assert isinstance(file_list_names, (tuple, list))
+        self.file_lists = file_list_names
+        self.insert = insert
+        self.from_imported = from_imported
+        self.destpath = destpath
+    
+    @property
+    def destpath(self):
+        """This defines the default location for self.destpath if not
+        manually set"""
+        if self._destpath: return self._destpath
+        dp = self.creator.destpath
+        if dp: return os.path.join(dp, "combinations")
+        return
+    
+    @destpath.setter
+    def destpath(self, val):
+        self._destpath = val
+        
+    def _process_fileinfo(self, fileinfo, defined_lists):
+        if isinstance(fileinfo, self.creator.Filelist):
+            fileinfo = fileinfo.name
+        if fileinfo in defined_lists:
+            return random.choice(defined_lists[fileinfo])
+            #first, check if a FileList has been defined with that name
+            # if not, then try to interpret the given name as an argument for
+            # custom_file_finder
+        else:
+            return self.creator.get_custom_file(fileinfo)
+    
+    def create(self, insert=None, from_imported=None):
+        insert = insert if insert else self.insert
+        from_imported = self.from_imported if from_imported is None else from_imported
+        creator = self.creator
+        lists = creator.imported_lists if from_imported else creator.file_paths
+        for name in self.file_lists:
+            file = self._process_fileinfo(name, lists)
+            if file: yield file
+            if insert:
+                if os.path.isfile(insert):
+                    yield insert #just return the input, in case it is a
+                    # explicit path
+                else:
+                    yield self._process_fileinfo(insert, lists)
+    
+    def write(self, name=None, destpath=None, overwrite=True, **kwargs):
+        name = name if name else self.name
+        destpath = destpath if destpath else self.destpath
+        filelist = tuple(self.create(**kwargs))
+        #print(filelist)
+        os.makedirs(destpath, exist_ok=True)
+        self.creator._write_filelist(name, filelist, destpath, overwrite=overwrite)
```

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/importtools.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/importtools.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/launcher.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/launcher.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/linux_checks.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/linux_checks.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/named.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/named.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/old/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/old/__init__.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/old/portable.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/old/portable.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/old/this_script.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/old/this_script.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/platform.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/platform.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/psutil_fix.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/psutil_fix.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/sphinx.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/sphinx.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dhelpers/strhandling.py` & `Dpowers-0.1.5rc2/Dlib/Dhelpers/strhandling.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/Dfuncs.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/Dfuncs.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     import Dhelpers
 except ModuleNotFoundError:
     sys.path.append(os.path.dirname(dpowers_folder))
     import Dpowers
     import Dhelpers
     
 
-__version__ = "0.1.5rc1"
+__version__ = "0.1.5rc2"
 #Dpowers and Dhelpers share version number
 if __version__ != Dhelpers.__version__:
     import warnings
     warnings.warn("Dpowers and Dhelpers packages do not share same version "\
                   "number")
 
 from Dhelpers.adaptor import (AdaptorBase, adaptionmethod, AdaptionError,
```

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/autoadapt.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/autoadapt.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/clipboardpower/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/clipboardpower/__init__.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/clipboardpower/adapt_xclip_bash.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/clipboardpower/adapt_xclip_bash.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/clipboardpower/adapt_xsel_bash.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/clipboardpower/adapt_xsel_bash.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/default_backends.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/default_backends.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/dialogpower/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/dialogpower/__init__.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/dialogpower/adapt_tkinter.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/dialogpower/adapt_tkinter.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/dialogpower/adapt_zenity_bash.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/dialogpower/adapt_zenity_bash.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/editing/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/editing/__init__.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/editing/imagepower/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/editing/imagepower/__init__.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/editing/imagepower/adapt_pil.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/editing/imagepower/adapt_pil.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/editing/imagepower/adapt_wand.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/editing/imagepower/adapt_wand.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/editing/mp3power/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/editing/mp3power/__init__.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/editing/mp3power/adapt_eyed3.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/editing/mp3power/adapt_eyed3.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/editing/ressource_classes.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/editing/ressource_classes.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/events/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/events/__init__.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/events/event_classes.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/events/event_classes.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/events/hookpower/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/events/hookpower/__init__.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/events/hookpower/adapt_evdev.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/events/hookpower/adapt_evdev.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/events/hookpower/adapt_pynput.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/events/hookpower/adapt_pynput.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/events/hookpower/baseclasses.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/events/hookpower/baseclasses.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/events/keybutton_classes.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/events/keybutton_classes.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/events/keybutton_names.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/events/keybutton_names.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/__init__.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/event_sender.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/event_sender.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/keybpower/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/keybpower/__init__.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/keybpower/adapt_evdev.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/keybpower/adapt_evdev.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/keybpower/adapt_pynput.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/keybpower/adapt_pynput.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/keybpower/adapt_xdotool_bash.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/keybpower/adapt_xdotool_bash.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/mousepower/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/mousepower/__init__.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/mousepower/adapt_evdev.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/mousepower/adapt_evdev.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/mousepower/adapt_pynput.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/mousepower/adapt_pynput.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/senderpower/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/senderpower/__init__.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/events/sending/senderpower/adapt_evdev.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/events/sending/senderpower/adapt_evdev.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/events/trigman.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/events/trigman.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/events/waiter.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/events/waiter.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/iconpower/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/iconpower/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,42 +40,34 @@
         self.path = os.path.join(os.path.dirname(__file__),"icons","Dicon.png")
         self.tooltip = "Dpowers"
         self.left_click = self.terminate_parent
             #by default a left click terminates this script
         self.child_process = None
         self.last_item = ("Quit", self.terminate_parent)
         self.parent_id = os.getpid()
-        self.menuitem("Display win info", Dfuncs.display_win_info)
-        self.menuitem("Get single key name(s)", Dfuncs.display_key_names)
-        self.menuitem("Monitor input events for 10s",
-                Dfuncs.monitor_input_events)
-        self.menuitem("Toggle notifications", ntfy.toggle)
-        self.menuitem("Save key stroke pattern", Dfuncs.save_key_replay)
-        self.menuitem("Replay last key stroke pattern", Dfuncs.replay_pressed_keys)
         self.queue = None
     
-        
-    
-    # def iconpath(self,path):
-    #     self.path = path
-    #
-    # def tooltip(self,text):
-    #     self.tooltip = text
-    # #
-    # def left_click(self,func):
-    #      self.left_click = func
-    
-    
     def menuitem(self, name, func=lambda: warnings.warn("No action defined.")):
         self._items.append((str(name), func))
         
     def additem(self,func):
+        """A decorator"""
         self.menuitem(func.__name__.replace("_"," "), func)
         return func
     
+    def add_default_menuitems(self):
+        self.menuitem("Display win info", Dfuncs.display_win_info)
+        self.menuitem("Get single key name(s)", Dfuncs.display_key_names)
+        self.menuitem("Monitor input events for 10s",
+                Dfuncs.monitor_input_events)
+        self.menuitem("Toggle notifications", ntfy.toggle)
+        self.menuitem("Save key stroke pattern", Dfuncs.save_key_replay)
+        self.menuitem("Replay last key stroke pattern",
+                Dfuncs.replay_pressed_keys)
+    
     @property
     def items(self):
         if self.last_item:
             return self._items + [self.last_item]
         else:
             return self._items
```

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/iconpower/adapt_pystray.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/iconpower/adapt_pystray.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/iconpower/adapt_yad_bash.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/iconpower/adapt_yad_bash.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/iconpower/icons/Dicon.png` & `Dpowers-0.1.5rc2/Dlib/Dpowers/iconpower/icons/Dicon.png`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/iconpower/icons/Dicon.svg` & `Dpowers-0.1.5rc2/Dlib/Dpowers/iconpower/icons/Dicon.svg`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/iconpower/icons/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/iconpower/icons/__init__.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/notificationpower/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/notificationpower/__init__.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/notificationpower/adapt_notify_send_bash.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/notificationpower/adapt_notify_send_bash.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/sound/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/sound/__init__.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/sound/ttspower/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/sound/ttspower/__init__.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/sound/ttspower/adapt_ttsx3.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/sound/ttspower/adapt_ttsx3.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/winapps.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/winapps.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/windowpower/__init__.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/windowpower/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         except NotImplementedError as e:
             raise self._error(prop_name,self.property_from_ID) from e
         if not val: val = None
         self.cached_properties[ID][prop_name]=val
         return val
     
     def id_exists(self, ID):
-        return bool(self.property_from_ID(ID, "title"))
+        return bool(self.property_from_ID(ID, "title", query_cache=False))
     
     @adaptionmethod
     def activate(self, ID):
         return self.activate.target_with_args()
     
     @adaptionmethod
     def map(self, ID):
```

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/windowpower/adapt_xtools_bash.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/windowpower/adapt_xtools_bash.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers/windowpower/windowobjects.py` & `Dpowers-0.1.5rc2/Dlib/Dpowers/windowpower/windowobjects.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers.egg-info/PKG-INFO` & `Dpowers-0.1.5rc2/Dlib/Dpowers.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dpowers
-Version: 0.1.5rc1
+Version: 0.1.5rc2
 Summary: Unified Interface for automatic interaction
 Home-page: https://github.com/dp0s/Dpowers
 Author: DPS
 Author-email: dps@my.mail.de
 License: UNKNOWN
 Description: Documentation see https://dpowers.readthedocs.io.
```

### Comparing `Dpowers-0.1.5rc1/Dlib/Dpowers.egg-info/SOURCES.txt` & `Dpowers-0.1.5rc2/Dlib/Dpowers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/Dlib/__init__.py` & `Dpowers-0.1.5rc2/Dlib/__init__.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/PKG-INFO` & `Dpowers-0.1.5rc2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dpowers
-Version: 0.1.5rc1
+Version: 0.1.5rc2
 Summary: Unified Interface for automatic interaction
 Home-page: https://github.com/dp0s/Dpowers
 Author: DPS
 Author-email: dps@my.mail.de
 License: UNKNOWN
 Description: Documentation see https://dpowers.readthedocs.io.
```

### Comparing `Dpowers-0.1.5rc1/README.md` & `Dpowers-0.1.5rc2/README.md`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/docs/Makefile` & `Dpowers-0.1.5rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/docs/conf.py` & `Dpowers-0.1.5rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/docs/index.rst` & `Dpowers-0.1.5rc2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/docs/intro.rst` & `Dpowers-0.1.5rc2/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/docs/make.bat` & `Dpowers-0.1.5rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/docs/preperation.rst` & `Dpowers-0.1.5rc2/docs/preperation.rst`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/docs/quickstart.rst` & `Dpowers-0.1.5rc2/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/docs/reference/power.rst` & `Dpowers-0.1.5rc2/docs/reference/power.rst`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/docs/reference/powerclasses.rst` & `Dpowers-0.1.5rc2/docs/reference/powerclasses.rst`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/licenseheader.txt` & `Dpowers-0.1.5rc2/licenseheader.txt`

 * *Files identical despite different names*

### Comparing `Dpowers-0.1.5rc1/setup.py` & `Dpowers-0.1.5rc2/setup.py`

 * *Files identical despite different names*


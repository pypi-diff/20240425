# Comparing `tmp/djangocms_frontend-1.3.1.tar.gz` & `tmp/djangocms_frontend-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms_frontend-1.3.1.tar", last modified: Sat Apr 13 13:34:20 2024, max compression
+gzip compressed data, was "djangocms_frontend-1.3.2.tar", last modified: Wed Apr 24 23:01:54 2024, max compression
```

## Comparing `djangocms_frontend-1.3.1.tar` & `djangocms_frontend-1.3.2.tar`

### file list

```diff
@@ -1,690 +1,689 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.456842 djangocms_frontend-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-04-13 13:34:20.456842 djangocms_frontend-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.360842 djangocms_frontend-1.3.1/djangocms_frontend/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/cms_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.360842 djangocms_frontend-1.3.1/djangocms_frontend/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/common/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/common/background.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.364842 djangocms_frontend-1.3.1/djangocms_frontend/common/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/common/bootstrap5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/common/bootstrap5/background.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/common/bootstrap5/responsive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/common/bootstrap5/sizing.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/common/responsive.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/common/sizing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/common/spacing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/common/title.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.364842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.364842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.364842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.364842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.332842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.332842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.364842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion.html
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.364842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.364842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/frameworks/foundation6.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.364842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.332842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.332842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.368842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/alert.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.368842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.368842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.368842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.368842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.368842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.332842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.368842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.368842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/badge.html
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/templates/djangocms_frontend/badge.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.368842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.368842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/frameworks/foundation6.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.372842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.336842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.336842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.372842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card.html
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.372842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.372842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.372842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.372842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.336842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.336842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.372842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/carousel.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.336842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.336842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.372842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.372842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.376842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.376842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.336842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.336842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.376842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/collapse.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.376842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-container.html
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.376842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.376842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.376842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.336842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.336842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.376842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/blockquote.html
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/figure.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.380842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/code.html
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/figure.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.380842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.380842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/frameworks/foundation6.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.380842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.380842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_container.html
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.380842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/grid_row.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.380842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.384842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.384842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.400842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    59572 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot
--rw-r--r--   0 runner    (1001) docker     (127)   277297 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg
--rw-r--r--   0 runner    (1001) docker     (127)    59388 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    63664 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff
--rw-r--r--   0 runner    (1001) docker     (127)   123564 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot
--rw-r--r--   0 runner    (1001) docker     (127)   516494 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg
--rw-r--r--   0 runner    (1001) docker     (127)   123376 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   123452 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)    89988 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)    76736 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   101648 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)    78268 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16276 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    54568 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot
--rw-r--r--   0 runner    (1001) docker     (127)   150535 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg
--rw-r--r--   0 runner    (1001) docker     (127)    56976 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    32020 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)    28196 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot
--rw-r--r--   0 runner    (1001) docker     (127)    20996 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf
--rw-r--r--   0 runner    (1001) docker     (127)    54789 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg
--rw-r--r--   0 runner    (1001) docker     (127)    28028 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    14984 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   729984 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot
--rw-r--r--   0 runner    (1001) docker     (127)  2883039 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg
--rw-r--r--   0 runner    (1001) docker     (127)   729800 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   386256 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)   282928 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    99774 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (127)   184969 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (127)    99564 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    56468 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    44720 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.408841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/
--rw-r--r--   0 runner    (1001) docker     (127)    48146 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json
--rw-r--r--   0 runner    (1001) docker     (127)    30533 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (127)    10004 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json
--rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (127)    48978 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json
--rw-r--r--   0 runner    (1001) docker     (127)    35481 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json
--rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json
--rw-r--r--   0 runner    (1001) docker     (127)    18498 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json
--rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json
--rw-r--r--   0 runner    (1001) docker     (127)    30092 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json
--rw-r--r--   0 runner    (1001) docker     (127)    23027 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json
--rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json
--rw-r--r--   0 runner    (1001) docker     (127)    24992 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json
--rw-r--r--   0 runner    (1001) docker     (127)    15565 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json
--rw-r--r--   0 runner    (1001) docker     (127)    25003 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json
--rw-r--r--   0 runner    (1001) docker     (127)    15576 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json
--rw-r--r--   0 runner    (1001) docker     (127)    24997 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json
--rw-r--r--   0 runner    (1001) docker     (127)    15570 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json
--rw-r--r--   0 runner    (1001) docker     (127)    24997 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json
--rw-r--r--   0 runner    (1001) docker     (127)    15570 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json
--rw-r--r--   0 runner    (1001) docker     (127)    25003 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json
--rw-r--r--   0 runner    (1001) docker     (127)    15576 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json
--rw-r--r--   0 runner    (1001) docker     (127)    35227 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json
--rw-r--r--   0 runner    (1001) docker     (127)    21372 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (127)    14032 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json
--rw-r--r--   0 runner    (1001) docker     (127)     8718 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.408841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.412842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)    21397 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js
--rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.412842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/
--rw-r--r--   0 runner    (1001) docker     (127)    10722 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)    30045 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)    28165 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    15830 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)    13288 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   137737 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)   115209 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    20997 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)    18213 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css
--rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    77647 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)    65062 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    32569 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)    26765 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_text_ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_text_ckeditor/ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_text_ckeditor/ckeditor/icon/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_text_ckeditor/ckeditor/icon/ckeditor.icons.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/icon.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/add_css.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templatetags/icon_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     9287 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/image_save.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/image.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.420842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.420842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/jumbotron.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.420842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/jumbotron.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.420842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    14745 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.420842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.420842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.420842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.420842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/link.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.420842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/icon.html
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.420842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/icon.html
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/list-group.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/media.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/media.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.428841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/brand.html
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navigation.html
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navlink.html
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/page_tree.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.428841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/icon.html
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/page_tree.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.428841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/page_tree.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.428841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.428841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/tabs.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/item.html
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/no_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/spacing.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/toc.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templatetags/fe_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    37745 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    28135 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    44784 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.436842 djangocms_frontend-1.3.1/djangocms_frontend/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    34087 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.436842 djangocms_frontend-1.3.1/djangocms_frontend/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    27932 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    45014 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.436842 djangocms_frontend-1.3.1/djangocms_frontend/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    29475 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    46279 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/locale/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.436842 djangocms_frontend-1.3.1/djangocms_frontend/locale/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19546 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    41787 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.436842 djangocms_frontend-1.3.1/djangocms_frontend/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    34140 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.436842 djangocms_frontend-1.3.1/djangocms_frontend/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    14324 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    38302 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/locale/sq/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.436842 djangocms_frontend-1.3.1/djangocms_frontend/locale/sq/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    24556 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    43934 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/sq/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.436842 djangocms_frontend-1.3.1/djangocms_frontend/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17985 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/bootstrap4_migration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.436842 djangocms_frontend-1.3.1/djangocms_frontend/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/commands/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.440842 djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/frequency_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/migrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/stale_references.py
--rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/sync_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/icon_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/styled_link_migration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.440842 djangocms_frontend-1.3.1/djangocms_frontend/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.440842 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/css/
--rw-r--r--   0 runner    (1001) docker     (127)    79431 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/css/base.css
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/css/base.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/css/button_group.css
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/css/div_select.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.440842 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/js/auto_input.js
--rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js
--rw-r--r--   0 runner    (1001) docker     (127)    95562 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/js/django_select2.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.440842 djangocms_frontend-1.3.1/djangocms_frontend/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.440842 djangocms_frontend-1.3.1/djangocms_frontend/templates/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/bootstrap5/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/bootstrap5/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/bootstrap5/menu.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.440842 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.444841 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/base-collapse.html
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/deprecated.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.444841 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/includes/
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.444841 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/select.html
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/html_container.html
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.444841 djangocms_frontend-1.3.1/djangocms_frontend/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templatetags/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.452841 djangocms_frontend-1.3.1/djangocms_frontend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-04-13 13:34:20.000000 djangocms_frontend-1.3.1/djangocms_frontend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    31500 2024-04-13 13:34:20.000000 djangocms_frontend-1.3.1/djangocms_frontend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:34:20.000000 djangocms_frontend-1.3.1/djangocms_frontend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:34:20.000000 djangocms_frontend-1.3.1/djangocms_frontend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-13 13:34:20.000000 djangocms_frontend-1.3.1/djangocms_frontend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-13 13:34:20.000000 djangocms_frontend-1.3.1/djangocms_frontend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-13 13:34:20.456842 djangocms_frontend-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.444841 djangocms_frontend-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.444841 djangocms_frontend-1.3.1/tests/accordion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/accordion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/accordion/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/accordion/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.444841 djangocms_frontend-1.3.1/tests/alert/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/alert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/alert/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/alert/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.448841 djangocms_frontend-1.3.1/tests/badge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/badge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/badge/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/badge/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.448841 djangocms_frontend-1.3.1/tests/card/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/card/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/card/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.448841 djangocms_frontend-1.3.1/tests/carousel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/carousel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/carousel/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/carousel/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.448841 djangocms_frontend-1.3.1/tests/collapse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/collapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/collapse/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/collapse/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.448841 djangocms_frontend-1.3.1/tests/content/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/content/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/content/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.448841 djangocms_frontend-1.3.1/tests/grid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/grid/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/grid/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.448841 djangocms_frontend-1.3.1/tests/icon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/icon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/icon/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/icon/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.448841 djangocms_frontend-1.3.1/tests/image/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/image/test_drag_n_drop.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/image/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/image/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.448841 djangocms_frontend-1.3.1/tests/jumbotron/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/jumbotron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/jumbotron/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/jumbotron/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.452841 djangocms_frontend-1.3.1/tests/link/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/link/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/link/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/link/test_urlconf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.452841 djangocms_frontend-1.3.1/tests/listgroup/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/listgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/listgroup/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/listgroup/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.452841 djangocms_frontend-1.3.1/tests/media/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/media/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/media/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.452841 djangocms_frontend-1.3.1/tests/navigation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/navigation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/navigation/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/navigation/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.452841 djangocms_frontend-1.3.1/tests/tabs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/tabs/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/tabs/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.452841 djangocms_frontend-1.3.1/tests/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/utilities/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/utilities/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.159474 djangocms_frontend-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-04-24 23:01:54.159474 djangocms_frontend-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.055473 djangocms_frontend-1.3.2/djangocms_frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/cms_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.059473 djangocms_frontend-1.3.2/djangocms_frontend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/common/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/common/background.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.059473 djangocms_frontend-1.3.2/djangocms_frontend/common/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/common/bootstrap5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/common/bootstrap5/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/common/bootstrap5/responsive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/common/bootstrap5/sizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/common/responsive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/common/sizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/common/spacing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/common/title.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.059473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.059473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/accordion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/accordion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/accordion/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/accordion/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.059473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/accordion/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/accordion/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.059473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/accordion/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/accordion/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/accordion/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/accordion/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.027473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/accordion/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.027473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.063473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.063473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.063473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/frameworks/foundation6.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.063473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.031473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.031473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.063473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/alert.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.063473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.063473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.063473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/badge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/badge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/badge/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/badge/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.063473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/badge/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/badge/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/badge/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.067473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/badge/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/badge/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/badge/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/badge/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.031473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/badge/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.067473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/badge/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.067473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/badge.html
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/badge/templates/djangocms_frontend/badge.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.067473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.067473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/frameworks/foundation6.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.067473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.031473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.031473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.067473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card.html
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.067473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.067473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.071473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.071473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.031473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.031473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.071473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/carousel.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.031473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.031473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.071473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.071473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/collapse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/collapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/collapse/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/collapse/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.071473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/collapse/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/collapse/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/collapse/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.071473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/collapse/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/collapse/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/collapse/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/collapse/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.035473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/collapse/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.035473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.071473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/collapse.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.071473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-container.html
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.075473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.075473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.075473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.035473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.035473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.075473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/blockquote.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/figure.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.075473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/code.html
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/figure.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.075473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.075473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/frameworks/foundation6.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.079473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.035473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.035473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.079473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_container.html
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.079473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/grid_row.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.079473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.079473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.079473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.039473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.035473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.035473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.035473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.039473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.099473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    59572 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   277297 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    59388 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    63664 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   123564 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   516494 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   123376 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   123452 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    89988 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    76736 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   101648 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    78268 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16276 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    54568 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   150535 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    56976 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    32020 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    28196 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    20996 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf
+-rw-r--r--   0 runner    (1001) docker     (127)    54789 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    28028 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    14984 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   729984 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (127)  2883039 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   729800 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   386256 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   282928 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    99774 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   184969 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    99564 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    56468 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    44720 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.107473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/
+-rw-r--r--   0 runner    (1001) docker     (127)    48146 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30533 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10004 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)    48978 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35481 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18498 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30092 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23027 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24992 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15565 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25003 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15576 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24997 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15570 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24997 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15570 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25003 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15576 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35227 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21372 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14032 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8718 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.107473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.107473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    21397 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.107473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/
+-rw-r--r--   0 runner    (1001) docker     (127)    10722 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.111473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)    30045 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)    28165 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15830 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)    13288 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   137737 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)   115209 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    20997 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18213 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    77647 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)    65062 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    32569 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)    26765 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.039473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_text_ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.039473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_text_ckeditor/ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.111473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_text_ckeditor/ckeditor/icon/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_text_ckeditor/ckeditor/icon/ckeditor.icons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.039473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.039473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.039473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.111473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.111473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/icon.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.111473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/add_css.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.111473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/templatetags/icon_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.115473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9029 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.115473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/image_save.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.115473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.039473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.039473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.115473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/image.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.039473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.115473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.115473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/jumbotron/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/jumbotron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/jumbotron/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/jumbotron/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.115473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/jumbotron/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/jumbotron/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/jumbotron/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.115473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/jumbotron/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/jumbotron/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/jumbotron/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.039473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/jumbotron/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.039473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.115473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/jumbotron.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.039473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.039473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.115473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/jumbotron.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.119473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14444 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.119473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.119473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.043473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.043473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.119473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.043473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.043473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.119473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/link.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.043473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.043473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.119473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/icon.html
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.043473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.043473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.119473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/icon.html
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.119473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/listgroup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/listgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/listgroup/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/listgroup/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/listgroup/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.123473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/listgroup/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/listgroup/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.123473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/listgroup/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/listgroup/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/listgroup/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.043473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/listgroup/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.043473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.123473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/list-group.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.123473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/media/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/media/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/media/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.123473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/media/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/media/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/media/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.123473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/media/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/media/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/media/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/media/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.043473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/media/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.043473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/media/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.123473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/media.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.123473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/media.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.123473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.123473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.123473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.043473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.043473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.127473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/brand.html
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navlink.html
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/page_tree.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.043473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.047473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.127473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/icon.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/page_tree.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.127473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/page_tree.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.131473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.131473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.131473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.047473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.047473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.131473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/tabs.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.047473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.047473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.131473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/item.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.131473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.131473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.131473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.047473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.131473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.131473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/no_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/spacing.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.135473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/toc.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.135473 djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/templatetags/fe_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.135473 djangocms_frontend-1.3.2/djangocms_frontend/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.051473 djangocms_frontend-1.3.2/djangocms_frontend/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.047473 djangocms_frontend-1.3.2/djangocms_frontend/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.135473 djangocms_frontend-1.3.2/djangocms_frontend/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    37745 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.047473 djangocms_frontend-1.3.2/djangocms_frontend/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.135473 djangocms_frontend-1.3.2/djangocms_frontend/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    28135 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    44784 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.047473 djangocms_frontend-1.3.2/djangocms_frontend/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.135473 djangocms_frontend-1.3.2/djangocms_frontend/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    34087 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.047473 djangocms_frontend-1.3.2/djangocms_frontend/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.135473 djangocms_frontend-1.3.2/djangocms_frontend/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    27932 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    45014 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.047473 djangocms_frontend-1.3.2/djangocms_frontend/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.135473 djangocms_frontend-1.3.2/djangocms_frontend/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    29475 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    46279 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.047473 djangocms_frontend-1.3.2/djangocms_frontend/locale/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.135473 djangocms_frontend-1.3.2/djangocms_frontend/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19546 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    41787 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.051473 djangocms_frontend-1.3.2/djangocms_frontend/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.139473 djangocms_frontend-1.3.2/djangocms_frontend/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    34140 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.051473 djangocms_frontend-1.3.2/djangocms_frontend/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.139473 djangocms_frontend-1.3.2/djangocms_frontend/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    14324 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    38302 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.051473 djangocms_frontend-1.3.2/djangocms_frontend/locale/sq/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.139473 djangocms_frontend-1.3.2/djangocms_frontend/locale/sq/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    24556 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    43934 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/locale/sq/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.139473 djangocms_frontend-1.3.2/djangocms_frontend/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17851 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/management/bootstrap4_migration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.139473 djangocms_frontend-1.3.2/djangocms_frontend/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/management/commands/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.139473 djangocms_frontend-1.3.2/djangocms_frontend/management/commands/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/management/commands/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/management/commands/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/management/commands/subcommands/frequency_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/management/commands/subcommands/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/management/commands/subcommands/stale_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/management/commands/subcommands/sync_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/management/icon_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/management/styled_link_migration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.139473 djangocms_frontend-1.3.2/djangocms_frontend/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.051473 djangocms_frontend-1.3.2/djangocms_frontend/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.051473 djangocms_frontend-1.3.2/djangocms_frontend/static/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.143473 djangocms_frontend-1.3.2/djangocms_frontend/static/djangocms_frontend/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    79924 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/static/djangocms_frontend/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/static/djangocms_frontend/css/base.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/static/djangocms_frontend/css/button_group.css
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/static/djangocms_frontend/css/div_select.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.143473 djangocms_frontend-1.3.2/djangocms_frontend/static/djangocms_frontend/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/static/djangocms_frontend/js/auto_input.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js
+-rw-r--r--   0 runner    (1001) docker     (127)    95562 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/static/djangocms_frontend/js/django_select2.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.143473 djangocms_frontend-1.3.2/djangocms_frontend/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.143473 djangocms_frontend-1.3.2/djangocms_frontend/templates/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/templates/bootstrap5/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/templates/bootstrap5/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/templates/bootstrap5/menu.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.143473 djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.143473 djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend/admin/base-collapse.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend/admin/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend/admin/deprecated.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.143473 djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend/admin/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.147473 djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/select.html
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend/html_container.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.147473 djangocms_frontend-1.3.2/djangocms_frontend/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/djangocms_frontend/templatetags/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.159474 djangocms_frontend-1.3.2/djangocms_frontend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-04-24 23:01:53.000000 djangocms_frontend-1.3.2/djangocms_frontend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    31460 2024-04-24 23:01:54.000000 djangocms_frontend-1.3.2/djangocms_frontend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 23:01:53.000000 djangocms_frontend-1.3.2/djangocms_frontend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 23:01:53.000000 djangocms_frontend-1.3.2/djangocms_frontend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-24 23:01:53.000000 djangocms_frontend-1.3.2/djangocms_frontend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 23:01:53.000000 djangocms_frontend-1.3.2/djangocms_frontend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-24 23:01:54.159474 djangocms_frontend-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.147473 djangocms_frontend-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.147473 djangocms_frontend-1.3.2/tests/accordion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/accordion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/accordion/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/accordion/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.151473 djangocms_frontend-1.3.2/tests/alert/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/alert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/alert/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/alert/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.151473 djangocms_frontend-1.3.2/tests/badge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/badge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/badge/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/badge/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.151473 djangocms_frontend-1.3.2/tests/card/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/card/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/card/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.151473 djangocms_frontend-1.3.2/tests/carousel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/carousel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/carousel/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/carousel/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.151473 djangocms_frontend-1.3.2/tests/collapse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/collapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/collapse/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/collapse/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.151473 djangocms_frontend-1.3.2/tests/content/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/content/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/content/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.151473 djangocms_frontend-1.3.2/tests/grid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/grid/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/grid/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.151473 djangocms_frontend-1.3.2/tests/icon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/icon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/icon/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/icon/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.155473 djangocms_frontend-1.3.2/tests/image/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/image/test_drag_n_drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/image/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/image/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.155473 djangocms_frontend-1.3.2/tests/jumbotron/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/jumbotron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/jumbotron/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/jumbotron/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.155473 djangocms_frontend-1.3.2/tests/link/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/link/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/link/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/link/test_urlconf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.155473 djangocms_frontend-1.3.2/tests/listgroup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/listgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/listgroup/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/listgroup/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.155473 djangocms_frontend-1.3.2/tests/media/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/media/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/media/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.155473 djangocms_frontend-1.3.2/tests/navigation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/navigation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/navigation/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/navigation/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.155473 djangocms_frontend-1.3.2/tests/tabs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/tabs/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/tabs/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:54.159474 djangocms_frontend-1.3.2/tests/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/utilities/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-24 23:01:50.000000 djangocms_frontend-1.3.2/tests/utilities/test_plugins.py
```

### Comparing `djangocms_frontend-1.3.1/LICENSE` & `djangocms_frontend-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/PKG-INFO` & `djangocms_frontend-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-frontend
-Version: 1.3.1
+Version: 1.3.2
 Summary: Adds abstract User Interface items as plugins to django CMS.
 Home-page: https://github.com/django-cms/djangocms-frontend
 Author: fsbraun
 Author-email: fsbraun@gmx.de
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `djangocms_frontend-1.3.1/README.rst` & `djangocms_frontend-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/__init__.py` & `djangocms_frontend-1.3.2/djangocms_frontend/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,8 @@
  9. git push
 10. Assure that all tests pass on https://github.com/django-cms/djangocms-frontend/actions
 11. Create a new release on https://github.com/django-cms/djangocms-frontend/releases/new
 12. Publish the release when ready
 13. Github actions will publish the new package to pypi
 """
 
-__version__ = "1.3.1"
+__version__ = "1.3.2"
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/common/attributes.py` & `djangocms_frontend-1.3.2/djangocms_frontend/common/attributes.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,17 +12,15 @@
             "collapse",
             "attributes",
         ),
     }
 
     def get_fieldsets(self, request, obj=None):
         meta = self.form._meta
-        fields = (
-            ["tag_type"] if "tag_type" in getattr(meta, "untangled_fields", ()) else []
-        )
+        fields = ["tag_type"] if "tag_type" in getattr(meta, "untangled_fields", ()) else []
         fields.append("attributes")
         return insert_fields(
             super().get_fieldsets(request, obj),
             fields,
             blockname=_("Advanced settings"),
             blockattrs=self.block_attr,
             position=-1,  # Always last
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/common/bootstrap5/background.py` & `djangocms_frontend-1.3.2/djangocms_frontend/common/bootstrap5/background.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,17 +43,15 @@
                 "background_shadow",
             ]
         }
 
     background_context = forms.ChoiceField(
         label=_("Background context"),
         required=False,
-        choices=settings.EMPTY_CHOICE
-        + settings.COLOR_STYLE_CHOICES
-        + (("transparent", _("Transparent")),),
+        choices=settings.EMPTY_CHOICE + settings.COLOR_STYLE_CHOICES + (("transparent", _("Transparent")),),
         initial=settings.EMPTY_CHOICE[0][0],
         widget=ColoredButtonGroup(),
     )
     background_opacity = forms.ChoiceField(
         label=_("Background opacity"),
         required=False,
         choices=settings.framework_settings.OPACITY_CHOICES,
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/common/bootstrap5/responsive.py` & `djangocms_frontend-1.3.2/djangocms_frontend/common/bootstrap5/responsive.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/common/bootstrap5/sizing.py` & `djangocms_frontend-1.3.2/djangocms_frontend/common/bootstrap5/sizing.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,21 +42,17 @@
 
     size_x = forms.ChoiceField(
         label=_("Horizontal size"),
         required=False,
         initial=settings.EMPTY_CHOICE[0][0],
         choices=settings.EMPTY_CHOICE + settings.SIZE_X_CHOICES,
         #        widget=ButtonGroup(attrs=dict(property="text")),
-        help_text=_(
-            "Sets the horizontal size relative to the surrounding container or the viewport."
-        ),
+        help_text=_("Sets the horizontal size relative to the surrounding container or the viewport."),
     )
     size_y = forms.ChoiceField(
         label=_("Vertical size"),
         required=False,
         initial=settings.EMPTY_CHOICE[0][0],
         choices=settings.EMPTY_CHOICE + settings.SIZE_Y_CHOICES,
         #       widget=ButtonGroup(attrs=dict(property="text")),
-        help_text=_(
-            "Sets the vertical size relative to the surrounding container or the viewport."
-        ),
+        help_text=_("Sets the vertical size relative to the surrounding container or the viewport."),
     )
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/common/spacing.py` & `djangocms_frontend-1.3.2/djangocms_frontend/common/spacing.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,20 +24,15 @@
     """2 component widget allowing to choose a side and the size of a spacing"""
 
     def __init__(self, **kwargs):
         self.property = kwargs.pop("property")
         self.side_choices = kwargs.pop("side_choices")
         super().__init__(
             [
-                IconGroup(
-                    choices=[
-                        (self.property + side, verbose)
-                        for side, verbose in self.side_choices
-                    ]
-                ),
+                IconGroup(choices=[(self.property + side, verbose) for side, verbose in self.side_choices]),
                 DivSelectWidget(choices=kwargs.pop("size_choices")),
             ],
             **kwargs,
         )
 
     def decompress(self, value):
         if isinstance(value, str) and value:
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/common/title.py` & `djangocms_frontend-1.3.2/djangocms_frontend/common/title.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,17 +32,15 @@
         )
         kwargs.setdefault("require_all_fields", False)
         kwargs.setdefault("widget", TitleWidget())
         super().__init__(*args, **kwargs)
 
     def clean(self, value):
         if value[0] and not value[1]:
-            raise ValidationError(
-                _("Please add a title if you want to publish it."), code="incomplete"
-            )
+            raise ValidationError(_("Please add a title if you want to publish it."), code="incomplete")
         return super().clean(value)
 
     def compress(self, data_list):
         return dict(show=data_list[0], title=data_list[1])
 
 
 class TitleMixin:
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/cms_plugins.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/accordion/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/forms.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/accordion/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,13 +11,9 @@
 class AccordionItemRenderMixin:
     render_template = "djangocms_frontend/bootstrap5/accordion_item.html"
 
     def render(self, context, instance, placeholder):
         instance.add_classes("accordion-collapse collapse")
         if instance.accordion_item_open:
             instance.add_classes("show")
-        instance.font_size = (
-            context["parent"]
-            .config.get("accordion_header_type", "")
-            .replace("h", "fs-")
-        )
+        instance.font_size = context["parent"].config.get("accordion_header_type", "").replace("h", "fs-")
         return super().render(context, instance, placeholder)
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/migrations/0001_initial.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/accordion/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/models.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/accordion/models.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/cms_plugins.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/cms_plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 from .. import alert
 from . import forms, models
 
 mixin_factory = settings.get_renderer(alert)
 
 
 @plugin_pool.register_plugin
-class AlertPlugin(
-    mixin_factory("Alert"), AttributesMixin, ResponsiveMixin, SpacingMixin, CMSUIPlugin
-):
+class AlertPlugin(mixin_factory("Alert"), AttributesMixin, ResponsiveMixin, SpacingMixin, CMSUIPlugin):
     """
     Components > "Alerts" Plugin
     https://getbootstrap.com/docs/5.0/components/alerts/
     """
 
     name = _("Alert")
     module = _("Frontend")
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/forms.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,15 @@
 from djangocms_frontend.helpers import first_choice
 from djangocms_frontend.models import FrontendUIItem
 from djangocms_frontend.settings import COLOR_STYLE_CHOICES
 
 mixin_factory = settings.get_forms(alert)
 
 
-class AlertForm(
-    mixin_factory("Alert"), ResponsiveFormMixin, SpacingFormMixin, EntangledModelForm
-):
+class AlertForm(mixin_factory("Alert"), ResponsiveFormMixin, SpacingFormMixin, EntangledModelForm):
     """
     Components > "Alerts" Plugin
     https://getbootstrap.com/docs/5.0/components/alerts/
     """
 
     class Meta:
         model = FrontendUIItem
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/migrations/0001_initial.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/cms_plugins.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/badge/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/forms.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/badge/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/migrations/0001_initial.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/badge/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/cms_plugins.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/constants.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/forms.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,15 @@
 from .constants import (
     CARD_ALIGNMENT_CHOICES,
     CARD_INNER_TYPE_CHOICES,
     CARD_LAYOUT_TYPE_CHOICES,
 )
 
 # card allow for a transparent color
-CARD_COLOR_STYLE_CHOICES = settings.COLOR_STYLE_CHOICES + (
-    ("transparent", _("Transparent")),
-)
+CARD_COLOR_STYLE_CHOICES = settings.COLOR_STYLE_CHOICES + (("transparent", _("Transparent")),)
 
 CARD_TEXT_STYLES = COLOR_STYLE_CHOICES + (("white", _("White")),)
 
 mixin_factory = settings.get_forms(card)
 
 
 class CardLayoutBaseForm(mixin_factory("CardLayout"), EntangledModelForm):
@@ -128,33 +126,29 @@
         if "card_outline" in getattr(settings, "EXCL_CARD_PROP", ())
         else ColoredButtonGroup(),
     )
     card_alignment = forms.ChoiceField(
         label=_("Alignment"),
         choices=settings.EMPTY_CHOICE + CARD_ALIGNMENT_CHOICES,
         required=False,
-        widget=forms.HiddenInput()
-        if "card_alignment" in getattr(settings, "EXCL_CARD_PROP", ())
-        else IconGroup(),
+        widget=forms.HiddenInput() if "card_alignment" in getattr(settings, "EXCL_CARD_PROP", ()) else IconGroup(),
     )
     card_text_color = forms.ChoiceField(
         label=_("Text context"),
         choices=settings.EMPTY_CHOICE + CARD_TEXT_STYLES,
         required=False,
         widget=forms.HiddenInput()
         if "card_text_color" in getattr(settings, "EXCL_CARD_PROP", ())
         else ColoredButtonGroup(),
     )
     card_full_height = forms.BooleanField(
         label=_("Full height"),
         initial=False,
         required=False,
-        help_text=_(
-            "If checked cards in one row will automatically extend to the full row height."
-        ),
+        help_text=_("If checked cards in one row will automatically extend to the full row height."),
         widget=forms.HiddenInput()
         if "card_full_height" in getattr(settings, "EXCL_CARD_PROP", ())
         else forms.CheckboxInput,
     )
     attributes = AttributesFormField()
     tag_type = TagTypeFormField()
 
@@ -189,17 +183,15 @@
         help_text=_("Define the structure of the plugin."),
         widget=ButtonGroup(attrs=dict(label_class="btn-secondary")),
     )
     text_alignment = forms.ChoiceField(
         label=_("Content alignment"),
         choices=settings.EMPTY_CHOICE + settings.ALIGN_CHOICES,
         required=False,
-        widget=forms.HiddenInput()
-        if "text_alignment" in getattr(settings, "EXCL_CARD_PROP", ())
-        else IconGroup(),
+        widget=forms.HiddenInput() if "text_alignment" in getattr(settings, "EXCL_CARD_PROP", ()) else IconGroup(),
     )
     attributes = AttributesFormField()
     tag_type = TagTypeFormField()
 
 
 class CardDeckBaseForm(EntangledModelForm):
     class Meta:
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/frameworks/foundation6.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/frameworks/foundation6.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/migrations/0001_initial.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/models.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/models.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/cms_plugins.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/cms_plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,17 +45,15 @@
                     ),
                 )
             },
         ),
     ]
 
     def get_render_template(self, context, instance, placeholder):
-        return get_plugin_template(
-            instance, "carousel", "carousel", CAROUSEL_TEMPLATE_CHOICES
-        )
+        return get_plugin_template(instance, "carousel", "carousel", CAROUSEL_TEMPLATE_CHOICES)
 
 
 @plugin_pool.register_plugin
 class CarouselSlidePlugin(
     mixin_factory("CarouselSlide"),
     AttributesMixin,
     BackgroundMixin,
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/constants.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,13 @@
     (1, 1),
     (3, 2),
     (4, 3),
     (21, 9),
     (18, 9),
 ) + tuple(getattr(settings, "DJANGOCMS_FRONTEND_CAROUSEL_ASPECT_RATIOS", tuple()))
 
-CAROUSEL_ASPECT_RATIO_CHOICES = tuple(
-    (f"{x}x{y}", f"{x}x{y}") for x, y in CAROUSEL_ASPECT_RATIOS
-)
+CAROUSEL_ASPECT_RATIO_CHOICES = tuple((f"{x}x{y}", f"{x}x{y}") for x, y in CAROUSEL_ASPECT_RATIOS)
 
 CAROUSEL_TRANSITION_CHOICES = (
     ("", _("Slide")),
     ("carousel-fade", _("Fade")),
 )
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/forms.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,27 +107,22 @@
             'first item. If "carousel", autoplays the carousel on load.'
         ),
     )
     carousel_wrap = forms.BooleanField(
         label=_("Wrap"),
         initial=True,
         required=False,
-        help_text=_(
-            "Whether the carousel should cycle continuously or have " "hard stops."
-        ),
+        help_text=_("Whether the carousel should cycle continuously or have " "hard stops."),
     )
     carousel_aspect_ratio = forms.ChoiceField(
         label=_("Aspect ratio"),
         choices=settings.EMPTY_CHOICE + CAROUSEL_ASPECT_RATIO_CHOICES,
         required=False,
         initial=settings.EMPTY_CHOICE[0][0],
-        help_text=_(
-            "Determines width and height of the image "
-            "according to the selected ratio."
-        ),
+        help_text=_("Determines width and height of the image " "according to the selected ratio."),
     )
     carousel_transition = forms.ChoiceField(
         label=_("Transition"),
         choices=CAROUSEL_TRANSITION_CHOICES,
         required=False,
         initial=CAROUSEL_TRANSITION_CHOICES[0][0],
         help_text=_("Determines if slides change by sliding or fading."),
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,15 @@
 class CarouselSlideRenderMixin:
     def render(self, context, instance, placeholder):
         parent = instance.parent.get_plugin_instance()[0]
         width = float(context.get("width") or CAROUSEL_DEFAULT_SIZE[0])
         height = float(context.get("height") or CAROUSEL_DEFAULT_SIZE[1])
 
         if parent.carousel_aspect_ratio:
-            aspect_width, aspect_height = tuple(
-                int(i) for i in parent.carousel_aspect_ratio.split("x")
-            )
+            aspect_width, aspect_height = tuple(int(i) for i in parent.carousel_aspect_ratio.split("x"))
             height = width * aspect_height / aspect_width
 
         instance.add_classes("carousel-item")
         if is_first_child(instance, parent):
             instance.add_classes("active")
         context["link"] = instance.get_link()
         context["aspect_ratio"] = str(width / height)
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/migrations/0001_initial.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/models.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,18 +47,15 @@
         image_text = content_text = ""
 
         if self.carousel_image:
             if self.rel_image is None:
                 image_text = _("<file is missing>")
             elif self.rel_image.name:
                 image_text = self.rel_image.name
-            elif (
-                self.rel_image.original_filename
-                and os.path.split(self.rel_image.original_filename)[1]
-            ):
+            elif self.rel_image.original_filename and os.path.split(self.rel_image.original_filename)[1]:
                 image_text = os.path.split(self.rel_image.original_filename)[1]
             else:
                 image_text = "Image"
         if self.carousel_content:
             text = strip_tags(self.carousel_content).strip()
             if len(text) > 100:
                 content_text = f"{text[:100]}..."
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/cms_plugins.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/collapse/cms_plugins.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,17 +34,15 @@
 
     fieldsets = [
         (None, {"fields": ("collapse_siblings",)}),
     ]
 
 
 @plugin_pool.register_plugin
-class CollapseTriggerPlugin(
-    mixin_factory("CollapseTrigger"), AttributesMixin, CMSUIPlugin
-):
+class CollapseTriggerPlugin(mixin_factory("CollapseTrigger"), AttributesMixin, CMSUIPlugin):
     """
     Component > "Collapse" Plugin
     https://getbootstrap.com/docs/5.0/components/collapse/
     """
 
     name = _("Collapse trigger")
     module = _("Frontend")
@@ -60,17 +58,15 @@
 
     fieldsets = [
         (None, {"fields": ("trigger_identifier",)}),
     ]
 
 
 @plugin_pool.register_plugin
-class CollapseContainerPlugin(
-    mixin_factory("CollapseContainer"), AttributesMixin, CMSUIPlugin
-):
+class CollapseContainerPlugin(mixin_factory("CollapseContainer"), AttributesMixin, CMSUIPlugin):
     """
     Component > "Collapse Container" Plugin
     https://getbootstrap.com/docs/5.0/components/collapse/
     """
 
     name = _("Collapse container")
     module = _("Frontend")
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/forms.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/collapse/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/migrations/0001_initial.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/collapse/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/models.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/collapse/models.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/cms_plugins.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/forms.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/migrations/0001_initial.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/models.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/models.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/cms_plugins.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/constants.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/forms.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,27 +178,19 @@
     attributes = AttributesFormField()
     tag_type = TagTypeFormField()
 
     def clean(self):
         super().clean()
         for size in settings.DEVICE_SIZES:
             if f"{size}_col" in self.cleaned_data:
-                if (
-                    isinstance(self.cleaned_data[f"{size}_col"], str)
-                    and self.cleaned_data[f"{size}_col"].isnumeric()
-                ):
-                    self.cleaned_data[f"{size}_col"] = int(
-                        self.cleaned_data[f"{size}_col"]
-                    )
+                if isinstance(self.cleaned_data[f"{size}_col"], str) and self.cleaned_data[f"{size}_col"].isnumeric():
+                    self.cleaned_data[f"{size}_col"] = int(self.cleaned_data[f"{size}_col"])
             else:
                 raise ValidationError(
-                    _(
-                        'Column size needs to be empty, "auto", or a '
-                        "number between 1 and %(cols)d"
-                    ),
+                    _('Column size needs to be empty, "auto", or a ' "number between 1 and %(cols)d"),
                     params=dict(cols=GRID_SIZE),
                     code="invalid_column",
                 )
 
 
 # convert regular text type fields to number
 # col_choices = [(col + 1, str(col + 1)) for col in range(GRID_SIZE)] + [("auto", "Auto")]
@@ -229,24 +221,20 @@
         widget=forms.HiddenInput()
         if "{size}_offset" in getattr(settings, "EXCL_COL_PROP", ())
         else forms.NumberInput(),
     )
     extra_fields_column[f"{size}_ms"] = forms.BooleanField(
         label="ms-auto" if size == "xs" else f"ms-{size}-auto",
         required=False,
-        widget=forms.HiddenInput()
-        if "{size}_ms" in getattr(settings, "EXCL_COL_PROP", ())
-        else forms.CheckboxInput(),
+        widget=forms.HiddenInput() if "{size}_ms" in getattr(settings, "EXCL_COL_PROP", ()) else forms.CheckboxInput(),
     )
     extra_fields_column[f"{size}_me"] = forms.BooleanField(
         label="me-auto" if size == "xs" else f"me-{size}-auto",
         required=False,
-        widget=forms.HiddenInput()
-        if "{size}_me" in getattr(settings, "EXCL_COL_PROP", ())
-        else forms.CheckboxInput(),
+        widget=forms.HiddenInput() if "{size}_me" in getattr(settings, "EXCL_COL_PROP", ()) else forms.CheckboxInput(),
     )
 
 GridColumnForm = type(
     "GridColumnForm",
     (GridColumnBaseForm,),
     copy(extra_fields_column),
 )
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,15 @@
 
 
 def get_grid_values(self):
     classes = []
     for device in settings.DEVICE_SIZES:
         for element in ("col", "order", "offset", "ms", "me"):
             size = getattr(self, f"{device}_{element}", None)
-            if isinstance(size, int) and (
-                element == "col" or element == "order" or element == "offset"
-            ):
+            if isinstance(size, int) and (element == "col" or element == "order" or element == "offset"):
                 if size == 0 and element == "col":  # 0 represents auto
                     size = "auto"
                 if device == "xs":
                     classes.append(f"{element}-{size}")
                 else:
                     classes.append(f"{element}-{device}-{size}")
             elif size:
@@ -58,14 +56,12 @@
 
     return classes
 
 
 class GridColumnRenderMixin:
     def render(self, context, instance, placeholder):
         instance.add_classes(
-            f"col text-{instance.text_alignment}"
-            if instance.config.get("text_alignment", None)
-            else "col"
+            f"col text-{instance.text_alignment}" if instance.config.get("text_alignment", None) else "col"
         )
         instance.add_classes(instance.column_alignment)
         instance.add_classes(get_grid_values(instance))
         return super().render(context, instance, placeholder)
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/frameworks/foundation6.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/frameworks/foundation6.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,17 +38,15 @@
             if isinstance(size, int):
                 if element == "col":
                     if size == 0:
                         classes.append(f"{foundation_sizes.get(device, device)}-auto")
                     else:
                         classes.append(f"{foundation_sizes.get(device, device)}-{size}")
                 else:
-                    classes.append(
-                        f"{foundation_sizes.get(device, device)}-{element}-{size}"
-                    )
+                    classes.append(f"{foundation_sizes.get(device, device)}-{element}-{size}")
 
     return classes
 
 
 class GridColumnRenderMixin:
     def render(self, context, instance, placeholder):
         instance.add_classes("cell", get_grid_values(instance))
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/migrations/0001_initial.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/models.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,17 +25,15 @@
 
     class Meta:
         proxy = True
         verbose_name = _("Container")
         _("GridContainer")
 
     def get_short_description(self):
-        text = self.config.get("plugin_title", {}).get("title", "") or self.config.get(
-            "attributes", {}
-        ).get("id", "")
+        text = self.config.get("plugin_title", {}).get("title", "") or self.config.get("attributes", {}).get("id", "")
         for item in GRID_CONTAINER_CHOICES[1:]:
             if item[0] == self.container_type:
                 text += f" ({item[1]})"
         return text
 
     @cached_property
     def image(self):
@@ -52,21 +50,17 @@
 
     class Meta:
         proxy = True
         verbose_name = _("Row")
         _("GridRow")
 
     def get_short_description(self):
-        descr = self.config.get("plugin_title", {}).get("title", "") or self.config.get(
-            "attributes", {}
-        ).get("id", "")
+        descr = self.config.get("plugin_title", {}).get("title", "") or self.config.get("attributes", {}).get("id", "")
         column_count = len(self.child_plugin_instances or [])
-        column_count_str = ngettext(
-            "(1 column)", "(%(count)i columns)", column_count
-        ) % {"count": column_count}
+        column_count_str = ngettext("(1 column)", "(%(count)i columns)", column_count) % {"count": column_count}
         if descr:
             column_count_str = f"{descr} {column_count_str}"
         return column_count_str
 
 
 class GridColumn(FrontendUIItem):
     """
@@ -76,16 +70,14 @@
 
     class Meta:
         proxy = True
         verbose_name = _("Column")
         _("GridColumn")
 
     def get_short_description(self):
-        text = self.config.get("plugin_title", {}).get("title", "") or self.config.get(
-            "attributes", {}
-        ).get("id", "")
+        text = self.config.get("plugin_title", {}).get("title", "") or self.config.get("attributes", {}).get("id", "")
 
         if self.xs_col:
             text += f" (col-{self.xs_col}) "
         else:
             text += " (auto) "
         return text.strip()
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/cms_plugins.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/cms_plugins.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     module = _("Frontend")
     model = models.Icon
     form = forms.IconForm
     text_enabled = True
     text_icon = (
         '<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" '
         'class="bi bi-emoji-sunglasses" viewBox="0 0 16 16"><path d="M4.968 9.75a.5.5 0 1 0-.866.5A4.5 4.5 '
-        '0 0 0 8 12.5a4.5 4.5 0 0 0 3.898-2.25.5.5 0 1 0-.866-.5A3.5 3.5 0 0 1 8 11.5a3.5 3.5 0 0 1-3.032-1.75M7 '
-        '5.116V5a1 1 0 0 0-1-1H3.28a1 1 0 0 0-.97 1.243l.311 1.242A2 2 0 0 0 4.561 8H5a2 2 0 0 0 1.994-1.839A3 '
-        '3 0 0 1 8 6c.393 0 .74.064 1.006.161A2 2 0 0 0 11 8h.438a2 2 0 0 0 1.94-1.515l.311-1.242A1 1 0 0 0 '
+        "0 0 0 8 12.5a4.5 4.5 0 0 0 3.898-2.25.5.5 0 1 0-.866-.5A3.5 3.5 0 0 1 8 11.5a3.5 3.5 0 0 1-3.032-1.75M7 "
+        "5.116V5a1 1 0 0 0-1-1H3.28a1 1 0 0 0-.97 1.243l.311 1.242A2 2 0 0 0 4.561 8H5a2 2 0 0 0 1.994-1.839A3 "
+        "3 0 0 1 8 6c.393 0 .74.064 1.006.161A2 2 0 0 0 11 8h.438a2 2 0 0 0 1.94-1.515l.311-1.242A1 1 0 0 0 "
         '12.72 4H10a1 1 0 0 0-1 1v.116A4.2 4.2 0 0 0 8 5c-.35 0-.69.04-1 .116"/><path d="M16 8A8 8 0 1 1 0 8a8 8 '
         '0 0 1 16 0m-1 0A7 7 0 1 0 1 8a7 7 0 0 0 14 0"/></svg>'
     )
     fieldsets = [
         (
             None,
             {
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/conf.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,41 +10,41 @@
     "material-icons-outlined": "https://fonts.googleapis.com/css2?family=Material+Icons+Outlined",
     "material-icons-round": "https://fonts.googleapis.com/css2?family=Material+Icons+Round",
     "material-icons-sharp": "https://fonts.googleapis.com/css2?family=Material+Icons+Sharp",
     "material-icons-two-tone": "https://fonts.googleapis.com/css2?family=Material+Icons+Two+Tone",
     "fomantic-ui": "fomantic-ui-icons.css",
 }
 
-ICON_LIBRARIES_SHOWN = getattr(settings, "DJANGOCMS_FRONTEND_ICONS_LIBRARIES_SHOWN", (
-    "font-awesome",
-    "bootstrap-icons",
-    "material-icons-filled",
-    "material-icons-outlined",
-    "material-icons-round",
-    "material-icons-sharp",
-    "material-icons-two-tone",
-    "fomantic-ui",
-    "foundation-icons",
-    "elegant-icons",
-    "feather-icons",
-    "open-iconic",
-    "tabler-icons",
-    "weather-icons",
-))
+ICON_LIBRARIES_SHOWN = getattr(
+    settings,
+    "DJANGOCMS_FRONTEND_ICONS_LIBRARIES_SHOWN",
+    (
+        "font-awesome",
+        "bootstrap-icons",
+        "material-icons-filled",
+        "material-icons-outlined",
+        "material-icons-round",
+        "material-icons-sharp",
+        "material-icons-two-tone",
+        "fomantic-ui",
+        "foundation-icons",
+        "elegant-icons",
+        "feather-icons",
+        "open-iconic",
+        "tabler-icons",
+        "weather-icons",
+    ),
+)
 
 ICON_LIBRARIES = getattr(
     settings,
     "DJANGOCMS_FRONTEND_ICON_LIBRARIES",
     {
         library: (f"{library}.min.json", ICON_CDN.get(library, f"{library}.css"))
-        for library in getattr(
-            settings,
-            "DJANGOCMS_FRONTEND_ICON_LIBRARIES_SHOWN",
-            ICON_LIBRARIES_SHOWN
-        )
+        for library in getattr(settings, "DJANGOCMS_FRONTEND_ICON_LIBRARIES_SHOWN", ICON_LIBRARIES_SHOWN)
     },
 )
 
 ICON_SIZE_CHOICES = getattr(
     settings,
     "DJANGOCMS_FRONTEND_ICON_SIZE_CHOICES",
     (
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/fields.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
         else:
             context["widget"]["preview"] = json_obj.get("iconHtml", "")
             context["widget"]["library"] = json_obj.get("library", "")
         context["icon_libraries"] = [
             (
                 key,
                 key.title(),
-                static(f'{VENDOR_PATH}/icons-libraries/{value[0]}'),
-                value[1] if "/" in value[1] else static(f'{VENDOR_PATH}/stylesheets/{value[1]}')
+                static(f"{VENDOR_PATH}/icons-libraries/{value[0]}"),
+                value[1] if "/" in value[1] else static(f"{VENDOR_PATH}/stylesheets/{value[1]}"),
             )
             for key, value in ICON_LIBRARIES.items()
         ]
         return context
 
 
 class IconPickerField(JSONField):
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/forms.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/forms.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,17 +32,15 @@
                 "icon",
                 "icon_size",
                 "icon_foreground",
                 "icon_rounded",
                 "attributes",
             ]
         }
-        untangled_fields = (
-            "tag_type",
-        )
+        untangled_fields = ("tag_type",)
 
     icon = IconPickerField()
     icon_size = forms.ChoiceField(
         label=_("Icon size"),
         choices=ICON_SIZE_CHOICES,
         initial=first_choice(ICON_SIZE_CHOICES),
         required=False,
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/migrations/0001_initial.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templatetags/icon_tags.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/icon/templatetags/icon_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,12 +8,10 @@
 
 @register.inclusion_tag("djangocms_frontend/icon/add_css.html", takes_context=True)
 def add_css_for_icon(context, icon):
     if icon and icon.get("library", "") in ICON_LIBRARIES:
         css_link = ICON_LIBRARIES[icon.get("library")][1]
         if css_link:
             if "/" not in css_link:  # static link?
-                css_link = static(
-                    f"djangocms_frontend/icon/vendor/assets/stylesheets/{css_link}"
-                )
+                css_link = static(f"djangocms_frontend/icon/vendor/assets/stylesheets/{css_link}")
             context["icon_css"] = css_link
     return context
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/cms_plugins.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/cms_plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     form = forms.ImageForm
 
     text_enabled = True
     text_icon = (
         '<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-image" '
         'viewBox="0 0 16 16"><path d="M6.002 5.5a1.5 1.5 0 1 1-3 0 1.5 1.5 0 0 1 3 0"/>'
         '<path d="M2.002 1a2 2 0 0 0-2 2v10a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V3a2 2 0 0 0-2-2zm12 1a1 1 0 0 1 1 '
-        '1v6.5l-3.777-1.947a.5.5 0 0 0-.577.093l-3.71 3.71-2.66-1.772a.5.5 0 0 0-.63.062L1.002 12V3a1 1 0 0 1 '
+        "1v6.5l-3.777-1.947a.5.5 0 0 0-.577.093l-3.71 3.71-2.66-1.772a.5.5 0 0 0-.63.062L1.002 12V3a1 1 0 0 1 "
         '1-1z"/></svg>'
     )
 
     change_form_template = "djangocms_frontend/admin/image.html"
 
     fieldsets = [
         (
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/forms.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,34 +118,28 @@
             "If provided, overrides the embedded image. "
             "Certain options such as cropping are not applicable to external images."
         ),
     )
     lazy_loading = forms.BooleanField(
         label=_("Load lazily"),
         required=False,
-        help_text=_(
-            "Use for images below the fold. This will load images only if user scrolls them into view. "
-        ),
+        help_text=_("Use for images below the fold. This will load images only if user scrolls them into view. "),
     )
 
     width = forms.IntegerField(
         label=_("Width"),
         required=False,
         min_value=1,
-        help_text=_(
-            "The image width as number in pixels. " 'Example: "720" and not "720px".'
-        ),
+        help_text=_("The image width as number in pixels. " 'Example: "720" and not "720px".'),
     )
     height = forms.IntegerField(
         label=_("Height"),
         required=False,
         min_value=1,
-        help_text=_(
-            "The image height as number in pixels. " 'Example: "720" and not "720px".'
-        ),
+        help_text=_("The image height as number in pixels. " 'Example: "720" and not "720px".'),
     )
     alignment = forms.ChoiceField(
         label=_("Alignment"),
         choices=settings.EMPTY_CHOICE + get_alignment(),
         initial=settings.EMPTY_CHOICE[0][0],
         required=False,
         help_text=_("Aligns the image according to the selected option."),
@@ -156,40 +150,34 @@
     )
 
     # cropping models
     # active per default
     use_automatic_scaling = forms.BooleanField(
         label=_("Automatic scaling"),
         required=False,
-        help_text=_(
-            "Uses the placeholder dimensions to automatically calculate the size."
-        ),
+        help_text=_("Uses the placeholder dimensions to automatically calculate the size."),
     )
     # ignores all other cropping options
     # throws validation error if other cropping options are selected
     use_no_cropping = forms.BooleanField(
         label=_("Use original image"),
         required=False,
         help_text=_("Outputs the raw image without cropping."),
     )
     # upscale and crop work together
     # throws validation error if other cropping options are selected
     use_crop = forms.BooleanField(
         label=_("Crop image"),
         required=False,
-        help_text=_(
-            "Crops the image according to the thumbnail settings provided in the template."
-        ),
+        help_text=_("Crops the image according to the thumbnail settings provided in the template."),
     )
     use_upscale = forms.BooleanField(
         label=_("Upscale image"),
         required=False,
-        help_text=_(
-            "Upscales the image to the size of the thumbnail settings in the template."
-        ),
+        help_text=_("Upscales the image to the size of the thumbnail settings in the template."),
     )
     use_responsive_image = forms.ChoiceField(
         label=_("Use responsive image"),
         choices=RESPONSIVE_IMAGE_CHOICES,
         initial=first_choice(RESPONSIVE_IMAGE_CHOICES),
         help_text=_(
             "Uses responsive image technique to choose better image to display based upon screen viewport. "
@@ -199,17 +187,15 @@
     # overrides all other options
     # throws validation error if other cropping options are selected
     thumbnail_options = forms.ModelChoiceField(
         queryset=ThumbnailOption.objects.all(),
         to_field_name="id",
         label=_("Thumbnail options"),
         required=False,
-        help_text=_(
-            "Overrides width, height, and crop; scales up to the provided preset dimensions."
-        ),
+        help_text=_("Overrides width, height, and crop; scales up to the provided preset dimensions."),
     )
     picture_fluid = forms.BooleanField(
         label=_("Responsive"),
         required=False,
         initial=True,
         help_text=_("Adds the .img-fluid class to make the image responsive."),
     )
@@ -248,18 +234,15 @@
                     "Only one option is allowed."
                 )
             )
 
         # you shall only set one image kind
         if not data.get("picture", False) and not data.get("external_picture", False):
             raise forms.ValidationError(
-                _(
-                    "You need to add either an image, "
-                    "or a URL linking to an external image."
-                )
+                _("You need to add either an image, " "or a URL linking to an external image.")
             )
 
         # certain cropping options do not work together, the following
         # list defines the disallowed options used in the ``clean`` method
         invalid_option_pairs = [
             ("use_automatic_scaling", "use_no_cropping"),
             ("use_automatic_scaling", "thumbnail_options"),
@@ -274,16 +257,13 @@
 
         for pair in invalid_option_pairs:
             if data.get(pair[0], False) and data.get(pair[1], False):
                 invalid_option_pair = pair
                 break
 
         if invalid_option_pair:
-            message = _(
-                "Invalid cropping settings. "
-                'You cannot combine "{field_a}" with "{field_b}".'
-            )
+            message = _("Invalid cropping settings. " 'You cannot combine "{field_a}" with "{field_b}".')
             message = message.format(
                 field_a=self.fields[invalid_option_pair[0]].label,
                 field_b=self.fields[invalid_option_pair[0]].label,
             )
             raise forms.ValidationError(message)
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/frameworks/bootstrap5.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,13 +19,11 @@
         if instance.picture_fluid:
             instance.add_classes("img-fluid")
         if instance.picture_rounded:
             instance.add_classes("rounded")
         if instance.picture_thumbnail:
             instance.add_classes("img-thumbnail")
         if instance.parent and instance.parent.plugin_type == "CardPlugin":
-            instance.add_classes(
-                "card-img-top" if is_first_child(instance, instance.parent) else "card-img-bottom"
-            )
+            instance.add_classes("card-img-top" if is_first_child(instance, instance.parent) else "card-img-bottom")
         elif instance.parent and instance.parent.plugin_type == "FigurePlugin":
             instance.add_classes("figure-img")
         return super().render(context, instance, placeholder)
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/image_save.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/image_save.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,31 +5,33 @@
 from djangocms_frontend.contrib.image.models import Image
 from djangocms_frontend.helpers import add_plugin, first_choice
 
 default_template = first_choice(get_templates())
 
 
 def create_image_plugin(filename, file, parent_plugin, **kwargs):
-
     # Set the FilerImageField value.
     from filer.settings import FILER_IMAGE_MODEL
     from filer.utils.loader import load_model
+
     image_class = load_model(FILER_IMAGE_MODEL)
     image_obj = image_class(file=ContentFile(file.read(), name=filename))
     image_obj.save()
 
     img = Image(
         parent=parent_plugin,
         position=parent_plugin.position + 1,
         placeholder=parent_plugin.placeholder,
         language=parent_plugin.language,
         plugin_type=ImagePlugin.__name__,
         ui_item=Image.__class__.__name__,
         config={},
     ).initialize_from_form()
-    img.config.update({
-        "picture": {"pk": image_obj.pk, "model": "filer.image"},
-        "use_no_cropping": True,
-    })
+    img.config.update(
+        {
+            "picture": {"pk": image_obj.pk, "model": "filer.image"},
+            "use_no_cropping": True,
+        }
+    )
     add_plugin(parent_plugin.placeholder, img)
 
     return img
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/migrations/0001_initial.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/models.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,17 +129,15 @@
             height=self.height or 0,
         )
 
         thumbnail_options = {
             "size": picture_options["size"],
             "crop": picture_options["crop"],
             "upscale": picture_options["upscale"],
-            "subject_location": self.rel_image.subject_location
-            if self.rel_image
-            else (),
+            "subject_location": self.rel_image.subject_location if self.rel_image else (),
         }
 
         try:
             thumbnailer = get_thumbnailer(self.rel_image)
             url = thumbnailer.get_thumbnail(thumbnail_options).url
         except ValueError:
             # get_thumbnailer() raises this if it can't establish a `relative_name`.
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/cms_plugins.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/jumbotron/cms_plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,10 +44,8 @@
                     "jumbotron_fluid",
                 )
             },
         ),
     ]
 
     def get_render_template(self, context, instance, placeholder):
-        return get_plugin_template(
-            instance, "jumbotron", "jumbotron", settings.JUMBOTRON_TEMPLATE_CHOICES
-        )
+        return get_plugin_template(instance, "jumbotron", "jumbotron", settings.JUMBOTRON_TEMPLATE_CHOICES)
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/forms.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/jumbotron/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,13 +45,11 @@
         choices=settings.JUMBOTRON_TEMPLATE_CHOICES,
         initial=first_choice(settings.JUMBOTRON_TEMPLATE_CHOICES),
     )
     jumbotron_fluid = forms.BooleanField(
         label=_("Fluid"),
         initial=False,
         required=False,
-        help_text=_(
-            "Makes the jumbotron fill the full width of the container or window."
-        ),
+        help_text=_("Makes the jumbotron fill the full width of the container or window."),
     )
     attributes = AttributesFormField()
     tag_type = TagTypeFormField()
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/cms_plugins.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/cms_plugins.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,40 @@
 from cms.plugin_pool import plugin_pool
 from django.apps import apps
 from django.conf import settings as django_settings
+from django.urls import path
 from django.utils.translation import gettext_lazy as _
 
 from djangocms_frontend.helpers import get_plugin_template, insert_fields
 
 from ... import settings
 from ...cms_plugins import CMSUIPlugin
 from ...common.attributes import AttributesMixin
 from ...common.spacing import SpacingMixin
 from .. import link
-from . import forms, models
+from . import forms, models, views
 from .constants import USE_LINK_ICONS
 
 mixin_factory = settings.get_renderer(link)
 
 
 UILINK_FIELDS = (
     ("name", "link_type"),
-    ("site", "url_grouper")
-    if apps.is_installed("djangocms_url_manager")
-    else ("external_link", "internal_link"),
+    ("site", "url_grouper") if apps.is_installed("djangocms_url_manager") else ("external_link", "internal_link"),
     ("link_context", "link_size"),
     ("link_outline", "link_block"),
     "link_stretched",
 )
 
 UILINK_FIELDSET = [
     (
         None,
         {
             "fields": ("template",)
-            + (
-                UILINK_FIELDS + (("icon_left", "icon_right"),)
-                if USE_LINK_ICONS
-                else UILINK_FIELDS
-            )
+            + (UILINK_FIELDS + (("icon_left", "icon_right"),) if USE_LINK_ICONS else UILINK_FIELDS)
         },
     ),
 ]
 if not apps.is_installed("djangocms_url_manager"):
     UILINK_FIELDSET += [
         (
             _("Link settings"),
@@ -82,42 +77,43 @@
                 self.link_fields,
                 blockname=_("Link settings"),
                 position=self.link_fieldset_position,
             )
         return fieldsets
 
 
-class LinkPlugin(
-    mixin_factory("Link"), AttributesMixin, SpacingMixin, LinkPluginMixin, CMSUIPlugin
-):
+class LinkPlugin(mixin_factory("Link"), AttributesMixin, SpacingMixin, LinkPluginMixin, CMSUIPlugin):
     """
     Components > "Button" Plugin
     https://getbootstrap.com/docs/5.0/components/buttons/
     """
 
     name = _("Link / Button")
     module = _("Frontend")
     model = models.Link
     form = forms.LinkForm
     change_form_template = "djangocms_frontend/admin/link.html"
     text_enabled = True
     text_icon = (
         '<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-link-45deg" '
         'viewBox="0 0 16 16"><path d="M4.715 6.542 3.343 7.914a3 3 0 1 0 4.243 4.243l1.828-1.829A3 3 0 0 0 8.586 '
-        '5.5L8 6.086a1 1 0 0 0-.154.199 2 2 0 0 1 .861 3.337L6.88 11.45a2 2 0 1 1-2.83-2.83l.793-.792a4 4 0 0 '
+        "5.5L8 6.086a1 1 0 0 0-.154.199 2 2 0 0 1 .861 3.337L6.88 11.45a2 2 0 1 1-2.83-2.83l.793-.792a4 4 0 0 "
         '1-.128-1.287z"/><path d="M6.586 4.672A3 3 0 0 0 7.414 9.5l.775-.776a2 2 0 0 1-.896-3.346L9.12 3.55a2 2 0 '
         '1 1 2.83 2.83l-.793.792c.112.42.155.855.128 1.287l1.372-1.372a3 3 0 1 0-4.243-4.243z"/></svg>'
     )
     allow_children = True
 
     fieldsets = UILINK_FIELDSET
 
     def get_render_template(self, context, instance, placeholder):
-        return get_plugin_template(
-            instance, "link", "link", settings.LINK_TEMPLATE_CHOICES
-        )
+        return get_plugin_template(instance, "link", "link", settings.LINK_TEMPLATE_CHOICES)
+
+    def get_plugin_urls(self):
+        return [
+            path("autocomplete/", views.AutocompleteJsonView.as_view(), name="link_link_autocomplete"),
+        ]
 
 
-if "djangocms_frontend.contrib.link" in django_settings.INSTALLED_APPS and 'LinkPlugin' not in plugin_pool.plugins:
+if "djangocms_frontend.contrib.link" in django_settings.INSTALLED_APPS and "LinkPlugin" not in plugin_pool.plugins:
     #  Only register plugin if in INSTALLED_APPS
 
     plugin_pool.register_plugin(LinkPlugin)
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/constants.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/forms.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/forms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import json
 from types import SimpleNamespace
 
+from cms.utils.urlutils import admin_reverse
 from django import apps, forms
 from django.conf import settings as django_settings
 from django.contrib.admin.widgets import SELECT2_TRANSLATIONS, AutocompleteMixin
 from django.contrib.contenttypes.models import ContentType
 from django.contrib.sites.models import Site
 from django.core.exceptions import ObjectDoesNotExist, ValidationError
 from django.db import models
 from django.db.models.fields.related import ManyToOneRel
-from django.urls import reverse
 from django.utils.encoding import force_str
 from django.utils.translation import get_language
 from django.utils.translation import gettext as _
 
 # from djangocms_link.validators import IntranetURLValidator
 from entangled.forms import EntangledModelForm
 from filer.fields.image import AdminFileFormField, FilerFileField
@@ -28,15 +28,15 @@
     TagTypeFormField,
     TemplateChoiceMixin,
 )
 from ...helpers import first_choice, get_related_object
 from ...models import FrontendUIItem
 from .. import link
 from .constants import LINK_CHOICES, LINK_SIZE_CHOICES, TARGET_CHOICES
-from .helpers import ensure_select2_url_is_available, get_choices, get_object_for_value
+from .helpers import get_choices, get_object_for_value
 
 mixin_factory = settings.get_forms(link)
 
 if "djangocms_frontend.contrib.icon" in django_settings.INSTALLED_APPS:
     # Weak dependency on djangocms_frontend.contrib.icon
     from djangocms_frontend.contrib.icon.fields import IconPickerField
 elif "djangocms_icon" in django_settings.INSTALLED_APPS:  # pragma: no cover
@@ -50,41 +50,37 @@
         def __init__(self, *args, **kwargs):
             kwargs["widget"] = forms.HiddenInput
             super().__init__(*args, **kwargs)
 
 
 HOSTNAME = getattr(settings, "DJANGOCMS_LINK_INTRANET_HOSTNAME_PATTERN", None)
 LINK_MODELS = getattr(django_settings, "DJANGOCMS_FRONTEND_LINK_MODELS", [])
-MINIMUM_INPUT_LENGTH = getattr(
-    django_settings, "DJANGOCMS_FRONTEND_MINIMUM_INPUT_LENGTH", 0
-)
+MINIMUM_INPUT_LENGTH = getattr(django_settings, "DJANGOCMS_FRONTEND_MINIMUM_INPUT_LENGTH", 0)
 
 
 class Select2jqWidget(AutocompleteMixin, forms.Select):
     empty_label = _("Select a destination")
 
     def __init__(self, *args, **kwargs):
         if MINIMUM_INPUT_LENGTH:
             if "attrs" in kwargs:
-                kwargs["attrs"].setdefault(
-                    "data-minimum-input-length", MINIMUM_INPUT_LENGTH
-                )
+                kwargs["attrs"].setdefault("data-minimum-input-length", MINIMUM_INPUT_LENGTH)
             else:
                 kwargs["attrs"] = {"data-minimum-input-length": MINIMUM_INPUT_LENGTH}
         kwargs.setdefault("admin_site", None)
         kwargs.setdefault(
             "field",
-            SimpleNamespace(name="", model=SimpleNamespace(
-                _meta=SimpleNamespace(app="djangocms_frontend", label="link")
-            ))
+            SimpleNamespace(
+                name="", model=SimpleNamespace(_meta=SimpleNamespace(app="djangocms_frontend", label="link"))
+            ),
         )  # Fake field properties for autocomplete field (unused by link)
         super().__init__(*args, **kwargs)
 
     def get_url(self):
-        return reverse("dcf_autocomplete:ac_view")
+        return admin_reverse("link_link_autocomplete")
 
     def build_attrs(self, base_attrs, extra_attrs=None):
         """
         Set select2's AJAX attributes.
 
         Attributes can be set using the html5 data attribute.
         Nested attributes require a double dash as per
@@ -102,36 +98,35 @@
                 "data-theme": "admin-autocomplete",
                 "data-app-label": "app",
                 "data-model-name": "model",
                 "data-field-name": "field",
                 "data-allow-clear": json.dumps(not self.is_required),
                 "data-placeholder": "",  # Allows clearing of the input.
                 "lang": i18n_name,
-                "class": attrs["class"]
-                + (" " if attrs["class"] else "")
-                + "admin-autocomplete",
+                "class": attrs["class"] + (" " if attrs["class"] else "") + "admin-autocomplete",
             }
         )
         return attrs
 
     def optgroups(self, name, value, attr=None):
-        return super(forms.Select, self).optgroups(name, value)
+        groups = super(forms.Select, self).optgroups(name, value)
+        if not self.is_required:
+            groups[0][1].insert(0, self.create_option(name, "", "", False, 0))
+        return groups
 
 
 class SmartLinkField(forms.ChoiceField):
     widget = Select2jqWidget
 
     def prepare_value(self, value):
         if value:
             if isinstance(value, dict):  # Entangled dictionary?
                 try:
                     app_label, model = value["model"].rsplit(".", 1)
-                    content_type = ContentType.objects.get(
-                        app_label=app_label, model=model
-                    )
+                    content_type = ContentType.objects.get(app_label=app_label, model=model)
                     return f"{content_type.id}-{value['pk']}"
                 except (TypeError, ValueError, KeyError, ObjectDoesNotExist):
                     pass
             elif isinstance(value, models.Model):
                 content_type = ContentType.objects.get_for_model(value)
                 return f"{content_type.id}-{value.id}"
         return ""
@@ -158,25 +153,21 @@
                     "url_grouper",
                 ]
             }
 
         site = forms.ModelChoiceField(
             label=_("Site"),
             queryset=Site.objects.all(),
-            widget=HtmlLinkSiteSelectWidget(
-                attrs={"data-placeholder": _("Select site")}
-            ),
+            widget=HtmlLinkSiteSelectWidget(attrs={"data-placeholder": _("Select site")}),
             required=False,
         )
         url_grouper = forms.ModelChoiceField(
             label=_("Url"),
             queryset=UrlGrouper.objects.all(),
-            widget=HtmlLinkUrlSelectWidget(
-                attrs={"data-placeholder": _("Select URL object from list")}
-            ),
+            widget=HtmlLinkUrlSelectWidget(attrs={"data-placeholder": _("Select URL object from list")}),
             required=False,
         )
 
 else:
 
     class AbstractLinkForm(EntangledModelForm):
         class Meta:
@@ -239,15 +230,14 @@
             label=_("Target"),
             choices=settings.EMPTY_CHOICE + TARGET_CHOICES,
             required=False,
         )
 
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
-            ensure_select2_url_is_available()
             self.fields["internal_link"].choices = self.get_choices
 
         def get_choices(self):
             if MINIMUM_INPUT_LENGTH == 0:
                 return get_choices(self.request)
             if not self.is_bound:  # find initial value
                 int_link_field = self.fields["internal_link"]
@@ -271,23 +261,17 @@
             anchor_field_name = "anchor"
             field_names_allowed_with_anchor = (
                 "external_link",
                 "internal_link",
             )
             anchor_field_verbose_name = force_str(self.fields[anchor_field_name].label)
             anchor_field_value = self.cleaned_data.get(anchor_field_name, None)
-            link_fields = {
-                key: self.cleaned_data.get(key, None) for key in link_field_names
-            }
-            link_field_verbose_names = {
-                key: force_str(self.fields[key].label) for key in link_fields.keys()
-            }
-            provided_link_fields = {
-                key: value for key, value in link_fields.items() if value
-            }
+            link_fields = {key: self.cleaned_data.get(key, None) for key in link_field_names}
+            link_field_verbose_names = {key: force_str(self.fields[key].label) for key in link_fields.keys()}
+            provided_link_fields = {key: value for key, value in link_fields.items() if value}
 
             if len(provided_link_fields) > 1:
                 # Too many fields have a value.
                 verbose_names = sorted(link_field_verbose_names.values())
                 error_msg = _("Only one of {0} or {1} may be given.").format(
                     ", ".join(verbose_names[:-1]),
                     verbose_names[-1],
@@ -301,31 +285,27 @@
                 and not self.link_is_optional
             ):
                 raise ValidationError(_("Please provide a link."))
 
             if anchor_field_value:
                 for field_name in provided_link_fields.keys():
                     if field_name not in field_names_allowed_with_anchor:
-                        error_msg = _(
-                            "%(anchor_field_verbose_name)s is not allowed together with %(field_name)s"
-                        ) % {
+                        error_msg = _("%(anchor_field_verbose_name)s is not allowed together with %(field_name)s") % {
                             "anchor_field_verbose_name": anchor_field_verbose_name,
                             "field_name": link_field_verbose_names.get(field_name),
                         }
                         raise ValidationError(
                             {
                                 anchor_field_name: error_msg,
                                 field_name: error_msg,
                             }
                         )
 
 
-class LinkForm(
-    mixin_factory("Link"), SpacingFormMixin, TemplateChoiceMixin, AbstractLinkForm
-):
+class LinkForm(mixin_factory("Link"), SpacingFormMixin, TemplateChoiceMixin, AbstractLinkForm):
     class Meta:
         model = FrontendUIItem
         entangled_fields = {
             "config": [
                 "name",
                 "template",
                 "link_type",
@@ -351,17 +331,15 @@
         choices=settings.LINK_TEMPLATE_CHOICES,
         initial=first_choice(settings.LINK_TEMPLATE_CHOICES),
     )
     link_stretched = forms.BooleanField(
         label=_("Stretch link"),
         required=False,
         initial=False,
-        help_text=_(
-            "Stretches the active link area to the containing block (with position: relative)."
-        ),
+        help_text=_("Stretches the active link area to the containing block (with position: relative)."),
     )
     link_type = forms.ChoiceField(
         label=_("Type"),
         choices=LINK_CHOICES,
         initial=first_choice(LINK_CHOICES),
         widget=forms.RadioSelect(attrs={"class": "inline-block"}),
         help_text=_("Adds either a text link or a button which links to the target."),
@@ -374,17 +352,15 @@
         widget=ColoredButtonGroup(),
     )
     link_size = forms.ChoiceField(
         label=_("Button size"),
         choices=LINK_SIZE_CHOICES,
         initial=LINK_SIZE_CHOICES[1][0],  # Medium
         required=False,
-        widget=ButtonGroup(
-            attrs=dict(property="link-size", label_class="btn-secondary")
-        ),
+        widget=ButtonGroup(attrs=dict(property="link-size", label_class="btn-secondary")),
     )
     link_outline = forms.BooleanField(
         label=_("Outline"),
         initial=False,
         required=False,
         help_text=_("Removes the coloring from a button and keeps the outline."),
     )
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/helpers.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 
 from cms.forms.utils import get_page_choices
 from cms.models import Page
 from django.conf import settings as django_settings
 from django.contrib.admin import site
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import FieldError, ObjectDoesNotExist
-from django.urls import NoReverseMatch, reverse
 from django.utils.encoding import force_str
 from django.utils.html import mark_safe
 
+from djangocms_frontend.settings import EMPTY_CHOICE
+
 LINK_MODELS = getattr(django_settings, "DJANGOCMS_FRONTEND_LINK_MODELS", [])
 
 
 def create_querysets(link_models):
     querysets = []
     for item in link_models:
         if item["class_path"] != "cms.models.Page":
@@ -62,15 +63,15 @@
 
 
 def get_link_choices(request, term="", lang=None, nbsp=None):
     global _querysets
 
     if nbsp is None:
         nbsp = "" if term else "\u2000"
-    available_objects = []
+    available_objects = [dict(id=EMPTY_CHOICE[0][0], text=EMPTY_CHOICE[0][1])]
     # Now create our list of cms pages
     type_id = ContentType.objects.get_for_model(Page).id
     for value, descr in get_page_choices(lang):
         if isinstance(descr, list):
             available_objects.append(
                 {
                     "text": value,
@@ -93,59 +94,31 @@
         model_admin = site._registry.get(cls, None)
         if search:
             try:
                 objects = qs.filter(**{search + "__icontains": term})
             except FieldError:
                 pass
         if objects is None:
-            objects = [
-                item
-                for item in qs.all()
-                if (not isinstance(term, str)) or term.upper() in str(item).upper()
-            ]
+            objects = [item for item in qs.all() if (not isinstance(term, str)) or term.upper() in str(item).upper()]
         if objects:
             type_class = ContentType.objects.get_for_model(objects[0].__class__)
             available_objects.append(
                 {
                     "text": force_str(section),
                     "children": [
                         dict(id=f"{type_class.id}-{obj.id}", text=str(obj))
                         for obj in objects
-                        if request is None
-                        or model_admin
-                        and model_admin.has_view_permission(request, obj=obj)
+                        if request is None or model_admin and model_admin.has_view_permission(request, obj=obj)
                     ],
                 }
             )
     return available_objects
 
 
 def get_choices(request, term="", lang=None) -> list:
     def to_choices(json):
         return list(
-            (elem["text"], to_choices(elem["children"]))
-            if "children" in elem
-            else (elem["id"], elem["text"])
+            (elem["text"], to_choices(elem["children"])) if "children" in elem else (elem["id"], elem["text"])
             for elem in json
         )
 
     return to_choices(get_link_choices(request, term, lang, "&nbsp;"))
-
-
-def ensure_select2_url_is_available() -> None:
-    """Install the URLs"""
-    try:
-        reverse("dcf_autocomplete:ac_view")
-    except NoReverseMatch:  # Not installed yet
-        urlconf_module = import_module(django_settings.ROOT_URLCONF)
-        from django.urls import clear_url_caches, include, path
-
-        urlconf_module.urlpatterns = [
-            path(
-                "@dcf-links/",
-                include(
-                    "djangocms_frontend.contrib.link.urls",
-                    namespace="dcf_autocomplete",
-                ),
-            )
-        ] + urlconf_module.urlpatterns
-        clear_url_caches()
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/migrations/0001_initial.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/models.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,17 +91,15 @@
 
         elif getattr(self, "mailto", None):
             link = f"mailto:{self.mailto}"
 
         else:
             link = ""
 
-        if (
-            not getattr(self, "phone", None) and not getattr(self, "mailto", None)
-        ) and getattr(self, "anchor", None):
+        if (not getattr(self, "phone", None) and not getattr(self, "mailto", None)) and getattr(self, "anchor", None):
             link += f"#{self.anchor}"
 
         return link
 
 
 class Link(GetLinkMixin, FrontendUIItem):
     """
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/link.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/link.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/views.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/link/views.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/cms_plugins.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/listgroup/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/forms.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/listgroup/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,17 +59,15 @@
             ]
         }
         untangled_fields = ("tag_type",)
 
     simple_content = forms.CharField(
         label=_("One line content"),
         required=False,
-        help_text=_(
-            "List item text. Is only show if this list item has no child plugins."
-        ),
+        help_text=_("List item text. Is only show if this list item has no child plugins."),
     )
     list_context = forms.ChoiceField(
         label=_("Context"),
         choices=settings.EMPTY_CHOICE + settings.COLOR_STYLE_CHOICES,
         initial=settings.EMPTY_CHOICE[0][0],
         required=False,
         widget=ColoredButtonGroup(),
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/models.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/listgroup/models.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/cms_plugins.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/media/cms_plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 from .. import media
 from . import forms, models
 
 mixin_factory = settings.get_renderer(media)
 
 
 @plugin_pool.register_plugin
-class MediaPlugin(
-    mixin_factory("Media"), AttributesMixin, ResponsiveMixin, CMSUIPlugin
-):
+class MediaPlugin(mixin_factory("Media"), AttributesMixin, ResponsiveMixin, CMSUIPlugin):
     """
     Layout > "Media" Plugin
     http://getbootstrap.com/docs/4.0/layout/media-object/
     """
 
     name = _("Media")
     module = _("Frontend")
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/forms.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/media/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/migrations/0001_initial.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/media/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/models.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/media/models.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/cms_plugins.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/cms_plugins.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,17 +51,15 @@
                     "navbar_container",
                 )
             },
         ),
     ]
 
     def get_render_template(self, context, instance, placeholder):
-        return get_plugin_template(
-            instance, "navigation", "navigation", settings.NAVIGATION_TEMPLATE_CHOICES
-        )
+        return get_plugin_template(instance, "navigation", "navigation", settings.NAVIGATION_TEMPLATE_CHOICES)
 
     def render(self, context, instance, placeholder):
         context["nav_template"] = instance.config.get("template", default_template)
         return super().render(context, instance, placeholder)
 
 
 @plugin_pool.register_plugin
@@ -71,32 +69,33 @@
     CMSUIPlugin,
 ):
     """
 
     The PageTreePlugin class is a plugin for Django CMS that allows users to display a hierarchical
     tree-like structure of pages on the frontend.
     """
+
     name = _("Page tree")
     module = _("Frontend")
     model = models.PageTree
     form = forms.PageTreeForm
     change_form_template = "djangocms_frontend/admin/page_tree.html"
     allow_children = False
-    parent_classes = ["NavigationPlugin",]
+    parent_classes = [
+        "NavigationPlugin",
+    ]
     fieldsets = [
         (
             None,
             {"fields": ("start_level",)},
         ),
     ]
 
     def get_render_template(self, context, instance, placeholder):
-        return get_template_path(
-            "navigation", context.get("nav_template", default_template), "page_tree"
-        )
+        return get_template_path("navigation", context.get("nav_template", default_template), "page_tree")
 
     def render(self, context, instance, placeholder):
         context["start_level"] = instance.config.get("start_level", 0)
         return super().render(context, instance, placeholder)
 
 
 @plugin_pool.register_plugin
@@ -107,45 +106,47 @@
     CMSUIPlugin,
 ):
     """
     The `NavBrandPlugin` class is a plugin used in Django CMS to create a navigation brand element.
     This plugin allows the user to define a brand logo or text that will be displayed in the
     navigation header. Content is added through child plugins.
     """
+
     name = _("Brand")
     module = _("Frontend")
     model = models.NavBrand
     form = forms.NavBrandForm
     change_form_template = "djangocms_frontend/admin/brand.html"
     allow_children = True
-    parent_classes = ["NavigationPlugin",]
+    parent_classes = [
+        "NavigationPlugin",
+    ]
     link_fieldset_position = -1
 
     fieldsets = [
         (
             None,
             {"fields": ("simple_content",)},
         ),
     ]
 
     def get_render_template(self, context, instance, placeholder):
-        return get_template_path(
-            "navigation", context.get("nav_template", default_template), "brand"
-        )
+        return get_template_path("navigation", context.get("nav_template", default_template), "brand")
 
 
 @plugin_pool.register_plugin
 class NavContainerPlugin(
     mixin_factory("NavLink"),
     AttributesMixin,
     CMSUIPlugin,
 ):
     """
     The `NavContainerPlugin` class is a deprecated plugin without functionality. It will be removed.
     """
+
     name = _("Navigation container")
     module = _("Frontend")
     model = models.NavContainer
     change_form_template = "djangocms_frontend/admin/deprecated.html"
     allow_children = True
     parent_classes = [""]  # No parent classes
     child_classes = [
@@ -177,14 +178,15 @@
     - `model` (Model): The Django model used to store the plugin's data.
     - `form` (Form): The form used to render the plugin's settings in the admin interface.
     - `change_form_template` (str): The path to the template used to render the plugin's change form in the admin interface.
     - `allow_children` (bool): Whether the plugin allows having child plugins.
     - `parent_classes` (list): List of parent plugin classes that this plugin can be nested within.
     - `child_classes` (list): List of child plugin classes that can be nested within this plugin.
     """
+
     name = _("Navigation link")
     module = _("Frontend")
     model = models.NavLink
     form = forms.NavLinkForm
     change_form_template = "djangocms_frontend/admin/navlink.html"
     allow_children = True
     parent_classes = ["NavigationPlugin", "NavLinkPlugin"]
@@ -192,10 +194,8 @@
         "NavLinkPlugin",
         "GridContainerPlugin",
         "GridRowPlugin",
         "ListGroupPlugin",
     ]
 
     def get_render_template(self, context, instance, placeholder):
-        return get_template_path(
-            "navigation", context.get("nav_template", default_template), "link"
-        )
+        return get_template_path("navigation", context.get("nav_template", default_template), "link")
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/forms.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,17 +76,15 @@
             ]
         }
         untangled_fields = ()
 
     start_level = forms.IntegerField(
         label=_("Start level"),
         initial=0,
-        help_text=_(
-            "Start level of this page tree (0: root, 1: level below root, etc.)"
-        ),
+        help_text=_("Start level of this page tree (0: root, 1: level below root, etc.)"),
     )
     attributes = AttributesFormField()
 
 
 class NavBrandForm(mixin_factory("NavBrand"), AbstractLinkForm, EntangledModelForm):
     class Meta:
         model = FrontendUIItem
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/migrations/0001_initial.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/models.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/models.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/cms_plugins.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/cms_plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,15 @@
     ]
 
     def get_render_template(self, context, instance, placeholder):
         return get_plugin_template(instance, "tabs", "tabs", TAB_TEMPLATE_CHOICES)
 
 
 @plugin_pool.register_plugin
-class TabItemPlugin(
-    mixin_factory("TabItem"), AttributesMixin, PaddingMixin, CMSUIPlugin
-):
+class TabItemPlugin(mixin_factory("TabItem"), AttributesMixin, PaddingMixin, CMSUIPlugin):
     """
     Components > "Navs - Tab Item" Plugin
     https://getbootstrap.com/docs/5.0/components/navs/
     """
 
     name = _("Tab item")
     module = _("Frontend")
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/constants.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/forms.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/migrations/0001_initial.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/models.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/models.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/cms_plugins.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/cms_plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,17 +49,15 @@
     name = _("Editor note")
     module = _("Frontend")
     allow_children = True
     change_form_template = "djangocms_frontend/admin/no_form.html"
 
 
 @plugin_pool.register_plugin
-class HeadingPlugin(
-    mixin_factory("Heading"), AttributesMixin, SpacingMixin, CMSUIPlugin
-):
+class HeadingPlugin(mixin_factory("Heading"), AttributesMixin, SpacingMixin, CMSUIPlugin):
     """Room for notes for editor only visible in edit mode"""
 
     name = _("Heading")
     module = _("Frontend")
     model = models.Heading
     form = forms.HeadingForm
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/forms.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,23 +60,19 @@
         widget=IconGroup(),
     )
     attributes = AttributesFormField()
     tag_type = TagTypeFormField()
 
     def clean(self):
         super().clean()
-        if (
-            self.cleaned_data["space_property"] == "p"
-            and self.cleaned_data["space_size"] == "auto"
-        ):
+        if self.cleaned_data["space_property"] == "p" and self.cleaned_data["space_size"] == "auto":
             raise ValidationError(
                 {
                     "space_property": _(
-                        "Padding does not have an auto spacing. Either "
-                        "switch to margin or a defined size."
+                        "Padding does not have an auto spacing. Either " "switch to margin or a defined size."
                     ),
                     "space_size": _(
                         "Padding does not have an auto spacing. Either "
                         "switch to a defined size or change the spacing property."
                     ),
                 }
             )
@@ -120,17 +116,15 @@
         label=_("Heading"),
         required=True,
     )
 
     heading_id = forms.CharField(
         label=_("ID"),
         required=False,
-        help_text=_(
-            "Fill in unique ID for table of contents. If empty heading will not appear in table of contents."
-        ),
+        help_text=_("Fill in unique ID for table of contents. If empty heading will not appear in table of contents."),
     )
     heading_context = forms.ChoiceField(
         label=_("Heading context"),
         required=False,
         choices=settings.EMPTY_CHOICE + settings.COLOR_STYLE_CHOICES,
         initial=settings.EMPTY_CHOICE,
         widget=ColoredButtonGroup(),
@@ -154,24 +148,18 @@
                 "attributes",
             ],
         }
         untangled_fields = ()
 
     list_attributes = AttributesFormField(
         label=_("List attributes"),
-        help_text=_(
-            "Attributes apply to the <b>list</b> for each level in the table of contents."
-        ),
+        help_text=_("Attributes apply to the <b>list</b> for each level in the table of contents."),
     )
 
     link_attributes = AttributesFormField(
         label=_("Link attributes"),
-        help_text=_(
-            "Attributes apply to the <b>link</b> for each entry in the table of contents."
-        ),
+        help_text=_("Attributes apply to the <b>link</b> for each entry in the table of contents."),
     )
     attributes = AttributesFormField(
         label=_("Item attributes"),
-        help_text=_(
-            "Attributes apply to the <b>list items</b> for each entry in the table of contents."
-        ),
+        help_text=_("Attributes apply to the <b>list items</b> for each entry in the table of contents."),
     )
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 class SpacingRenderMixin:
     def render(self, context, instance, placeholder):
         if not instance.space_device or instance.space_device == "xs":
-            instance.add_classes(
-                f"{instance.space_property}{instance.space_sides}-{instance.space_size}"
-            )
+            instance.add_classes(f"{instance.space_property}{instance.space_sides}-{instance.space_size}")
         else:
             instance.add_classes(
-                f"{instance.space_property}{instance.space_sides}-{ instance.space_device }-{instance.space_size}"
+                f"{instance.space_property}{instance.space_sides}-{instance.space_device}-{instance.space_size}"
             )
         return super().render(context, instance, placeholder)
 
 
 class EditorNoteRenderMixin:
     render_template = "djangocms_frontend/bootstrap5/editor_note.html"
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/migrations/0001_initial.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/models.py` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/models.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html` & `djangocms_frontend-1.3.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/fields.py` & `djangocms_frontend-1.3.2/djangocms_frontend/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,32 +14,28 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if "template" in self.fields:
             template_field = self.fields["template"]
             choices = template_field.choices
             instance = kwargs.get("instance", None)
-            if len(choices) == 1 and (
-                instance is None or instance.config.get("template", "") == choices[0][0]
-            ):
+            if len(choices) == 1 and (instance is None or instance.config.get("template", "") == choices[0][0]):
                 template_field.widget = forms.HiddenInput()
 
 
 class ButtonGroup(forms.RadioSelect):
     template_name = "djangocms_frontend/admin/widgets/button_group.html"
     option_template_name = "djangocms_frontend/admin/widgets/button_group_option.html"
 
     class Media:
         css = {"all": ("djangocms_frontend/css/button_group.css",)}
 
 
 class ColoredButtonGroup(ButtonGroup):  # lgtm [py/missing-call-to-init]
-    option_template_name = (
-        "djangocms_frontend/admin/widgets/button_group_color_option.html"
-    )
+    option_template_name = "djangocms_frontend/admin/widgets/button_group_color_option.html"
 
     class Media:
         css = settings.ADMIN_CSS
 
     def __init__(self, *args, **kwargs):
         kwargs.update({"attrs": {**kwargs.get("attrs", {}), **dict(property="color")}})
         super().__init__(*args, **kwargs)
@@ -61,17 +57,15 @@
         css = {"all": ("djangocms_frontend/css/button_group.css",)}
 
     def __init__(self, *args, **kwargs):
         kwargs.update({"attrs": {**kwargs.get("attrs", {}), **dict(property="icon")}})
         super().__init__(*args, **kwargs)
 
 
-class OptionalDeviceChoiceField(
-    forms.MultipleChoiceField
-):  # lgtm [py/missing-call-to-init]
+class OptionalDeviceChoiceField(forms.MultipleChoiceField):  # lgtm [py/missing-call-to-init]
     def __init__(self, **kwargs):
         kwargs.setdefault("choices", settings.DEVICE_CHOICES)
         kwargs.setdefault("initial", None)
         kwargs.setdefault("widget", IconMultiselect())
         super().__init__(**kwargs)
 
     def prepare_value(self, value):
@@ -86,17 +80,15 @@
         return value
 
 
 class DeviceChoiceField(OptionalDeviceChoiceField):
     def clean(self, value):
         value = super().clean(value)
         if isinstance(value, list) and len(value) == 0:
-            raise ValidationError(
-                _("Please select at least one device size"), code="invalid"
-            )
+            raise ValidationError(_("Please select at least one device size"), code="invalid")
         return value
 
 
 class AttributesField(fields.AttributesField):
     def __init__(self, *args, **kwargs):
         if "verbose_name" not in kwargs:
             kwargs["verbose_name"] = _("Attributes")
@@ -111,17 +103,15 @@
         kwargs.setdefault("required", False)
         kwargs.setdefault("widget", fields.AttributesWidget)
         self.excluded_keys = kwargs.pop("excluded_keys", [])
         super().__init__(*args, **kwargs)
 
 
 try:
-    fields.AttributesWidget(
-        sorted=True
-    )  # does djangocms-attributes-field support sorted param?
+    fields.AttributesWidget(sorted=True)  # does djangocms-attributes-field support sorted param?
     CHOICESWIDGETPARAMS = dict(sorted=False)  # use unsorted variant
 except TypeError:
     CHOICESWIDGETPARAMS = dict()  # Fallback for djangocms-attributes-field < 2.1
 
 
 class ChoicesFormField(fields.AttributesFormField):
     """Simple choices field based on attributes field. Needs to be extended to
@@ -133,19 +123,15 @@
         kwargs.setdefault("widget", fields.AttributesWidget(**CHOICESWIDGETPARAMS))
         self.excluded_keys = kwargs.pop("excluded_keys", [])
         super().__init__(*args, **kwargs)
 
     def clean(self, value):
         if not value:
             raise ValidationError(
-                mark_safe(
-                    _(
-                        "Please enter at least one choice. Use the <code>+</code> symbol to add a choice."
-                    )
-                ),
+                mark_safe(_("Please enter at least one choice. Use the <code>+</code> symbol to add a choice.")),
                 code="empty",
             )
         return [(key, value) for key, value in value.items()]
 
     def prepare_value(self, value):
         if not value:
             return {}
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.2/djangocms_frontend/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/helpers.py` & `djangocms_frontend-1.3.2/djangocms_frontend/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,17 +21,15 @@
         Model = apps.get_model(scope[field_name]["model"])
         relobj = Model.objects.get(pk=scope[field_name]["pk"])
     except (ObjectDoesNotExist, LookupError):
         relobj = None
     return relobj
 
 
-def insert_fields(
-    fieldsets, new_fields, block=None, position=-1, blockname=None, blockattrs=None
-):
+def insert_fields(fieldsets, new_fields, block=None, position=-1, blockname=None, blockattrs=None):
     """
     creates a copy of fieldsets inserting the new fields either in the indexed block at the position,
     or - if no block is given - at the end
     """
     if blockattrs is None:
         blockattrs = dict()
     if block is None:
@@ -49,17 +47,15 @@
             ]
             + list(fieldsets[position:] if position != -1 else [])
         )
         return fs
     modify = copy.deepcopy(fieldsets[block])
     fields = modify[1]["fields"]
     if position >= 0:
-        modify[1]["fields"] = (
-            list(fields[:position]) + list(new_fields) + list(fields[position:])
-        )
+        modify[1]["fields"] = list(fields[:position]) + list(new_fields) + list(fields[position:])
     else:
         modify[1]["fields"] = (
             list(fields[: position + 1] if position != -1 else fields)
             + list(new_fields)
             + list(fields[position + 1 :] if position != -1 else [])
         )
     fs = (
@@ -104,30 +100,26 @@
 mark_safe_lazy = lazy(mark_safe, str)
 
 
 def link_to_framework_doc(ui_item, topic):
     link = FRAMEWORK_PLUGIN_INFO.get(ui_item, {}).get(topic, None)
     if link:
         return mark_safe_lazy(
-            _(
-                'Read more in the <a href="{link}" target="_blank">documentation</a>.'
-            ).format(link=link)
+            _('Read more in the <a href="{link}" target="_blank">documentation</a>.').format(link=link)
         )
     return None
 
 
 def add_plugin(placeholder, plugin):
     """CMS version-save function to add a plugin to a placeholder"""
     if hasattr(placeholder, "add_plugin"):  # available as of CMS v4
         placeholder.add_plugin(plugin)
     else:  # CMS < v4
         if plugin.parent:
-            plugin.position -= (
-                plugin.parent.position + 1
-            )  # Restart position counting at 0
+            plugin.position -= plugin.parent.position + 1  # Restart position counting at 0
         else:
             plugin.position -= 1  # 0-based counting in v3
         plugin.save()
 
 
 def delete_plugin(plugin):
     """CMS version save function to delete a plugin (and its descendants) from a placeholder"""
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/locale/ar/LC_MESSAGES/django.mo` & `djangocms_frontend-1.3.2/djangocms_frontend/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/locale/ar/LC_MESSAGES/django.po` & `djangocms_frontend-1.3.2/djangocms_frontend/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/locale/de/LC_MESSAGES/django.mo` & `djangocms_frontend-1.3.2/djangocms_frontend/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/locale/de/LC_MESSAGES/django.po` & `djangocms_frontend-1.3.2/djangocms_frontend/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/locale/en/LC_MESSAGES/django.po` & `djangocms_frontend-1.3.2/djangocms_frontend/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/locale/es/LC_MESSAGES/django.mo` & `djangocms_frontend-1.3.2/djangocms_frontend/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/locale/es/LC_MESSAGES/django.po` & `djangocms_frontend-1.3.2/djangocms_frontend/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/locale/fr/LC_MESSAGES/django.mo` & `djangocms_frontend-1.3.2/djangocms_frontend/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/locale/fr/LC_MESSAGES/django.po` & `djangocms_frontend-1.3.2/djangocms_frontend/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/locale/hr/LC_MESSAGES/django.mo` & `djangocms_frontend-1.3.2/djangocms_frontend/locale/hr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/locale/hr/LC_MESSAGES/django.po` & `djangocms_frontend-1.3.2/djangocms_frontend/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/locale/it/LC_MESSAGES/django.po` & `djangocms_frontend-1.3.2/djangocms_frontend/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/locale/nl/LC_MESSAGES/django.mo` & `djangocms_frontend-1.3.2/djangocms_frontend/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/locale/nl/LC_MESSAGES/django.po` & `djangocms_frontend-1.3.2/djangocms_frontend/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo` & `djangocms_frontend-1.3.2/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/locale/sq/LC_MESSAGES/django.po` & `djangocms_frontend-1.3.2/djangocms_frontend/locale/sq/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/management/bootstrap4_migration.py` & `djangocms_frontend-1.3.2/djangocms_frontend/management/bootstrap4_migration.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,32 +360,26 @@
         new_obj.config[field].replace("text-center", "center")
         new_obj.config[field].replace("text-right", "end")
 
 
 def m001_spacing_mixin(obj, new_obj, type):
     classes = new_obj.config["attributes"].get("class", "").split()
     if classes:
-        for size, _ in list(settings.SPACER_SIZE_CHOICES) + (
-            [("auto", "auto")] if type == "margin" else []
-        ):
+        for size, _ in list(settings.SPACER_SIZE_CHOICES) + ([("auto", "auto")] if type == "margin" else []):
             if f"{type[0]}-{size}" in classes:
                 classes.remove(f"{type[0]}-{size}")
                 classes.append(f"{type[0]}x-{size}")
                 classes.append(f"{type[0]}y-{size}")
             for side, _ in settings.SPACER_X_SIDES_CHOICES:
-                if f"{type[0]}{side}-{size}" in classes and not new_obj.config.get(
-                    f"{type}_x", None
-                ):
+                if f"{type[0]}{side}-{size}" in classes and not new_obj.config.get(f"{type}_x", None):
                     new_obj.config[f"{type}_x"] = f"{type[0]}{side}-{size}"
                     new_obj.config[f"{type}_devices"] = None
                     classes.remove(f"{type[0]}{side}-{size}")
             for side, _ in settings.SPACER_Y_SIDES_CHOICES:
-                if f"{type[0]}{side}-{size}" in classes and not new_obj.config.get(
-                    f"{type}_y", None
-                ):
+                if f"{type[0]}{side}-{size}" in classes and not new_obj.config.get(f"{type}_y", None):
                     new_obj.config[f"{type}_y"] = f"{type[0]}{side}-{size}"
                     new_obj.config[f"{type}_devices"] = None
                     classes.remove(f"{type[0]}{side}-{size}")
         if classes:
             new_obj.config["attributes"]["class"] = " ".join(classes)
         else:
             new_obj.config["attributes"].pop("class")
@@ -485,17 +479,15 @@
     if obj.template == "default":
         return
     BS4 = getattr(django_setting, bs4_setting, ())
     DCF = getattr(django_setting, dcf_setting, ())
     if not in_choices(obj.template, BS4):
         print(f"=> Template '{obj.template}' in {obj.plugin_type} (id: {obj.id})")
         print(f"   but not declared in {bs4_setting}")
-        print(
-            "   You will be able to edit the plugin but up saving the template will be changed."
-        )
+        print("   You will be able to edit the plugin but up saving the template will be changed.")
         if not DCF and bs4_setting != dcf_setting:
             print(f"   Remember to put {dcf_setting} in your settings.py")
 
 
 data_migration = {
     "P001": p001_left_right_migration,
     "X002": x002_replace_card_deck,
@@ -505,17 +497,15 @@
     "A001_picture": lambda x, y: a001_alignment(x, y, "alignment"),
     "A001_card": lambda x, y: a001_alignment(x, y, "card_alignment"),
     "G001": g001_col_text_alignment,
     "M001-m": lambda x, y: m001_spacing_mixin(x, y, "margin"),
     "M001-p": lambda x, y: m001_spacing_mixin(x, y, "padding"),
     "M002": m002_responsive_mixin,
     "M003": m003_background_mixin,
-    "T001_PICTURE": lambda x, y: t001_template(
-        x, y, "DJANGOCMS_PICTURE_TEMPLATES", "DJANGOCMS_PICTURE_TEMPLATES"
-    ),
+    "T001_PICTURE": lambda x, y: t001_template(x, y, "DJANGOCMS_PICTURE_TEMPLATES", "DJANGOCMS_PICTURE_TEMPLATES"),
     "T001_LINK": lambda x, y: t001_template(
         x, y, "DJANGOCMS_LINK_TEMPLATES", "DJANGOCMS_FRONTEND_LINK_TEMPLATE_CHOICES"
     ),
     "T001_TABS": lambda x, y: t001_template(
         x, y, "DJANGOCMS_BOOTSTRAP4_TAB_TEMPLATES", "DJANGOCMS_FRONTEND_TAB_TEMPLATES"
     ),
     "T001_CAROUSEL": lambda x, y: t001_template(
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/management/commands/frontend.py` & `djangocms_frontend-1.3.2/djangocms_frontend/management/commands/frontend.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/base.py` & `djangocms_frontend-1.3.2/djangocms_frontend/management/commands/subcommands/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,15 @@
             "DJANGO_SETTINGS_MODULE environment variable will be used."
         ),
     )
     parser.add_argument(
         "--pythonpath",
         help='A directory to add to the Python path, e.g. "/home/djangoprojects/myproject".',
     )
-    parser.add_argument(
-        "--traceback", action="store_true", help="Raise on CommandError exceptions"
-    )
+    parser.add_argument("--traceback", action="store_true", help="Raise on CommandError exceptions")
     parser.add_argument(
         "--no-color",
         action="store_true",
         dest="no_color",
         default=False,
         help="Don't colorize the command output.",
     )
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/frequency_analysis.py` & `djangocms_frontend-1.3.2/djangocms_frontend/management/commands/subcommands/frequency_analysis.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,10 @@
 
 
 class FrequencyAnalysis(SubcommandsCommand):
     help = "Migrates plugins djangocms_bootstrap4 to djangocms_frontend"
     command_name = "frequency_analysis"
 
     def handle(self, *args, **options):
-        analysis = (
-            FrontendUIItem.objects.values("ui_item")
-            .annotate(count=Count("ui_item"))
-            .order_by("-count")
-        )
+        analysis = FrontendUIItem.objects.values("ui_item").annotate(count=Count("ui_item")).order_by("-count")
         for element in analysis:
             self.stdout.write(f"{element['ui_item']:20}\t{element['count']:6}")
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/migrate.py` & `djangocms_frontend-1.3.2/djangocms_frontend/management/commands/subcommands/migrate.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,17 +32,15 @@
 if "djangocms_icon" in apps.all_models:
     from djangocms_frontend.management import icon_migration
 
     plugin_migrations.update(icon_migration.plugin_migration)
     data_migration.update(icon_migration.data_migration)
     plugin_prefixes.append(icon_migration.plugin_prefix)
 
-additional_migrations = getattr(
-    settings, "DJANGOCMS_FRONTEND_ADDITIONAL_MIGRATIONS", None
-)
+additional_migrations = getattr(settings, "DJANGOCMS_FRONTEND_ADDITIONAL_MIGRATIONS", None)
 if additional_migrations:
     if isinstance(additional_migrations, str):
         additional_migrations = [additional_migrations]
 
     for migration_module_path in additional_migrations:
         try:
             migration_module = importlib.import_module(migration_module_path)
@@ -74,49 +72,39 @@
                 new_obj.position = obj.position
                 new_obj.language = obj.language
                 new_obj.creation_date = obj.creation_date
                 if hasattr(obj, "depth"):  # cms v3
                     new_obj.depth = obj.depth
                     new_obj.numchild = obj.numchild
                     new_obj.path = obj.path
-                new_obj.plugin_type = (
-                    plugin_names[new_model]
-                    if new_model in plugin_names
-                    else new_model + "Plugin"
-                )
+                new_obj.plugin_type = plugin_names[new_model] if new_model in plugin_names else new_model + "Plugin"
                 # Add something like `new_obj.field_name = obj.field_name` for any field in the the new plugin
                 for field in fields:
                     if field in data_migration:
                         data_migration[field](obj, new_obj)
                     else:
                         if " -> " in field:
                             old_field, new_field = field.split(" -> ")
                         else:
                             old_field, new_field = field, field
-                        value = (
-                            old_field[1:-1]
-                            if old_field[0] == "("
-                            else getattr(obj, old_field)
-                        )
+                        value = old_field[1:-1] if old_field[0] == "(" else getattr(obj, old_field)
                         if value == "":
                             value = None
                         if new_field in new_obj_fields:
                             setattr(new_obj, new_field, value)
                         else:
                             if isinstance(value, models.Model):  # related field
                                 value = {
                                     "model": "{}.{}".format(
                                         value._meta.app_label,
                                         value._meta.model_name,
                                     ),
                                     "pk": value.pk,
                                 }
-                            elif isinstance(
-                                value, models.QuerySet
-                            ):  # related many field
+                            elif isinstance(value, models.QuerySet):  # related many field
                                 value = {
                                     "model": "{}.{}".format(
                                         value.model._meta.app_label,
                                         value.model._meta.model_name,
                                     ),
                                     "p_keys": list(value.values_list("pk", flat=True)),
                                 }
@@ -175,16 +163,15 @@
     command_name = "migrate"
 
     def handle(self, *args, **options):
         tables = connection.introspection.table_names()
         if "djangocms_frontend_frontenduiitem" not in tables:
             self.stdout.write(
                 self.style.ERROR(
-                    "I cannot find djangocms-frontend's tables in the database. Did you run\n"
-                    "./manage.py migrate ?"
+                    "I cannot find djangocms-frontend's tables in the database. Did you run\n" "./manage.py migrate ?"
                 )
             )
             return
 
         self.migrate_to_djangocms_frontend()
         if getattr(settings, "DJANGOCMS_FRONTEND_LINK_MODELS", None) is None:
             self.check_for_link_targets()
@@ -196,53 +183,39 @@
         self.stdout.write(self.style.SUCCESS("================="))
         changes = migrate_to_djangocms_frontend(apps, None)
         not_migrated = []
         for plugin in CMSPlugin.objects.all():
             if any([prefix in plugin.plugin_type for prefix in plugin_prefixes]):
                 if plugin.plugin_type not in not_migrated:
                     not_migrated.append(plugin.plugin_type)
-                    self.stdout.write(
-                        self.style.WARNING(f"{plugin.plugin_type} not migrated.")
-                    )
+                    self.stdout.write(self.style.WARNING(f"{plugin.plugin_type} not migrated."))
         if not not_migrated:
             if changes:
                 self.stdout.write(self.style.SUCCESS("Successfully migrated plugins."))
             else:
                 self.stdout.write("Nothing to migrate")
 
     def check_for_link_targets(self):
         self.stdout.write()
-        self.stdout.write(
-            self.style.SUCCESS(
-                "Checking installed apps for potential link destinations"
-            )
-        )
-        self.stdout.write(
-            self.style.SUCCESS(
-                "======================================================="
-            )
-        )
+        self.stdout.write(self.style.SUCCESS("Checking installed apps for potential link destinations"))
+        self.stdout.write(self.style.SUCCESS("======================================================="))
         blog = False
         count = 0
         for app, app_models in apps.all_models.items():
             if app != "cms":
                 for _, model in app_models.items():
                     if hasattr(model, "get_absolute_url"):
                         count += 1
                         self.stdout.write(
-                            self.style.NOTICE(
-                                f"App {app}'s {model.__name__} model is a suitable link destination."
-                            )
+                            self.style.NOTICE(f"App {app}'s {model.__name__} model is a suitable link destination.")
                         )
             if app == "djangocms_blog":
                 blog = True
         if count:
-            self.stdout.write(
-                self.style.SUCCESS(f"{count} potential link destinations found.")
-            )
+            self.stdout.write(self.style.SUCCESS(f"{count} potential link destinations found."))
             if blog:
                 self.stdout.write(self.style.WARNING(blog_example))
             else:
                 self.stdout.write(self.style.WARNING(doc_reference))
 
         else:
             self.stdout.write("No further link destinations found. Setup complete.")
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/stale_references.py` & `djangocms_frontend-1.3.2/djangocms_frontend/management/commands/subcommands/stale_references.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,19 +17,13 @@
                         if obj is None:
                             msg = f"{ui_item.ui_item} (pk={ui_item.pk}) stale field {key}."
                             pages = ui_item.placeholder.page_set.all()
                             self.stdout.write(self.style.ERROR(msg))
                             if pages:
                                 for page in pages:
                                     self.stdout.write(
-                                        self.style.WARNING(
-                                            f"... on page #{page.id}, at {page.get_absolute_url()}"
-                                        )
+                                        self.style.WARNING(f"... on page #{page.id}, at {page.get_absolute_url()}")
                                     )
                             else:
-                                self.stdout.write(
-                                    self.style.WARNING(
-                                        f"... in placeholder #{ui_item.placeholder.id}"
-                                    )
-                                )
+                                self.stdout.write(self.style.WARNING(f"... in placeholder #{ui_item.placeholder.id}"))
 
         self.stdout.write(self.style.SUCCESS("Finished checking references"))
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/sync_permissions.py` & `djangocms_frontend-1.3.2/djangocms_frontend/management/commands/subcommands/sync_permissions.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,105 +27,77 @@
         else:
             ok_to_delete = "yes"
 
         if ok_to_delete != "yes":
             self.stdout.write(self.style.ERROR("Aborted."))
             return
 
-        dcf_models = [
-            m
-            for m in apps.get_models()
-            if m.__module__.startswith("djangocms_frontend.")
-        ]
+        dcf_models = [m for m in apps.get_models() if m.__module__.startswith("djangocms_frontend.")]
         reference_model = [m for m in dcf_models if m.__name__ == "FrontendUIItem"][0]
         dcf_models.remove(reference_model)
         ctype = ContentType.objects.get(
             app_label=reference_model._meta.app_label,
             model=reference_model._meta.object_name.lower(),
         )
         permission_set = Permission.objects.filter(content_type=ctype)
         if "users" in options["scope"]:
             for user in User.objects.all():
                 self.stdout.write(self.style.SUCCESS(f"Snycing {user}"))
                 reduced = permission_set.filter(user=user)
                 reduced = [perm.codename.split("_")[0] for perm in reduced]
                 if reduced:
-                    self.stdout.write(
-                        self.style.NOTICE(f"... has {', '.join(reduced)}")
-                    )
+                    self.stdout.write(self.style.NOTICE(f"... has {', '.join(reduced)}"))
                 for model in dcf_models:
                     perms = _get_all_permissions(model._meta)
                     for perm, name in perms:
                         ok = perm.split("_")[0] in reduced
                         ctype = ContentType.objects.get(
                             app_label=model._meta.app_label,
                             model=model._meta.object_name.lower(),
                         )
                         new_perm, created = Permission.objects.get_or_create(
                             codename=perm,
                             content_type=ctype,
                             defaults=dict(name=name),
                         )
                         if created:
-                            self.stdout.write(
-                                self.style.WARNING(f"Created permission {new_perm}")
-                            )
+                            self.stdout.write(self.style.WARNING(f"Created permission {new_perm}"))
                         if ok:
-                            if not user.user_permissions.filter(
-                                codename=new_perm.codename, content_type=ctype
-                            ):
-                                self.stdout.write(
-                                    self.style.NOTICE(f"Added {new_perm} for {user}")
-                                )
+                            if not user.user_permissions.filter(codename=new_perm.codename, content_type=ctype):
+                                self.stdout.write(self.style.NOTICE(f"Added {new_perm} for {user}"))
                                 user.user_permissions.add(new_perm)
                         else:
-                            if user.user_permissions.filter(
-                                codename=new_perm.codename, content_type=ctype
-                            ):
-                                self.stdout.write(
-                                    self.style.WARNING(f"Removed {new_perm} for {user}")
-                                )
+                            if user.user_permissions.filter(codename=new_perm.codename, content_type=ctype):
+                                self.stdout.write(self.style.WARNING(f"Removed {new_perm} for {user}"))
                                 user.user_permissions.remove(new_perm)
                 user.save()
         if "groups" in options["scope"]:
             for group in Group.objects.all():
                 self.stdout.write(self.style.SUCCESS(f"Snycing {group}"))
                 reduced = permission_set.filter(group=group)
                 reduced = [perm.codename.split("_")[0] for perm in reduced]
                 if reduced:
-                    self.stdout.write(
-                        self.style.NOTICE(f"... has {', '.join(reduced)}")
-                    )
+                    self.stdout.write(self.style.NOTICE(f"... has {', '.join(reduced)}"))
                 for model in dcf_models:
                     perms = _get_all_permissions(model._meta)
                     for perm, name in perms:
                         ok = perm.split("_")[0] in reduced
                         ctype = ContentType.objects.get(
                             app_label=model._meta.app_label,
                             model=model._meta.object_name.lower(),
                         )
                         new_perm, created = Permission.objects.get_or_create(
                             codename=perm,
                             content_type=ctype,
                             defaults=dict(name=name),
                         )
                         if ok:
-                            if not group.permissions.filter(
-                                codename=new_perm.codename, content_type=ctype
-                            ):
-                                self.stdout.write(
-                                    self.style.NOTICE(f"Added {new_perm} for {group}")
-                                )
+                            if not group.permissions.filter(codename=new_perm.codename, content_type=ctype):
+                                self.stdout.write(self.style.NOTICE(f"Added {new_perm} for {group}"))
                                 group.permissions.add(new_perm)
                         else:
-                            if group.permissions.filter(
-                                codename=new_perm.codename, content_type=ctype
-                            ):
-                                self.stdout.write(
-                                    self.style.WARNING(
-                                        f"Removed {new_perm} for {group}"
-                                    )
-                                )
+                            if group.permissions.filter(codename=new_perm.codename, content_type=ctype):
+                                self.stdout.write(self.style.WARNING(f"Removed {new_perm} for {group}"))
                                 group.permissions.remove(new_perm)
                 group.save()
 
         self.stdout.write(self.style.SUCCESS("Finished syncing permissions"))
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/management/icon_migration.py` & `djangocms_frontend-1.3.2/djangocms_frontend/management/icon_migration.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,32 +90,26 @@
         "library": "font-awesome",
     }
 
 
 def m001_spacing_mixin(obj, new_obj, type):
     classes = new_obj.config["attributes"].get("class", "").split()
     if classes:
-        for size, _ in list(settings.SPACER_SIZE_CHOICES) + (
-            [("auto", "auto")] if type == "margin" else []
-        ):
+        for size, _ in list(settings.SPACER_SIZE_CHOICES) + ([("auto", "auto")] if type == "margin" else []):
             if f"{type[0]}-{size}" in classes:
                 classes.remove(f"{type[0]}-{size}")
                 classes.append(f"{type[0]}x-{size}")
                 classes.append(f"{type[0]}y-{size}")
             for side, _ in settings.SPACER_X_SIDES_CHOICES:
-                if f"{type[0]}{side}-{size}" in classes and not new_obj.config.get(
-                    f"{type}_x", None
-                ):
+                if f"{type[0]}{side}-{size}" in classes and not new_obj.config.get(f"{type}_x", None):
                     new_obj.config[f"{type}_x"] = f"{type[0]}{side}-{size}"
                     new_obj.config[f"{type}_devices"] = None
                     classes.remove(f"{type[0]}{side}-{size}")
             for side, _ in settings.SPACER_Y_SIDES_CHOICES:
-                if f"{type[0]}{side}-{size}" in classes and not new_obj.config.get(
-                    f"{type}_y", None
-                ):
+                if f"{type[0]}{side}-{size}" in classes and not new_obj.config.get(f"{type}_y", None):
                     new_obj.config[f"{type}_y"] = f"{type[0]}{side}-{size}"
                     new_obj.config[f"{type}_devices"] = None
                     classes.remove(f"{type[0]}{side}-{size}")
         if classes:
             new_obj.config["attributes"]["class"] = " ".join(classes)
         else:
             new_obj.config["attributes"].pop("class")
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/management/styled_link_migration.py` & `djangocms_frontend-1.3.2/djangocms_frontend/management/styled_link_migration.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,22 +33,18 @@
     if obj.int_destination_type_id:
         content_type = ContentType.objects.get(id=obj.int_destination_type_id)
         new_obj.config["internal_link"] = dict(
             model=f"{content_type.app_label}.{content_type.model}",
             pk=obj.int_destination_id,
         )
         styles = obj.styles.all()
-        new_obj.config["attributes"] = {
-            "class": " ".join(style.link_class for style in styles)
-        }
+        new_obj.config["attributes"] = {"class": " ".join(style.link_class for style in styles)}
         for style in styles:
             obj.styles.remove(style)
-        new_obj.config["link_type"] = (
-            "btn" if "btn" in new_obj.attributes["class"] else "link"
-        )
+        new_obj.config["link_type"] = "btn" if "btn" in new_obj.attributes["class"] else "link"
 
 
 def s002_migrate_image_container(obj, new_obj):
     new_obj.config["attributes"] = {}
     if obj.additional_classes:
         new_obj.config["attributes"]["class"] = obj.additional_classes
     if obj.additional_styles:
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/migrations/0001_initial.py` & `djangocms_frontend-1.3.2/djangocms_frontend/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/models.py` & `djangocms_frontend-1.3.2/djangocms_frontend/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,17 +52,15 @@
 
     def __init__(self, *args, **kwargs):
         self._additional_classes = []
         super().__init__(*args, **kwargs)
 
     def __getattr__(self, item):
         """Makes properties of plugin config available as plugin properties."""
-        if (
-            item[0] != "_" and item in self.config
-        ):  # Avoid infinite recursion trying to get .config from db
+        if item[0] != "_" and item in self.config:  # Avoid infinite recursion trying to get .config from db
             return self.config[item]
         return super().__getattribute__(item)
 
     def __str__(self):
         if "__str__" in self.config:
             return self.config["__str__"]
         return f"{gettext(self.ui_item)} ({str(self.pk)})"
@@ -81,38 +79,31 @@
 
     def get_attributes(self):
         attributes = self.config.get("attributes", {})
         classes = set(attributes.get("class", "").split())
         classes.update(self._additional_classes)
         if classes:
             attributes["class"] = " ".join(classes)
-        parts = (
-            f'{item}="{conditional_escape(value)}"' if value else f"{item}"
-            for item, value in attributes.items()
-        )
+        parts = (f'{item}="{conditional_escape(value)}"' if value else f"{item}" for item, value in attributes.items())
         attributes_string = " ".join(parts)
         return mark_safe(" " + attributes_string) if attributes_string else ""
 
     def save(self, *args, **kwargs):
         self.ui_item = self.__class__.__name__
         return super().save(*args, **kwargs)
 
     def initialize_from_form(self, form=None):
         """Populates the config JSON field based on initial values provided by the fields of form"""
         if form is None:
             form = self.get_plugin_class().form
         if isinstance(form, type):  # if is class
             form = form()  # instantiate
-        entangled_fields = getattr(
-            getattr(form, "Meta", None), "entangled_fields", {}
-        ).get("config", ())
+        entangled_fields = getattr(getattr(form, "Meta", None), "entangled_fields", {}).get("config", ())
         for field in entangled_fields:
-            self.config.setdefault(
-                field, {} if field == "attributes" else form[field].initial or ""
-            )
+            self.config.setdefault(field, {} if field == "attributes" else form[field].initial or "")
         return self
 
     def get_short_description(self):
         """Plugin-specific short description (to be defined by subclasses)"""
         return ""
 
     @property
@@ -137,9 +128,10 @@
     Attributes:
     - verbose_name (str): The verbose name of the UI item.
 
     Methods:
     None
 
     """
+
     class Meta:
         verbose_name = _("UI item")
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/settings.py` & `djangocms_frontend-1.3.2/djangocms_frontend/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 EMPTY_CHOICE = (("", "-----"),)
 
 EMPTY_FIELDSET = [
     (
         None,
         {
             "fields": (),
-            "description": _(
-                "There are no further settings for this plugin. Please press save."
-            ),
+            "description": _("There are no further settings for this plugin. Please press save."),
         },
     )
 ]
 
 # Only adding block elements
 TAG_CHOICES = getattr(
     django_settings,
@@ -76,17 +74,15 @@
 
 FORM_OPTIONS = getattr(django_settings, "DJANGOCMS_FRONTEND_FORM_OPTIONS", {})
 
 
 framework = getattr(django_settings, "DJANGOCMS_FRONTEND_FRAMEWORK", "bootstrap5")
 theme = getattr(django_settings, "DJANGOCMS_FRONTEND_THEME", "djangocms_frontend")
 
-framework_settings = importlib.import_module(
-    f"djangocms_frontend.frameworks.{framework}"
-)
+framework_settings = importlib.import_module(f"djangocms_frontend.frameworks.{framework}")
 
 DEVICE_SIZES = framework_settings.DEVICE_SIZES
 DEVICE_CHOICES = framework_settings.DEVICE_CHOICES
 COLOR_STYLE_CHOICES = framework_settings.COLOR_STYLE_CHOICES
 COLOR_CODES = framework_settings.COLOR_CODES
 FORM_TEMPLATE = getattr(framework_settings, "FORM_TEMPLATE", None)
 SPACER_PROPERTY_CHOICES = framework_settings.SPACER_PROPERTY_CHOICES
@@ -122,26 +118,20 @@
     except ModuleNotFoundError:
         theme_module = None
     try:
         render_module = importlib.import_module(mixin_path) if mixin_path else None
     except ModuleNotFoundError:
         render_module = None
 
-    return lambda name: render_factory(
-        naming.format(name=name), theme_module, render_module
-    )
+    return lambda name: render_factory(naming.format(name=name), theme_module, render_module)
 
 
 def get_renderer(my_module):
     if not isinstance(my_module, str):
         my_module = my_module.__name__
-    return get_mixins(
-        "{name}RenderMixin", theme_render_path, f"{my_module}.frameworks.{framework}"
-    )
+    return get_mixins("{name}RenderMixin", theme_render_path, f"{my_module}.frameworks.{framework}")
 
 
 def get_forms(my_module):
     if not isinstance(my_module, str):
         my_module = my_module.__name__
-    return get_mixins(
-        "{name}FormMixin", theme_forms_path, f"{my_module}.frameworks.{framework}"
-    )
+    return get_mixins("{name}FormMixin", theme_forms_path, f"{my_module}.frameworks.{framework}")
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/css/base.css` & `djangocms_frontend-1.3.2/djangocms_frontend/static/djangocms_frontend/css/base.css`

 * *Files 1% similar despite different names*

```diff
@@ -2579,2387 +2579,2418 @@
 0000a120: 6976 653b 6469 7370 6c61 793a 2d6d 732d  ive;display:-ms-
 0000a130: 666c 6578 626f 783b 6469 7370 6c61 793a  flexbox;display:
 0000a140: 666c 6578 3b70 6164 6469 6e67 3a30 3b6d  flex;padding:0;m
 0000a150: 696e 2d77 6964 7468 3a38 3030 7078 7d2e  in-width:800px}.
 0000a160: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
 0000a170: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
 0000a180: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
-0000a190: 202e 6669 656c 642d 626f 783a 6669 7273   .field-box:firs
-0000a1a0: 742d 6368 696c 642c 2e64 6a61 6e67 6f63  t-child,.djangoc
-0000a1b0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000a1c0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000a1d0: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
-0000a1e0: 626f 783a 6669 7273 742d 6368 696c 642c  box:first-child,
-0000a1f0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000a200: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000a210: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d73  -row.field-xs_ms
-0000a220: 202e 6669 656c 642d 626f 783a 6669 7273   .field-box:firs
-0000a230: 742d 6368 696c 642c 2e64 6a61 6e67 6f63  t-child,.djangoc
-0000a240: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000a250: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000a260: 6c64 2d78 735f 6f66 6673 6574 202e 6669  ld-xs_offset .fi
-0000a270: 656c 642d 626f 783a 6669 7273 742d 6368  eld-box:first-ch
-0000a280: 696c 642c 2e64 6a61 6e67 6f63 6d73 2d66  ild,.djangocms-f
-0000a290: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000a2a0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000a2b0: 735f 6f72 6465 7220 2e66 6965 6c64 2d62  s_order .field-b
-0000a2c0: 6f78 3a66 6972 7374 2d63 6869 6c64 2c2e  ox:first-child,.
-0000a2d0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000a2e0: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
-0000a2f0: 2e66 6965 6c64 2d72 6f77 5f63 6f6c 735f  .field-row_cols_
-0000a300: 7873 202e 6669 656c 642d 626f 783a 6669  xs .field-box:fi
-0000a310: 7273 742d 6368 696c 647b 7769 6474 683a  rst-child{width:
-0000a320: 3131 3570 7821 696d 706f 7274 616e 747d  115px!important}
-0000a330: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000a340: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000a350: 2d72 6f77 2e66 6965 6c64 2d78 735f 636f  -row.field-xs_co
-0000a360: 6c20 2e66 6965 6c64 2d62 6f78 2c2e 646a  l .field-box,.dj
-0000a370: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000a380: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
-0000a390: 772e 6669 656c 642d 7873 5f63 6f6c 202e  w.field-xs_col .
-0000a3a0: 6669 656c 6442 6f78 2c2e 646a 616e 676f  fieldBox,.django
-0000a3b0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000a3c0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000a3d0: 656c 642d 7873 5f6d 6520 2e66 6965 6c64  eld-xs_me .field
-0000a3e0: 2d62 6f78 2c2e 646a 616e 676f 636d 732d  -box,.djangocms-
-0000a3f0: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-0000a400: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000a410: 7873 5f6d 6520 2e66 6965 6c64 426f 782c  xs_me .fieldBox,
-0000a420: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000a430: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000a440: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d73  -row.field-xs_ms
-0000a450: 202e 6669 656c 642d 626f 782c 2e64 6a61   .field-box,.dja
-0000a460: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000a470: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000a480: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
-0000a490: 656c 6442 6f78 2c2e 646a 616e 676f 636d  eldBox,.djangocm
-0000a4a0: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
-0000a4b0: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
-0000a4c0: 642d 7873 5f6f 6666 7365 7420 2e66 6965  d-xs_offset .fie
-0000a4d0: 6c64 2d62 6f78 2c2e 646a 616e 676f 636d  ld-box,.djangocm
-0000a4e0: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
-0000a4f0: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
-0000a500: 642d 7873 5f6f 6666 7365 7420 2e66 6965  d-xs_offset .fie
-0000a510: 6c64 426f 782c 2e64 6a61 6e67 6f63 6d73  ldBox,.djangocms
-0000a520: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000a530: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000a540: 2d78 735f 6f72 6465 7220 2e66 6965 6c64  -xs_order .field
-0000a550: 2d62 6f78 2c2e 646a 616e 676f 636d 732d  -box,.djangocms-
-0000a560: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-0000a570: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000a580: 7873 5f6f 7264 6572 202e 6669 656c 6442  xs_order .fieldB
-0000a590: 6f78 2c2e 646a 616e 676f 636d 732d 6672  ox,.djangocms-fr
-0000a5a0: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
-0000a5b0: 2d72 6f77 2e66 6965 6c64 2d72 6f77 5f63  -row.field-row_c
-0000a5c0: 6f6c 735f 7873 202e 6669 656c 642d 626f  ols_xs .field-bo
-0000a5d0: 782c 2e64 6a61 6e67 6f63 6d73 2d66 726f  x,.djangocms-fro
-0000a5e0: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-0000a5f0: 726f 772e 6669 656c 642d 726f 775f 636f  row.field-row_co
-0000a600: 6c73 5f78 7320 2e66 6965 6c64 426f 787b  ls_xs .fieldBox{
-0000a610: 706f 7369 7469 6f6e 3a72 656c 6174 6976  position:relativ
-0000a620: 653b 626f 782d 7369 7a69 6e67 3a63 6f6e  e;box-sizing:con
-0000a630: 7465 6e74 2d62 6f78 3b77 6964 7468 3a38  tent-box;width:8
-0000a640: 3670 7821 696d 706f 7274 616e 743b 2d6d  6px!important;-m
-0000a650: 732d 666c 6578 3a6e 6f6e 653b 666c 6578  s-flex:none;flex
-0000a660: 3a6e 6f6e 653b 7061 6464 696e 673a 3135  :none;padding:15
-0000a670: 7078 2031 3070 783b 6d61 7267 696e 3a30  px 10px;margin:0
-0000a680: 2169 6d70 6f72 7461 6e74 3b62 6f72 6465  !important;borde
-0000a690: 722d 626f 7474 6f6d 3a31 7078 2073 6f6c  r-bottom:1px sol
-0000a6a0: 6964 2023 6565 653b 666c 6f61 743a 6c65  id #eee;float:le
-0000a6b0: 6674 2169 6d70 6f72 7461 6e74 7d2e 646a  ft!important}.dj
-0000a6c0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000a6d0: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
-0000a6e0: 772e 6669 656c 642d 7873 5f63 6f6c 202e  w.field-xs_col .
-0000a6f0: 6669 656c 642d 626f 7820 696e 7075 743a  field-box input:
-0000a700: 6e6f 7428 5b74 7970 653d 6368 6563 6b62  not([type=checkb
-0000a710: 6f78 5d29 2c2e 646a 616e 676f 636d 732d  ox]),.djangocms-
-0000a720: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-0000a730: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000a740: 7873 5f63 6f6c 202e 6669 656c 6442 6f78  xs_col .fieldBox
-0000a750: 2069 6e70 7574 3a6e 6f74 285b 7479 7065   input:not([type
-0000a760: 3d63 6865 636b 626f 785d 292c 2e64 6a61  =checkbox]),.dja
-0000a770: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000a780: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000a790: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
-0000a7a0: 656c 642d 626f 7820 696e 7075 743a 6e6f  eld-box input:no
-0000a7b0: 7428 5b74 7970 653d 6368 6563 6b62 6f78  t([type=checkbox
-0000a7c0: 5d29 2c2e 646a 616e 676f 636d 732d 6672  ]),.djangocms-fr
-0000a7d0: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-0000a7e0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000a7f0: 5f6d 6520 2e66 6965 6c64 426f 7820 696e  _me .fieldBox in
-0000a800: 7075 743a 6e6f 7428 5b74 7970 653d 6368  put:not([type=ch
-0000a810: 6563 6b62 6f78 5d29 2c2e 646a 616e 676f  eckbox]),.django
-0000a820: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000a830: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000a840: 656c 642d 7873 5f6d 7320 2e66 6965 6c64  eld-xs_ms .field
-0000a850: 2d62 6f78 2069 6e70 7574 3a6e 6f74 285b  -box input:not([
-0000a860: 7479 7065 3d63 6865 636b 626f 785d 292c  type=checkbox]),
-0000a870: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000a880: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000a890: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d73  -row.field-xs_ms
-0000a8a0: 202e 6669 656c 6442 6f78 2069 6e70 7574   .fieldBox input
-0000a8b0: 3a6e 6f74 285b 7479 7065 3d63 6865 636b  :not([type=check
-0000a8c0: 626f 785d 292c 2e64 6a61 6e67 6f63 6d73  box]),.djangocms
-0000a8d0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000a8e0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000a8f0: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
-0000a900: 642d 626f 7820 696e 7075 743a 6e6f 7428  d-box input:not(
-0000a910: 5b74 7970 653d 6368 6563 6b62 6f78 5d29  [type=checkbox])
-0000a920: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000a930: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000a940: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-0000a950: 6666 7365 7420 2e66 6965 6c64 426f 7820  ffset .fieldBox 
-0000a960: 696e 7075 743a 6e6f 7428 5b74 7970 653d  input:not([type=
-0000a970: 6368 6563 6b62 6f78 5d29 2c2e 646a 616e  checkbox]),.djan
-0000a980: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
-0000a990: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
-0000a9a0: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
-0000a9b0: 6669 656c 642d 626f 7820 696e 7075 743a  field-box input:
-0000a9c0: 6e6f 7428 5b74 7970 653d 6368 6563 6b62  not([type=checkb
-0000a9d0: 6f78 5d29 2c2e 646a 616e 676f 636d 732d  ox]),.djangocms-
-0000a9e0: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-0000a9f0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000aa00: 7873 5f6f 7264 6572 202e 6669 656c 6442  xs_order .fieldB
-0000aa10: 6f78 2069 6e70 7574 3a6e 6f74 285b 7479  ox input:not([ty
-0000aa20: 7065 3d63 6865 636b 626f 785d 292c 2e64  pe=checkbox]),.d
-0000aa30: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000aa40: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-0000aa50: 6669 656c 642d 726f 775f 636f 6c73 5f78  field-row_cols_x
-0000aa60: 7320 2e66 6965 6c64 2d62 6f78 2069 6e70  s .field-box inp
-0000aa70: 7574 3a6e 6f74 285b 7479 7065 3d63 6865  ut:not([type=che
-0000aa80: 636b 626f 785d 292c 2e64 6a61 6e67 6f63  ckbox]),.djangoc
-0000aa90: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-0000aaa0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000aab0: 726f 775f 636f 6c73 5f78 7320 2e66 6965  row_cols_xs .fie
-0000aac0: 6c64 426f 7820 696e 7075 743a 6e6f 7428  ldBox input:not(
-0000aad0: 5b74 7970 653d 6368 6563 6b62 6f78 5d29  [type=checkbox])
-0000aae0: 7b74 6578 742d 616c 6967 6e3a 656e 643b  {text-align:end;
-0000aaf0: 7061 6464 696e 672d 696e 6c69 6e65 2d65  padding-inline-e
-0000ab00: 6e64 3a35 7078 2169 6d70 6f72 7461 6e74  nd:5px!important
-0000ab10: 3b62 6f78 2d73 697a 696e 673a 626f 7264  ;box-sizing:bord
-0000ab20: 6572 2d62 6f78 3b77 6964 7468 3a31 3030  er-box;width:100
-0000ab30: 257d 2e64 6a61 6e67 6f63 6d73 2d66 726f  %}.djangocms-fro
-0000ab40: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000ab50: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000ab60: 636f 6c20 2e66 6965 6c64 2d62 6f78 206c  col .field-box l
-0000ab70: 6162 656c 2c2e 646a 616e 676f 636d 732d  abel,.djangocms-
-0000ab80: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-0000ab90: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000aba0: 7873 5f63 6f6c 202e 6669 656c 6442 6f78  xs_col .fieldBox
-0000abb0: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
-0000abc0: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
-0000abd0: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
-0000abe0: 642d 7873 5f6d 6520 2e66 6965 6c64 2d62  d-xs_me .field-b
-0000abf0: 6f78 206c 6162 656c 2c2e 646a 616e 676f  ox label,.django
-0000ac00: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000ac10: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000ac20: 656c 642d 7873 5f6d 6520 2e66 6965 6c64  eld-xs_me .field
-0000ac30: 426f 7820 6c61 6265 6c2c 2e64 6a61 6e67  Box label,.djang
-0000ac40: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000ac50: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000ac60: 6965 6c64 2d78 735f 6d73 202e 6669 656c  ield-xs_ms .fiel
-0000ac70: 642d 626f 7820 6c61 6265 6c2c 2e64 6a61  d-box label,.dja
-0000ac80: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000ac90: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000aca0: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
-0000acb0: 656c 6442 6f78 206c 6162 656c 2c2e 646a  eldBox label,.dj
-0000acc0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000acd0: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
-0000ace0: 772e 6669 656c 642d 7873 5f6f 6666 7365  w.field-xs_offse
-0000acf0: 7420 2e66 6965 6c64 2d62 6f78 206c 6162  t .field-box lab
-0000ad00: 656c 2c2e 646a 616e 676f 636d 732d 6672  el,.djangocms-fr
-0000ad10: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-0000ad20: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000ad30: 5f6f 6666 7365 7420 2e66 6965 6c64 426f  _offset .fieldBo
-0000ad40: 7820 6c61 6265 6c2c 2e64 6a61 6e67 6f63  x label,.djangoc
-0000ad50: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000ad60: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000ad70: 6c64 2d78 735f 6f72 6465 7220 2e66 6965  ld-xs_order .fie
-0000ad80: 6c64 2d62 6f78 206c 6162 656c 2c2e 646a  ld-box label,.dj
-0000ad90: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000ada0: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
-0000adb0: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
-0000adc0: 202e 6669 656c 6442 6f78 206c 6162 656c   .fieldBox label
-0000add0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000ade0: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
-0000adf0: 6f77 2e66 6965 6c64 2d72 6f77 5f63 6f6c  ow.field-row_col
-0000ae00: 735f 7873 202e 6669 656c 642d 626f 7820  s_xs .field-box 
-0000ae10: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-0000ae20: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-0000ae30: 6f72 6d2d 726f 772e 6669 656c 642d 726f  orm-row.field-ro
-0000ae40: 775f 636f 6c73 5f78 7320 2e66 6965 6c64  w_cols_xs .field
-0000ae50: 426f 7820 6c61 6265 6c7b 666f 6e74 2d73  Box label{font-s
-0000ae60: 697a 653a 3132 7078 2169 6d70 6f72 7461  ize:12px!importa
-0000ae70: 6e74 3b66 6f6e 742d 7765 6967 6874 3a34  nt;font-weight:4
-0000ae80: 3030 2169 6d70 6f72 7461 6e74 3b63 6f6c  00!important;col
-0000ae90: 6f72 3a23 6363 6321 696d 706f 7274 616e  or:#ccc!importan
-0000aea0: 743b 706f 7369 7469 6f6e 3a61 6273 6f6c  t;position:absol
-0000aeb0: 7574 653b 696e 7365 742d 696e 6c69 6e65  ute;inset-inline
-0000aec0: 2d73 7461 7274 3a31 3570 783b 696e 7365  -start:15px;inse
-0000aed0: 742d 626c 6f63 6b2d 656e 643a 3137 7078  t-block-end:17px
-0000aee0: 3b74 6578 742d 7472 616e 7366 6f72 6d3a  ;text-transform:
-0000aef0: 6c6f 7765 7263 6173 657d 2e64 6a61 6e67  lowercase}.djang
-0000af00: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000af10: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000af20: 6965 6c64 2d78 735f 636f 6c20 2e66 6965  ield-xs_col .fie
-0000af30: 6c64 2d62 6f78 202e 6469 7361 626c 6564  ld-box .disabled
-0000af40: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000af50: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000af60: 6d2d 726f 772e 6669 656c 642d 7873 5f63  m-row.field-xs_c
-0000af70: 6f6c 202e 6669 656c 6442 6f78 202e 6469  ol .fieldBox .di
-0000af80: 7361 626c 6564 2c2e 646a 616e 676f 636d  sabled,.djangocm
-0000af90: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
-0000afa0: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
-0000afb0: 642d 7873 5f6d 6520 2e66 6965 6c64 2d62  d-xs_me .field-b
-0000afc0: 6f78 202e 6469 7361 626c 6564 2c2e 646a  ox .disabled,.dj
-0000afd0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000afe0: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
-0000aff0: 772e 6669 656c 642d 7873 5f6d 6520 2e66  w.field-xs_me .f
-0000b000: 6965 6c64 426f 7820 2e64 6973 6162 6c65  ieldBox .disable
-0000b010: 642c 2e64 6a61 6e67 6f63 6d73 2d66 726f  d,.djangocms-fro
-0000b020: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000b030: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000b040: 6d73 202e 6669 656c 642d 626f 7820 2e64  ms .field-box .d
-0000b050: 6973 6162 6c65 642c 2e64 6a61 6e67 6f63  isabled,.djangoc
-0000b060: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000b070: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000b080: 6c64 2d78 735f 6d73 202e 6669 656c 6442  ld-xs_ms .fieldB
-0000b090: 6f78 202e 6469 7361 626c 6564 2c2e 646a  ox .disabled,.dj
-0000b0a0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000b0b0: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
-0000b0c0: 772e 6669 656c 642d 7873 5f6f 6666 7365  w.field-xs_offse
-0000b0d0: 7420 2e66 6965 6c64 2d62 6f78 202e 6469  t .field-box .di
-0000b0e0: 7361 626c 6564 2c2e 646a 616e 676f 636d  sabled,.djangocm
+0000a190: 3e64 6976 3e64 6976 3a6e 6f74 285b 636c  >div>div:not([cl
+0000a1a0: 6173 735d 292c 2e64 6a61 6e67 6f63 6d73  ass]),.djangocms
+0000a1b0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000a1c0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000a1d0: 2d78 735f 6d65 3e64 6976 3e64 6976 3a6e  -xs_me>div>div:n
+0000a1e0: 6f74 285b 636c 6173 735d 292c 2e64 6a61  ot([class]),.dja
+0000a1f0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000a200: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000a210: 2e66 6965 6c64 2d78 735f 6d73 3e64 6976  .field-xs_ms>div
+0000a220: 3e64 6976 3a6e 6f74 285b 636c 6173 735d  >div:not([class]
+0000a230: 292c 2e64 6a61 6e67 6f63 6d73 2d66 726f  ),.djangocms-fro
+0000a240: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000a250: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000a260: 6f66 6673 6574 3e64 6976 3e64 6976 3a6e  offset>div>div:n
+0000a270: 6f74 285b 636c 6173 735d 292c 2e64 6a61  ot([class]),.dja
+0000a280: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000a290: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000a2a0: 2e66 6965 6c64 2d78 735f 6f72 6465 723e  .field-xs_order>
+0000a2b0: 6469 763e 6469 763a 6e6f 7428 5b63 6c61  div>div:not([cla
+0000a2c0: 7373 5d29 2c2e 646a 616e 676f 636d 732d  ss]),.djangocms-
+0000a2d0: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
+0000a2e0: 726d 2d72 6f77 2e66 6965 6c64 2d72 6f77  rm-row.field-row
+0000a2f0: 5f63 6f6c 735f 7873 3e64 6976 3e64 6976  _cols_xs>div>div
+0000a300: 3a6e 6f74 285b 636c 6173 735d 297b 7769  :not([class]){wi
+0000a310: 6474 683a 756e 7365 7421 696d 706f 7274  dth:unset!import
+0000a320: 616e 743b 6d61 782d 7769 6474 683a 756e  ant;max-width:un
+0000a330: 7365 7421 696d 706f 7274 616e 747d 2e64  set!important}.d
+0000a340: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000a350: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000a360: 6f77 2e66 6965 6c64 2d78 735f 636f 6c20  ow.field-xs_col 
+0000a370: 2e66 6965 6c64 2d62 6f78 3a66 6972 7374  .field-box:first
+0000a380: 2d63 6869 6c64 2c2e 646a 616e 676f 636d  -child,.djangocm
+0000a390: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
+0000a3a0: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
+0000a3b0: 642d 7873 5f6d 6520 2e66 6965 6c64 2d62  d-xs_me .field-b
+0000a3c0: 6f78 3a66 6972 7374 2d63 6869 6c64 2c2e  ox:first-child,.
+0000a3d0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000a3e0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000a3f0: 726f 772e 6669 656c 642d 7873 5f6d 7320  row.field-xs_ms 
+0000a400: 2e66 6965 6c64 2d62 6f78 3a66 6972 7374  .field-box:first
+0000a410: 2d63 6869 6c64 2c2e 646a 616e 676f 636d  -child,.djangocm
+0000a420: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
+0000a430: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
+0000a440: 642d 7873 5f6f 6666 7365 7420 2e66 6965  d-xs_offset .fie
+0000a450: 6c64 2d62 6f78 3a66 6972 7374 2d63 6869  ld-box:first-chi
+0000a460: 6c64 2c2e 646a 616e 676f 636d 732d 6672  ld,.djangocms-fr
+0000a470: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+0000a480: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000a490: 5f6f 7264 6572 202e 6669 656c 642d 626f  _order .field-bo
+0000a4a0: 783a 6669 7273 742d 6368 696c 642c 2e64  x:first-child,.d
+0000a4b0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000a4c0: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+0000a4d0: 6669 656c 642d 726f 775f 636f 6c73 5f78  field-row_cols_x
+0000a4e0: 7320 2e66 6965 6c64 2d62 6f78 3a66 6972  s .field-box:fir
+0000a4f0: 7374 2d63 6869 6c64 7b77 6964 7468 3a31  st-child{width:1
+0000a500: 3135 7078 2169 6d70 6f72 7461 6e74 7d2e  15px!important}.
+0000a510: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000a520: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000a530: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
+0000a540: 202e 6669 656c 642d 626f 782c 2e64 6a61   .field-box,.dja
+0000a550: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000a560: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000a570: 2e66 6965 6c64 2d78 735f 636f 6c20 2e66  .field-xs_col .f
+0000a580: 6965 6c64 426f 782c 2e64 6a61 6e67 6f63  ieldBox,.djangoc
+0000a590: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000a5a0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000a5b0: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
+0000a5c0: 626f 782c 2e64 6a61 6e67 6f63 6d73 2d66  box,.djangocms-f
+0000a5d0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000a5e0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000a5f0: 735f 6d65 202e 6669 656c 6442 6f78 2c2e  s_me .fieldBox,.
+0000a600: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000a610: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000a620: 726f 772e 6669 656c 642d 7873 5f6d 7320  row.field-xs_ms 
+0000a630: 2e66 6965 6c64 2d62 6f78 2c2e 646a 616e  .field-box,.djan
+0000a640: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
+0000a650: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
+0000a660: 6669 656c 642d 7873 5f6d 7320 2e66 6965  field-xs_ms .fie
+0000a670: 6c64 426f 782c 2e64 6a61 6e67 6f63 6d73  ldBox,.djangocms
+0000a680: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000a690: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000a6a0: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
+0000a6b0: 642d 626f 782c 2e64 6a61 6e67 6f63 6d73  d-box,.djangocms
+0000a6c0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000a6d0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000a6e0: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
+0000a6f0: 6442 6f78 2c2e 646a 616e 676f 636d 732d  dBox,.djangocms-
+0000a700: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000a710: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000a720: 7873 5f6f 7264 6572 202e 6669 656c 642d  xs_order .field-
+0000a730: 626f 782c 2e64 6a61 6e67 6f63 6d73 2d66  box,.djangocms-f
+0000a740: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000a750: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000a760: 735f 6f72 6465 7220 2e66 6965 6c64 426f  s_order .fieldBo
+0000a770: 782c 2e64 6a61 6e67 6f63 6d73 2d66 726f  x,.djangocms-fro
+0000a780: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+0000a790: 726f 772e 6669 656c 642d 726f 775f 636f  row.field-row_co
+0000a7a0: 6c73 5f78 7320 2e66 6965 6c64 2d62 6f78  ls_xs .field-box
+0000a7b0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000a7c0: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
+0000a7d0: 6f77 2e66 6965 6c64 2d72 6f77 5f63 6f6c  ow.field-row_col
+0000a7e0: 735f 7873 202e 6669 656c 6442 6f78 7b70  s_xs .fieldBox{p
+0000a7f0: 6f73 6974 696f 6e3a 7265 6c61 7469 7665  osition:relative
+0000a800: 3b62 6f78 2d73 697a 696e 673a 636f 6e74  ;box-sizing:cont
+0000a810: 656e 742d 626f 783b 7769 6474 683a 3836  ent-box;width:86
+0000a820: 7078 2169 6d70 6f72 7461 6e74 3b2d 6d73  px!important;-ms
+0000a830: 2d66 6c65 783a 6e6f 6e65 3b66 6c65 783a  -flex:none;flex:
+0000a840: 6e6f 6e65 3b64 6973 706c 6179 3a62 6c6f  none;display:blo
+0000a850: 636b 3b70 6164 6469 6e67 3a31 3570 7820  ck;padding:15px 
+0000a860: 3130 7078 3b6d 6172 6769 6e3a 3021 696d  10px;margin:0!im
+0000a870: 706f 7274 616e 743b 626f 7264 6572 2d62  portant;border-b
+0000a880: 6f74 746f 6d3a 3170 7820 736f 6c69 6420  ottom:1px solid 
+0000a890: 2365 6565 3b66 6c6f 6174 3a6c 6566 7421  #eee;float:left!
+0000a8a0: 696d 706f 7274 616e 747d 2e64 6a61 6e67  important}.djang
+0000a8b0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000a8c0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000a8d0: 6965 6c64 2d78 735f 636f 6c20 2e66 6965  ield-xs_col .fie
+0000a8e0: 6c64 2d62 6f78 2069 6e70 7574 3a6e 6f74  ld-box input:not
+0000a8f0: 285b 7479 7065 3d63 6865 636b 626f 785d  ([type=checkbox]
+0000a900: 292c 2e64 6a61 6e67 6f63 6d73 2d66 726f  ),.djangocms-fro
+0000a910: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000a920: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000a930: 636f 6c20 2e66 6965 6c64 426f 7820 696e  col .fieldBox in
+0000a940: 7075 743a 6e6f 7428 5b74 7970 653d 6368  put:not([type=ch
+0000a950: 6563 6b62 6f78 5d29 2c2e 646a 616e 676f  eckbox]),.django
+0000a960: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000a970: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000a980: 656c 642d 7873 5f6d 6520 2e66 6965 6c64  eld-xs_me .field
+0000a990: 2d62 6f78 2069 6e70 7574 3a6e 6f74 285b  -box input:not([
+0000a9a0: 7479 7065 3d63 6865 636b 626f 785d 292c  type=checkbox]),
+0000a9b0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000a9c0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000a9d0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
+0000a9e0: 202e 6669 656c 6442 6f78 2069 6e70 7574   .fieldBox input
+0000a9f0: 3a6e 6f74 285b 7479 7065 3d63 6865 636b  :not([type=check
+0000aa00: 626f 785d 292c 2e64 6a61 6e67 6f63 6d73  box]),.djangocms
+0000aa10: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000aa20: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000aa30: 2d78 735f 6d73 202e 6669 656c 642d 626f  -xs_ms .field-bo
+0000aa40: 7820 696e 7075 743a 6e6f 7428 5b74 7970  x input:not([typ
+0000aa50: 653d 6368 6563 6b62 6f78 5d29 2c2e 646a  e=checkbox]),.dj
+0000aa60: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000aa70: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000aa80: 772e 6669 656c 642d 7873 5f6d 7320 2e66  w.field-xs_ms .f
+0000aa90: 6965 6c64 426f 7820 696e 7075 743a 6e6f  ieldBox input:no
+0000aaa0: 7428 5b74 7970 653d 6368 6563 6b62 6f78  t([type=checkbox
+0000aab0: 5d29 2c2e 646a 616e 676f 636d 732d 6672  ]),.djangocms-fr
+0000aac0: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+0000aad0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000aae0: 5f6f 6666 7365 7420 2e66 6965 6c64 2d62  _offset .field-b
+0000aaf0: 6f78 2069 6e70 7574 3a6e 6f74 285b 7479  ox input:not([ty
+0000ab00: 7065 3d63 6865 636b 626f 785d 292c 2e64  pe=checkbox]),.d
+0000ab10: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000ab20: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000ab30: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
+0000ab40: 6574 202e 6669 656c 6442 6f78 2069 6e70  et .fieldBox inp
+0000ab50: 7574 3a6e 6f74 285b 7479 7065 3d63 6865  ut:not([type=che
+0000ab60: 636b 626f 785d 292c 2e64 6a61 6e67 6f63  ckbox]),.djangoc
+0000ab70: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000ab80: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000ab90: 6c64 2d78 735f 6f72 6465 7220 2e66 6965  ld-xs_order .fie
+0000aba0: 6c64 2d62 6f78 2069 6e70 7574 3a6e 6f74  ld-box input:not
+0000abb0: 285b 7479 7065 3d63 6865 636b 626f 785d  ([type=checkbox]
+0000abc0: 292c 2e64 6a61 6e67 6f63 6d73 2d66 726f  ),.djangocms-fro
+0000abd0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000abe0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000abf0: 6f72 6465 7220 2e66 6965 6c64 426f 7820  order .fieldBox 
+0000ac00: 696e 7075 743a 6e6f 7428 5b74 7970 653d  input:not([type=
+0000ac10: 6368 6563 6b62 6f78 5d29 2c2e 646a 616e  checkbox]),.djan
+0000ac20: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
+0000ac30: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
+0000ac40: 6c64 2d72 6f77 5f63 6f6c 735f 7873 202e  ld-row_cols_xs .
+0000ac50: 6669 656c 642d 626f 7820 696e 7075 743a  field-box input:
+0000ac60: 6e6f 7428 5b74 7970 653d 6368 6563 6b62  not([type=checkb
+0000ac70: 6f78 5d29 2c2e 646a 616e 676f 636d 732d  ox]),.djangocms-
+0000ac80: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
+0000ac90: 726d 2d72 6f77 2e66 6965 6c64 2d72 6f77  rm-row.field-row
+0000aca0: 5f63 6f6c 735f 7873 202e 6669 656c 6442  _cols_xs .fieldB
+0000acb0: 6f78 2069 6e70 7574 3a6e 6f74 285b 7479  ox input:not([ty
+0000acc0: 7065 3d63 6865 636b 626f 785d 297b 7465  pe=checkbox]){te
+0000acd0: 7874 2d61 6c69 676e 3a65 6e64 3b70 6164  xt-align:end;pad
+0000ace0: 6469 6e67 2d69 6e6c 696e 652d 656e 643a  ding-inline-end:
+0000acf0: 3570 7821 696d 706f 7274 616e 743b 626f  5px!important;bo
+0000ad00: 782d 7369 7a69 6e67 3a62 6f72 6465 722d  x-sizing:border-
+0000ad10: 626f 783b 7769 6474 683a 3130 3025 7d2e  box;width:100%}.
+0000ad20: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000ad30: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000ad40: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
+0000ad50: 202e 6669 656c 642d 626f 7820 6c61 6265   .field-box labe
+0000ad60: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
+0000ad70: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000ad80: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000ad90: 636f 6c20 2e66 6965 6c64 426f 7820 6c61  col .fieldBox la
+0000ada0: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
+0000adb0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000adc0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000add0: 735f 6d65 202e 6669 656c 642d 626f 7820  s_me .field-box 
+0000ade0: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000adf0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000ae00: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000ae10: 2d78 735f 6d65 202e 6669 656c 6442 6f78  -xs_me .fieldBox
+0000ae20: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
+0000ae30: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
+0000ae40: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
+0000ae50: 642d 7873 5f6d 7320 2e66 6965 6c64 2d62  d-xs_ms .field-b
+0000ae60: 6f78 206c 6162 656c 2c2e 646a 616e 676f  ox label,.django
+0000ae70: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000ae80: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000ae90: 656c 642d 7873 5f6d 7320 2e66 6965 6c64  eld-xs_ms .field
+0000aea0: 426f 7820 6c61 6265 6c2c 2e64 6a61 6e67  Box label,.djang
+0000aeb0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000aec0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000aed0: 6965 6c64 2d78 735f 6f66 6673 6574 202e  ield-xs_offset .
+0000aee0: 6669 656c 642d 626f 7820 6c61 6265 6c2c  field-box label,
+0000aef0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000af00: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000af10: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f66  -row.field-xs_of
+0000af20: 6673 6574 202e 6669 656c 6442 6f78 206c  fset .fieldBox l
+0000af30: 6162 656c 2c2e 646a 616e 676f 636d 732d  abel,.djangocms-
+0000af40: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000af50: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000af60: 7873 5f6f 7264 6572 202e 6669 656c 642d  xs_order .field-
+0000af70: 626f 7820 6c61 6265 6c2c 2e64 6a61 6e67  box label,.djang
+0000af80: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000af90: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000afa0: 6965 6c64 2d78 735f 6f72 6465 7220 2e66  ield-xs_order .f
+0000afb0: 6965 6c64 426f 7820 6c61 6265 6c2c 2e64  ieldBox label,.d
+0000afc0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000afd0: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+0000afe0: 6669 656c 642d 726f 775f 636f 6c73 5f78  field-row_cols_x
+0000aff0: 7320 2e66 6965 6c64 2d62 6f78 206c 6162  s .field-box lab
+0000b000: 656c 2c2e 646a 616e 676f 636d 732d 6672  el,.djangocms-fr
+0000b010: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
+0000b020: 2d72 6f77 2e66 6965 6c64 2d72 6f77 5f63  -row.field-row_c
+0000b030: 6f6c 735f 7873 202e 6669 656c 6442 6f78  ols_xs .fieldBox
+0000b040: 206c 6162 656c 7b66 6f6e 742d 7369 7a65   label{font-size
+0000b050: 3a31 3270 7821 696d 706f 7274 616e 743b  :12px!important;
+0000b060: 666f 6e74 2d77 6569 6768 743a 3430 3021  font-weight:400!
+0000b070: 696d 706f 7274 616e 743b 636f 6c6f 723a  important;color:
+0000b080: 2363 6363 2169 6d70 6f72 7461 6e74 3b70  #ccc!important;p
+0000b090: 6f73 6974 696f 6e3a 6162 736f 6c75 7465  osition:absolute
+0000b0a0: 3b69 6e73 6574 2d69 6e6c 696e 652d 7374  ;inset-inline-st
+0000b0b0: 6172 743a 3135 7078 3b69 6e73 6574 2d62  art:15px;inset-b
+0000b0c0: 6c6f 636b 2d65 6e64 3a31 3770 783b 7465  lock-end:17px;te
+0000b0d0: 7874 2d74 7261 6e73 666f 726d 3a6c 6f77  xt-transform:low
+0000b0e0: 6572 6361 7365 7d2e 646a 616e 676f 636d  ercase}.djangocm
 0000b0f0: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
 0000b100: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
-0000b110: 642d 7873 5f6f 6666 7365 7420 2e66 6965  d-xs_offset .fie
-0000b120: 6c64 426f 7820 2e64 6973 6162 6c65 642c  ldBox .disabled,
-0000b130: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000b140: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000b150: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f72  -row.field-xs_or
-0000b160: 6465 7220 2e66 6965 6c64 2d62 6f78 202e  der .field-box .
-0000b170: 6469 7361 626c 6564 2c2e 646a 616e 676f  disabled,.django
-0000b180: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000b190: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000b1a0: 656c 642d 7873 5f6f 7264 6572 202e 6669  eld-xs_order .fi
-0000b1b0: 656c 6442 6f78 202e 6469 7361 626c 6564  eldBox .disabled
-0000b1c0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000b1d0: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
-0000b1e0: 6f77 2e66 6965 6c64 2d72 6f77 5f63 6f6c  ow.field-row_col
-0000b1f0: 735f 7873 202e 6669 656c 642d 626f 7820  s_xs .field-box 
-0000b200: 2e64 6973 6162 6c65 642c 2e64 6a61 6e67  .disabled,.djang
-0000b210: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-0000b220: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-0000b230: 642d 726f 775f 636f 6c73 5f78 7320 2e66  d-row_cols_xs .f
-0000b240: 6965 6c64 426f 7820 2e64 6973 6162 6c65  ieldBox .disable
-0000b250: 647b 636f 6c6f 723a 2363 6363 3b62 6163  d{color:#ccc;bac
-0000b260: 6b67 726f 756e 643a 2365 6565 7d2e 646a  kground:#eee}.dj
-0000b270: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000b280: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
-0000b290: 772e 6669 656c 642d 7873 5f63 6f6c 202e  w.field-xs_col .
-0000b2a0: 6669 656c 642d 626f 783a 6c61 7374 2d63  field-box:last-c
-0000b2b0: 6869 6c64 2c2e 646a 616e 676f 636d 732d  hild,.djangocms-
-0000b2c0: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-0000b2d0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000b2e0: 7873 5f63 6f6c 202e 6669 656c 6442 6f78  xs_col .fieldBox
-0000b2f0: 3a6c 6173 742d 6368 696c 642c 2e64 6a61  :last-child,.dja
-0000b300: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000b310: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000b320: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
-0000b330: 656c 642d 626f 783a 6c61 7374 2d63 6869  eld-box:last-chi
-0000b340: 6c64 2c2e 646a 616e 676f 636d 732d 6672  ld,.djangocms-fr
-0000b350: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-0000b360: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000b370: 5f6d 6520 2e66 6965 6c64 426f 783a 6c61  _me .fieldBox:la
-0000b380: 7374 2d63 6869 6c64 2c2e 646a 616e 676f  st-child,.django
-0000b390: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000b3a0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000b3b0: 656c 642d 7873 5f6d 7320 2e66 6965 6c64  eld-xs_ms .field
-0000b3c0: 2d62 6f78 3a6c 6173 742d 6368 696c 642c  -box:last-child,
-0000b3d0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000b3e0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000b3f0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d73  -row.field-xs_ms
-0000b400: 202e 6669 656c 6442 6f78 3a6c 6173 742d   .fieldBox:last-
-0000b410: 6368 696c 642c 2e64 6a61 6e67 6f63 6d73  child,.djangocms
-0000b420: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000b430: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000b440: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
-0000b450: 642d 626f 783a 6c61 7374 2d63 6869 6c64  d-box:last-child
-0000b460: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000b470: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000b480: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-0000b490: 6666 7365 7420 2e66 6965 6c64 426f 783a  ffset .fieldBox:
-0000b4a0: 6c61 7374 2d63 6869 6c64 2c2e 646a 616e  last-child,.djan
-0000b4b0: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
-0000b4c0: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
-0000b4d0: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
-0000b4e0: 6669 656c 642d 626f 783a 6c61 7374 2d63  field-box:last-c
-0000b4f0: 6869 6c64 2c2e 646a 616e 676f 636d 732d  hild,.djangocms-
-0000b500: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-0000b510: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000b520: 7873 5f6f 7264 6572 202e 6669 656c 6442  xs_order .fieldB
-0000b530: 6f78 3a6c 6173 742d 6368 696c 642c 2e64  ox:last-child,.d
-0000b540: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000b550: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-0000b560: 6669 656c 642d 726f 775f 636f 6c73 5f78  field-row_cols_x
-0000b570: 7320 2e66 6965 6c64 2d62 6f78 3a6c 6173  s .field-box:las
-0000b580: 742d 6368 696c 642c 2e64 6a61 6e67 6f63  t-child,.djangoc
-0000b590: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-0000b5a0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000b5b0: 726f 775f 636f 6c73 5f78 7320 2e66 6965  row_cols_xs .fie
-0000b5c0: 6c64 426f 783a 6c61 7374 2d63 6869 6c64  ldBox:last-child
-0000b5d0: 7b62 6f72 6465 722d 696e 6c69 6e65 2d65  {border-inline-e
-0000b5e0: 6e64 3a6e 6f6e 657d 2e64 6a61 6e67 6f63  nd:none}.djangoc
-0000b5f0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000b600: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000b610: 6c64 2d78 735f 636f 6c20 2e65 7272 6f72  ld-xs_col .error
-0000b620: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
-0000b630: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000b640: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000b650: 6d65 202e 6572 726f 7273 2c2e 646a 616e  me .errors,.djan
-0000b660: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
-0000b670: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
-0000b680: 6669 656c 642d 7873 5f6d 7320 2e65 7272  field-xs_ms .err
-0000b690: 6f72 732c 2e64 6a61 6e67 6f63 6d73 2d66  ors,.djangocms-f
-0000b6a0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000b6b0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000b6c0: 735f 6f66 6673 6574 202e 6572 726f 7273  s_offset .errors
-0000b6d0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000b6e0: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000b6f0: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-0000b700: 7264 6572 202e 6572 726f 7273 2c2e 646a  rder .errors,.dj
-0000b710: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000b720: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
-0000b730: 6965 6c64 2d72 6f77 5f63 6f6c 735f 7873  ield-row_cols_xs
-0000b740: 202e 6572 726f 7273 7b6d 6172 6769 6e2d   .errors{margin-
-0000b750: 626f 7474 6f6d 3a30 7d2e 646a 616e 676f  bottom:0}.django
-0000b760: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000b770: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000b780: 656c 642d 7873 5f63 6f6c 202e 6572 726f  eld-xs_col .erro
-0000b790: 726c 6973 742c 2e64 6a61 6e67 6f63 6d73  rlist,.djangocms
-0000b7a0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000b7b0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000b7c0: 2d78 735f 6d65 202e 6572 726f 726c 6973  -xs_me .errorlis
-0000b7d0: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
-0000b7e0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000b7f0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000b800: 6d73 202e 6572 726f 726c 6973 742c 2e64  ms .errorlist,.d
-0000b810: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000b820: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000b830: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
-0000b840: 6574 202e 6572 726f 726c 6973 742c 2e64  et .errorlist,.d
-0000b850: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000b860: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000b870: 6f77 2e66 6965 6c64 2d78 735f 6f72 6465  ow.field-xs_orde
-0000b880: 7220 2e65 7272 6f72 6c69 7374 2c2e 646a  r .errorlist,.dj
-0000b890: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000b8a0: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
-0000b8b0: 6965 6c64 2d72 6f77 5f63 6f6c 735f 7873  ield-row_cols_xs
-0000b8c0: 202e 6572 726f 726c 6973 747b 706f 7369   .errorlist{posi
-0000b8d0: 7469 6f6e 3a61 6273 6f6c 7574 6521 696d  tion:absolute!im
-0000b8e0: 706f 7274 616e 743b 7769 6474 683a 3170  portant;width:1p
-0000b8f0: 7821 696d 706f 7274 616e 743b 6865 6967  x!important;heig
-0000b900: 6874 3a31 7078 2169 6d70 6f72 7461 6e74  ht:1px!important
-0000b910: 3b70 6164 6469 6e67 3a30 2169 6d70 6f72  ;padding:0!impor
-0000b920: 7461 6e74 3b6d 6172 6769 6e3a 2d31 7078  tant;margin:-1px
-0000b930: 2169 6d70 6f72 7461 6e74 3b6f 7665 7266  !important;overf
-0000b940: 6c6f 773a 6869 6464 656e 2169 6d70 6f72  low:hidden!impor
-0000b950: 7461 6e74 3b63 6c69 703a 7265 6374 2830  tant;clip:rect(0
-0000b960: 2c30 2c30 2c30 2921 696d 706f 7274 616e  ,0,0,0)!importan
-0000b970: 743b 7768 6974 652d 7370 6163 653a 6e6f  t;white-space:no
-0000b980: 7772 6170 2169 6d70 6f72 7461 6e74 3b62  wrap!important;b
-0000b990: 6f72 6465 723a 3021 696d 706f 7274 616e  order:0!importan
-0000b9a0: 747d 2e64 6a61 6e67 6f63 6d73 2d66 726f  t}.djangocms-fro
-0000b9b0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000b9c0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000b9d0: 636f 6c2e 6669 656c 642d 7873 5f6d 6520  col.field-xs_me 
-0000b9e0: 2e66 6965 6c64 2d62 6f78 2c2e 646a 616e  .field-box,.djan
-0000b9f0: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
-0000ba00: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
-0000ba10: 6669 656c 642d 7873 5f6d 652e 6669 656c  field-xs_me.fiel
-0000ba20: 642d 7873 5f6d 6520 2e66 6965 6c64 2d62  d-xs_me .field-b
-0000ba30: 6f78 2c2e 646a 616e 676f 636d 732d 6672  ox,.djangocms-fr
-0000ba40: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-0000ba50: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000ba60: 5f6d 732e 6669 656c 642d 7873 5f6d 6520  _ms.field-xs_me 
-0000ba70: 2e66 6965 6c64 2d62 6f78 2c2e 646a 616e  .field-box,.djan
-0000ba80: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
-0000ba90: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
-0000baa0: 6669 656c 642d 7873 5f6f 6666 7365 742e  field-xs_offset.
-0000bab0: 6669 656c 642d 7873 5f6d 6520 2e66 6965  field-xs_me .fie
-0000bac0: 6c64 2d62 6f78 2c2e 646a 616e 676f 636d  ld-box,.djangocm
-0000bad0: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
-0000bae0: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
-0000baf0: 642d 7873 5f6f 7264 6572 2e66 6965 6c64  d-xs_order.field
-0000bb00: 2d78 735f 6d65 202e 6669 656c 642d 626f  -xs_me .field-bo
-0000bb10: 782c 2e64 6a61 6e67 6f63 6d73 2d66 726f  x,.djangocms-fro
-0000bb20: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-0000bb30: 726f 772e 6669 656c 642d 726f 775f 636f  row.field-row_co
-0000bb40: 6c73 5f78 732e 6669 656c 642d 7873 5f6d  ls_xs.field-xs_m
-0000bb50: 6520 2e66 6965 6c64 2d62 6f78 7b62 6f72  e .field-box{bor
-0000bb60: 6465 722d 626f 7474 6f6d 3a6e 6f6e 657d  der-bottom:none}
-0000bb70: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000bb80: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000bb90: 2d72 6f77 2e66 6965 6c64 2d78 735f 636f  -row.field-xs_co
-0000bba0: 6c20 2e66 6965 6c64 2d62 6f78 2d6c 6162  l .field-box-lab
-0000bbb0: 656c 2c2e 646a 616e 676f 636d 732d 6672  el,.djangocms-fr
-0000bbc0: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-0000bbd0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000bbe0: 5f6d 6520 2e66 6965 6c64 2d62 6f78 2d6c  _me .field-box-l
-0000bbf0: 6162 656c 2c2e 646a 616e 676f 636d 732d  abel,.djangocms-
-0000bc00: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-0000bc10: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000bc20: 7873 5f6d 7320 2e66 6965 6c64 2d62 6f78  xs_ms .field-box
-0000bc30: 2d6c 6162 656c 2c2e 646a 616e 676f 636d  -label,.djangocm
-0000bc40: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
-0000bc50: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
-0000bc60: 642d 7873 5f6f 6666 7365 7420 2e66 6965  d-xs_offset .fie
-0000bc70: 6c64 2d62 6f78 2d6c 6162 656c 2c2e 646a  ld-box-label,.dj
-0000bc80: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000bc90: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
-0000bca0: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
-0000bcb0: 202e 6669 656c 642d 626f 782d 6c61 6265   .field-box-labe
-0000bcc0: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
-0000bcd0: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-0000bce0: 726f 772e 6669 656c 642d 726f 775f 636f  row.field-row_co
-0000bcf0: 6c73 5f78 7320 2e66 6965 6c64 2d62 6f78  ls_xs .field-box
-0000bd00: 2d6c 6162 656c 7b64 6973 706c 6179 3a2d  -label{display:-
-0000bd10: 6d73 2d66 6c65 7862 6f78 3b64 6973 706c  ms-flexbox;displ
-0000bd20: 6179 3a66 6c65 783b 6d61 7267 696e 2d74  ay:flex;margin-t
-0000bd30: 6f70 3a61 7574 6f3b 636f 6c6f 723a 2339  op:auto;color:#9
-0000bd40: 3939 7d2e 646a 616e 676f 636d 732d 6672  99}.djangocms-fr
-0000bd50: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-0000bd60: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000bd70: 5f63 6f6c 202e 6669 656c 642d 626f 782d  _col .field-box-
-0000bd80: 6c61 6265 6c20 612c 2e64 6a61 6e67 6f63  label a,.djangoc
-0000bd90: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000bda0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000bdb0: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
-0000bdc0: 626f 782d 6c61 6265 6c20 612c 2e64 6a61  box-label a,.dja
-0000bdd0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000bde0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000bdf0: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
-0000be00: 656c 642d 626f 782d 6c61 6265 6c20 612c  eld-box-label a,
-0000be10: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000be20: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000be30: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f66  -row.field-xs_of
-0000be40: 6673 6574 202e 6669 656c 642d 626f 782d  fset .field-box-
-0000be50: 6c61 6265 6c20 612c 2e64 6a61 6e67 6f63  label a,.djangoc
-0000be60: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000be70: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000be80: 6c64 2d78 735f 6f72 6465 7220 2e66 6965  ld-xs_order .fie
-0000be90: 6c64 2d62 6f78 2d6c 6162 656c 2061 2c2e  ld-box-label a,.
-0000bea0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000beb0: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
-0000bec0: 2e66 6965 6c64 2d72 6f77 5f63 6f6c 735f  .field-row_cols_
-0000bed0: 7873 202e 6669 656c 642d 626f 782d 6c61  xs .field-box-la
-0000bee0: 6265 6c20 617b 7769 6474 683a 3130 3025  bel a{width:100%
-0000bef0: 3b6d 6172 6769 6e2d 746f 703a 6175 746f  ;margin-top:auto
-0000bf00: 3b63 6f6c 6f72 3a23 3939 397d 2e64 6a61  ;color:#999}.dja
-0000bf10: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000bf20: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000bf30: 2e66 6965 6c64 2d78 735f 636f 6c20 2e66  .field-xs_col .f
-0000bf40: 6965 6c64 2d62 6f78 2d6c 6162 656c 2061  ield-box-label a
-0000bf50: 2061 2c2e 646a 616e 676f 636d 732d 6672   a,.djangocms-fr
-0000bf60: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-0000bf70: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000bf80: 5f6d 6520 2e66 6965 6c64 2d62 6f78 2d6c  _me .field-box-l
-0000bf90: 6162 656c 2061 2061 2c2e 646a 616e 676f  abel a a,.django
-0000bfa0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000bfb0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000bfc0: 656c 642d 7873 5f6d 7320 2e66 6965 6c64  eld-xs_ms .field
-0000bfd0: 2d62 6f78 2d6c 6162 656c 2061 2061 2c2e  -box-label a a,.
-0000bfe0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000bff0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
-0000c000: 726f 772e 6669 656c 642d 7873 5f6f 6666  row.field-xs_off
-0000c010: 7365 7420 2e66 6965 6c64 2d62 6f78 2d6c  set .field-box-l
-0000c020: 6162 656c 2061 2061 2c2e 646a 616e 676f  abel a a,.django
-0000c030: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000c040: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000c050: 656c 642d 7873 5f6f 7264 6572 202e 6669  eld-xs_order .fi
-0000c060: 656c 642d 626f 782d 6c61 6265 6c20 6120  eld-box-label a 
-0000c070: 612c 2e64 6a61 6e67 6f63 6d73 2d66 726f  a,.djangocms-fro
-0000c080: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-0000c090: 726f 772e 6669 656c 642d 726f 775f 636f  row.field-row_co
-0000c0a0: 6c73 5f78 7320 2e66 6965 6c64 2d62 6f78  ls_xs .field-box
-0000c0b0: 2d6c 6162 656c 2061 2061 7b77 6964 7468  -label a a{width
-0000c0c0: 3a31 3030 253b 6d61 7267 696e 2d74 6f70  :100%;margin-top
-0000c0d0: 3a61 7574 6f7d 2e64 6a61 6e67 6f63 6d73  :auto}.djangocms
-0000c0e0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000c0f0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000c100: 2d78 735f 636f 6c20 2e66 6965 6c64 2d6c  -xs_col .field-l
-0000c110: 675f 6d65 2c2e 646a 616e 676f 636d 732d  g_me,.djangocms-
-0000c120: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-0000c130: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000c140: 7873 5f63 6f6c 202e 6669 656c 642d 6c67  xs_col .field-lg
-0000c150: 5f6d 732c 2e64 6a61 6e67 6f63 6d73 2d66  _ms,.djangocms-f
-0000c160: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000c170: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000c180: 735f 636f 6c20 2e66 6965 6c64 2d6d 645f  s_col .field-md_
-0000c190: 6d65 2c2e 646a 616e 676f 636d 732d 6672  me,.djangocms-fr
-0000c1a0: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-0000c1b0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000c1c0: 5f63 6f6c 202e 6669 656c 642d 6d64 5f6d  _col .field-md_m
-0000c1d0: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
-0000c1e0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000c1f0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000c200: 636f 6c20 2e66 6965 6c64 2d73 6d5f 6d65  col .field-sm_me
-0000c210: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000c220: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000c230: 6d2d 726f 772e 6669 656c 642d 7873 5f63  m-row.field-xs_c
-0000c240: 6f6c 202e 6669 656c 642d 736d 5f6d 732c  ol .field-sm_ms,
-0000c250: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000c260: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000c270: 2d72 6f77 2e66 6965 6c64 2d78 735f 636f  -row.field-xs_co
-0000c280: 6c20 2e66 6965 6c64 2d78 6c5f 6d65 2c2e  l .field-xl_me,.
-0000c290: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000c2a0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
-0000c2b0: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
-0000c2c0: 202e 6669 656c 642d 786c 5f6d 732c 2e64   .field-xl_ms,.d
-0000c2d0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000c2e0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000c2f0: 6f77 2e66 6965 6c64 2d78 735f 636f 6c20  ow.field-xs_col 
-0000c300: 2e66 6965 6c64 2d78 735f 6d65 2c2e 646a  .field-xs_me,.dj
-0000c310: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000c320: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
-0000c330: 772e 6669 656c 642d 7873 5f63 6f6c 202e  w.field-xs_col .
-0000c340: 6669 656c 642d 7873 5f6d 732c 2e64 6a61  field-xs_ms,.dja
-0000c350: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000c360: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000c370: 2e66 6965 6c64 2d78 735f 636f 6c20 2e66  .field-xs_col .f
-0000c380: 6965 6c64 2d78 786c 5f6d 652c 2e64 6a61  ield-xxl_me,.dja
-0000c390: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000c3a0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000c3b0: 2e66 6965 6c64 2d78 735f 636f 6c20 2e66  .field-xs_col .f
-0000c3c0: 6965 6c64 2d78 786c 5f6d 732c 2e64 6a61  ield-xxl_ms,.dja
-0000c3d0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000c3e0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000c3f0: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
-0000c400: 656c 642d 6c67 5f6d 652c 2e64 6a61 6e67  eld-lg_me,.djang
-0000c410: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000c420: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000c430: 6965 6c64 2d78 735f 6d65 202e 6669 656c  ield-xs_me .fiel
-0000c440: 642d 6c67 5f6d 732c 2e64 6a61 6e67 6f63  d-lg_ms,.djangoc
-0000c450: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000c460: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000c470: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
-0000c480: 6d64 5f6d 652c 2e64 6a61 6e67 6f63 6d73  md_me,.djangocms
-0000c490: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000c4a0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000c4b0: 2d78 735f 6d65 202e 6669 656c 642d 6d64  -xs_me .field-md
-0000c4c0: 5f6d 732c 2e64 6a61 6e67 6f63 6d73 2d66  _ms,.djangocms-f
-0000c4d0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000c4e0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000c4f0: 735f 6d65 202e 6669 656c 642d 736d 5f6d  s_me .field-sm_m
-0000c500: 652c 2e64 6a61 6e67 6f63 6d73 2d66 726f  e,.djangocms-fro
-0000c510: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000c520: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000c530: 6d65 202e 6669 656c 642d 736d 5f6d 732c  me .field-sm_ms,
-0000c540: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000c550: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000c560: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
-0000c570: 202e 6669 656c 642d 786c 5f6d 652c 2e64   .field-xl_me,.d
-0000c580: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000c590: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000c5a0: 6f77 2e66 6965 6c64 2d78 735f 6d65 202e  ow.field-xs_me .
-0000c5b0: 6669 656c 642d 786c 5f6d 732c 2e64 6a61  field-xl_ms,.dja
-0000c5c0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000c5d0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000c5e0: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
-0000c5f0: 656c 642d 7873 5f6d 652c 2e64 6a61 6e67  eld-xs_me,.djang
-0000c600: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000c610: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000c620: 6965 6c64 2d78 735f 6d65 202e 6669 656c  ield-xs_me .fiel
-0000c630: 642d 7873 5f6d 732c 2e64 6a61 6e67 6f63  d-xs_ms,.djangoc
-0000c640: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000c650: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000c660: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
-0000c670: 7878 6c5f 6d65 2c2e 646a 616e 676f 636d  xxl_me,.djangocm
-0000c680: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
-0000c690: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
-0000c6a0: 642d 7873 5f6d 6520 2e66 6965 6c64 2d78  d-xs_me .field-x
-0000c6b0: 786c 5f6d 732c 2e64 6a61 6e67 6f63 6d73  xl_ms,.djangocms
-0000c6c0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000c6d0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000c6e0: 2d78 735f 6d73 202e 6669 656c 642d 6c67  -xs_ms .field-lg
-0000c6f0: 5f6d 652c 2e64 6a61 6e67 6f63 6d73 2d66  _me,.djangocms-f
-0000c700: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000c710: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000c720: 735f 6d73 202e 6669 656c 642d 6c67 5f6d  s_ms .field-lg_m
-0000c730: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
-0000c740: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000c750: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000c760: 6d73 202e 6669 656c 642d 6d64 5f6d 652c  ms .field-md_me,
-0000c770: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000c780: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000c790: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d73  -row.field-xs_ms
-0000c7a0: 202e 6669 656c 642d 6d64 5f6d 732c 2e64   .field-md_ms,.d
-0000c7b0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000c7c0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000c7d0: 6f77 2e66 6965 6c64 2d78 735f 6d73 202e  ow.field-xs_ms .
-0000c7e0: 6669 656c 642d 736d 5f6d 652c 2e64 6a61  field-sm_me,.dja
-0000c7f0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000c800: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000c810: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
-0000c820: 656c 642d 736d 5f6d 732c 2e64 6a61 6e67  eld-sm_ms,.djang
-0000c830: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000c840: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000c850: 6965 6c64 2d78 735f 6d73 202e 6669 656c  ield-xs_ms .fiel
-0000c860: 642d 786c 5f6d 652c 2e64 6a61 6e67 6f63  d-xl_me,.djangoc
-0000c870: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000c880: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000c890: 6c64 2d78 735f 6d73 202e 6669 656c 642d  ld-xs_ms .field-
-0000c8a0: 786c 5f6d 732c 2e64 6a61 6e67 6f63 6d73  xl_ms,.djangocms
-0000c8b0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000c8c0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000c8d0: 2d78 735f 6d73 202e 6669 656c 642d 7873  -xs_ms .field-xs
-0000c8e0: 5f6d 652c 2e64 6a61 6e67 6f63 6d73 2d66  _me,.djangocms-f
-0000c8f0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000c900: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000c910: 735f 6d73 202e 6669 656c 642d 7873 5f6d  s_ms .field-xs_m
-0000c920: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
-0000c930: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000c940: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000c950: 6d73 202e 6669 656c 642d 7878 6c5f 6d65  ms .field-xxl_me
-0000c960: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000c970: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000c980: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
-0000c990: 7320 2e66 6965 6c64 2d78 786c 5f6d 732c  s .field-xxl_ms,
-0000c9a0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000c9b0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000c9c0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f66  -row.field-xs_of
-0000c9d0: 6673 6574 202e 6669 656c 642d 6c67 5f6d  fset .field-lg_m
-0000c9e0: 652c 2e64 6a61 6e67 6f63 6d73 2d66 726f  e,.djangocms-fro
-0000c9f0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000ca00: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000ca10: 6f66 6673 6574 202e 6669 656c 642d 6c67  offset .field-lg
-0000ca20: 5f6d 732c 2e64 6a61 6e67 6f63 6d73 2d66  _ms,.djangocms-f
-0000ca30: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000ca40: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000ca50: 735f 6f66 6673 6574 202e 6669 656c 642d  s_offset .field-
-0000ca60: 6d64 5f6d 652c 2e64 6a61 6e67 6f63 6d73  md_me,.djangocms
-0000ca70: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000ca80: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000ca90: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
-0000caa0: 642d 6d64 5f6d 732c 2e64 6a61 6e67 6f63  d-md_ms,.djangoc
-0000cab0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000cac0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000cad0: 6c64 2d78 735f 6f66 6673 6574 202e 6669  ld-xs_offset .fi
-0000cae0: 656c 642d 736d 5f6d 652c 2e64 6a61 6e67  eld-sm_me,.djang
-0000caf0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000cb00: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000cb10: 6965 6c64 2d78 735f 6f66 6673 6574 202e  ield-xs_offset .
-0000cb20: 6669 656c 642d 736d 5f6d 732c 2e64 6a61  field-sm_ms,.dja
-0000cb30: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000cb40: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000cb50: 2e66 6965 6c64 2d78 735f 6f66 6673 6574  .field-xs_offset
-0000cb60: 202e 6669 656c 642d 786c 5f6d 652c 2e64   .field-xl_me,.d
-0000cb70: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000cb80: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000cb90: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
-0000cba0: 6574 202e 6669 656c 642d 786c 5f6d 732c  et .field-xl_ms,
-0000cbb0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000cbc0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000cbd0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f66  -row.field-xs_of
-0000cbe0: 6673 6574 202e 6669 656c 642d 7873 5f6d  fset .field-xs_m
-0000cbf0: 652c 2e64 6a61 6e67 6f63 6d73 2d66 726f  e,.djangocms-fro
-0000cc00: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000cc10: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000cc20: 6f66 6673 6574 202e 6669 656c 642d 7873  offset .field-xs
-0000cc30: 5f6d 732c 2e64 6a61 6e67 6f63 6d73 2d66  _ms,.djangocms-f
-0000cc40: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000cc50: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000cc60: 735f 6f66 6673 6574 202e 6669 656c 642d  s_offset .field-
-0000cc70: 7878 6c5f 6d65 2c2e 646a 616e 676f 636d  xxl_me,.djangocm
-0000cc80: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
-0000cc90: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
-0000cca0: 642d 7873 5f6f 6666 7365 7420 2e66 6965  d-xs_offset .fie
-0000ccb0: 6c64 2d78 786c 5f6d 732c 2e64 6a61 6e67  ld-xxl_ms,.djang
-0000ccc0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000ccd0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000cce0: 6965 6c64 2d78 735f 6f72 6465 7220 2e66  ield-xs_order .f
-0000ccf0: 6965 6c64 2d6c 675f 6d65 2c2e 646a 616e  ield-lg_me,.djan
-0000cd00: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
-0000cd10: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
-0000cd20: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
-0000cd30: 6669 656c 642d 6c67 5f6d 732c 2e64 6a61  field-lg_ms,.dja
-0000cd40: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000cd50: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000cd60: 2e66 6965 6c64 2d78 735f 6f72 6465 7220  .field-xs_order 
-0000cd70: 2e66 6965 6c64 2d6d 645f 6d65 2c2e 646a  .field-md_me,.dj
-0000cd80: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000cd90: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
-0000cda0: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
-0000cdb0: 202e 6669 656c 642d 6d64 5f6d 732c 2e64   .field-md_ms,.d
-0000cdc0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000cdd0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000cde0: 6f77 2e66 6965 6c64 2d78 735f 6f72 6465  ow.field-xs_orde
-0000cdf0: 7220 2e66 6965 6c64 2d73 6d5f 6d65 2c2e  r .field-sm_me,.
-0000ce00: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000ce10: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
-0000ce20: 726f 772e 6669 656c 642d 7873 5f6f 7264  row.field-xs_ord
-0000ce30: 6572 202e 6669 656c 642d 736d 5f6d 732c  er .field-sm_ms,
-0000ce40: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000ce50: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000ce60: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f72  -row.field-xs_or
-0000ce70: 6465 7220 2e66 6965 6c64 2d78 6c5f 6d65  der .field-xl_me
-0000ce80: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000ce90: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000cea0: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-0000ceb0: 7264 6572 202e 6669 656c 642d 786c 5f6d  rder .field-xl_m
-0000cec0: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
-0000ced0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000cee0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000cef0: 6f72 6465 7220 2e66 6965 6c64 2d78 735f  order .field-xs_
-0000cf00: 6d65 2c2e 646a 616e 676f 636d 732d 6672  me,.djangocms-fr
-0000cf10: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-0000cf20: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000cf30: 5f6f 7264 6572 202e 6669 656c 642d 7873  _order .field-xs
-0000cf40: 5f6d 732c 2e64 6a61 6e67 6f63 6d73 2d66  _ms,.djangocms-f
-0000cf50: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000cf60: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000cf70: 735f 6f72 6465 7220 2e66 6965 6c64 2d78  s_order .field-x
-0000cf80: 786c 5f6d 652c 2e64 6a61 6e67 6f63 6d73  xl_me,.djangocms
-0000cf90: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000cfa0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000cfb0: 2d78 735f 6f72 6465 7220 2e66 6965 6c64  -xs_order .field
-0000cfc0: 2d78 786c 5f6d 732c 2e64 6a61 6e67 6f63  -xxl_ms,.djangoc
-0000cfd0: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-0000cfe0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000cff0: 726f 775f 636f 6c73 5f78 7320 2e66 6965  row_cols_xs .fie
-0000d000: 6c64 2d6c 675f 6d65 2c2e 646a 616e 676f  ld-lg_me,.django
-0000d010: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
-0000d020: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000d030: 2d72 6f77 5f63 6f6c 735f 7873 202e 6669  -row_cols_xs .fi
-0000d040: 656c 642d 6c67 5f6d 732c 2e64 6a61 6e67  eld-lg_ms,.djang
-0000d050: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-0000d060: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-0000d070: 642d 726f 775f 636f 6c73 5f78 7320 2e66  d-row_cols_xs .f
-0000d080: 6965 6c64 2d6d 645f 6d65 2c2e 646a 616e  ield-md_me,.djan
-0000d090: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
-0000d0a0: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
-0000d0b0: 6c64 2d72 6f77 5f63 6f6c 735f 7873 202e  ld-row_cols_xs .
-0000d0c0: 6669 656c 642d 6d64 5f6d 732c 2e64 6a61  field-md_ms,.dja
-0000d0d0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000d0e0: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
-0000d0f0: 656c 642d 726f 775f 636f 6c73 5f78 7320  eld-row_cols_xs 
-0000d100: 2e66 6965 6c64 2d73 6d5f 6d65 2c2e 646a  .field-sm_me,.dj
-0000d110: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000d120: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
-0000d130: 6965 6c64 2d72 6f77 5f63 6f6c 735f 7873  ield-row_cols_xs
-0000d140: 202e 6669 656c 642d 736d 5f6d 732c 2e64   .field-sm_ms,.d
-0000d150: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000d160: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-0000d170: 6669 656c 642d 726f 775f 636f 6c73 5f78  field-row_cols_x
-0000d180: 7320 2e66 6965 6c64 2d78 6c5f 6d65 2c2e  s .field-xl_me,.
-0000d190: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000d1a0: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
-0000d1b0: 2e66 6965 6c64 2d72 6f77 5f63 6f6c 735f  .field-row_cols_
-0000d1c0: 7873 202e 6669 656c 642d 786c 5f6d 732c  xs .field-xl_ms,
-0000d1d0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000d1e0: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
-0000d1f0: 772e 6669 656c 642d 726f 775f 636f 6c73  w.field-row_cols
-0000d200: 5f78 7320 2e66 6965 6c64 2d78 735f 6d65  _xs .field-xs_me
-0000d210: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000d220: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
-0000d230: 6f77 2e66 6965 6c64 2d72 6f77 5f63 6f6c  ow.field-row_col
-0000d240: 735f 7873 202e 6669 656c 642d 7873 5f6d  s_xs .field-xs_m
-0000d250: 732c 2e64 6a61 6e67 6f63 6d73 2d66 726f  s,.djangocms-fro
-0000d260: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-0000d270: 726f 772e 6669 656c 642d 726f 775f 636f  row.field-row_co
-0000d280: 6c73 5f78 7320 2e66 6965 6c64 2d78 786c  ls_xs .field-xxl
-0000d290: 5f6d 652c 2e64 6a61 6e67 6f63 6d73 2d66  _me,.djangocms-f
-0000d2a0: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
-0000d2b0: 6d2d 726f 772e 6669 656c 642d 726f 775f  m-row.field-row_
-0000d2c0: 636f 6c73 5f78 7320 2e66 6965 6c64 2d78  cols_xs .field-x
-0000d2d0: 786c 5f6d 737b 7465 7874 2d61 6c69 676e  xl_ms{text-align
-0000d2e0: 3a73 7461 7274 7d2e 646a 616e 676f 636d  :start}.djangocm
-0000d2f0: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
-0000d300: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
-0000d310: 642d 7873 5f63 6f6c 202e 6669 656c 642d  d-xs_col .field-
-0000d320: 6c67 5f6d 6520 6c61 6265 6c2c 2e64 6a61  lg_me label,.dja
-0000d330: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000d340: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000d350: 2e66 6965 6c64 2d78 735f 636f 6c20 2e66  .field-xs_col .f
-0000d360: 6965 6c64 2d6c 675f 6d73 206c 6162 656c  ield-lg_ms label
-0000d370: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000d380: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000d390: 6d2d 726f 772e 6669 656c 642d 7873 5f63  m-row.field-xs_c
-0000d3a0: 6f6c 202e 6669 656c 642d 6d64 5f6d 6520  ol .field-md_me 
-0000d3b0: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-0000d3c0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000d3d0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000d3e0: 2d78 735f 636f 6c20 2e66 6965 6c64 2d6d  -xs_col .field-m
-0000d3f0: 645f 6d73 206c 6162 656c 2c2e 646a 616e  d_ms label,.djan
-0000d400: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
-0000d410: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
-0000d420: 6669 656c 642d 7873 5f63 6f6c 202e 6669  field-xs_col .fi
-0000d430: 656c 642d 736d 5f6d 6520 6c61 6265 6c2c  eld-sm_me label,
-0000d440: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000d450: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000d460: 2d72 6f77 2e66 6965 6c64 2d78 735f 636f  -row.field-xs_co
-0000d470: 6c20 2e66 6965 6c64 2d73 6d5f 6d73 206c  l .field-sm_ms l
-0000d480: 6162 656c 2c2e 646a 616e 676f 636d 732d  abel,.djangocms-
-0000d490: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-0000d4a0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000d4b0: 7873 5f63 6f6c 202e 6669 656c 642d 786c  xs_col .field-xl
-0000d4c0: 5f6d 6520 6c61 6265 6c2c 2e64 6a61 6e67  _me label,.djang
-0000d4d0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000d4e0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000d4f0: 6965 6c64 2d78 735f 636f 6c20 2e66 6965  ield-xs_col .fie
-0000d500: 6c64 2d78 6c5f 6d73 206c 6162 656c 2c2e  ld-xl_ms label,.
-0000d510: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000d520: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
-0000d530: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
-0000d540: 202e 6669 656c 642d 7873 5f6d 6520 6c61   .field-xs_me la
-0000d550: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
-0000d560: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000d570: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000d580: 735f 636f 6c20 2e66 6965 6c64 2d78 735f  s_col .field-xs_
-0000d590: 6d73 206c 6162 656c 2c2e 646a 616e 676f  ms label,.django
-0000d5a0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000d5b0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000d5c0: 656c 642d 7873 5f63 6f6c 202e 6669 656c  eld-xs_col .fiel
-0000d5d0: 642d 7878 6c5f 6d65 206c 6162 656c 2c2e  d-xxl_me label,.
-0000d5e0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000d5f0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
-0000d600: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
-0000d610: 202e 6669 656c 642d 7878 6c5f 6d73 206c   .field-xxl_ms l
-0000d620: 6162 656c 2c2e 646a 616e 676f 636d 732d  abel,.djangocms-
-0000d630: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-0000d640: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000d650: 7873 5f6d 6520 2e66 6965 6c64 2d6c 675f  xs_me .field-lg_
-0000d660: 6d65 206c 6162 656c 2c2e 646a 616e 676f  me label,.django
-0000d670: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000d680: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000d690: 656c 642d 7873 5f6d 6520 2e66 6965 6c64  eld-xs_me .field
-0000d6a0: 2d6c 675f 6d73 206c 6162 656c 2c2e 646a  -lg_ms label,.dj
-0000d6b0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000d6c0: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
-0000d6d0: 772e 6669 656c 642d 7873 5f6d 6520 2e66  w.field-xs_me .f
-0000d6e0: 6965 6c64 2d6d 645f 6d65 206c 6162 656c  ield-md_me label
-0000d6f0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000d700: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000d710: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
-0000d720: 6520 2e66 6965 6c64 2d6d 645f 6d73 206c  e .field-md_ms l
-0000d730: 6162 656c 2c2e 646a 616e 676f 636d 732d  abel,.djangocms-
-0000d740: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-0000d750: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000d760: 7873 5f6d 6520 2e66 6965 6c64 2d73 6d5f  xs_me .field-sm_
-0000d770: 6d65 206c 6162 656c 2c2e 646a 616e 676f  me label,.django
-0000d780: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000d790: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000d7a0: 656c 642d 7873 5f6d 6520 2e66 6965 6c64  eld-xs_me .field
-0000d7b0: 2d73 6d5f 6d73 206c 6162 656c 2c2e 646a  -sm_ms label,.dj
-0000d7c0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000d7d0: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
-0000d7e0: 772e 6669 656c 642d 7873 5f6d 6520 2e66  w.field-xs_me .f
-0000d7f0: 6965 6c64 2d78 6c5f 6d65 206c 6162 656c  ield-xl_me label
-0000d800: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000d810: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000d820: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
-0000d830: 6520 2e66 6965 6c64 2d78 6c5f 6d73 206c  e .field-xl_ms l
-0000d840: 6162 656c 2c2e 646a 616e 676f 636d 732d  abel,.djangocms-
-0000d850: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-0000d860: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000d870: 7873 5f6d 6520 2e66 6965 6c64 2d78 735f  xs_me .field-xs_
-0000d880: 6d65 206c 6162 656c 2c2e 646a 616e 676f  me label,.django
-0000d890: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000d8a0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000d8b0: 656c 642d 7873 5f6d 6520 2e66 6965 6c64  eld-xs_me .field
-0000d8c0: 2d78 735f 6d73 206c 6162 656c 2c2e 646a  -xs_ms label,.dj
-0000d8d0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000d8e0: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
-0000d8f0: 772e 6669 656c 642d 7873 5f6d 6520 2e66  w.field-xs_me .f
-0000d900: 6965 6c64 2d78 786c 5f6d 6520 6c61 6265  ield-xxl_me labe
-0000d910: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
-0000d920: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000d930: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000d940: 6d65 202e 6669 656c 642d 7878 6c5f 6d73  me .field-xxl_ms
-0000d950: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
-0000d960: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
-0000d970: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
-0000d980: 642d 7873 5f6d 7320 2e66 6965 6c64 2d6c  d-xs_ms .field-l
-0000d990: 675f 6d65 206c 6162 656c 2c2e 646a 616e  g_me label,.djan
-0000d9a0: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
-0000d9b0: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
-0000d9c0: 6669 656c 642d 7873 5f6d 7320 2e66 6965  field-xs_ms .fie
-0000d9d0: 6c64 2d6c 675f 6d73 206c 6162 656c 2c2e  ld-lg_ms label,.
-0000d9e0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000d9f0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
-0000da00: 726f 772e 6669 656c 642d 7873 5f6d 7320  row.field-xs_ms 
-0000da10: 2e66 6965 6c64 2d6d 645f 6d65 206c 6162  .field-md_me lab
-0000da20: 656c 2c2e 646a 616e 676f 636d 732d 6672  el,.djangocms-fr
-0000da30: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-0000da40: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000da50: 5f6d 7320 2e66 6965 6c64 2d6d 645f 6d73  _ms .field-md_ms
-0000da60: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
-0000da70: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
-0000da80: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
-0000da90: 642d 7873 5f6d 7320 2e66 6965 6c64 2d73  d-xs_ms .field-s
-0000daa0: 6d5f 6d65 206c 6162 656c 2c2e 646a 616e  m_me label,.djan
-0000dab0: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
-0000dac0: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
-0000dad0: 6669 656c 642d 7873 5f6d 7320 2e66 6965  field-xs_ms .fie
-0000dae0: 6c64 2d73 6d5f 6d73 206c 6162 656c 2c2e  ld-sm_ms label,.
-0000daf0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000db00: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
-0000db10: 726f 772e 6669 656c 642d 7873 5f6d 7320  row.field-xs_ms 
-0000db20: 2e66 6965 6c64 2d78 6c5f 6d65 206c 6162  .field-xl_me lab
-0000db30: 656c 2c2e 646a 616e 676f 636d 732d 6672  el,.djangocms-fr
-0000db40: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-0000db50: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000db60: 5f6d 7320 2e66 6965 6c64 2d78 6c5f 6d73  _ms .field-xl_ms
-0000db70: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
-0000db80: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
-0000db90: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
-0000dba0: 642d 7873 5f6d 7320 2e66 6965 6c64 2d78  d-xs_ms .field-x
-0000dbb0: 735f 6d65 206c 6162 656c 2c2e 646a 616e  s_me label,.djan
-0000dbc0: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
-0000dbd0: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
-0000dbe0: 6669 656c 642d 7873 5f6d 7320 2e66 6965  field-xs_ms .fie
-0000dbf0: 6c64 2d78 735f 6d73 206c 6162 656c 2c2e  ld-xs_ms label,.
-0000dc00: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000dc10: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
-0000dc20: 726f 772e 6669 656c 642d 7873 5f6d 7320  row.field-xs_ms 
-0000dc30: 2e66 6965 6c64 2d78 786c 5f6d 6520 6c61  .field-xxl_me la
-0000dc40: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
-0000dc50: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000dc60: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000dc70: 735f 6d73 202e 6669 656c 642d 7878 6c5f  s_ms .field-xxl_
-0000dc80: 6d73 206c 6162 656c 2c2e 646a 616e 676f  ms label,.django
-0000dc90: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000dca0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000dcb0: 656c 642d 7873 5f6f 6666 7365 7420 2e66  eld-xs_offset .f
-0000dcc0: 6965 6c64 2d6c 675f 6d65 206c 6162 656c  ield-lg_me label
-0000dcd0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000dce0: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000dcf0: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-0000dd00: 6666 7365 7420 2e66 6965 6c64 2d6c 675f  ffset .field-lg_
-0000dd10: 6d73 206c 6162 656c 2c2e 646a 616e 676f  ms label,.django
-0000dd20: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000dd30: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000dd40: 656c 642d 7873 5f6f 6666 7365 7420 2e66  eld-xs_offset .f
-0000dd50: 6965 6c64 2d6d 645f 6d65 206c 6162 656c  ield-md_me label
-0000dd60: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000dd70: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000dd80: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-0000dd90: 6666 7365 7420 2e66 6965 6c64 2d6d 645f  ffset .field-md_
-0000dda0: 6d73 206c 6162 656c 2c2e 646a 616e 676f  ms label,.django
-0000ddb0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000ddc0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000ddd0: 656c 642d 7873 5f6f 6666 7365 7420 2e66  eld-xs_offset .f
-0000dde0: 6965 6c64 2d73 6d5f 6d65 206c 6162 656c  ield-sm_me label
-0000ddf0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000de00: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000de10: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-0000de20: 6666 7365 7420 2e66 6965 6c64 2d73 6d5f  ffset .field-sm_
-0000de30: 6d73 206c 6162 656c 2c2e 646a 616e 676f  ms label,.django
-0000de40: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000de50: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000de60: 656c 642d 7873 5f6f 6666 7365 7420 2e66  eld-xs_offset .f
-0000de70: 6965 6c64 2d78 6c5f 6d65 206c 6162 656c  ield-xl_me label
-0000de80: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000de90: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000dea0: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-0000deb0: 6666 7365 7420 2e66 6965 6c64 2d78 6c5f  ffset .field-xl_
-0000dec0: 6d73 206c 6162 656c 2c2e 646a 616e 676f  ms label,.django
-0000ded0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000dee0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000def0: 656c 642d 7873 5f6f 6666 7365 7420 2e66  eld-xs_offset .f
-0000df00: 6965 6c64 2d78 735f 6d65 206c 6162 656c  ield-xs_me label
-0000df10: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000df20: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000df30: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-0000df40: 6666 7365 7420 2e66 6965 6c64 2d78 735f  ffset .field-xs_
-0000df50: 6d73 206c 6162 656c 2c2e 646a 616e 676f  ms label,.django
-0000df60: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000df70: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000df80: 656c 642d 7873 5f6f 6666 7365 7420 2e66  eld-xs_offset .f
-0000df90: 6965 6c64 2d78 786c 5f6d 6520 6c61 6265  ield-xxl_me labe
-0000dfa0: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
-0000dfb0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000dfc0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000dfd0: 6f66 6673 6574 202e 6669 656c 642d 7878  offset .field-xx
-0000dfe0: 6c5f 6d73 206c 6162 656c 2c2e 646a 616e  l_ms label,.djan
-0000dff0: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
-0000e000: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
-0000e010: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
-0000e020: 6669 656c 642d 6c67 5f6d 6520 6c61 6265  field-lg_me labe
-0000e030: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
-0000e040: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000e050: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000e060: 6f72 6465 7220 2e66 6965 6c64 2d6c 675f  order .field-lg_
-0000e070: 6d73 206c 6162 656c 2c2e 646a 616e 676f  ms label,.django
-0000e080: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000e090: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000e0a0: 656c 642d 7873 5f6f 7264 6572 202e 6669  eld-xs_order .fi
-0000e0b0: 656c 642d 6d64 5f6d 6520 6c61 6265 6c2c  eld-md_me label,
-0000e0c0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000e0d0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000e0e0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f72  -row.field-xs_or
-0000e0f0: 6465 7220 2e66 6965 6c64 2d6d 645f 6d73  der .field-md_ms
-0000e100: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
-0000e110: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
-0000e120: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
-0000e130: 642d 7873 5f6f 7264 6572 202e 6669 656c  d-xs_order .fiel
-0000e140: 642d 736d 5f6d 6520 6c61 6265 6c2c 2e64  d-sm_me label,.d
-0000e150: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000e160: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000e170: 6f77 2e66 6965 6c64 2d78 735f 6f72 6465  ow.field-xs_orde
-0000e180: 7220 2e66 6965 6c64 2d73 6d5f 6d73 206c  r .field-sm_ms l
-0000e190: 6162 656c 2c2e 646a 616e 676f 636d 732d  abel,.djangocms-
-0000e1a0: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-0000e1b0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000e1c0: 7873 5f6f 7264 6572 202e 6669 656c 642d  xs_order .field-
-0000e1d0: 786c 5f6d 6520 6c61 6265 6c2c 2e64 6a61  xl_me label,.dja
-0000e1e0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000e1f0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000e200: 2e66 6965 6c64 2d78 735f 6f72 6465 7220  .field-xs_order 
-0000e210: 2e66 6965 6c64 2d78 6c5f 6d73 206c 6162  .field-xl_ms lab
-0000e220: 656c 2c2e 646a 616e 676f 636d 732d 6672  el,.djangocms-fr
-0000e230: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-0000e240: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000e250: 5f6f 7264 6572 202e 6669 656c 642d 7873  _order .field-xs
-0000e260: 5f6d 6520 6c61 6265 6c2c 2e64 6a61 6e67  _me label,.djang
-0000e270: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000e280: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000e290: 6965 6c64 2d78 735f 6f72 6465 7220 2e66  ield-xs_order .f
-0000e2a0: 6965 6c64 2d78 735f 6d73 206c 6162 656c  ield-xs_ms label
-0000e2b0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000e2c0: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000e2d0: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-0000e2e0: 7264 6572 202e 6669 656c 642d 7878 6c5f  rder .field-xxl_
-0000e2f0: 6d65 206c 6162 656c 2c2e 646a 616e 676f  me label,.django
-0000e300: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000e310: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000e320: 656c 642d 7873 5f6f 7264 6572 202e 6669  eld-xs_order .fi
-0000e330: 656c 642d 7878 6c5f 6d73 206c 6162 656c  eld-xxl_ms label
-0000e340: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000e350: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
-0000e360: 6f77 2e66 6965 6c64 2d72 6f77 5f63 6f6c  ow.field-row_col
-0000e370: 735f 7873 202e 6669 656c 642d 6c67 5f6d  s_xs .field-lg_m
-0000e380: 6520 6c61 6265 6c2c 2e64 6a61 6e67 6f63  e label,.djangoc
-0000e390: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-0000e3a0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000e3b0: 726f 775f 636f 6c73 5f78 7320 2e66 6965  row_cols_xs .fie
-0000e3c0: 6c64 2d6c 675f 6d73 206c 6162 656c 2c2e  ld-lg_ms label,.
-0000e3d0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000e3e0: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
-0000e3f0: 2e66 6965 6c64 2d72 6f77 5f63 6f6c 735f  .field-row_cols_
-0000e400: 7873 202e 6669 656c 642d 6d64 5f6d 6520  xs .field-md_me 
-0000e410: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
-0000e420: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-0000e430: 6f72 6d2d 726f 772e 6669 656c 642d 726f  orm-row.field-ro
-0000e440: 775f 636f 6c73 5f78 7320 2e66 6965 6c64  w_cols_xs .field
-0000e450: 2d6d 645f 6d73 206c 6162 656c 2c2e 646a  -md_ms label,.dj
-0000e460: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000e470: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
-0000e480: 6965 6c64 2d72 6f77 5f63 6f6c 735f 7873  ield-row_cols_xs
-0000e490: 202e 6669 656c 642d 736d 5f6d 6520 6c61   .field-sm_me la
-0000e4a0: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
-0000e4b0: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
-0000e4c0: 6d2d 726f 772e 6669 656c 642d 726f 775f  m-row.field-row_
-0000e4d0: 636f 6c73 5f78 7320 2e66 6965 6c64 2d73  cols_xs .field-s
-0000e4e0: 6d5f 6d73 206c 6162 656c 2c2e 646a 616e  m_ms label,.djan
-0000e4f0: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
-0000e500: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
-0000e510: 6c64 2d72 6f77 5f63 6f6c 735f 7873 202e  ld-row_cols_xs .
-0000e520: 6669 656c 642d 786c 5f6d 6520 6c61 6265  field-xl_me labe
-0000e530: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
-0000e540: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
-0000e550: 726f 772e 6669 656c 642d 726f 775f 636f  row.field-row_co
-0000e560: 6c73 5f78 7320 2e66 6965 6c64 2d78 6c5f  ls_xs .field-xl_
-0000e570: 6d73 206c 6162 656c 2c2e 646a 616e 676f  ms label,.django
-0000e580: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
-0000e590: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000e5a0: 2d72 6f77 5f63 6f6c 735f 7873 202e 6669  -row_cols_xs .fi
-0000e5b0: 656c 642d 7873 5f6d 6520 6c61 6265 6c2c  eld-xs_me label,
-0000e5c0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000e5d0: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
-0000e5e0: 772e 6669 656c 642d 726f 775f 636f 6c73  w.field-row_cols
-0000e5f0: 5f78 7320 2e66 6965 6c64 2d78 735f 6d73  _xs .field-xs_ms
-0000e600: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
-0000e610: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
-0000e620: 666f 726d 2d72 6f77 2e66 6965 6c64 2d72  form-row.field-r
-0000e630: 6f77 5f63 6f6c 735f 7873 202e 6669 656c  ow_cols_xs .fiel
-0000e640: 642d 7878 6c5f 6d65 206c 6162 656c 2c2e  d-xxl_me label,.
-0000e650: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000e660: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
-0000e670: 2e66 6965 6c64 2d72 6f77 5f63 6f6c 735f  .field-row_cols_
-0000e680: 7873 202e 6669 656c 642d 7878 6c5f 6d73  xs .field-xxl_ms
-0000e690: 206c 6162 656c 7b69 6e73 6574 2d69 6e6c   label{inset-inl
-0000e6a0: 696e 652d 7374 6172 743a 3330 7078 3b69  ine-start:30px;i
-0000e6b0: 6e73 6574 2d62 6c6f 636b 2d73 7461 7274  nset-block-start
-0000e6c0: 3a31 3470 787d 2e64 6a61 6e67 6f63 6d73  :14px}.djangocms
-0000e6d0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000e6e0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000e6f0: 2d78 735f 636f 6c20 2e66 6965 6c64 2d6c  -xs_col .field-l
-0000e700: 675f 6d65 2069 6e70 7574 2c2e 646a 616e  g_me input,.djan
-0000e710: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
-0000e720: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
-0000e730: 6669 656c 642d 7873 5f63 6f6c 202e 6669  field-xs_col .fi
-0000e740: 656c 642d 6c67 5f6d 7320 696e 7075 742c  eld-lg_ms input,
-0000e750: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000e760: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000e770: 2d72 6f77 2e66 6965 6c64 2d78 735f 636f  -row.field-xs_co
-0000e780: 6c20 2e66 6965 6c64 2d6d 645f 6d65 2069  l .field-md_me i
-0000e790: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
-0000e7a0: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
-0000e7b0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000e7c0: 7873 5f63 6f6c 202e 6669 656c 642d 6d64  xs_col .field-md
-0000e7d0: 5f6d 7320 696e 7075 742c 2e64 6a61 6e67  _ms input,.djang
-0000e7e0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000e7f0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000e800: 6965 6c64 2d78 735f 636f 6c20 2e66 6965  ield-xs_col .fie
-0000e810: 6c64 2d73 6d5f 6d65 2069 6e70 7574 2c2e  ld-sm_me input,.
-0000e820: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000e830: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
-0000e840: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
-0000e850: 202e 6669 656c 642d 736d 5f6d 7320 696e   .field-sm_ms in
-0000e860: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
-0000e870: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000e880: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000e890: 735f 636f 6c20 2e66 6965 6c64 2d78 6c5f  s_col .field-xl_
-0000e8a0: 6d65 2069 6e70 7574 2c2e 646a 616e 676f  me input,.django
-0000e8b0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000e8c0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000e8d0: 656c 642d 7873 5f63 6f6c 202e 6669 656c  eld-xs_col .fiel
-0000e8e0: 642d 786c 5f6d 7320 696e 7075 742c 2e64  d-xl_ms input,.d
-0000e8f0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000e900: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000e910: 6f77 2e66 6965 6c64 2d78 735f 636f 6c20  ow.field-xs_col 
-0000e920: 2e66 6965 6c64 2d78 735f 6d65 2069 6e70  .field-xs_me inp
-0000e930: 7574 2c2e 646a 616e 676f 636d 732d 6672  ut,.djangocms-fr
-0000e940: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-0000e950: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000e960: 5f63 6f6c 202e 6669 656c 642d 7873 5f6d  _col .field-xs_m
-0000e970: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
-0000e980: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000e990: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000e9a0: 6c64 2d78 735f 636f 6c20 2e66 6965 6c64  ld-xs_col .field
-0000e9b0: 2d78 786c 5f6d 6520 696e 7075 742c 2e64  -xxl_me input,.d
-0000e9c0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000e9d0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000e9e0: 6f77 2e66 6965 6c64 2d78 735f 636f 6c20  ow.field-xs_col 
-0000e9f0: 2e66 6965 6c64 2d78 786c 5f6d 7320 696e  .field-xxl_ms in
-0000ea00: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
-0000ea10: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000ea20: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000ea30: 735f 6d65 202e 6669 656c 642d 6c67 5f6d  s_me .field-lg_m
-0000ea40: 6520 696e 7075 742c 2e64 6a61 6e67 6f63  e input,.djangoc
-0000ea50: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000ea60: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000ea70: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
-0000ea80: 6c67 5f6d 7320 696e 7075 742c 2e64 6a61  lg_ms input,.dja
-0000ea90: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000eaa0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000eab0: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
-0000eac0: 656c 642d 6d64 5f6d 6520 696e 7075 742c  eld-md_me input,
-0000ead0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000eae0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000eaf0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
-0000eb00: 202e 6669 656c 642d 6d64 5f6d 7320 696e   .field-md_ms in
-0000eb10: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
-0000eb20: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000eb30: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000eb40: 735f 6d65 202e 6669 656c 642d 736d 5f6d  s_me .field-sm_m
-0000eb50: 6520 696e 7075 742c 2e64 6a61 6e67 6f63  e input,.djangoc
-0000eb60: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000eb70: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000eb80: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
-0000eb90: 736d 5f6d 7320 696e 7075 742c 2e64 6a61  sm_ms input,.dja
-0000eba0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000ebb0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000ebc0: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
-0000ebd0: 656c 642d 786c 5f6d 6520 696e 7075 742c  eld-xl_me input,
-0000ebe0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000ebf0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000ec00: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
-0000ec10: 202e 6669 656c 642d 786c 5f6d 7320 696e   .field-xl_ms in
-0000ec20: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
-0000ec30: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000ec40: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000ec50: 735f 6d65 202e 6669 656c 642d 7873 5f6d  s_me .field-xs_m
-0000ec60: 6520 696e 7075 742c 2e64 6a61 6e67 6f63  e input,.djangoc
-0000ec70: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000ec80: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000ec90: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
-0000eca0: 7873 5f6d 7320 696e 7075 742c 2e64 6a61  xs_ms input,.dja
-0000ecb0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000ecc0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
-0000ecd0: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
-0000ece0: 656c 642d 7878 6c5f 6d65 2069 6e70 7574  eld-xxl_me input
-0000ecf0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000ed00: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000ed10: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
-0000ed20: 6520 2e66 6965 6c64 2d78 786c 5f6d 7320  e .field-xxl_ms 
-0000ed30: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
-0000ed40: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000ed50: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000ed60: 2d78 735f 6d73 202e 6669 656c 642d 6c67  -xs_ms .field-lg
-0000ed70: 5f6d 6520 696e 7075 742c 2e64 6a61 6e67  _me input,.djang
-0000ed80: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000ed90: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000eda0: 6965 6c64 2d78 735f 6d73 202e 6669 656c  ield-xs_ms .fiel
-0000edb0: 642d 6c67 5f6d 7320 696e 7075 742c 2e64  d-lg_ms input,.d
-0000edc0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000edd0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000ede0: 6f77 2e66 6965 6c64 2d78 735f 6d73 202e  ow.field-xs_ms .
-0000edf0: 6669 656c 642d 6d64 5f6d 6520 696e 7075  field-md_me inpu
-0000ee00: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
-0000ee10: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000ee20: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000ee30: 6d73 202e 6669 656c 642d 6d64 5f6d 7320  ms .field-md_ms 
-0000ee40: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
-0000ee50: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000ee60: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000ee70: 2d78 735f 6d73 202e 6669 656c 642d 736d  -xs_ms .field-sm
-0000ee80: 5f6d 6520 696e 7075 742c 2e64 6a61 6e67  _me input,.djang
-0000ee90: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000eea0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000eeb0: 6965 6c64 2d78 735f 6d73 202e 6669 656c  ield-xs_ms .fiel
-0000eec0: 642d 736d 5f6d 7320 696e 7075 742c 2e64  d-sm_ms input,.d
-0000eed0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000eee0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000eef0: 6f77 2e66 6965 6c64 2d78 735f 6d73 202e  ow.field-xs_ms .
-0000ef00: 6669 656c 642d 786c 5f6d 6520 696e 7075  field-xl_me inpu
-0000ef10: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
-0000ef20: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000ef30: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000ef40: 6d73 202e 6669 656c 642d 786c 5f6d 7320  ms .field-xl_ms 
-0000ef50: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
-0000ef60: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000ef70: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000ef80: 2d78 735f 6d73 202e 6669 656c 642d 7873  -xs_ms .field-xs
-0000ef90: 5f6d 6520 696e 7075 742c 2e64 6a61 6e67  _me input,.djang
-0000efa0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000efb0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000efc0: 6965 6c64 2d78 735f 6d73 202e 6669 656c  ield-xs_ms .fiel
-0000efd0: 642d 7873 5f6d 7320 696e 7075 742c 2e64  d-xs_ms input,.d
-0000efe0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000eff0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
-0000f000: 6f77 2e66 6965 6c64 2d78 735f 6d73 202e  ow.field-xs_ms .
-0000f010: 6669 656c 642d 7878 6c5f 6d65 2069 6e70  field-xxl_me inp
-0000f020: 7574 2c2e 646a 616e 676f 636d 732d 6672  ut,.djangocms-fr
-0000f030: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
-0000f040: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
-0000f050: 5f6d 7320 2e66 6965 6c64 2d78 786c 5f6d  _ms .field-xxl_m
-0000f060: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
-0000f070: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000f080: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000f090: 6c64 2d78 735f 6f66 6673 6574 202e 6669  ld-xs_offset .fi
-0000f0a0: 656c 642d 6c67 5f6d 6520 696e 7075 742c  eld-lg_me input,
-0000f0b0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000f0c0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000f0d0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f66  -row.field-xs_of
-0000f0e0: 6673 6574 202e 6669 656c 642d 6c67 5f6d  fset .field-lg_m
-0000f0f0: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
-0000f100: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000f110: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000f120: 6c64 2d78 735f 6f66 6673 6574 202e 6669  ld-xs_offset .fi
-0000f130: 656c 642d 6d64 5f6d 6520 696e 7075 742c  eld-md_me input,
-0000f140: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000f150: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000f160: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f66  -row.field-xs_of
-0000f170: 6673 6574 202e 6669 656c 642d 6d64 5f6d  fset .field-md_m
-0000f180: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
-0000f190: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000f1a0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000f1b0: 6c64 2d78 735f 6f66 6673 6574 202e 6669  ld-xs_offset .fi
-0000f1c0: 656c 642d 736d 5f6d 6520 696e 7075 742c  eld-sm_me input,
-0000f1d0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000f1e0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000f1f0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f66  -row.field-xs_of
-0000f200: 6673 6574 202e 6669 656c 642d 736d 5f6d  fset .field-sm_m
-0000f210: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
-0000f220: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000f230: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000f240: 6c64 2d78 735f 6f66 6673 6574 202e 6669  ld-xs_offset .fi
-0000f250: 656c 642d 786c 5f6d 6520 696e 7075 742c  eld-xl_me input,
-0000f260: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000f270: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000f280: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f66  -row.field-xs_of
-0000f290: 6673 6574 202e 6669 656c 642d 786c 5f6d  fset .field-xl_m
-0000f2a0: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
-0000f2b0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000f2c0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000f2d0: 6c64 2d78 735f 6f66 6673 6574 202e 6669  ld-xs_offset .fi
-0000f2e0: 656c 642d 7873 5f6d 6520 696e 7075 742c  eld-xs_me input,
-0000f2f0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000f300: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000f310: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f66  -row.field-xs_of
-0000f320: 6673 6574 202e 6669 656c 642d 7873 5f6d  fset .field-xs_m
-0000f330: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
-0000f340: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000f350: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000f360: 6c64 2d78 735f 6f66 6673 6574 202e 6669  ld-xs_offset .fi
-0000f370: 656c 642d 7878 6c5f 6d65 2069 6e70 7574  eld-xxl_me input
-0000f380: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000f390: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000f3a0: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-0000f3b0: 6666 7365 7420 2e66 6965 6c64 2d78 786c  ffset .field-xxl
-0000f3c0: 5f6d 7320 696e 7075 742c 2e64 6a61 6e67  _ms input,.djang
-0000f3d0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
-0000f3e0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
-0000f3f0: 6965 6c64 2d78 735f 6f72 6465 7220 2e66  ield-xs_order .f
-0000f400: 6965 6c64 2d6c 675f 6d65 2069 6e70 7574  ield-lg_me input
-0000f410: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000f420: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
-0000f430: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
-0000f440: 7264 6572 202e 6669 656c 642d 6c67 5f6d  rder .field-lg_m
-0000f450: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
-0000f460: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000f470: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000f480: 6c64 2d78 735f 6f72 6465 7220 2e66 6965  ld-xs_order .fie
-0000f490: 6c64 2d6d 645f 6d65 2069 6e70 7574 2c2e  ld-md_me input,.
-0000f4a0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000f4b0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
-0000f4c0: 726f 772e 6669 656c 642d 7873 5f6f 7264  row.field-xs_ord
-0000f4d0: 6572 202e 6669 656c 642d 6d64 5f6d 7320  er .field-md_ms 
-0000f4e0: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
-0000f4f0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
-0000f500: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-0000f510: 2d78 735f 6f72 6465 7220 2e66 6965 6c64  -xs_order .field
-0000f520: 2d73 6d5f 6d65 2069 6e70 7574 2c2e 646a  -sm_me input,.dj
-0000f530: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000f540: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
-0000f550: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
-0000f560: 202e 6669 656c 642d 736d 5f6d 7320 696e   .field-sm_ms in
-0000f570: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
-0000f580: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
-0000f590: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
-0000f5a0: 735f 6f72 6465 7220 2e66 6965 6c64 2d78  s_order .field-x
-0000f5b0: 6c5f 6d65 2069 6e70 7574 2c2e 646a 616e  l_me input,.djan
-0000f5c0: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
-0000f5d0: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
-0000f5e0: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
-0000f5f0: 6669 656c 642d 786c 5f6d 7320 696e 7075  field-xl_ms inpu
-0000f600: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
-0000f610: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
-0000f620: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
-0000f630: 6f72 6465 7220 2e66 6965 6c64 2d78 735f  order .field-xs_
-0000f640: 6d65 2069 6e70 7574 2c2e 646a 616e 676f  me input,.django
-0000f650: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
-0000f660: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
-0000f670: 656c 642d 7873 5f6f 7264 6572 202e 6669  eld-xs_order .fi
-0000f680: 656c 642d 7873 5f6d 7320 696e 7075 742c  eld-xs_ms input,
-0000f690: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000f6a0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
-0000f6b0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f72  -row.field-xs_or
-0000f6c0: 6465 7220 2e66 6965 6c64 2d78 786c 5f6d  der .field-xxl_m
-0000f6d0: 6520 696e 7075 742c 2e64 6a61 6e67 6f63  e input,.djangoc
-0000f6e0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
-0000f6f0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
-0000f700: 6c64 2d78 735f 6f72 6465 7220 2e66 6965  ld-xs_order .fie
-0000f710: 6c64 2d78 786c 5f6d 7320 696e 7075 742c  ld-xxl_ms input,
-0000f720: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000f730: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
-0000f740: 772e 6669 656c 642d 726f 775f 636f 6c73  w.field-row_cols
-0000f750: 5f78 7320 2e66 6965 6c64 2d6c 675f 6d65  _xs .field-lg_me
-0000f760: 2069 6e70 7574 2c2e 646a 616e 676f 636d   input,.djangocm
-0000f770: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
-0000f780: 666f 726d 2d72 6f77 2e66 6965 6c64 2d72  form-row.field-r
-0000f790: 6f77 5f63 6f6c 735f 7873 202e 6669 656c  ow_cols_xs .fiel
-0000f7a0: 642d 6c67 5f6d 7320 696e 7075 742c 2e64  d-lg_ms input,.d
-0000f7b0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000f7c0: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-0000f7d0: 6669 656c 642d 726f 775f 636f 6c73 5f78  field-row_cols_x
-0000f7e0: 7320 2e66 6965 6c64 2d6d 645f 6d65 2069  s .field-md_me i
-0000f7f0: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
-0000f800: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
-0000f810: 726d 2d72 6f77 2e66 6965 6c64 2d72 6f77  rm-row.field-row
-0000f820: 5f63 6f6c 735f 7873 202e 6669 656c 642d  _cols_xs .field-
-0000f830: 6d64 5f6d 7320 696e 7075 742c 2e64 6a61  md_ms input,.dja
-0000f840: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-0000f850: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
-0000f860: 656c 642d 726f 775f 636f 6c73 5f78 7320  eld-row_cols_xs 
-0000f870: 2e66 6965 6c64 2d73 6d5f 6d65 2069 6e70  .field-sm_me inp
-0000f880: 7574 2c2e 646a 616e 676f 636d 732d 6672  ut,.djangocms-fr
-0000f890: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
-0000f8a0: 2d72 6f77 2e66 6965 6c64 2d72 6f77 5f63  -row.field-row_c
-0000f8b0: 6f6c 735f 7873 202e 6669 656c 642d 736d  ols_xs .field-sm
-0000f8c0: 5f6d 7320 696e 7075 742c 2e64 6a61 6e67  _ms input,.djang
-0000f8d0: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
-0000f8e0: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
-0000f8f0: 642d 726f 775f 636f 6c73 5f78 7320 2e66  d-row_cols_xs .f
-0000f900: 6965 6c64 2d78 6c5f 6d65 2069 6e70 7574  ield-xl_me input
-0000f910: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
-0000f920: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
-0000f930: 6f77 2e66 6965 6c64 2d72 6f77 5f63 6f6c  ow.field-row_col
-0000f940: 735f 7873 202e 6669 656c 642d 786c 5f6d  s_xs .field-xl_m
-0000f950: 7320 696e 7075 742c 2e64 6a61 6e67 6f63  s input,.djangoc
-0000f960: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
-0000f970: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
-0000f980: 726f 775f 636f 6c73 5f78 7320 2e66 6965  row_cols_xs .fie
-0000f990: 6c64 2d78 735f 6d65 2069 6e70 7574 2c2e  ld-xs_me input,.
-0000f9a0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-0000f9b0: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
-0000f9c0: 2e66 6965 6c64 2d72 6f77 5f63 6f6c 735f  .field-row_cols_
-0000f9d0: 7873 202e 6669 656c 642d 7873 5f6d 7320  xs .field-xs_ms 
-0000f9e0: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
-0000f9f0: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
-0000fa00: 6f72 6d2d 726f 772e 6669 656c 642d 726f  orm-row.field-ro
-0000fa10: 775f 636f 6c73 5f78 7320 2e66 6965 6c64  w_cols_xs .field
-0000fa20: 2d78 786c 5f6d 6520 696e 7075 742c 2e64  -xxl_me input,.d
-0000fa30: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-0000fa40: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
-0000fa50: 6669 656c 642d 726f 775f 636f 6c73 5f78  field-row_cols_x
-0000fa60: 7320 2e66 6965 6c64 2d78 786c 5f6d 7320  s .field-xxl_ms 
-0000fa70: 696e 7075 747b 706f 7369 7469 6f6e 3a72  input{position:r
-0000fa80: 656c 6174 6976 653b 626f 782d 7369 7a69  elative;box-sizi
-0000fa90: 6e67 3a62 6f72 6465 722d 626f 783b 746f  ng:border-box;to
-0000faa0: 703a 2d33 7078 7d2e 6772 6964 2d72 6573  p:-3px}.grid-res
-0000fab0: 6574 7b70 6f73 6974 696f 6e3a 6162 736f  et{position:abso
-0000fac0: 6c75 7465 3b69 6e73 6574 2d69 6e6c 696e  lute;inset-inlin
-0000fad0: 652d 656e 643a 3570 783b 696e 7365 742d  e-end:5px;inset-
-0000fae0: 626c 6f63 6b2d 7374 6172 743a 307d 2e69  block-start:0}.i
-0000faf0: 636f 6e2d 7468 6561 647b 7465 7874 2d61  con-thead{text-a
-0000fb00: 6c69 676e 3a63 656e 7465 723b 6d61 7267  lign:center;marg
-0000fb10: 696e 2d62 6f74 746f 6d3a 3135 7078 7d2e  in-bottom:15px}.
-0000fb20: 6963 6f6e 2d74 6865 6164 202e 6963 6f6e  icon-thead .icon
-0000fb30: 7b66 6f6e 742d 7369 7a65 3a33 3070 787d  {font-size:30px}
-0000fb40: 2e69 636f 6e2d 7468 6561 6420 2e69 636f  .icon-thead .ico
-0000fb50: 6e2d 7369 7a65 2d73 6d7b 7472 616e 7366  n-size-sm{transf
-0000fb60: 6f72 6d3a 726f 7461 7465 2839 3064 6567  orm:rotate(90deg
-0000fb70: 297d 2e69 636f 6e2d 7469 746c 657b 6469  )}.icon-title{di
-0000fb80: 7370 6c61 793a 626c 6f63 6b3b 666f 6e74  splay:block;font
-0000fb90: 2d73 697a 653a 3132 7078 3b63 6f6c 6f72  -size:12px;color
-0000fba0: 3a23 3939 393b 7061 6464 696e 673a 3570  :#999;padding:5p
-0000fbb0: 7820 3020 307d 2e64 6a61 6e67 6f63 6d73  x 0 0}.djangocms
-0000fbc0: 2d66 726f 6e74 656e 642d 7072 6576 6965  -frontend-previe
-0000fbd0: 777b 706f 7369 7469 6f6e 3a66 6978 6564  w{position:fixed
-0000fbe0: 3b69 6e73 6574 2d62 6c6f 636b 2d73 7461  ;inset-block-sta
-0000fbf0: 7274 3a30 3b69 6e73 6574 2d69 6e6c 696e  rt:0;inset-inlin
-0000fc00: 652d 656e 643a 303b 7a2d 696e 6465 783a  e-end:0;z-index:
-0000fc10: 3130 3b74 6578 742d 616c 6967 6e3a 6365  10;text-align:ce
-0000fc20: 6e74 6572 3b62 6f72 6465 722d 7261 6469  nter;border-radi
-0000fc30: 7573 3a30 2030 2030 2033 7078 3b70 6164  us:0 0 0 3px;pad
-0000fc40: 6469 6e67 3a31 3070 7820 3230 7078 2032  ding:10px 20px 2
-0000fc50: 3770 783b 626f 7264 6572 3a31 7078 2073  7px;border:1px s
-0000fc60: 6f6c 6964 2076 6172 282d 2d64 6361 2d67  olid var(--dca-g
-0000fc70: 7261 792c 7661 7228 2d2d 6861 6972 6c69  ray,var(--hairli
-0000fc80: 6e65 2d63 6f6c 6f72 2c23 6363 6329 293b  ne-color,#ccc));
-0000fc90: 626f 7264 6572 2d62 6c6f 636b 2d73 7461  border-block-sta
-0000fca0: 7274 3a6e 6f6e 653b 626f 7264 6572 2d69  rt:none;border-i
-0000fcb0: 6e6c 696e 652d 656e 643a 6e6f 6e65 3b62  nline-end:none;b
-0000fcc0: 6163 6b67 726f 756e 643a 7661 7228 2d2d  ackground:var(--
-0000fcd0: 626f 6479 2d62 672c 2366 6666 297d 406d  body-bg,#fff)}@m
-0000fce0: 6564 6961 2028 7072 6566 6572 732d 636f  edia (prefers-co
-0000fcf0: 6c6f 722d 7363 6865 6d65 3a64 6172 6b29  lor-scheme:dark)
-0000fd00: 7b2e 646a 616e 676f 636d 732d 6672 6f6e  {.djangocms-fron
-0000fd10: 7465 6e64 2d70 7265 7669 6577 7b62 6163  tend-preview{bac
-0000fd20: 6b67 726f 756e 643a 7661 7228 2d2d 626f  kground:var(--bo
-0000fd30: 6479 2d62 672c 2330 3030 297d 7d2e 646a  dy-bg,#000)}}.dj
-0000fd40: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
-0000fd50: 2d70 7265 7669 6577 2068 327b 666f 6e74  -preview h2{font
-0000fd60: 2d73 697a 653a 3134 7078 3b6d 696e 2d77  -size:14px;min-w
-0000fd70: 6964 7468 3a31 3530 7078 3b6d 6172 6769  idth:150px;margi
-0000fd80: 6e3a 3020 3020 3132 7078 7d2e 646a 616e  n:0 0 12px}.djan
-0000fd90: 676f 636d 732d 6672 6f6e 7465 6e64 2d70  gocms-frontend-p
-0000fda0: 7265 7669 6577 202e 6234 2d70 7265 7669  review .b4-previ
-0000fdb0: 6577 7b6d 6172 6769 6e3a 3020 3020 2d31  ew{margin:0 0 -1
-0000fdc0: 3570 787d 2e64 6a61 6e67 6f63 6d73 2d66  5px}.djangocms-f
-0000fdd0: 726f 6e74 656e 642d 7072 6576 6965 7720  rontend-preview 
-0000fde0: 2e62 342d 636c 6f73 657b 706f 7369 7469  .b4-close{positi
-0000fdf0: 6f6e 3a61 6273 6f6c 7574 653b 696e 7365  on:absolute;inse
-0000fe00: 742d 696e 6c69 6e65 2d65 6e64 3a31 3070  t-inline-end:10p
-0000fe10: 783b 696e 7365 742d 626c 6f63 6b2d 7374  x;inset-block-st
-0000fe20: 6172 743a 3870 783b 7a2d 696e 6465 783a  art:8px;z-index:
-0000fe30: 3130 303b 6469 7370 6c61 793a 626c 6f63  100;display:bloc
-0000fe40: 6b3b 636f 6c6f 723a 2335 6535 6535 653b  k;color:#5e5e5e;
-0000fe50: 666f 6e74 2d73 697a 653a 3132 7078 3b6c  font-size:12px;l
-0000fe60: 696e 652d 6865 6967 6874 3a32 3070 783b  ine-height:20px;
-0000fe70: 666f 6e74 2d77 6569 6768 743a 3730 303b  font-weight:700;
-0000fe80: 7465 7874 2d74 7261 6e73 666f 726d 3a75  text-transform:u
-0000fe90: 7070 6572 6361 7365 3b77 6964 7468 3a32  ppercase;width:2
-0000fea0: 3070 783b 6865 6967 6874 3a32 3070 783b  0px;height:20px;
-0000feb0: 626f 7264 6572 2d72 6164 6975 733a 3370  border-radius:3p
-0000fec0: 783b 6261 636b 6772 6f75 6e64 3a23 6464  x;background:#dd
-0000fed0: 647d 2e64 6a61 6e67 6f63 6d73 2d66 726f  d}.djangocms-fro
-0000fee0: 6e74 656e 642d 7072 6576 6965 7720 2e62  ntend-preview .b
-0000fef0: 342d 636c 6f73 653a 686f 7665 727b 636f  4-close:hover{co
-0000ff00: 6c6f 723a 2366 6666 2169 6d70 6f72 7461  lor:#fff!importa
-0000ff10: 6e74 3b74 6578 742d 6465 636f 7261 7469  nt;text-decorati
-0000ff20: 6f6e 3a6e 6f6e 653b 6261 636b 6772 6f75  on:none;backgrou
-0000ff30: 6e64 3a23 3062 667d 2e64 6a61 6e67 6f63  nd:#0bf}.djangoc
-0000ff40: 6d73 2d66 726f 6e74 656e 642d 7072 6576  ms-frontend-prev
-0000ff50: 6965 7720 2e62 746e 3e73 7061 6e7b 7665  iew .btn>span{ve
-0000ff60: 7274 6963 616c 2d61 6c69 676e 3a6d 6964  rtical-align:mid
-0000ff70: 646c 657d 2e64 6a61 6e67 6f63 6d73 2d66  dle}.djangocms-f
-0000ff80: 726f 6e74 656e 642d 7072 6576 6965 7720  rontend-preview 
-0000ff90: 2e62 746e 3e73 7061 6e3e 2e69 636f 6e7b  .btn>span>.icon{
-0000ffa0: 7665 7274 6963 616c 2d61 6c69 676e 3a6d  vertical-align:m
-0000ffb0: 6964 646c 657d 2e64 6a61 6e67 6f63 6d73  iddle}.djangocms
-0000ffc0: 2d66 726f 6e74 656e 642d 7072 6576 6965  -frontend-previe
-0000ffd0: 7720 2e62 746e 3e73 7061 6e20 7376 672c  w .btn>span svg,
-0000ffe0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-0000fff0: 656e 642d 7072 6576 6965 7720 2e62 746e  end-preview .btn
-00010000: 3e73 7061 6e20 7573 657b 6669 6c6c 3a63  >span use{fill:c
-00010010: 7572 7265 6e74 436f 6c6f 727d 2e64 6a61  urrentColor}.dja
-00010020: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
-00010030: 626c 6f63 6b71 756f 7465 2074 6578 7461  blockquote texta
-00010040: 7265 617b 6865 6967 6874 3a31 3130 7078  rea{height:110px
-00010050: 7d23 6964 5f6c 696e 6b5f 7479 7065 7b70  }#id_link_type{p
-00010060: 6164 6469 6e67 3a30 3b6d 6172 6769 6e3a  adding:0;margin:
-00010070: 303b 626f 7264 6572 3a6e 6f6e 657d 2369  0;border:none}#i
-00010080: 645f 6c69 6e6b 5f74 7970 6520 6c69 7b70  d_link_type li{p
-00010090: 6164 6469 6e67 3a30 3b6d 6172 6769 6e3a  adding:0;margin:
-000100a0: 3020 3135 7078 2035 7078 2030 3b62 6f72  0 15px 5px 0;bor
-000100b0: 6465 723a 6e6f 6e65 7d23 6964 5f6c 696e  der:none}#id_lin
-000100c0: 6b5f 7479 7065 206c 6162 656c 2069 6e70  k_type label inp
-000100d0: 7574 7b70 6f73 6974 696f 6e3a 7265 6c61  ut{position:rela
-000100e0: 7469 7665 3b74 6f70 3a2d 3470 787d 615b  tive;top:-4px}a[
-000100f0: 6461 7461 2d70 6b5d 7b70 6f73 6974 696f  data-pk]{positio
-00010100: 6e3a 7265 6c61 7469 7665 7d61 5b64 6174  n:relative}a[dat
-00010110: 612d 706b 5d3a 6166 7465 727b 636f 6e74  a-pk]:after{cont
-00010120: 656e 743a 6174 7472 2864 6174 612d 706b  ent:attr(data-pk
-00010130: 293b 7669 7369 6269 6c69 7479 3a68 6964  );visibility:hid
-00010140: 6465 6e3b 7769 6474 683a 6175 746f 3b66  den;width:auto;f
-00010150: 6f6e 742d 7765 6967 6874 3a34 3030 3b66  ont-weight:400;f
-00010160: 6f6e 742d 7369 7a65 3a38 3025 3b62 6163  ont-size:80%;bac
-00010170: 6b67 726f 756e 642d 636f 6c6f 723a 7661  kground-color:va
-00010180: 7228 2d2d 6463 612d 7768 6974 652c 7661  r(--dca-white,va
-00010190: 7228 2d2d 626f 6479 2d62 672c 2366 6666  r(--body-bg,#fff
-000101a0: 2929 3b63 6f6c 6f72 3a76 6172 282d 2d64  ));color:var(--d
-000101b0: 6361 2d67 7261 792c 7661 7228 2d2d 626f  ca-gray,var(--bo
-000101c0: 6479 2d66 672c 2333 3333 2929 3b62 6f72  dy-fg,#333));bor
-000101d0: 6465 723a 736f 6c69 6420 3170 7820 7661  der:solid 1px va
-000101e0: 7228 2d2d 6463 612d 6772 6179 2c76 6172  r(--dca-gray,var
-000101f0: 282d 2d62 6f64 792d 6667 2c23 3333 3329  (--body-fg,#333)
-00010200: 293b 7465 7874 2d61 6c69 676e 3a63 656e  );text-align:cen
-00010210: 7465 723b 7061 6464 696e 673a 3570 7820  ter;padding:5px 
-00010220: 3130 7078 3b70 6f73 6974 696f 6e3a 6162  10px;position:ab
-00010230: 736f 6c75 7465 3b7a 2d69 6e64 6578 3a31  solute;z-index:1
-00010240: 3b74 6f70 3a31 3130 253b 696e 7365 742d  ;top:110%;inset-
-00010250: 696e 6c69 6e65 2d73 7461 7274 3a35 3025  inline-start:50%
-00010260: 3b6d 6172 6769 6e2d 696e 6c69 6e65 2d73  ;margin-inline-s
-00010270: 7461 7274 3a2d 3530 257d 615b 6461 7461  tart:-50%}a[data
-00010280: 2d70 6b5d 3a68 6f76 6572 3a61 6674 6572  -pk]:hover:after
-00010290: 7b76 6973 6962 696c 6974 793a 7669 7369  {visibility:visi
-000102a0: 626c 657d 2e64 6a61 6e67 6f63 6d73 2d61  ble}.djangocms-a
-000102b0: 646d 696e 2d73 7479 6c65 202e 666f 726d  dmin-style .form
-000102c0: 2d72 6f77 2e66 6965 6c64 2d70 6c75 6769  -row.field-plugi
-000102d0: 6e5f 7469 746c 6520 696e 7075 745b 6e61  n_title input[na
-000102e0: 6d65 3d70 6c75 6769 6e5f 7469 746c 655f  me=plugin_title_
-000102f0: 305d 7b6d 6172 6769 6e2d 626f 7474 6f6d  0]{margin-bottom
-00010300: 3a2e 3565 6d21 696d 706f 7274 616e 747d  :.5em!important}
-00010310: 2e64 6a61 6e67 6f63 6d73 2d61 646d 696e  .djangocms-admin
-00010320: 2d73 7479 6c65 202e 666f 726d 2d72 6f77  -style .form-row
-00010330: 2e66 6965 6c64 2d70 6c75 6769 6e5f 7469  .field-plugin_ti
-00010340: 746c 6520 696e 7075 745b 6e61 6d65 3d70  tle input[name=p
-00010350: 6c75 6769 6e5f 7469 746c 655f 315d 7b77  lugin_title_1]{w
-00010360: 6964 7468 3a63 616c 6328 3130 3025 202d  idth:calc(100% -
-00010370: 2032 656d 2921 696d 706f 7274 616e 747d   2em)!important}
-00010380: 626f 6479 3a6e 6f74 282e 646a 616e 676f  body:not(.django
-00010390: 636d 732d 6164 6d69 6e2d 7374 796c 6529  cms-admin-style)
-000103a0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
-000103b0: 2d70 6c75 6769 6e5f 7469 746c 6520 696e  -plugin_title in
-000103c0: 7075 745b 6e61 6d65 3d70 6c75 6769 6e5f  put[name=plugin_
-000103d0: 7469 746c 655f 315d 7b77 6964 7468 3a63  title_1]{width:c
-000103e0: 616c 6328 3130 3025 202d 2032 3030 7078  alc(100% - 200px
-000103f0: 202d 2031 656d 2921 696d 706f 7274 616e   - 1em)!importan
-00010400: 743b 6d61 7267 696e 2d69 6e6c 696e 652d  t;margin-inline-
-00010410: 7374 6172 743a 3165 6d7d 2e66 726f 6e74  start:1em}.front
-00010420: 656e 642d 6963 6f6e 2d70 6963 6b65 727b  end-icon-picker{
-00010430: 7465 7874 2d61 6c69 676e 3a63 656e 7465  text-align:cente
-00010440: 723b 6469 7370 6c61 793a 696e 6c69 6e65  r;display:inline
-00010450: 2d62 6c6f 636b 7d2e 6672 6f6e 7465 6e64  -block}.frontend
-00010460: 2d69 636f 6e2d 7069 636b 6572 202e 6963  -icon-picker .ic
-00010470: 6f6e 2d63 6f6e 7461 696e 6572 7b70 6f73  on-container{pos
-00010480: 6974 696f 6e3a 7265 6c61 7469 7665 3b6d  ition:relative;m
-00010490: 6172 6769 6e3a 2e35 656d 2061 7574 6f3b  argin:.5em auto;
-000104a0: 7769 6474 683a 3765 6d3b 6865 6967 6874  width:7em;height
-000104b0: 3a37 656d 3b62 6f72 6465 723a 3170 7820  :7em;border:1px 
-000104c0: 7661 7228 2d2d 6463 612d 6772 6179 2d6c  var(--dca-gray-l
-000104d0: 6967 6874 2c76 6172 282d 2d62 6f72 6465  ight,var(--borde
-000104e0: 722d 636f 6c6f 722c 2364 3364 3364 3329  r-color,#d3d3d3)
-000104f0: 2920 736f 6c69 643b 7472 616e 7369 7469  ) solid;transiti
-00010500: 6f6e 3a62 6163 6b67 726f 756e 642d 636f  on:background-co
-00010510: 6c6f 7220 2e31 3573 2c63 6f6c 6f72 202e  lor .15s,color .
-00010520: 3135 737d 2e66 726f 6e74 656e 642d 6963  15s}.frontend-ic
-00010530: 6f6e 2d70 6963 6b65 7220 2e69 636f 6e2d  on-picker .icon-
-00010540: 636f 6e74 6169 6e65 7220 2e69 636f 6e2d  container .icon-
-00010550: 7072 6576 6965 777b 7769 6474 683a 3765  preview{width:7e
-00010560: 6d3b 6865 6967 6874 3a37 656d 3b64 6973  m;height:7em;dis
-00010570: 706c 6179 3a2d 6d73 2d66 6c65 7862 6f78  play:-ms-flexbox
-00010580: 3b64 6973 706c 6179 3a66 6c65 783b 2d6d  ;display:flex;-m
-00010590: 732d 666c 6578 2d64 6972 6563 7469 6f6e  s-flex-direction
-000105a0: 3a63 6f6c 756d 6e3b 666c 6578 2d64 6972  :column;flex-dir
-000105b0: 6563 7469 6f6e 3a63 6f6c 756d 6e3b 2d6d  ection:column;-m
-000105c0: 732d 666c 6578 2d70 6163 6b3a 6365 6e74  s-flex-pack:cent
-000105d0: 6572 3b6a 7573 7469 6679 2d63 6f6e 7465  er;justify-conte
-000105e0: 6e74 3a63 656e 7465 727d 2e66 726f 6e74  nt:center}.front
-000105f0: 656e 642d 6963 6f6e 2d70 6963 6b65 7220  end-icon-picker 
-00010600: 2e69 636f 6e2d 636f 6e74 6169 6e65 7220  .icon-container 
-00010610: 2e69 636f 6e2d 7072 6576 6965 7720 2e69  .icon-preview .i
-00010620: 636f 6e2d 626f 787b 666f 6e74 2d73 697a  con-box{font-siz
-00010630: 653a 3530 3025 3b6c 696e 652d 6865 6967  e:500%;line-heig
-00010640: 6874 3a31 2e33 3b6d 6172 6769 6e3a 303b  ht:1.3;margin:0;
-00010650: 7465 7874 2d61 6c69 676e 3a63 656e 7465  text-align:cente
-00010660: 727d 2e66 726f 6e74 656e 642d 6963 6f6e  r}.frontend-icon
-00010670: 2d70 6963 6b65 7220 2e69 636f 6e2d 636f  -picker .icon-co
-00010680: 6e74 6169 6e65 7220 2e69 636f 6e2d 7072  ntainer .icon-pr
-00010690: 6576 6965 7720 2e69 636f 6e2d 626f 7820  eview .icon-box 
-000106a0: 692c 2e66 726f 6e74 656e 642d 6963 6f6e  i,.frontend-icon
-000106b0: 2d70 6963 6b65 7220 2e69 636f 6e2d 636f  -picker .icon-co
-000106c0: 6e74 6169 6e65 7220 2e69 636f 6e2d 7072  ntainer .icon-pr
-000106d0: 6576 6965 7720 2e69 636f 6e2d 626f 7820  eview .icon-box 
-000106e0: 7370 616e 7b66 6f6e 742d 7369 7a65 3a75  span{font-size:u
-000106f0: 6e73 6574 7d2e 6672 6f6e 7465 6e64 2d69  nset}.frontend-i
-00010700: 636f 6e2d 7069 636b 6572 202e 6963 6f6e  con-picker .icon
-00010710: 2d63 6f6e 7461 696e 6572 202e 6963 6f6e  -container .icon
-00010720: 2d70 7265 7669 6577 202e 656d 7074 792d  -preview .empty-
-00010730: 626f 787b 7465 7874 2d61 6c69 676e 3a63  box{text-align:c
-00010740: 656e 7465 723b 6f76 6572 666c 6f77 3a68  enter;overflow:h
-00010750: 6964 6465 6e3b 7465 7874 2d6f 7665 7266  idden;text-overf
-00010760: 6c6f 773a 656c 6c69 7073 6973 3b6c 696e  low:ellipsis;lin
-00010770: 652d 6865 6967 6874 3a31 3b66 6f6e 742d  e-height:1;font-
-00010780: 7369 7a65 3a31 3030 257d 2e66 726f 6e74  size:100%}.front
-00010790: 656e 642d 6963 6f6e 2d70 6963 6b65 7220  end-icon-picker 
-000107a0: 2e69 636f 6e2d 636f 6e74 6169 6e65 7220  .icon-container 
-000107b0: 2e69 636f 6e2d 7072 6576 6965 7720 2e65  .icon-preview .e
-000107c0: 6d70 7479 2d62 6f78 2e68 6964 6465 6e7b  mpty-box.hidden{
-000107d0: 6469 7370 6c61 793a 6e6f 6e65 7d2e 6672  display:none}.fr
-000107e0: 6f6e 7465 6e64 2d69 636f 6e2d 7069 636b  ontend-icon-pick
-000107f0: 6572 202e 6963 6f6e 2d63 6f6e 7461 696e  er .icon-contain
-00010800: 6572 202e 6963 6f6e 2d70 7265 7669 6577  er .icon-preview
-00010810: 3a68 6f76 6572 7b62 6163 6b67 726f 756e  :hover{backgroun
-00010820: 643a 7661 7228 2d2d 6463 612d 6772 6179  d:var(--dca-gray
-00010830: 2d6c 6967 6874 2c76 6172 282d 2d62 6f72  -light,var(--bor
-00010840: 6465 722d 636f 6c6f 722c 2364 3364 3364  der-color,#d3d3d
-00010850: 3329 293b 6375 7273 6f72 3a70 6f69 6e74  3));cursor:point
-00010860: 6572 7d2e 6672 6f6e 7465 6e64 2d69 636f  er}.frontend-ico
-00010870: 6e2d 7069 636b 6572 202e 6963 6f6e 2d63  n-picker .icon-c
-00010880: 6f6e 7461 696e 6572 202e 6963 6f6e 2d63  ontainer .icon-c
-00010890: 6c6f 7365 2d69 6e64 6963 6174 6f72 7b64  lose-indicator{d
-000108a0: 6973 706c 6179 3a62 6c6f 636b 3b62 6f72  isplay:block;bor
-000108b0: 6465 722d 7261 6469 7573 3a35 3025 3b63  der-radius:50%;c
-000108c0: 6f6c 6f72 3a76 6172 282d 2d64 6361 2d62  olor:var(--dca-b
-000108d0: 6c61 636b 2c76 6172 282d 2d62 6f64 792d  lack,var(--body-
-000108e0: 6667 2c23 3030 3029 293b 6261 636b 6772  fg,#000));backgr
-000108f0: 6f75 6e64 2d63 6f6c 6f72 3a76 6172 282d  ound-color:var(-
-00010900: 2d64 6361 2d77 6869 7465 2c76 6172 282d  -dca-white,var(-
-00010910: 2d62 6f64 792d 6267 2c23 6666 6629 293b  -body-bg,#fff));
-00010920: 7061 6464 696e 673a 2e33 7265 6d3b 626f  padding:.3rem;bo
-00010930: 7264 6572 3a31 7078 2073 6f6c 6964 2076  rder:1px solid v
-00010940: 6172 282d 2d64 6361 2d62 6c61 636b 2c76  ar(--dca-black,v
-00010950: 6172 282d 2d62 6f64 792d 6667 2c23 3030  ar(--body-fg,#00
-00010960: 3029 293b 7472 616e 7366 6f72 6d3a 7472  0));transform:tr
-00010970: 616e 736c 6174 6528 2d35 3025 2c2d 3530  anslate(-50%,-50
-00010980: 2529 3b74 6f70 3a30 3b69 6e73 6574 2d69  %);top:0;inset-i
-00010990: 6e6c 696e 652d 7374 6172 743a 3130 3025  nline-start:100%
-000109a0: 3b77 6964 7468 3a2e 3665 6d3b 6865 6967  ;width:.6em;heig
-000109b0: 6874 3a2e 3665 6d3b 6c69 6e65 2d68 6569  ht:.6em;line-hei
-000109c0: 6768 743a 2e35 656d 3b70 6f73 6974 696f  ght:.5em;positio
-000109d0: 6e3a 6162 736f 6c75 7465 3b74 7261 6e73  n:absolute;trans
-000109e0: 6974 696f 6e3a 6261 636b 6772 6f75 6e64  ition:background
-000109f0: 2d63 6f6c 6f72 202e 3135 737d 2e66 726f  -color .15s}.fro
-00010a00: 6e74 656e 642d 6963 6f6e 2d70 6963 6b65  ntend-icon-picke
-00010a10: 7220 2e69 636f 6e2d 636f 6e74 6169 6e65  r .icon-containe
-00010a20: 7220 2e69 636f 6e2d 636c 6f73 652d 696e  r .icon-close-in
-00010a30: 6469 6361 746f 723a 6265 666f 7265 7b63  dicator:before{c
-00010a40: 6f6e 7465 6e74 3a22 c397 227d 2e66 726f  ontent:".."}.fro
-00010a50: 6e74 656e 642d 6963 6f6e 2d70 6963 6b65  ntend-icon-picke
-00010a60: 7220 2e69 636f 6e2d 636f 6e74 6169 6e65  r .icon-containe
-00010a70: 7220 2e69 636f 6e2d 636c 6f73 652d 696e  r .icon-close-in
-00010a80: 6469 6361 746f 723a 686f 7665 727b 6261  dicator:hover{ba
-00010a90: 636b 6772 6f75 6e64 3a76 6172 282d 2d64  ckground:var(--d
-00010aa0: 656c 6574 652d 6275 7474 6f6e 2d62 672c  elete-button-bg,
-00010ab0: 7265 6429 3b63 6f6c 6f72 3a76 6172 282d  red);color:var(-
-00010ac0: 2d64 656c 6574 652d 6275 7474 6f6e 2d66  -delete-button-f
-00010ad0: 672c 2366 6666 293b 6375 7273 6f72 3a70  g,#fff);cursor:p
-00010ae0: 6f69 6e74 6572 7d2e 7569 702d 6d6f 6461  ointer}.uip-moda
-00010af0: 6c7b 706f 7369 7469 6f6e 3a66 6978 6564  l{position:fixed
-00010b00: 3b68 6569 6768 743a 3130 3025 3b77 6964  ;height:100%;wid
-00010b10: 7468 3a31 3030 253b 696e 7365 742d 626c  th:100%;inset-bl
-00010b20: 6f63 6b2d 656e 643a 303b 696e 7365 742d  ock-end:0;inset-
-00010b30: 696e 6c69 6e65 2d73 7461 7274 3a30 3b62  inline-start:0;b
-00010b40: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
-00010b50: 7267 6261 2830 2c30 2c30 2c2e 3829 3b7a  rgba(0,0,0,.8);z
-00010b60: 2d69 6e64 6578 3a39 3939 393b 2d77 6562  -index:9999;-web
-00010b70: 6b69 742d 7573 6572 2d73 656c 6563 743a  kit-user-select:
-00010b80: 6e6f 6e65 3b2d 6d73 2d75 7365 722d 7365  none;-ms-user-se
-00010b90: 6c65 6374 3a6e 6f6e 653b 7573 6572 2d73  lect:none;user-s
-00010ba0: 656c 6563 743a 6e6f 6e65 3b64 6973 706c  elect:none;displ
-00010bb0: 6179 3a2d 6d73 2d66 6c65 7862 6f78 3b64  ay:-ms-flexbox;d
-00010bc0: 6973 706c 6179 3a66 6c65 783b 2d6d 732d  isplay:flex;-ms-
-00010bd0: 666c 6578 2d61 6c69 676e 3a63 656e 7465  flex-align:cente
-00010be0: 723b 616c 6967 6e2d 6974 656d 733a 6365  r;align-items:ce
-00010bf0: 6e74 6572 7d2e 7569 702d 6d6f 6461 6c20  nter}.uip-modal 
-00010c00: 2a2c 2e75 6970 2d6d 6f64 616c 203a 6166  *,.uip-modal :af
-00010c10: 7465 722c 2e75 6970 2d6d 6f64 616c 203a  ter,.uip-modal :
-00010c20: 6265 666f 7265 7b62 6f78 2d73 697a 696e  before{box-sizin
-00010c30: 673a 626f 7264 6572 2d62 6f78 7d2e 7569  g:border-box}.ui
-00010c40: 702d 6d6f 6461 6c2e 7569 702d 636c 6f73  p-modal.uip-clos
-00010c50: 657b 6f70 6163 6974 793a 303b 7669 7369  e{opacity:0;visi
-00010c60: 6269 6c69 7479 3a68 6964 6465 6e3b 7472  bility:hidden;tr
-00010c70: 616e 7369 7469 6f6e 3a61 6c6c 202e 3473  ansition:all .4s
-00010c80: 2065 6173 652d 696e 2d6f 7574 7d2e 7569   ease-in-out}.ui
-00010c90: 702d 6d6f 6461 6c2e 7569 702d 6f70 656e  p-modal.uip-open
-00010ca0: 7b6f 7061 6369 7479 3a31 3b76 6973 6962  {opacity:1;visib
-00010cb0: 696c 6974 793a 7669 7369 626c 653b 7472  ility:visible;tr
-00010cc0: 616e 7369 7469 6f6e 3a61 6c6c 202e 3473  ansition:all .4s
-00010cd0: 2065 6173 652d 696e 2d6f 7574 7d2e 7569   ease-in-out}.ui
-00010ce0: 702d 6d6f 6461 6c20 2e75 6970 2d6d 6f64  p-modal .uip-mod
-00010cf0: 616c 2d2d 636f 6e74 656e 747b 706f 7369  al--content{posi
-00010d00: 7469 6f6e 3a61 6273 6f6c 7574 653b 626f  tion:absolute;bo
-00010d10: 7264 6572 2d72 6164 6975 733a 3370 783b  rder-radius:3px;
-00010d20: 626f 782d 7368 6164 6f77 3a32 7078 2038  box-shadow:2px 8
-00010d30: 7078 2032 3370 7820 3370 7820 7267 6261  px 23px 3px rgba
-00010d40: 2830 2c30 2c30 2c2e 3229 3b6f 7665 7266  (0,0,0,.2);overf
-00010d50: 6c6f 773a 6869 6464 656e 3b66 6f6e 742d  low:hidden;font-
-00010d60: 6661 6d69 6c79 3a52 6f62 6f74 6f2c 4172  family:Roboto,Ar
-00010d70: 6961 6c2c 4865 6c76 6574 6963 612c 5665  ial,Helvetica,Ve
-00010d80: 7264 616e 612c 7361 6e73 2d73 6572 6966  rdana,sans-serif
-00010d90: 3b62 6163 6b67 726f 756e 642d 636f 6c6f  ;background-colo
-00010da0: 723a 7661 7228 2d2d 6463 612d 6772 6179  r:var(--dca-gray
-00010db0: 2d6c 6967 6874 6573 742c 7661 7228 2d2d  -lightest,var(--
-00010dc0: 6461 726b 656e 6564 2d62 672c 2366 3866  darkened-bg,#f8f
-00010dd0: 3866 3829 293b 7769 6474 683a 3130 3025  8f8));width:100%
-00010de0: 3b6d 6172 6769 6e3a 6175 746f 3b6c 6566  ;margin:auto;lef
-00010df0: 743a 303b 7269 6768 743a 303b 6d61 7267  t:0;right:0;marg
-00010e00: 696e 2d62 6f74 746f 6d3a 3265 6d7d 2e75  in-bottom:2em}.u
-00010e10: 6970 2d6d 6f64 616c 202e 7569 702d 6d6f  ip-modal .uip-mo
-00010e20: 6461 6c2d 2d63 6f6e 7465 6e74 202e 7569  dal--content .ui
-00010e30: 702d 6d6f 6461 6c2d 2d68 6561 6465 727b  p-modal--header{
-00010e40: 7061 6464 696e 673a 3135 7078 2031 3570  padding:15px 15p
-00010e50: 783b 6261 636b 6772 6f75 6e64 2d63 6f6c  x;background-col
-00010e60: 6f72 3a76 6172 282d 2d64 6361 2d77 6869  or:var(--dca-whi
-00010e70: 7465 2c76 6172 282d 2d62 672d 636f 6c6f  te,var(--bg-colo
-00010e80: 722c 2366 6666 2929 3b62 6f78 2d73 6861  r,#fff));box-sha
-00010e90: 646f 773a 3020 3020 3870 7820 7267 6261  dow:0 0 8px rgba
-00010ea0: 2830 2c30 2c30 2c2e 3129 3b70 6f73 6974  (0,0,0,.1);posit
-00010eb0: 696f 6e3a 7265 6c61 7469 7665 3b7a 2d69  ion:relative;z-i
-00010ec0: 6e64 6578 3a31 3b66 6f6e 742d 7369 7a65  ndex:1;font-size
-00010ed0: 3a31 3570 783b 636f 6c6f 723a 7661 7228  :15px;color:var(
-00010ee0: 2d2d 6463 612d 6772 6179 2c76 6172 282d  --dca-gray,var(-
-00010ef0: 2d62 6f64 792d 7175 6965 742d 636f 6c6f  -body-quiet-colo
-00010f00: 722c 2336 3636 2929 3b66 6f6e 742d 7765  r,#666));font-we
-00010f10: 6967 6874 3a35 3030 3b64 6973 706c 6179  ight:500;display
-00010f20: 3a2d 6d73 2d66 6c65 7862 6f78 3b64 6973  :-ms-flexbox;dis
-00010f30: 706c 6179 3a66 6c65 783b 2d6d 732d 666c  play:flex;-ms-fl
-00010f40: 6578 2d61 6c69 676e 3a63 656e 7465 723b  ex-align:center;
-00010f50: 616c 6967 6e2d 6974 656d 733a 6365 6e74  align-items:cent
-00010f60: 6572 3b2d 6d73 2d66 6c65 782d 7061 636b  er;-ms-flex-pack
-00010f70: 3a6a 7573 7469 6679 3b6a 7573 7469 6679  :justify;justify
-00010f80: 2d63 6f6e 7465 6e74 3a73 7061 6365 2d62  -content:space-b
-00010f90: 6574 7765 656e 7d2e 7569 702d 6d6f 6461  etween}.uip-moda
-00010fa0: 6c20 2e75 6970 2d6d 6f64 616c 2d2d 636f  l .uip-modal--co
-00010fb0: 6e74 656e 7420 2e75 6970 2d6d 6f64 616c  ntent .uip-modal
-00010fc0: 2d2d 6865 6164 6572 202e 7569 702d 6d6f  --header .uip-mo
-00010fd0: 6461 6c2d 2d68 6561 6465 722d 6c6f 676f  dal--header-logo
-00010fe0: 2d74 6974 6c65 7b70 6164 6469 6e67 2d74  -title{padding-t
-00010ff0: 6f70 3a32 7078 3b6c 696e 652d 6865 6967  op:2px;line-heig
-00011000: 6874 3a31 3b74 6578 742d 7472 616e 7366  ht:1;text-transf
-00011010: 6f72 6d3a 7570 7065 7263 6173 653b 666f  orm:uppercase;fo
-00011020: 6e74 2d77 6569 6768 743a 3730 303b 6375  nt-weight:700;cu
-00011030: 7273 6f72 3a70 6f69 6e74 6572 7d2e 7569  rsor:pointer}.ui
-00011040: 702d 6d6f 6461 6c20 2e75 6970 2d6d 6f64  p-modal .uip-mod
-00011050: 616c 2d2d 636f 6e74 656e 7420 2e75 6970  al--content .uip
-00011060: 2d6d 6f64 616c 2d2d 6865 6164 6572 202e  -modal--header .
-00011070: 7569 702d 6d6f 6461 6c2d 2d68 6561 6465  uip-modal--heade
-00011080: 722d 636c 6f73 652d 6274 6e7b 6375 7273  r-close-btn{curs
-00011090: 6f72 3a70 6f69 6e74 6572 7d2e 7569 702d  or:pointer}.uip-
-000110a0: 6d6f 6461 6c20 2e75 6970 2d6d 6f64 616c  modal .uip-modal
-000110b0: 2d2d 636f 6e74 656e 7420 2e75 6970 2d6d  --content .uip-m
-000110c0: 6f64 616c 2d2d 626f 6479 7b66 6f6e 742d  odal--body{font-
-000110d0: 7369 7a65 3a31 3270 783b 6c69 6e65 2d68  size:12px;line-h
-000110e0: 6569 6768 743a 312e 353b 626f 782d 7369  eight:1.5;box-si
-000110f0: 7a69 6e67 3a62 6f72 6465 722d 626f 783b  zing:border-box;
-00011100: 7061 6464 696e 673a 303b 6865 6967 6874  padding:0;height
-00011110: 3a37 3076 683b 6469 7370 6c61 793a 2d6d  :70vh;display:-m
-00011120: 732d 666c 6578 626f 783b 6469 7370 6c61  s-flexbox;displa
-00011130: 793a 666c 6578 3b6d 696e 2d68 6569 6768  y:flex;min-heigh
-00011140: 743a 3530 7078 3b6d 6178 2d68 6569 6768  t:50px;max-heigh
-00011150: 743a 3835 7668 3b6f 7665 7266 6c6f 773a  t:85vh;overflow:
-00011160: 6175 746f 7d2e 7569 702d 6d6f 6461 6c20  auto}.uip-modal 
-00011170: 2e75 6970 2d6d 6f64 616c 2d2d 636f 6e74  .uip-modal--cont
-00011180: 656e 7420 2e75 6970 2d6d 6f64 616c 2d2d  ent .uip-modal--
-00011190: 626f 6479 202e 7569 702d 6d6f 6461 6c2d  body .uip-modal-
-000111a0: 2d73 6964 6562 6172 7b2d 6d73 2d66 6c65  -sidebar{-ms-fle
-000111b0: 782d 6e65 6761 7469 7665 3a30 3b66 6c65  x-negative:0;fle
-000111c0: 782d 7368 7269 6e6b 3a30 3b6d 6178 2d77  x-shrink:0;max-w
-000111d0: 6964 7468 3a32 3525 7d2e 7569 702d 6d6f  idth:25%}.uip-mo
-000111e0: 6461 6c20 2e75 6970 2d6d 6f64 616c 2d2d  dal .uip-modal--
-000111f0: 636f 6e74 656e 7420 2e75 6970 2d6d 6f64  content .uip-mod
-00011200: 616c 2d2d 626f 6479 202e 7569 702d 6d6f  al--body .uip-mo
-00011210: 6461 6c2d 2d73 6964 6562 6172 202e 7569  dal--sidebar .ui
-00011220: 702d 6d6f 6461 6c2d 2d73 6964 6562 6172  p-modal--sidebar
-00011230: 2d74 6162 737b 6d61 7267 696e 2d74 6f70  -tabs{margin-top
-00011240: 3a33 3070 787d 2e75 6970 2d6d 6f64 616c  :30px}.uip-modal
-00011250: 202e 7569 702d 6d6f 6461 6c2d 2d63 6f6e   .uip-modal--con
-00011260: 7465 6e74 202e 7569 702d 6d6f 6461 6c2d  tent .uip-modal-
-00011270: 2d62 6f64 7920 2e75 6970 2d6d 6f64 616c  -body .uip-modal
-00011280: 2d2d 7369 6465 6261 7220 2e75 6970 2d6d  --sidebar .uip-m
-00011290: 6f64 616c 2d2d 7369 6465 6261 722d 7461  odal--sidebar-ta
-000112a0: 6273 202e 7569 702d 6d6f 6461 6c2d 2d73  bs .uip-modal--s
-000112b0: 6964 6562 6172 2d74 6162 2d69 7465 6d7b  idebar-tab-item{
-000112c0: 7061 6464 696e 673a 3135 7078 3b66 6f6e  padding:15px;fon
-000112d0: 742d 7369 7a65 3a31 3470 783b 636f 6c6f  t-size:14px;colo
-000112e0: 723a 7661 7228 2d2d 6463 612d 6772 6179  r:var(--dca-gray
-000112f0: 2c76 6172 282d 2d62 6f64 792d 7175 6965  ,var(--body-quie
-00011300: 742d 636f 6c6f 722c 2336 3636 2929 3b74  t-color,#666));t
-00011310: 6578 742d 616c 6967 6e3a 7374 6172 743b  ext-align:start;
-00011320: 6375 7273 6f72 3a70 6f69 6e74 6572 3b70  cursor:pointer;p
-00011330: 6f73 6974 696f 6e3a 7265 6c61 7469 7665  osition:relative
-00011340: 3b64 6973 706c 6179 3a2d 6d73 2d66 6c65  ;display:-ms-fle
-00011350: 7862 6f78 3b64 6973 706c 6179 3a66 6c65  xbox;display:fle
-00011360: 783b 2d6d 732d 666c 6578 2d61 6c69 676e  x;-ms-flex-align
-00011370: 3a63 656e 7465 723b 616c 6967 6e2d 6974  :center;align-it
-00011380: 656d 733a 6365 6e74 6572 3b74 6578 742d  ems:center;text-
-00011390: 7472 616e 7366 6f72 6d3a 6361 7069 7461  transform:capita
-000113a0: 6c69 7a65 7d2e 7569 702d 6d6f 6461 6c20  lize}.uip-modal 
-000113b0: 2e75 6970 2d6d 6f64 616c 2d2d 636f 6e74  .uip-modal--cont
-000113c0: 656e 7420 2e75 6970 2d6d 6f64 616c 2d2d  ent .uip-modal--
-000113d0: 626f 6479 202e 7569 702d 6d6f 6461 6c2d  body .uip-modal-
-000113e0: 2d73 6964 6562 6172 202e 7569 702d 6d6f  -sidebar .uip-mo
-000113f0: 6461 6c2d 2d73 6964 6562 6172 2d74 6162  dal--sidebar-tab
-00011400: 7320 2e75 6970 2d6d 6f64 616c 2d2d 7369  s .uip-modal--si
-00011410: 6465 6261 722d 7461 622d 6974 656d 2069  debar-tab-item i
-00011420: 7b66 6f6e 742d 7369 7a65 3a32 3070 783b  {font-size:20px;
-00011430: 7061 6464 696e 672d 696e 6c69 6e65 2d65  padding-inline-e
-00011440: 6e64 3a31 3570 783b 636f 6c6f 723a 7661  nd:15px;color:va
-00011450: 7228 2d2d 6463 612d 6772 6179 2d6c 6967  r(--dca-gray-lig
-00011460: 6874 6572 2c76 6172 282d 2d62 6f72 6465  hter,var(--borde
-00011470: 722d 636f 6c6f 722c 2363 6363 2929 7d2e  r-color,#ccc))}.
-00011480: 7569 702d 6d6f 6461 6c20 2e75 6970 2d6d  uip-modal .uip-m
-00011490: 6f64 616c 2d2d 636f 6e74 656e 7420 2e75  odal--content .u
-000114a0: 6970 2d6d 6f64 616c 2d2d 626f 6479 202e  ip-modal--body .
-000114b0: 7569 702d 6d6f 6461 6c2d 2d73 6964 6562  uip-modal--sideb
-000114c0: 6172 202e 7569 702d 6d6f 6461 6c2d 2d73  ar .uip-modal--s
-000114d0: 6964 6562 6172 2d74 6162 7320 2e75 6970  idebar-tabs .uip
-000114e0: 2d6d 6f64 616c 2d2d 7369 6465 6261 722d  -modal--sidebar-
-000114f0: 7461 622d 6974 656d 2069 6d67 7b70 6164  tab-item img{pad
-00011500: 6469 6e67 2d69 6e6c 696e 652d 656e 643a  ding-inline-end:
-00011510: 3135 7078 7d2e 7569 702d 6d6f 6461 6c20  15px}.uip-modal 
-00011520: 2e75 6970 2d6d 6f64 616c 2d2d 636f 6e74  .uip-modal--cont
-00011530: 656e 7420 2e75 6970 2d6d 6f64 616c 2d2d  ent .uip-modal--
-00011540: 626f 6479 202e 7569 702d 6d6f 6461 6c2d  body .uip-modal-
-00011550: 2d73 6964 6562 6172 202e 7569 702d 6d6f  -sidebar .uip-mo
-00011560: 6461 6c2d 2d73 6964 6562 6172 2d74 6162  dal--sidebar-tab
-00011570: 7320 2e75 6970 2d6d 6f64 616c 2d2d 7369  s .uip-modal--si
-00011580: 6465 6261 722d 7461 622d 6974 656d 2e75  debar-tab-item.u
-00011590: 6e69 7665 7273 616c 2d61 6374 6976 657b  niversal-active{
-000115a0: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
-000115b0: 3a76 6172 282d 2d64 6361 2d77 6869 7465  :var(--dca-white
-000115c0: 2c76 6172 282d 2d62 672d 636f 6c6f 722c  ,var(--bg-color,
-000115d0: 2366 6666 2929 3b62 6f78 2d73 6861 646f  #fff));box-shado
-000115e0: 773a 3020 3670 7820 3230 7078 2030 2072  w:0 6px 20px 0 r
-000115f0: 6762 6128 302c 302c 302c 2e31 297d 2e75  gba(0,0,0,.1)}.u
-00011600: 6970 2d6d 6f64 616c 202e 7569 702d 6d6f  ip-modal .uip-mo
-00011610: 6461 6c2d 2d63 6f6e 7465 6e74 202e 7569  dal--content .ui
-00011620: 702d 6d6f 6461 6c2d 2d62 6f64 7920 2e75  p-modal--body .u
-00011630: 6970 2d6d 6f64 616c 2d2d 7369 6465 6261  ip-modal--sideba
-00011640: 7220 2e75 6970 2d6d 6f64 616c 2d2d 7369  r .uip-modal--si
-00011650: 6465 6261 722d 7461 6273 202e 7569 702d  debar-tabs .uip-
-00011660: 6d6f 6461 6c2d 2d73 6964 6562 6172 2d74  modal--sidebar-t
-00011670: 6162 2d69 7465 6d2e 756e 6976 6572 7361  ab-item.universa
-00011680: 6c2d 6163 7469 7665 3a61 6674 6572 7b63  l-active:after{c
-00011690: 6f6e 7465 6e74 3a22 223b 706f 7369 7469  ontent:"";positi
-000116a0: 6f6e 3a61 6273 6f6c 7574 653b 6865 6967  on:absolute;heig
-000116b0: 6874 3a31 3030 253b 7769 6474 683a 3570  ht:100%;width:5p
-000116c0: 783b 696e 7365 742d 626c 6f63 6b2d 7374  x;inset-block-st
-000116d0: 6172 743a 303b 696e 7365 742d 696e 6c69  art:0;inset-inli
-000116e0: 6e65 2d73 7461 7274 3a30 3b62 6163 6b67  ne-start:0;backg
-000116f0: 726f 756e 642d 636f 6c6f 723a 2330 6266  round-color:#0bf
-00011700: 7d2e 7569 702d 6d6f 6461 6c20 2e75 6970  }.uip-modal .uip
-00011710: 2d6d 6f64 616c 2d2d 636f 6e74 656e 7420  -modal--content 
-00011720: 2e75 6970 2d6d 6f64 616c 2d2d 626f 6479  .uip-modal--body
-00011730: 202e 7569 702d 6d6f 6461 6c2d 2d73 6964   .uip-modal--sid
-00011740: 6562 6172 202e 7569 702d 6d6f 6461 6c2d  ebar .uip-modal-
-00011750: 2d73 6964 6562 6172 2d74 6162 7320 2e75  -sidebar-tabs .u
-00011760: 6970 2d6d 6f64 616c 2d2d 7369 6465 6261  ip-modal--sideba
-00011770: 722d 7461 622d 6974 656d 2e75 6e69 7665  r-tab-item.unive
-00011780: 7273 616c 2d61 6374 6976 6520 697b 636f  rsal-active i{co
-00011790: 6c6f 723a 2330 6266 7d2e 7569 702d 6d6f  lor:#0bf}.uip-mo
-000117a0: 6461 6c20 2e75 6970 2d6d 6f64 616c 2d2d  dal .uip-modal--
-000117b0: 636f 6e74 656e 7420 2e75 6970 2d6d 6f64  content .uip-mod
-000117c0: 616c 2d2d 626f 6479 202e 7569 702d 6d6f  al--body .uip-mo
-000117d0: 6461 6c2d 2d73 6964 6562 6172 202e 7569  dal--sidebar .ui
-000117e0: 702d 6d6f 6461 6c2d 2d73 6964 6562 6172  p-modal--sidebar
-000117f0: 2d74 6162 7320 2e75 6970 2d6d 6f64 616c  -tabs .uip-modal
-00011800: 2d2d 7369 6465 6261 722d 7461 622d 6974  --sidebar-tab-it
-00011810: 656d 3a6f 6e6c 792d 6368 696c 647b 6469  em:only-child{di
-00011820: 7370 6c61 793a 6e6f 6e65 7d2e 7569 702d  splay:none}.uip-
-00011830: 6d6f 6461 6c20 2e75 6970 2d6d 6f64 616c  modal .uip-modal
-00011840: 2d2d 636f 6e74 656e 7420 2e75 6970 2d6d  --content .uip-m
-00011850: 6f64 616c 2d2d 626f 6479 202e 7569 702d  odal--body .uip-
-00011860: 6d6f 6461 6c2d 2d69 636f 6e2d 7072 6576  modal--icon-prev
-00011870: 6965 772d 7772 6170 7b64 6973 706c 6179  iew-wrap{display
-00011880: 3a2d 6d73 2d66 6c65 7862 6f78 3b64 6973  :-ms-flexbox;dis
-00011890: 706c 6179 3a66 6c65 783b 2d6d 732d 666c  play:flex;-ms-fl
-000118a0: 6578 2d64 6972 6563 7469 6f6e 3a63 6f6c  ex-direction:col
-000118b0: 756d 6e3b 666c 6578 2d64 6972 6563 7469  umn;flex-directi
-000118c0: 6f6e 3a63 6f6c 756d 6e3b 7061 6464 696e  on:column;paddin
-000118d0: 673a 3330 7078 2038 3070 7820 303b 7769  g:30px 80px 0;wi
-000118e0: 6474 683a 3130 3025 7d2e 7569 702d 6d6f  dth:100%}.uip-mo
-000118f0: 6461 6c20 2e75 6970 2d6d 6f64 616c 2d2d  dal .uip-modal--
-00011900: 636f 6e74 656e 7420 2e75 6970 2d6d 6f64  content .uip-mod
-00011910: 616c 2d2d 626f 6479 202e 7569 702d 6d6f  al--body .uip-mo
-00011920: 6461 6c2d 2d69 636f 6e2d 7072 6576 6965  dal--icon-previe
-00011930: 772d 7772 6170 202e 7569 702d 6d6f 6461  w-wrap .uip-moda
-00011940: 6c2d 2d69 636f 6e2d 7072 6576 6965 772d  l--icon-preview-
-00011950: 696e 6e65 727b 6f76 6572 666c 6f77 3a61  inner{overflow:a
-00011960: 7574 6f3b 6d61 7267 696e 3a32 3570 7820  uto;margin:25px 
-00011970: 2d31 3570 7820 303b 7061 6464 696e 673a  -15px 0;padding:
-00011980: 3020 3135 7078 2031 3570 787d 2e75 6970  0 15px 15px}.uip
-00011990: 2d6d 6f64 616c 202e 7569 702d 6d6f 6461  -modal .uip-moda
-000119a0: 6c2d 2d63 6f6e 7465 6e74 202e 7569 702d  l--content .uip-
-000119b0: 6d6f 6461 6c2d 2d62 6f64 7920 2e75 6970  modal--body .uip
-000119c0: 2d6d 6f64 616c 2d2d 6963 6f6e 2d70 7265  -modal--icon-pre
-000119d0: 7669 6577 2d77 7261 7020 2e75 6970 2d6d  view-wrap .uip-m
-000119e0: 6f64 616c 2d2d 6963 6f6e 2d70 7265 7669  odal--icon-previ
-000119f0: 6577 2d69 6e6e 6572 202e 7569 702d 6d6f  ew-inner .uip-mo
-00011a00: 6461 6c2d 2d69 636f 6e2d 7072 6576 6965  dal--icon-previe
-00011a10: 777b 6469 7370 6c61 793a 2d6d 732d 6772  w{display:-ms-gr
-00011a20: 6964 3b64 6973 706c 6179 3a67 7269 643b  id;display:grid;
-00011a30: 6772 6964 2d67 6170 3a32 3070 783b 6d61  grid-gap:20px;ma
-00011a40: 7267 696e 3a32 3070 7820 307d 2e75 6970  rgin:20px 0}.uip
-00011a50: 2d6d 6f64 616c 202e 7569 702d 6d6f 6461  -modal .uip-moda
-00011a60: 6c2d 2d63 6f6e 7465 6e74 202e 7569 702d  l--content .uip-
-00011a70: 6d6f 6461 6c2d 2d62 6f64 7920 2e75 6970  modal--body .uip
-00011a80: 2d6d 6f64 616c 2d2d 6963 6f6e 2d70 7265  -modal--icon-pre
-00011a90: 7669 6577 2d77 7261 7020 2e75 6970 2d6d  view-wrap .uip-m
-00011aa0: 6f64 616c 2d2d 6963 6f6e 2d70 7265 7669  odal--icon-previ
-00011ab0: 6577 2d69 6e6e 6572 202e 7569 702d 6d6f  ew-inner .uip-mo
-00011ac0: 6461 6c2d 2d69 636f 6e2d 7072 6576 6965  dal--icon-previe
-00011ad0: 7720 2e75 6970 2d69 636f 6e2d 6974 656d  w .uip-icon-item
-00011ae0: 7b70 6f73 6974 696f 6e3a 7265 6c61 7469  {position:relati
-00011af0: 7665 3b70 6164 6469 6e67 3a31 3070 783b  ve;padding:10px;
-00011b00: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
-00011b10: 3a76 6172 282d 2d64 6361 2d77 6869 7465  :var(--dca-white
-00011b20: 2c76 6172 282d 2d62 672d 636f 6c6f 722c  ,var(--bg-color,
-00011b30: 2366 6666 2929 3b62 6f78 2d73 6861 646f  #fff));box-shado
-00011b40: 773a 3020 3170 7820 3132 7078 2072 6762  w:0 1px 12px rgb
-00011b50: 6128 302c 302c 302c 2e30 3529 3b62 6f72  a(0,0,0,.05);bor
-00011b60: 6465 722d 7261 6469 7573 3a33 7078 3b63  der-radius:3px;c
-00011b70: 7572 736f 723a 706f 696e 7465 723b 7472  ursor:pointer;tr
-00011b80: 616e 7369 7469 6f6e 3a61 6c6c 202e 3373  ansition:all .3s
-00011b90: 3b6f 7665 7266 6c6f 773a 6869 6464 656e  ;overflow:hidden
-00011ba0: 7d2e 7569 702d 6d6f 6461 6c20 2e75 6970  }.uip-modal .uip
-00011bb0: 2d6d 6f64 616c 2d2d 636f 6e74 656e 7420  -modal--content 
-00011bc0: 2e75 6970 2d6d 6f64 616c 2d2d 626f 6479  .uip-modal--body
-00011bd0: 202e 7569 702d 6d6f 6461 6c2d 2d69 636f   .uip-modal--ico
-00011be0: 6e2d 7072 6576 6965 772d 7772 6170 202e  n-preview-wrap .
-00011bf0: 7569 702d 6d6f 6461 6c2d 2d69 636f 6e2d  uip-modal--icon-
-00011c00: 7072 6576 6965 772d 696e 6e65 7220 2e75  preview-inner .u
-00011c10: 6970 2d6d 6f64 616c 2d2d 6963 6f6e 2d70  ip-modal--icon-p
-00011c20: 7265 7669 6577 202e 7569 702d 6963 6f6e  review .uip-icon
-00011c30: 2d69 7465 6d3a 686f 7665 727b 626f 782d  -item:hover{box-
-00011c40: 7368 6164 6f77 3a30 2031 7078 2031 3470  shadow:0 1px 14p
-00011c50: 7820 7267 6261 2830 2c30 2c30 2c2e 3136  x rgba(0,0,0,.16
-00011c60: 297d 2e75 6970 2d6d 6f64 616c 202e 7569  )}.uip-modal .ui
-00011c70: 702d 6d6f 6461 6c2d 2d63 6f6e 7465 6e74  p-modal--content
-00011c80: 202e 7569 702d 6d6f 6461 6c2d 2d62 6f64   .uip-modal--bod
-00011c90: 7920 2e75 6970 2d6d 6f64 616c 2d2d 6963  y .uip-modal--ic
-00011ca0: 6f6e 2d70 7265 7669 6577 2d77 7261 7020  on-preview-wrap 
-00011cb0: 2e75 6970 2d6d 6f64 616c 2d2d 6963 6f6e  .uip-modal--icon
-00011cc0: 2d70 7265 7669 6577 2d69 6e6e 6572 202e  -preview-inner .
-00011cd0: 7569 702d 6d6f 6461 6c2d 2d69 636f 6e2d  uip-modal--icon-
-00011ce0: 7072 6576 6965 7720 2e75 6970 2d69 636f  preview .uip-ico
-00011cf0: 6e2d 6974 656d 2e75 6e69 7665 7273 616c  n-item.universal
-00011d00: 2d73 656c 6563 7465 647b 626f 782d 7368  -selected{box-sh
-00011d10: 6164 6f77 3a30 2031 7078 2031 3270 7820  adow:0 1px 12px 
-00011d20: 7267 6261 2830 2c30 2c30 2c2e 3035 292c  rgba(0,0,0,.05),
-00011d30: 3020 3020 3020 3370 7820 2330 6266 7d2e  0 0 0 3px #0bf}.
-00011d40: 7569 702d 6d6f 6461 6c20 2e75 6970 2d6d  uip-modal .uip-m
-00011d50: 6f64 616c 2d2d 636f 6e74 656e 7420 2e75  odal--content .u
-00011d60: 6970 2d6d 6f64 616c 2d2d 626f 6479 202e  ip-modal--body .
-00011d70: 7569 702d 6d6f 6461 6c2d 2d69 636f 6e2d  uip-modal--icon-
-00011d80: 7072 6576 6965 772d 7772 6170 202e 7569  preview-wrap .ui
-00011d90: 702d 6d6f 6461 6c2d 2d69 636f 6e2d 7072  p-modal--icon-pr
-00011da0: 6576 6965 772d 696e 6e65 7220 2e75 6970  eview-inner .uip
-00011db0: 2d6d 6f64 616c 2d2d 6963 6f6e 2d70 7265  -modal--icon-pre
-00011dc0: 7669 6577 202e 7569 702d 6963 6f6e 2d69  view .uip-icon-i
-00011dd0: 7465 6d20 2e75 6970 2d69 636f 6e2d 6974  tem .uip-icon-it
-00011de0: 656d 2d69 6e6e 6572 7b64 6973 706c 6179  em-inner{display
-00011df0: 3a2d 6d73 2d66 6c65 7862 6f78 3b64 6973  :-ms-flexbox;dis
-00011e00: 706c 6179 3a66 6c65 783b 2d6d 732d 666c  play:flex;-ms-fl
-00011e10: 6578 2d64 6972 6563 7469 6f6e 3a63 6f6c  ex-direction:col
-00011e20: 756d 6e3b 666c 6578 2d64 6972 6563 7469  umn;flex-directi
-00011e30: 6f6e 3a63 6f6c 756d 6e3b 2d6d 732d 666c  on:column;-ms-fl
-00011e40: 6578 2d61 6c69 676e 3a63 656e 7465 723b  ex-align:center;
-00011e50: 616c 6967 6e2d 6974 656d 733a 6365 6e74  align-items:cent
-00011e60: 6572 3b70 6164 6469 6e67 3a31 7078 7d2e  er;padding:1px}.
-00011e70: 7569 702d 6d6f 6461 6c20 2e75 6970 2d6d  uip-modal .uip-m
-00011e80: 6f64 616c 2d2d 636f 6e74 656e 7420 2e75  odal--content .u
-00011e90: 6970 2d6d 6f64 616c 2d2d 626f 6479 202e  ip-modal--body .
-00011ea0: 7569 702d 6d6f 6461 6c2d 2d69 636f 6e2d  uip-modal--icon-
-00011eb0: 7072 6576 6965 772d 7772 6170 202e 7569  preview-wrap .ui
-00011ec0: 702d 6d6f 6461 6c2d 2d69 636f 6e2d 7072  p-modal--icon-pr
-00011ed0: 6576 6965 772d 696e 6e65 7220 2e75 6970  eview-inner .uip
-00011ee0: 2d6d 6f64 616c 2d2d 6963 6f6e 2d70 7265  -modal--icon-pre
-00011ef0: 7669 6577 202e 7569 702d 6963 6f6e 2d69  view .uip-icon-i
-00011f00: 7465 6d20 2e75 6970 2d69 636f 6e2d 6974  tem .uip-icon-it
-00011f10: 656d 2d69 6e6e 6572 202e 7569 702d 6963  em-inner .uip-ic
-00011f20: 6f6e 2d69 7465 6d5f 5f69 636f 6e2c 2e75  on-item__icon,.u
-00011f30: 6970 2d6d 6f64 616c 202e 7569 702d 6d6f  ip-modal .uip-mo
-00011f40: 6461 6c2d 2d63 6f6e 7465 6e74 202e 7569  dal--content .ui
-00011f50: 702d 6d6f 6461 6c2d 2d62 6f64 7920 2e75  p-modal--body .u
-00011f60: 6970 2d6d 6f64 616c 2d2d 6963 6f6e 2d70  ip-modal--icon-p
-00011f70: 7265 7669 6577 2d77 7261 7020 2e75 6970  review-wrap .uip
-00011f80: 2d6d 6f64 616c 2d2d 6963 6f6e 2d70 7265  -modal--icon-pre
-00011f90: 7669 6577 2d69 6e6e 6572 202e 7569 702d  view-inner .uip-
-00011fa0: 6d6f 6461 6c2d 2d69 636f 6e2d 7072 6576  modal--icon-prev
-00011fb0: 6965 7720 2e75 6970 2d69 636f 6e2d 6974  iew .uip-icon-it
-00011fc0: 656d 202e 7569 702d 6963 6f6e 2d69 7465  em .uip-icon-ite
-00011fd0: 6d2d 696e 6e65 7220 697b 666f 6e74 2d73  m-inner i{font-s
-00011fe0: 697a 653a 3235 7078 3b63 6f6c 6f72 3a76  ize:25px;color:v
-00011ff0: 6172 282d 2d64 6361 2d67 7261 792d 6461  ar(--dca-gray-da
-00012000: 726b 6573 742c 7661 7228 2d2d 626f 6479  rkest,var(--body
-00012010: 2d66 672c 2333 3333 2929 7d2e 7569 702d  -fg,#333))}.uip-
-00012020: 6d6f 6461 6c20 2e75 6970 2d6d 6f64 616c  modal .uip-modal
-00012030: 2d2d 636f 6e74 656e 7420 2e75 6970 2d6d  --content .uip-m
-00012040: 6f64 616c 2d2d 626f 6479 202e 7569 702d  odal--body .uip-
-00012050: 6d6f 6461 6c2d 2d69 636f 6e2d 7072 6576  modal--icon-prev
-00012060: 6965 772d 7772 6170 202e 7569 702d 6d6f  iew-wrap .uip-mo
-00012070: 6461 6c2d 2d69 636f 6e2d 7072 6576 6965  dal--icon-previe
-00012080: 772d 696e 6e65 7220 2e75 6970 2d6d 6f64  w-inner .uip-mod
-00012090: 616c 2d2d 6963 6f6e 2d70 7265 7669 6577  al--icon-preview
-000120a0: 202e 7569 702d 6963 6f6e 2d69 7465 6d20   .uip-icon-item 
-000120b0: 2e75 6970 2d69 636f 6e2d 6974 656d 2d69  .uip-icon-item-i
-000120c0: 6e6e 6572 202e 7569 702d 6963 6f6e 2d69  nner .uip-icon-i
-000120d0: 7465 6d2d 6e61 6d65 7b63 6f6c 6f72 3a76  tem-name{color:v
-000120e0: 6172 282d 2d64 6361 2d67 7261 792c 7661  ar(--dca-gray,va
-000120f0: 7228 2d2d 626f 6479 2d71 7569 6574 2d63  r(--body-quiet-c
-00012100: 6f6c 6f72 2c23 3636 3629 293b 666f 6e74  olor,#666));font
-00012110: 2d73 697a 653a 3131 7078 3b70 6164 6469  -size:11px;paddi
-00012120: 6e67 3a31 3370 7820 3020 303b 6d61 782d  ng:13px 0 0;max-
-00012130: 7769 6474 683a 3130 3025 3b77 6869 7465  width:100%;white
-00012140: 2d73 7061 6365 3a6e 6f77 7261 703b 7465  -space:nowrap;te
-00012150: 7874 2d6f 7665 7266 6c6f 773a 656c 6c69  xt-overflow:elli
-00012160: 7073 6973 3b6f 7665 7266 6c6f 773a 6869  psis;overflow:hi
-00012170: 6464 656e 3b74 6578 742d 7472 616e 7366  dden;text-transf
-00012180: 6f72 6d3a 6361 7069 7461 6c69 7a65 7d2e  orm:capitalize}.
-00012190: 7569 702d 6d6f 6461 6c20 2e75 6970 2d6d  uip-modal .uip-m
-000121a0: 6f64 616c 2d2d 636f 6e74 656e 7420 2e75  odal--content .u
-000121b0: 6970 2d6d 6f64 616c 2d2d 626f 6479 202e  ip-modal--body .
-000121c0: 7569 702d 6d6f 6461 6c2d 2d69 636f 6e2d  uip-modal--icon-
-000121d0: 7072 6576 6965 772d 7772 6170 202e 7569  preview-wrap .ui
-000121e0: 702d 6d6f 6461 6c2d 2d69 636f 6e2d 7365  p-modal--icon-se
-000121f0: 6172 6368 7b70 6f73 6974 696f 6e3a 7265  arch{position:re
-00012200: 6c61 7469 7665 7d2e 7569 702d 6d6f 6461  lative}.uip-moda
-00012210: 6c20 2e75 6970 2d6d 6f64 616c 2d2d 636f  l .uip-modal--co
-00012220: 6e74 656e 7420 2e75 6970 2d6d 6f64 616c  ntent .uip-modal
-00012230: 2d2d 626f 6479 202e 7569 702d 6d6f 6461  --body .uip-moda
-00012240: 6c2d 2d69 636f 6e2d 7072 6576 6965 772d  l--icon-preview-
-00012250: 7772 6170 202e 7569 702d 6d6f 6461 6c2d  wrap .uip-modal-
-00012260: 2d69 636f 6e2d 7365 6172 6368 2069 6e70  -icon-search inp
-00012270: 7574 7b77 6964 7468 3a31 3030 253b 7061  ut{width:100%;pa
-00012280: 6464 696e 673a 3870 7820 3135 7078 3b62  dding:8px 15px;b
-00012290: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
-000122a0: 7661 7228 2d2d 6463 612d 7768 6974 652c  var(--dca-white,
-000122b0: 7661 7228 2d2d 6267 2d63 6f6c 6f72 2c23  var(--bg-color,#
-000122c0: 6666 6629 293b 626f 7264 6572 3a6e 6f6e  fff));border:non
-000122d0: 657d 2e75 6970 2d6d 6f64 616c 202e 7569  e}.uip-modal .ui
-000122e0: 702d 6d6f 6461 6c2d 2d63 6f6e 7465 6e74  p-modal--content
-000122f0: 202e 7569 702d 6d6f 6461 6c2d 2d62 6f64   .uip-modal--bod
-00012300: 7920 2e75 6970 2d6d 6f64 616c 2d2d 6963  y .uip-modal--ic
-00012310: 6f6e 2d70 7265 7669 6577 2d77 7261 7020  on-preview-wrap 
-00012320: 2e75 6970 2d6d 6f64 616c 2d2d 6963 6f6e  .uip-modal--icon
-00012330: 2d73 6561 7263 6820 696e 7075 743a 2d6d  -search input:-m
-00012340: 732d 696e 7075 742d 706c 6163 6568 6f6c  s-input-placehol
-00012350: 6465 727b 666f 6e74 2d73 7479 6c65 3a69  der{font-style:i
-00012360: 7461 6c69 637d 2e75 6970 2d6d 6f64 616c  talic}.uip-modal
-00012370: 202e 7569 702d 6d6f 6461 6c2d 2d63 6f6e   .uip-modal--con
-00012380: 7465 6e74 202e 7569 702d 6d6f 6461 6c2d  tent .uip-modal-
-00012390: 2d62 6f64 7920 2e75 6970 2d6d 6f64 616c  -body .uip-modal
-000123a0: 2d2d 6963 6f6e 2d70 7265 7669 6577 2d77  --icon-preview-w
-000123b0: 7261 7020 2e75 6970 2d6d 6f64 616c 2d2d  rap .uip-modal--
-000123c0: 6963 6f6e 2d73 6561 7263 6820 696e 7075  icon-search inpu
-000123d0: 743a 3a70 6c61 6365 686f 6c64 6572 7b66  t::placeholder{f
-000123e0: 6f6e 742d 7374 796c 653a 6974 616c 6963  ont-style:italic
-000123f0: 7d2e 7569 702d 6d6f 6461 6c20 2e75 6970  }.uip-modal .uip
-00012400: 2d6d 6f64 616c 2d2d 636f 6e74 656e 7420  -modal--content 
-00012410: 2e75 6970 2d6d 6f64 616c 2d2d 626f 6479  .uip-modal--body
-00012420: 202e 7569 702d 6d6f 6461 6c2d 2d69 636f   .uip-modal--ico
-00012430: 6e2d 7072 6576 6965 772d 7772 6170 202e  n-preview-wrap .
-00012440: 7569 702d 6d6f 6461 6c2d 2d69 636f 6e2d  uip-modal--icon-
-00012450: 7365 6172 6368 2069 6d67 7b70 6f73 6974  search img{posit
-00012460: 696f 6e3a 6162 736f 6c75 7465 3b74 6f70  ion:absolute;top
-00012470: 3a35 3025 3b74 7261 6e73 666f 726d 3a74  :50%;transform:t
-00012480: 7261 6e73 6c61 7465 5928 2d35 3025 293b  ranslateY(-50%);
-00012490: 696e 7365 742d 696e 6c69 6e65 2d65 6e64  inset-inline-end
-000124a0: 3a31 3070 787d 2e75 6970 2d6d 6f64 616c  :10px}.uip-modal
-000124b0: 202e 7569 702d 6d6f 6461 6c2d 2d66 6f6f   .uip-modal--foo
-000124c0: 7465 727b 626f 7264 6572 2d74 6f70 3a31  ter{border-top:1
-000124d0: 7078 2073 6f6c 6964 2076 6172 282d 2d64  px solid var(--d
-000124e0: 6361 2d67 7261 792d 6c69 6768 7465 722c  ca-gray-lighter,
-000124f0: 7661 7228 2d2d 626f 7264 6572 2d63 6f6c  var(--border-col
-00012500: 6f72 2c23 6363 6329 293b 7465 7874 2d61  or,#ccc));text-a
-00012510: 6c69 676e 3a63 656e 7465 723b 6261 636b  lign:center;back
-00012520: 6772 6f75 6e64 2d63 6f6c 6f72 3a76 6172  ground-color:var
-00012530: 282d 2d64 6361 2d77 6869 7465 2c76 6172  (--dca-white,var
-00012540: 282d 2d62 672d 636f 6c6f 722c 2366 6666  (--bg-color,#fff
-00012550: 2929 3b62 6f72 6465 723a 6e6f 6e65 3b64  ));border:none;d
-00012560: 6973 706c 6179 3a6e 6f6e 653b 2d6d 732d  isplay:none;-ms-
-00012570: 666c 6578 2d70 6163 6b3a 656e 643b 6a75  flex-pack:end;ju
-00012580: 7374 6966 792d 636f 6e74 656e 743a 666c  stify-content:fl
-00012590: 6578 2d65 6e64 3b70 6164 6469 6e67 3a35  ex-end;padding:5
-000125a0: 7078 3b62 6f78 2d73 6861 646f 773a 3020  px;box-shadow:0 
-000125b0: 3020 3870 7820 7267 6261 2830 2c30 2c30  0 8px rgba(0,0,0
-000125c0: 2c2e 3129 3b70 6f73 6974 696f 6e3a 7265  ,.1);position:re
-000125d0: 6c61 7469 7665 3b64 6973 706c 6179 3a2d  lative;display:-
-000125e0: 6d73 2d66 6c65 7862 6f78 3b64 6973 706c  ms-flexbox;displ
-000125f0: 6179 3a66 6c65 787d 2e75 6970 2d6d 6f64  ay:flex}.uip-mod
-00012600: 616c 202e 7569 702d 6d6f 6461 6c2d 2d66  al .uip-modal--f
-00012610: 6f6f 7465 7220 6275 7474 6f6e 2e75 6970  ooter button.uip
-00012620: 2d69 6e73 6572 742d 6963 6f6e 2d62 7574  -insert-icon-but
-00012630: 746f 6e7b 7061 6464 696e 673a 3130 7078  ton{padding:10px
-00012640: 2033 3570 7821 696d 706f 7274 616e 743b   35px!important;
-00012650: 636f 6c6f 723a 7661 7228 2d2d 6463 612d  color:var(--dca-
-00012660: 7768 6974 652c 7661 7228 2d2d 6267 2d63  white,var(--bg-c
-00012670: 6f6c 6f72 2c23 6666 6629 2921 696d 706f  olor,#fff))!impo
-00012680: 7274 616e 743b 6261 636b 6772 6f75 6e64  rtant;background
-00012690: 2d63 6f6c 6f72 3a23 3062 6621 696d 706f  -color:#0bf!impo
-000126a0: 7274 616e 743b 626f 7264 6572 3a6e 6f6e  rtant;border:non
-000126b0: 653b 6375 7273 6f72 3a70 6f69 6e74 6572  e;cursor:pointer
-000126c0: 3b6f 7574 6c69 6e65 3a30 7d2e 7569 702d  ;outline:0}.uip-
-000126d0: 6d6f 6461 6c20 2e75 6970 2d6d 6f64 616c  modal .uip-modal
-000126e0: 2d2d 666f 6f74 6572 202e 756e 6976 6572  --footer .univer
-000126f0: 7361 6c2d 6275 7474 6f6e 7b68 6569 6768  sal-button{heigh
-00012700: 743a 3430 7078 3b6d 6172 6769 6e2d 696e  t:40px;margin-in
-00012710: 6c69 6e65 2d73 7461 7274 3a35 7078 7d2e  line-start:5px}.
-00012720: 7569 702d 6d6f 6461 6c20 2e75 6970 2d6d  uip-modal .uip-m
-00012730: 6f64 616c 2d2d 666f 6f74 6572 202e 756e  odal--footer .un
-00012740: 6976 6572 7361 6c2d 6275 7474 6f6e 2d73  iversal-button-s
-00012750: 7563 6365 7373 7b70 6164 6469 6e67 3a31  uccess{padding:1
-00012760: 3270 7820 3336 7078 3b63 6f6c 6f72 3a76  2px 36px;color:v
-00012770: 6172 282d 2d64 6361 2d77 6869 7465 2c76  ar(--dca-white,v
-00012780: 6172 282d 2d62 672d 636f 6c6f 722c 2366  ar(--bg-color,#f
-00012790: 6666 2929 3b77 6964 7468 3a69 6e69 7469  ff));width:initi
-000127a0: 616c 7d2e 7569 702d 6d6f 6461 6c20 2e75  al}.uip-modal .u
-000127b0: 6970 2d6d 6f64 616c 2d2d 666f 6f74 6572  ip-modal--footer
-000127c0: 202e 756e 6976 6572 7361 6c2d 6275 7474   .universal-butt
-000127d0: 6f6e 2d73 7563 6365 7373 3a68 6f76 6572  on-success:hover
-000127e0: 7b62 6163 6b67 726f 756e 642d 636f 6c6f  {background-colo
-000127f0: 723a 2330 6266 7d40 6d65 6469 6120 286d  r:#0bf}@media (m
-00012800: 696e 2d77 6964 7468 3a31 3434 3070 7829  in-width:1440px)
-00012810: 7b62 6f64 793a 6e6f 7428 2e63 6d73 2d61  {body:not(.cms-a
-00012820: 646d 696e 2d6d 6f64 616c 2920 2e75 6970  dmin-modal) .uip
-00012830: 2d6d 6f64 616c 202e 7569 702d 6d6f 6461  -modal .uip-moda
-00012840: 6c2d 2d63 6f6e 7465 6e74 7b6d 6178 2d77  l--content{max-w
-00012850: 6964 7468 3a31 3230 3070 787d 7d40 6d65  idth:1200px}}@me
-00012860: 6469 6120 286d 6178 2d77 6964 7468 3a31  dia (max-width:1
-00012870: 3433 3970 7829 7b62 6f64 793a 6e6f 7428  439px){body:not(
-00012880: 2e63 6d73 2d61 646d 696e 2d6d 6f64 616c  .cms-admin-modal
-00012890: 2920 2e75 6970 2d6d 6f64 616c 202e 7569  ) .uip-modal .ui
-000128a0: 702d 6d6f 6461 6c2d 2d63 6f6e 7465 6e74  p-modal--content
-000128b0: 7b6d 6178 2d77 6964 7468 3a39 3930 7078  {max-width:990px
-000128c0: 7d2e 7569 702d 6d6f 6461 6c2d 2d69 636f  }.uip-modal--ico
-000128d0: 6e2d 7072 6576 6965 772d 7772 6170 7b70  n-preview-wrap{p
-000128e0: 6164 6469 6e67 3a33 3070 7820 3530 7078  adding:30px 50px
-000128f0: 2030 7d7d 406d 6564 6961 2028 6d61 782d   0}}@media (max-
-00012900: 7769 6474 683a 3130 3233 7078 297b 626f  width:1023px){bo
-00012910: 6479 3a6e 6f74 282e 636d 732d 6164 6d69  dy:not(.cms-admi
-00012920: 6e2d 6d6f 6461 6c29 202e 7569 702d 6d6f  n-modal) .uip-mo
-00012930: 6461 6c20 2e75 6970 2d6d 6f64 616c 2d2d  dal .uip-modal--
-00012940: 636f 6e74 656e 747b 6d61 782d 7769 6474  content{max-widt
-00012950: 683a 3734 3070 787d 7d40 6d65 6469 6120  h:740px}}@media 
-00012960: 286d 6178 2d77 6964 7468 3a37 3637 7078  (max-width:767px
-00012970: 297b 2e75 6970 2d6d 6f64 616c 2d2d 6963  ){.uip-modal--ic
-00012980: 6f6e 2d70 7265 7669 6577 2d77 7261 707b  on-preview-wrap{
-00012990: 7061 6464 696e 673a 3135 7078 2169 6d70  padding:15px!imp
-000129a0: 6f72 7461 6e74 7d2e 7569 702d 6d6f 6461  ortant}.uip-moda
-000129b0: 6c2d 2d73 6964 6562 6172 7b64 6973 706c  l--sidebar{displ
-000129c0: 6179 3a6e 6f6e 657d 7d40 6d65 6469 6120  ay:none}}@media 
-000129d0: 286d 696e 2d77 6964 7468 3a31 3434 3070  (min-width:1440p
-000129e0: 7829 7b2e 7569 702d 6d6f 6461 6c2d 2d69  x){.uip-modal--i
-000129f0: 636f 6e2d 7072 6576 6965 777b 2d6d 732d  con-preview{-ms-
-00012a00: 6772 6964 2d63 6f6c 756d 6e73 3a28 3166  grid-columns:(1f
-00012a10: 7229 5b37 5d3b 6772 6964 2d74 656d 706c  r)[7];grid-templ
-00012a20: 6174 652d 636f 6c75 6d6e 733a 7265 7065  ate-columns:repe
-00012a30: 6174 2837 2c31 6672 297d 7d40 6d65 6469  at(7,1fr)}}@medi
-00012a40: 6120 286d 6178 2d77 6964 7468 3a31 3433  a (max-width:143
-00012a50: 3970 7829 7b2e 7569 702d 6d6f 6461 6c2d  9px){.uip-modal-
-00012a60: 2d69 636f 6e2d 7072 6576 6965 777b 2d6d  -icon-preview{-m
-00012a70: 732d 6772 6964 2d63 6f6c 756d 6e73 3a28  s-grid-columns:(
-00012a80: 3166 7229 5b36 5d3b 6772 6964 2d74 656d  1fr)[6];grid-tem
-00012a90: 706c 6174 652d 636f 6c75 6d6e 733a 7265  plate-columns:re
-00012aa0: 7065 6174 2836 2c31 6672 297d 7d40 6d65  peat(6,1fr)}}@me
-00012ab0: 6469 6120 286d 6178 2d77 6964 7468 3a31  dia (max-width:1
-00012ac0: 3032 3470 7829 7b2e 7569 702d 6d6f 6461  024px){.uip-moda
-00012ad0: 6c2d 2d69 636f 6e2d 7072 6576 6965 777b  l--icon-preview{
-00012ae0: 2d6d 732d 6772 6964 2d63 6f6c 756d 6e73  -ms-grid-columns
-00012af0: 3a28 3166 7229 5b35 5d3b 6772 6964 2d74  :(1fr)[5];grid-t
-00012b00: 656d 706c 6174 652d 636f 6c75 6d6e 733a  emplate-columns:
-00012b10: 7265 7065 6174 2835 2c31 6672 297d 7d40  repeat(5,1fr)}}@
-00012b20: 6d65 6469 6120 286d 6178 2d77 6964 7468  media (max-width
-00012b30: 3a37 3637 7078 297b 2e75 6970 2d6d 6f64  :767px){.uip-mod
-00012b40: 616c 2d2d 6963 6f6e 2d70 7265 7669 6577  al--icon-preview
-00012b50: 7b2d 6d73 2d67 7269 642d 636f 6c75 6d6e  {-ms-grid-column
-00012b60: 733a 2831 6672 295b 345d 3b67 7269 642d  s:(1fr)[4];grid-
-00012b70: 7465 6d70 6c61 7465 2d63 6f6c 756d 6e73  template-columns
-00012b80: 3a72 6570 6561 7428 342c 3166 7229 7d7d  :repeat(4,1fr)}}
-00012b90: 406d 6564 6961 2028 6d61 782d 7769 6474  @media (max-widt
-00012ba0: 683a 3437 3970 7829 7b2e 7569 702d 6d6f  h:479px){.uip-mo
-00012bb0: 6461 6c2d 2d69 636f 6e2d 7072 6576 6965  dal--icon-previe
-00012bc0: 777b 2d6d 732d 6772 6964 2d63 6f6c 756d  w{-ms-grid-colum
-00012bd0: 6e73 3a28 3166 7229 5b33 5d3b 6772 6964  ns:(1fr)[3];grid
-00012be0: 2d74 656d 706c 6174 652d 636f 6c75 6d6e  -template-column
-00012bf0: 733a 7265 7065 6174 2833 2c31 6672 297d  s:repeat(3,1fr)}
-00012c00: 7d40 6d65 6469 6120 286d 6178 2d77 6964  }@media (max-wid
-00012c10: 7468 3a31 3433 3970 7829 7b2e 7569 702d  th:1439px){.uip-
-00012c20: 6d6f 6461 6c2d 2d73 6964 6562 6172 2d74  modal--sidebar-t
-00012c30: 6162 2d69 7465 6d7b 7061 6464 696e 673a  ab-item{padding:
-00012c40: 3135 7078 2031 3570 7820 3135 7078 2032  15px 15px 15px 2
-00012c50: 3570 783b 666f 6e74 2d73 697a 653a 3131  5px;font-size:11
-00012c60: 7078 7d2e 7569 702d 6d6f 6461 6c2d 2d73  px}.uip-modal--s
-00012c70: 6964 6562 6172 2d74 6162 2d69 7465 6d20  idebar-tab-item 
-00012c80: 697b 666f 6e74 2d73 697a 653a 3135 7078  i{font-size:15px
-00012c90: 7d7d 406d 6564 6961 2028 6d61 782d 7769  }}@media (max-wi
-00012ca0: 6474 683a 3130 3234 7078 297b 2e75 6970  dth:1024px){.uip
-00012cb0: 2d6d 6f64 616c 2d2d 7369 6465 6261 722d  -modal--sidebar-
-00012cc0: 7461 622d 6974 656d 2069 2c2e 7569 702d  tab-item i,.uip-
-00012cd0: 6d6f 6461 6c2d 2d73 6964 6562 6172 2d74  modal--sidebar-t
-00012ce0: 6162 2d69 7465 6d20 696d 677b 6469 7370  ab-item img{disp
-00012cf0: 6c61 793a 6e6f 6e65 7d7d 2e73 722d 6f6e  lay:none}}.sr-on
-00012d00: 6c79 7b70 6f73 6974 696f 6e3a 6162 736f  ly{position:abso
-00012d10: 6c75 7465 2169 6d70 6f72 7461 6e74 3b77  lute!important;w
-00012d20: 6964 7468 3a31 7078 2169 6d70 6f72 7461  idth:1px!importa
-00012d30: 6e74 3b68 6569 6768 743a 3170 7821 696d  nt;height:1px!im
-00012d40: 706f 7274 616e 743b 7061 6464 696e 673a  portant;padding:
-00012d50: 3021 696d 706f 7274 616e 743b 6d61 7267  0!important;marg
-00012d60: 696e 3a2d 3170 7821 696d 706f 7274 616e  in:-1px!importan
-00012d70: 743b 6f76 6572 666c 6f77 3a68 6964 6465  t;overflow:hidde
-00012d80: 6e21 696d 706f 7274 616e 743b 636c 6970  n!important;clip
-00012d90: 3a72 6563 7428 302c 302c 302c 3029 2169  :rect(0,0,0,0)!i
-00012da0: 6d70 6f72 7461 6e74 3b77 6869 7465 2d73  mportant;white-s
-00012db0: 7061 6365 3a6e 6f77 7261 7021 696d 706f  pace:nowrap!impo
-00012dc0: 7274 616e 743b 626f 7264 6572 3a30 2169  rtant;border:0!i
-00012dd0: 6d70 6f72 7461 6e74 7d75 6c2e 6e61 767b  mportant}ul.nav{
-00012de0: 6d61 7267 696e 2d62 6f74 746f 6d3a 3165  margin-bottom:1e
-00012df0: 6d7d 756c 2e6e 6176 3e6c 692e 6e61 762d  m}ul.nav>li.nav-
-00012e00: 6974 656d 7b6c 6973 742d 7374 796c 652d  item{list-style-
-00012e10: 7479 7065 3a6e 6f6e 653b 7061 6464 696e  type:none;paddin
-00012e20: 673a 696e 6865 7269 747d 2e63 6f6c 4d20  g:inherit}.colM 
-00012e30: 756c 3a6e 6f74 282e 6f62 6a65 6374 2d74  ul:not(.object-t
-00012e40: 6f6f 6c73 292e 6e61 767b 6d61 7267 696e  ools).nav{margin
-00012e50: 2d74 6f70 3a30 3b6d 6172 6769 6e2d 626f  -top:0;margin-bo
-00012e60: 7474 6f6d 3a32 3070 787d 756c 2e6e 6176  ttom:20px}ul.nav
-00012e70: 202e 6e61 762d 6974 656d 7b6d 6172 6769   .nav-item{margi
-00012e80: 6e2d 696e 6c69 6e65 2d65 6e64 3a31 7265  n-inline-end:1re
-00012e90: 6d7d 756c 2e6e 6176 202e 6e61 762d 6c69  m}ul.nav .nav-li
-00012ea0: 6e6b 7b70 6f73 6974 696f 6e3a 7265 6c61  nk{position:rela
-00012eb0: 7469 7665 3b74 6578 742d 6465 636f 7261  tive;text-decora
-00012ec0: 7469 6f6e 3a6e 6f6e 657d 756c 2e6e 6176  tion:none}ul.nav
-00012ed0: 202e 6e61 762d 6c69 6e6b 2073 7061 6e2e   .nav-link span.
-00012ee0: 696e 6469 6361 746f 727b 6469 7370 6c61  indicator{displa
-00012ef0: 793a 6e6f 6e65 3b62 6f72 6465 722d 7261  y:none;border-ra
-00012f00: 6469 7573 3a35 3025 3b70 6164 6469 6e67  dius:50%;padding
-00012f10: 3a2e 3572 656d 3b62 6f72 6465 723a 3170  :.5rem;border:1p
-00012f20: 7820 736f 6c69 6420 7661 7228 2d2d 6463  x solid var(--dc
-00012f30: 612d 7768 6974 652c 7661 7228 2d2d 626f  a-white,var(--bo
-00012f40: 6479 2d62 672c 2366 6666 2929 3b74 7261  dy-bg,#fff));tra
-00012f50: 6e73 666f 726d 3a74 7261 6e73 6c61 7465  nsform:translate
-00012f60: 282d 3530 252c 2d35 3025 293b 696e 7365  (-50%,-50%);inse
-00012f70: 742d 626c 6f63 6b2d 7374 6172 743a 303b  t-block-start:0;
-00012f80: 696e 7365 742d 696e 6c69 6e65 2d73 7461  inset-inline-sta
-00012f90: 7274 3a31 3030 253b 706f 7369 7469 6f6e  rt:100%;position
-00012fa0: 3a61 6273 6f6c 7574 657d 756c 2e6e 6176  :absolute}ul.nav
-00012fb0: 202e 6e61 762d 6c69 6e6b 2073 7061 6e2e   .nav-link span.
-00012fc0: 696e 6469 6361 746f 722e 6572 726f 727b  indicator.error{
-00012fd0: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
-00012fe0: 3a76 6172 282d 2d62 732d 6461 6e67 6572  :var(--bs-danger
-00012ff0: 297d 756c 2e6e 6176 202e 6e61 762d 6c69  )}ul.nav .nav-li
-00013000: 6e6b 2073 7061 6e2e 696e 6469 6361 746f  nk span.indicato
-00013010: 722e 6174 7472 6962 7574 6573 7b62 6163  r.attributes{bac
-00013020: 6b67 726f 756e 642d 636f 6c6f 723a 7661  kground-color:va
-00013030: 7228 2d2d 6273 2d69 6e66 6f29 3b64 6973  r(--bs-info);dis
-00013040: 706c 6179 3a62 6c6f 636b 7d75 6c2e 6e61  play:block}ul.na
-00013050: 7620 2e6e 6176 2d6c 696e 6b2e 6572 726f  v .nav-link.erro
-00013060: 723e 7370 616e 2e69 6e64 6963 6174 6f72  r>span.indicator
-00013070: 7b64 6973 706c 6179 3a62 6c6f 636b 7d75  {display:block}u
-00013080: 6c2e 6e61 762e 6e61 762d 7069 6c6c 7320  l.nav.nav-pills 
-00013090: 2e6e 6176 2d6c 696e 6b3a 6e6f 7428 2e61  .nav-link:not(.a
-000130a0: 6374 6976 6529 7b62 6f72 6465 722d 7374  ctive){border-st
-000130b0: 796c 653a 736f 6c69 643b 626f 7264 6572  yle:solid;border
-000130c0: 2d77 6964 7468 3a31 7078 7d62 6f64 793a  -width:1px}body:
-000130d0: 6e6f 7428 2e64 6a61 6e67 6f63 6d73 2d61  not(.djangocms-a
-000130e0: 646d 696e 2d73 7479 6c65 2920 756c 2e64  dmin-style) ul.d
-000130f0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
-00013100: 642e 6e61 762d 7461 6273 2b64 6976 2e74  d.nav-tabs+div.t
-00013110: 6162 2d63 6f6e 7465 6e74 202e 7461 622d  ab-content .tab-
-00013120: 7061 6e65 7b62 6f72 6465 722d 6c65 6674  pane{border-left
-00013130: 2d73 7479 6c65 3a73 6f6c 6964 3b62 6f72  -style:solid;bor
-00013140: 6465 722d 626f 7474 6f6d 2d73 7479 6c65  der-bottom-style
-00013150: 3a73 6f6c 6964 3b62 6f72 6465 722d 7269  :solid;border-ri
-00013160: 6768 742d 7374 796c 653a 736f 6c69 643b  ght-style:solid;
-00013170: 626f 7264 6572 2d6c 6566 742d 636f 6c6f  border-left-colo
-00013180: 723a 7661 7228 2d2d 6861 6972 6c69 6e65  r:var(--hairline
-00013190: 2d63 6f6c 6f72 293b 626f 7264 6572 2d62  -color);border-b
-000131a0: 6f74 746f 6d2d 636f 6c6f 723a 7661 7228  ottom-color:var(
-000131b0: 2d2d 6861 6972 6c69 6e65 2d63 6f6c 6f72  --hairline-color
-000131c0: 293b 626f 7264 6572 2d72 6967 6874 2d63  );border-right-c
-000131d0: 6f6c 6f72 3a76 6172 282d 2d68 6169 726c  olor:var(--hairl
-000131e0: 696e 652d 636f 6c6f 7229 3b62 6f72 6465  ine-color);borde
-000131f0: 722d 7769 6474 683a 3170 787d 626f 6479  r-width:1px}body
-00013200: 3a6e 6f74 282e 646a 616e 676f 636d 732d  :not(.djangocms-
-00013210: 6164 6d69 6e2d 7374 796c 6529 2075 6c2e  admin-style) ul.
-00013220: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-00013230: 6e64 2e6e 6176 2d74 6162 732b 6469 762e  nd.nav-tabs+div.
-00013240: 7461 622d 636f 6e74 656e 7420 2e74 6162  tab-content .tab
-00013250: 2d70 616e 6520 6669 656c 6473 6574 3a6c  -pane fieldset:l
-00013260: 6173 742d 6368 696c 647b 6d61 7267 696e  ast-child{margin
-00013270: 2d62 6f74 746f 6d3a 307d 6469 762e 7461  -bottom:0}div.ta
-00013280: 622d 706b 7b2d 6d73 2d66 6c65 782d 6974  b-pk{-ms-flex-it
-00013290: 656d 2d61 6c69 676e 3a63 656e 7465 723b  em-align:center;
-000132a0: 2d6d 732d 6772 6964 2d72 6f77 2d61 6c69  -ms-grid-row-ali
-000132b0: 676e 3a63 656e 7465 723b 616c 6967 6e2d  gn:center;align-
-000132c0: 7365 6c66 3a63 656e 7465 723b 636f 6c6f  self:center;colo
-000132d0: 723a 7661 7228 2d2d 6463 612d 6772 6179  r:var(--dca-gray
-000132e0: 2d64 6172 6b65 722c 7661 7228 2d2d 626f  -darker,var(--bo
-000132f0: 6479 2d66 672c 2333 3333 2929 3b66 6f6e  dy-fg,#333));fon
-00013300: 742d 7369 7a65 3a38 3025 3b6d 6172 6769  t-size:80%;margi
-00013310: 6e2d 696e 6c69 6e65 2d73 7461 7274 3a61  n-inline-start:a
-00013320: 7574 6f7d 2e64 6a61 6e67 6f63 6d73 2d61  uto}.djangocms-a
-00013330: 646d 696e 2d73 7479 6c65 202e 636f 6c4d  dmin-style .colM
-00013340: 2075 6c2e 6e61 763a 6e6f 7428 2e6f 626a   ul.nav:not(.obj
-00013350: 6563 742d 746f 6f6c 7329 3a6e 6f74 282e  ect-tools):not(.
-00013360: 6d65 7373 6167 656c 6973 7429 7b6d 6172  messagelist){mar
-00013370: 6769 6e2d 746f 703a 307d 2e64 6a61 6e67  gin-top:0}.djang
-00013380: 6f63 6d73 2d61 646d 696e 2d73 7479 6c65  ocms-admin-style
-00013390: 202e 636f 6c4d 2075 6c2e 6e61 763a 6e6f   .colM ul.nav:no
-000133a0: 7428 2e6f 626a 6563 742d 746f 6f6c 7329  t(.object-tools)
-000133b0: 3a6e 6f74 282e 6d65 7373 6167 656c 6973  :not(.messagelis
-000133c0: 7429 206c 692e 6e61 762d 6974 656d 7b62  t) li.nav-item{b
-000133d0: 6f72 6465 722d 746f 703a 6e6f 6e65 7d69  order-top:none}i
-000133e0: 6e70 7574 5b74 7970 653d 6e75 6d62 6572  nput[type=number
-000133f0: 5d2e 6175 746f 2d66 6965 6c64 2b73 7061  ].auto-field+spa
-00013400: 6e7b 6469 7370 6c61 793a 6e6f 6e65 3b70  n{display:none;p
-00013410: 6f73 6974 696f 6e3a 6162 736f 6c75 7465  osition:absolute
-00013420: 3b69 6e73 6574 2d62 6c6f 636b 2d65 6e64  ;inset-block-end
-00013430: 3a30 3b69 6e73 6574 2d69 6e6c 696e 652d  :0;inset-inline-
-00013440: 656e 643a 303b 7465 7874 2d61 6c69 676e  end:0;text-align
-00013450: 3a65 6e64 3b6d 6172 6769 6e2d 696e 6c69  :end;margin-inli
-00013460: 6e65 2d65 6e64 3a33 3170 783b 6d61 7267  ne-end:31px;marg
-00013470: 696e 2d62 6c6f 636b 2d65 6e64 3a32 3370  in-block-end:23p
-00013480: 783b 6375 7273 6f72 3a70 6f69 6e74 6572  x;cursor:pointer
-00013490: 7d62 6f64 793a 6e6f 7428 2e64 6a61 6e67  }body:not(.djang
-000134a0: 6f63 6d73 2d61 646d 696e 2d73 7479 6c65  ocms-admin-style
-000134b0: 2920 696e 7075 745b 7479 7065 3d6e 756d  ) input[type=num
-000134c0: 6265 725d 2e61 7574 6f2d 6669 656c 642b  ber].auto-field+
-000134d0: 7370 616e 7b6d 6172 6769 6e2d 626f 7474  span{margin-bott
-000134e0: 6f6d 3a32 3370 787d 406d 6564 6961 2028  om:23px}@media (
-000134f0: 6d61 782d 7769 6474 683a 3130 3234 7078  max-width:1024px
-00013500: 297b 626f 6479 3a6e 6f74 282e 646a 616e  ){body:not(.djan
-00013510: 676f 636d 732d 6164 6d69 6e2d 7374 796c  gocms-admin-styl
-00013520: 6529 2069 6e70 7574 5b74 7970 653d 6e75  e) input[type=nu
-00013530: 6d62 6572 5d2e 6175 746f 2d66 6965 6c64  mber].auto-field
-00013540: 2b73 7061 6e7b 6d61 7267 696e 2d62 6f74  +span{margin-bot
-00013550: 746f 6d3a 3234 7078 7d7d 696e 7075 745b  tom:24px}}input[
-00013560: 7479 7065 3d6e 756d 6265 725d 2e61 7574  type=number].aut
-00013570: 6f2d 6669 656c 642b 7370 616e 3a61 6674  o-field+span:aft
-00013580: 6572 7b63 6f6e 7465 6e74 3a22 6175 746f  er{content:"auto
-00013590: 227d 696e 7075 745b 7479 7065 3d6e 756d  "}input[type=num
-000135a0: 6265 725d 2e61 7574 6f2d 6669 656c 642e  ber].auto-field.
-000135b0: 6175 746f 7b63 6f6c 6f72 3a76 6172 282d  auto{color:var(-
-000135c0: 2d64 6361 2d77 6869 7465 2c76 6172 282d  -dca-white,var(-
-000135d0: 2d62 6f64 792d 6267 2c23 6666 6629 293b  -body-bg,#fff));
-000135e0: 6361 7265 742d 636f 6c6f 723a 7661 7228  caret-color:var(
-000135f0: 2d2d 6463 612d 626c 6163 6b2c 7661 7228  --dca-black,var(
-00013600: 2d2d 626f 6479 2d66 672c 2330 3030 2929  --body-fg,#000))
-00013610: 7d69 6e70 7574 5b74 7970 653d 6e75 6d62  }input[type=numb
-00013620: 6572 5d2e 6175 746f 2d66 6965 6c64 2e61  er].auto-field.a
-00013630: 7574 6f2b 7370 616e 7b64 6973 706c 6179  uto+span{display
-00013640: 3a62 6c6f 636b 7d                        :block}
+0000b110: 642d 7873 5f63 6f6c 202e 6669 656c 642d  d-xs_col .field-
+0000b120: 626f 7820 2e64 6973 6162 6c65 642c 2e64  box .disabled,.d
+0000b130: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000b140: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000b150: 6f77 2e66 6965 6c64 2d78 735f 636f 6c20  ow.field-xs_col 
+0000b160: 2e66 6965 6c64 426f 7820 2e64 6973 6162  .fieldBox .disab
+0000b170: 6c65 642c 2e64 6a61 6e67 6f63 6d73 2d66  led,.djangocms-f
+0000b180: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000b190: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000b1a0: 735f 6d65 202e 6669 656c 642d 626f 7820  s_me .field-box 
+0000b1b0: 2e64 6973 6162 6c65 642c 2e64 6a61 6e67  .disabled,.djang
+0000b1c0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000b1d0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000b1e0: 6965 6c64 2d78 735f 6d65 202e 6669 656c  ield-xs_me .fiel
+0000b1f0: 6442 6f78 202e 6469 7361 626c 6564 2c2e  dBox .disabled,.
+0000b200: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000b210: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000b220: 726f 772e 6669 656c 642d 7873 5f6d 7320  row.field-xs_ms 
+0000b230: 2e66 6965 6c64 2d62 6f78 202e 6469 7361  .field-box .disa
+0000b240: 626c 6564 2c2e 646a 616e 676f 636d 732d  bled,.djangocms-
+0000b250: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000b260: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000b270: 7873 5f6d 7320 2e66 6965 6c64 426f 7820  xs_ms .fieldBox 
+0000b280: 2e64 6973 6162 6c65 642c 2e64 6a61 6e67  .disabled,.djang
+0000b290: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000b2a0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000b2b0: 6965 6c64 2d78 735f 6f66 6673 6574 202e  ield-xs_offset .
+0000b2c0: 6669 656c 642d 626f 7820 2e64 6973 6162  field-box .disab
+0000b2d0: 6c65 642c 2e64 6a61 6e67 6f63 6d73 2d66  led,.djangocms-f
+0000b2e0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000b2f0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000b300: 735f 6f66 6673 6574 202e 6669 656c 6442  s_offset .fieldB
+0000b310: 6f78 202e 6469 7361 626c 6564 2c2e 646a  ox .disabled,.dj
+0000b320: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000b330: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000b340: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
+0000b350: 202e 6669 656c 642d 626f 7820 2e64 6973   .field-box .dis
+0000b360: 6162 6c65 642c 2e64 6a61 6e67 6f63 6d73  abled,.djangocms
+0000b370: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000b380: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000b390: 2d78 735f 6f72 6465 7220 2e66 6965 6c64  -xs_order .field
+0000b3a0: 426f 7820 2e64 6973 6162 6c65 642c 2e64  Box .disabled,.d
+0000b3b0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000b3c0: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+0000b3d0: 6669 656c 642d 726f 775f 636f 6c73 5f78  field-row_cols_x
+0000b3e0: 7320 2e66 6965 6c64 2d62 6f78 202e 6469  s .field-box .di
+0000b3f0: 7361 626c 6564 2c2e 646a 616e 676f 636d  sabled,.djangocm
+0000b400: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
+0000b410: 666f 726d 2d72 6f77 2e66 6965 6c64 2d72  form-row.field-r
+0000b420: 6f77 5f63 6f6c 735f 7873 202e 6669 656c  ow_cols_xs .fiel
+0000b430: 6442 6f78 202e 6469 7361 626c 6564 7b63  dBox .disabled{c
+0000b440: 6f6c 6f72 3a23 6363 633b 6261 636b 6772  olor:#ccc;backgr
+0000b450: 6f75 6e64 3a23 6565 657d 2e64 6a61 6e67  ound:#eee}.djang
+0000b460: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000b470: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000b480: 6965 6c64 2d78 735f 636f 6c20 2e66 6965  ield-xs_col .fie
+0000b490: 6c64 2d62 6f78 3a6c 6173 742d 6368 696c  ld-box:last-chil
+0000b4a0: 642c 2e64 6a61 6e67 6f63 6d73 2d66 726f  d,.djangocms-fro
+0000b4b0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000b4c0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000b4d0: 636f 6c20 2e66 6965 6c64 426f 783a 6c61  col .fieldBox:la
+0000b4e0: 7374 2d63 6869 6c64 2c2e 646a 616e 676f  st-child,.django
+0000b4f0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000b500: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000b510: 656c 642d 7873 5f6d 6520 2e66 6965 6c64  eld-xs_me .field
+0000b520: 2d62 6f78 3a6c 6173 742d 6368 696c 642c  -box:last-child,
+0000b530: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000b540: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000b550: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
+0000b560: 202e 6669 656c 6442 6f78 3a6c 6173 742d   .fieldBox:last-
+0000b570: 6368 696c 642c 2e64 6a61 6e67 6f63 6d73  child,.djangocms
+0000b580: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000b590: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000b5a0: 2d78 735f 6d73 202e 6669 656c 642d 626f  -xs_ms .field-bo
+0000b5b0: 783a 6c61 7374 2d63 6869 6c64 2c2e 646a  x:last-child,.dj
+0000b5c0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000b5d0: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000b5e0: 772e 6669 656c 642d 7873 5f6d 7320 2e66  w.field-xs_ms .f
+0000b5f0: 6965 6c64 426f 783a 6c61 7374 2d63 6869  ieldBox:last-chi
+0000b600: 6c64 2c2e 646a 616e 676f 636d 732d 6672  ld,.djangocms-fr
+0000b610: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+0000b620: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000b630: 5f6f 6666 7365 7420 2e66 6965 6c64 2d62  _offset .field-b
+0000b640: 6f78 3a6c 6173 742d 6368 696c 642c 2e64  ox:last-child,.d
+0000b650: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000b660: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000b670: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
+0000b680: 6574 202e 6669 656c 6442 6f78 3a6c 6173  et .fieldBox:las
+0000b690: 742d 6368 696c 642c 2e64 6a61 6e67 6f63  t-child,.djangoc
+0000b6a0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000b6b0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000b6c0: 6c64 2d78 735f 6f72 6465 7220 2e66 6965  ld-xs_order .fie
+0000b6d0: 6c64 2d62 6f78 3a6c 6173 742d 6368 696c  ld-box:last-chil
+0000b6e0: 642c 2e64 6a61 6e67 6f63 6d73 2d66 726f  d,.djangocms-fro
+0000b6f0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000b700: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000b710: 6f72 6465 7220 2e66 6965 6c64 426f 783a  order .fieldBox:
+0000b720: 6c61 7374 2d63 6869 6c64 2c2e 646a 616e  last-child,.djan
+0000b730: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
+0000b740: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
+0000b750: 6c64 2d72 6f77 5f63 6f6c 735f 7873 202e  ld-row_cols_xs .
+0000b760: 6669 656c 642d 626f 783a 6c61 7374 2d63  field-box:last-c
+0000b770: 6869 6c64 2c2e 646a 616e 676f 636d 732d  hild,.djangocms-
+0000b780: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
+0000b790: 726d 2d72 6f77 2e66 6965 6c64 2d72 6f77  rm-row.field-row
+0000b7a0: 5f63 6f6c 735f 7873 202e 6669 656c 6442  _cols_xs .fieldB
+0000b7b0: 6f78 3a6c 6173 742d 6368 696c 647b 626f  ox:last-child{bo
+0000b7c0: 7264 6572 2d69 6e6c 696e 652d 656e 643a  rder-inline-end:
+0000b7d0: 6e6f 6e65 7d2e 646a 616e 676f 636d 732d  none}.djangocms-
+0000b7e0: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000b7f0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000b800: 7873 5f63 6f6c 202e 6572 726f 7273 2c2e  xs_col .errors,.
+0000b810: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000b820: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000b830: 726f 772e 6669 656c 642d 7873 5f6d 6520  row.field-xs_me 
+0000b840: 2e65 7272 6f72 732c 2e64 6a61 6e67 6f63  .errors,.djangoc
+0000b850: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000b860: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000b870: 6c64 2d78 735f 6d73 202e 6572 726f 7273  ld-xs_ms .errors
+0000b880: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000b890: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000b8a0: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
+0000b8b0: 6666 7365 7420 2e65 7272 6f72 732c 2e64  ffset .errors,.d
+0000b8c0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000b8d0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000b8e0: 6f77 2e66 6965 6c64 2d78 735f 6f72 6465  ow.field-xs_orde
+0000b8f0: 7220 2e65 7272 6f72 732c 2e64 6a61 6e67  r .errors,.djang
+0000b900: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+0000b910: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+0000b920: 642d 726f 775f 636f 6c73 5f78 7320 2e65  d-row_cols_xs .e
+0000b930: 7272 6f72 737b 6d61 7267 696e 2d62 6f74  rrors{margin-bot
+0000b940: 746f 6d3a 307d 2e64 6a61 6e67 6f63 6d73  tom:0}.djangocms
+0000b950: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000b960: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000b970: 2d78 735f 636f 6c20 2e65 7272 6f72 6c69  -xs_col .errorli
+0000b980: 7374 2c2e 646a 616e 676f 636d 732d 6672  st,.djangocms-fr
+0000b990: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+0000b9a0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000b9b0: 5f6d 6520 2e65 7272 6f72 6c69 7374 2c2e  _me .errorlist,.
+0000b9c0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000b9d0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000b9e0: 726f 772e 6669 656c 642d 7873 5f6d 7320  row.field-xs_ms 
+0000b9f0: 2e65 7272 6f72 6c69 7374 2c2e 646a 616e  .errorlist,.djan
+0000ba00: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
+0000ba10: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
+0000ba20: 6669 656c 642d 7873 5f6f 6666 7365 7420  field-xs_offset 
+0000ba30: 2e65 7272 6f72 6c69 7374 2c2e 646a 616e  .errorlist,.djan
+0000ba40: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
+0000ba50: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
+0000ba60: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
+0000ba70: 6572 726f 726c 6973 742c 2e64 6a61 6e67  errorlist,.djang
+0000ba80: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+0000ba90: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+0000baa0: 642d 726f 775f 636f 6c73 5f78 7320 2e65  d-row_cols_xs .e
+0000bab0: 7272 6f72 6c69 7374 7b70 6f73 6974 696f  rrorlist{positio
+0000bac0: 6e3a 6162 736f 6c75 7465 2169 6d70 6f72  n:absolute!impor
+0000bad0: 7461 6e74 3b77 6964 7468 3a31 7078 2169  tant;width:1px!i
+0000bae0: 6d70 6f72 7461 6e74 3b68 6569 6768 743a  mportant;height:
+0000baf0: 3170 7821 696d 706f 7274 616e 743b 7061  1px!important;pa
+0000bb00: 6464 696e 673a 3021 696d 706f 7274 616e  dding:0!importan
+0000bb10: 743b 6d61 7267 696e 3a2d 3170 7821 696d  t;margin:-1px!im
+0000bb20: 706f 7274 616e 743b 6f76 6572 666c 6f77  portant;overflow
+0000bb30: 3a68 6964 6465 6e21 696d 706f 7274 616e  :hidden!importan
+0000bb40: 743b 636c 6970 3a72 6563 7428 302c 302c  t;clip:rect(0,0,
+0000bb50: 302c 3029 2169 6d70 6f72 7461 6e74 3b77  0,0)!important;w
+0000bb60: 6869 7465 2d73 7061 6365 3a6e 6f77 7261  hite-space:nowra
+0000bb70: 7021 696d 706f 7274 616e 743b 626f 7264  p!important;bord
+0000bb80: 6572 3a30 2169 6d70 6f72 7461 6e74 7d2e  er:0!important}.
+0000bb90: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000bba0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000bbb0: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
+0000bbc0: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
+0000bbd0: 656c 642d 626f 782c 2e64 6a61 6e67 6f63  eld-box,.djangoc
+0000bbe0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000bbf0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000bc00: 6c64 2d78 735f 6d65 2e66 6965 6c64 2d78  ld-xs_me.field-x
+0000bc10: 735f 6d65 202e 6669 656c 642d 626f 782c  s_me .field-box,
+0000bc20: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000bc30: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000bc40: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d73  -row.field-xs_ms
+0000bc50: 2e66 6965 6c64 2d78 735f 6d65 202e 6669  .field-xs_me .fi
+0000bc60: 656c 642d 626f 782c 2e64 6a61 6e67 6f63  eld-box,.djangoc
+0000bc70: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000bc80: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000bc90: 6c64 2d78 735f 6f66 6673 6574 2e66 6965  ld-xs_offset.fie
+0000bca0: 6c64 2d78 735f 6d65 202e 6669 656c 642d  ld-xs_me .field-
+0000bcb0: 626f 782c 2e64 6a61 6e67 6f63 6d73 2d66  box,.djangocms-f
+0000bcc0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000bcd0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000bce0: 735f 6f72 6465 722e 6669 656c 642d 7873  s_order.field-xs
+0000bcf0: 5f6d 6520 2e66 6965 6c64 2d62 6f78 2c2e  _me .field-box,.
+0000bd00: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000bd10: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
+0000bd20: 2e66 6965 6c64 2d72 6f77 5f63 6f6c 735f  .field-row_cols_
+0000bd30: 7873 2e66 6965 6c64 2d78 735f 6d65 202e  xs.field-xs_me .
+0000bd40: 6669 656c 642d 626f 787b 626f 7264 6572  field-box{border
+0000bd50: 2d62 6f74 746f 6d3a 6e6f 6e65 7d2e 646a  -bottom:none}.dj
+0000bd60: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000bd70: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000bd80: 772e 6669 656c 642d 7873 5f63 6f6c 202e  w.field-xs_col .
+0000bd90: 6669 656c 642d 626f 782d 6c61 6265 6c2c  field-box-label,
+0000bda0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000bdb0: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000bdc0: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
+0000bdd0: 202e 6669 656c 642d 626f 782d 6c61 6265   .field-box-labe
+0000bde0: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
+0000bdf0: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000be00: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000be10: 6d73 202e 6669 656c 642d 626f 782d 6c61  ms .field-box-la
+0000be20: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
+0000be30: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000be40: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000be50: 735f 6f66 6673 6574 202e 6669 656c 642d  s_offset .field-
+0000be60: 626f 782d 6c61 6265 6c2c 2e64 6a61 6e67  box-label,.djang
+0000be70: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000be80: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000be90: 6965 6c64 2d78 735f 6f72 6465 7220 2e66  ield-xs_order .f
+0000bea0: 6965 6c64 2d62 6f78 2d6c 6162 656c 2c2e  ield-box-label,.
+0000beb0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000bec0: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
+0000bed0: 2e66 6965 6c64 2d72 6f77 5f63 6f6c 735f  .field-row_cols_
+0000bee0: 7873 202e 6669 656c 642d 626f 782d 6c61  xs .field-box-la
+0000bef0: 6265 6c7b 6469 7370 6c61 793a 2d6d 732d  bel{display:-ms-
+0000bf00: 666c 6578 626f 783b 6469 7370 6c61 793a  flexbox;display:
+0000bf10: 666c 6578 3b6d 6172 6769 6e2d 746f 703a  flex;margin-top:
+0000bf20: 6175 746f 3b63 6f6c 6f72 3a23 3939 397d  auto;color:#999}
+0000bf30: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000bf40: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000bf50: 2d72 6f77 2e66 6965 6c64 2d78 735f 636f  -row.field-xs_co
+0000bf60: 6c20 2e66 6965 6c64 2d62 6f78 2d6c 6162  l .field-box-lab
+0000bf70: 656c 2061 2c2e 646a 616e 676f 636d 732d  el a,.djangocms-
+0000bf80: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000bf90: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000bfa0: 7873 5f6d 6520 2e66 6965 6c64 2d62 6f78  xs_me .field-box
+0000bfb0: 2d6c 6162 656c 2061 2c2e 646a 616e 676f  -label a,.django
+0000bfc0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000bfd0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000bfe0: 656c 642d 7873 5f6d 7320 2e66 6965 6c64  eld-xs_ms .field
+0000bff0: 2d62 6f78 2d6c 6162 656c 2061 2c2e 646a  -box-label a,.dj
+0000c000: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000c010: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000c020: 772e 6669 656c 642d 7873 5f6f 6666 7365  w.field-xs_offse
+0000c030: 7420 2e66 6965 6c64 2d62 6f78 2d6c 6162  t .field-box-lab
+0000c040: 656c 2061 2c2e 646a 616e 676f 636d 732d  el a,.djangocms-
+0000c050: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000c060: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000c070: 7873 5f6f 7264 6572 202e 6669 656c 642d  xs_order .field-
+0000c080: 626f 782d 6c61 6265 6c20 612c 2e64 6a61  box-label a,.dja
+0000c090: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000c0a0: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
+0000c0b0: 656c 642d 726f 775f 636f 6c73 5f78 7320  eld-row_cols_xs 
+0000c0c0: 2e66 6965 6c64 2d62 6f78 2d6c 6162 656c  .field-box-label
+0000c0d0: 2061 7b77 6964 7468 3a31 3030 253b 6d61   a{width:100%;ma
+0000c0e0: 7267 696e 2d74 6f70 3a61 7574 6f3b 636f  rgin-top:auto;co
+0000c0f0: 6c6f 723a 2339 3939 7d2e 646a 616e 676f  lor:#999}.django
+0000c100: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000c110: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000c120: 656c 642d 7873 5f63 6f6c 202e 6669 656c  eld-xs_col .fiel
+0000c130: 642d 626f 782d 6c61 6265 6c20 6120 612c  d-box-label a a,
+0000c140: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000c150: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000c160: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d65  -row.field-xs_me
+0000c170: 202e 6669 656c 642d 626f 782d 6c61 6265   .field-box-labe
+0000c180: 6c20 6120 612c 2e64 6a61 6e67 6f63 6d73  l a a,.djangocms
+0000c190: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000c1a0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000c1b0: 2d78 735f 6d73 202e 6669 656c 642d 626f  -xs_ms .field-bo
+0000c1c0: 782d 6c61 6265 6c20 6120 612c 2e64 6a61  x-label a a,.dja
+0000c1d0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000c1e0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000c1f0: 2e66 6965 6c64 2d78 735f 6f66 6673 6574  .field-xs_offset
+0000c200: 202e 6669 656c 642d 626f 782d 6c61 6265   .field-box-labe
+0000c210: 6c20 6120 612c 2e64 6a61 6e67 6f63 6d73  l a a,.djangocms
+0000c220: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000c230: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000c240: 2d78 735f 6f72 6465 7220 2e66 6965 6c64  -xs_order .field
+0000c250: 2d62 6f78 2d6c 6162 656c 2061 2061 2c2e  -box-label a a,.
+0000c260: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000c270: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
+0000c280: 2e66 6965 6c64 2d72 6f77 5f63 6f6c 735f  .field-row_cols_
+0000c290: 7873 202e 6669 656c 642d 626f 782d 6c61  xs .field-box-la
+0000c2a0: 6265 6c20 6120 617b 7769 6474 683a 3130  bel a a{width:10
+0000c2b0: 3025 3b6d 6172 6769 6e2d 746f 703a 6175  0%;margin-top:au
+0000c2c0: 746f 7d2e 646a 616e 676f 636d 732d 6672  to}.djangocms-fr
+0000c2d0: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+0000c2e0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000c2f0: 5f63 6f6c 202e 6669 656c 642d 6c67 5f6d  _col .field-lg_m
+0000c300: 652c 2e64 6a61 6e67 6f63 6d73 2d66 726f  e,.djangocms-fro
+0000c310: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000c320: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000c330: 636f 6c20 2e66 6965 6c64 2d6c 675f 6d73  col .field-lg_ms
+0000c340: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000c350: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000c360: 6d2d 726f 772e 6669 656c 642d 7873 5f63  m-row.field-xs_c
+0000c370: 6f6c 202e 6669 656c 642d 6d64 5f6d 652c  ol .field-md_me,
+0000c380: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000c390: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000c3a0: 2d72 6f77 2e66 6965 6c64 2d78 735f 636f  -row.field-xs_co
+0000c3b0: 6c20 2e66 6965 6c64 2d6d 645f 6d73 2c2e  l .field-md_ms,.
+0000c3c0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000c3d0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000c3e0: 726f 772e 6669 656c 642d 7873 5f63 6f6c  row.field-xs_col
+0000c3f0: 202e 6669 656c 642d 736d 5f6d 652c 2e64   .field-sm_me,.d
+0000c400: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000c410: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000c420: 6f77 2e66 6965 6c64 2d78 735f 636f 6c20  ow.field-xs_col 
+0000c430: 2e66 6965 6c64 2d73 6d5f 6d73 2c2e 646a  .field-sm_ms,.dj
+0000c440: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000c450: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000c460: 772e 6669 656c 642d 7873 5f63 6f6c 202e  w.field-xs_col .
+0000c470: 6669 656c 642d 786c 5f6d 652c 2e64 6a61  field-xl_me,.dja
+0000c480: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000c490: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000c4a0: 2e66 6965 6c64 2d78 735f 636f 6c20 2e66  .field-xs_col .f
+0000c4b0: 6965 6c64 2d78 6c5f 6d73 2c2e 646a 616e  ield-xl_ms,.djan
+0000c4c0: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
+0000c4d0: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
+0000c4e0: 6669 656c 642d 7873 5f63 6f6c 202e 6669  field-xs_col .fi
+0000c4f0: 656c 642d 7873 5f6d 652c 2e64 6a61 6e67  eld-xs_me,.djang
+0000c500: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000c510: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000c520: 6965 6c64 2d78 735f 636f 6c20 2e66 6965  ield-xs_col .fie
+0000c530: 6c64 2d78 735f 6d73 2c2e 646a 616e 676f  ld-xs_ms,.django
+0000c540: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000c550: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000c560: 656c 642d 7873 5f63 6f6c 202e 6669 656c  eld-xs_col .fiel
+0000c570: 642d 7878 6c5f 6d65 2c2e 646a 616e 676f  d-xxl_me,.django
+0000c580: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000c590: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000c5a0: 656c 642d 7873 5f63 6f6c 202e 6669 656c  eld-xs_col .fiel
+0000c5b0: 642d 7878 6c5f 6d73 2c2e 646a 616e 676f  d-xxl_ms,.django
+0000c5c0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000c5d0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000c5e0: 656c 642d 7873 5f6d 6520 2e66 6965 6c64  eld-xs_me .field
+0000c5f0: 2d6c 675f 6d65 2c2e 646a 616e 676f 636d  -lg_me,.djangocm
+0000c600: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
+0000c610: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
+0000c620: 642d 7873 5f6d 6520 2e66 6965 6c64 2d6c  d-xs_me .field-l
+0000c630: 675f 6d73 2c2e 646a 616e 676f 636d 732d  g_ms,.djangocms-
+0000c640: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000c650: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000c660: 7873 5f6d 6520 2e66 6965 6c64 2d6d 645f  xs_me .field-md_
+0000c670: 6d65 2c2e 646a 616e 676f 636d 732d 6672  me,.djangocms-fr
+0000c680: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+0000c690: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000c6a0: 5f6d 6520 2e66 6965 6c64 2d6d 645f 6d73  _me .field-md_ms
+0000c6b0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000c6c0: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000c6d0: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
+0000c6e0: 6520 2e66 6965 6c64 2d73 6d5f 6d65 2c2e  e .field-sm_me,.
+0000c6f0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000c700: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000c710: 726f 772e 6669 656c 642d 7873 5f6d 6520  row.field-xs_me 
+0000c720: 2e66 6965 6c64 2d73 6d5f 6d73 2c2e 646a  .field-sm_ms,.dj
+0000c730: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000c740: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000c750: 772e 6669 656c 642d 7873 5f6d 6520 2e66  w.field-xs_me .f
+0000c760: 6965 6c64 2d78 6c5f 6d65 2c2e 646a 616e  ield-xl_me,.djan
+0000c770: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
+0000c780: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
+0000c790: 6669 656c 642d 7873 5f6d 6520 2e66 6965  field-xs_me .fie
+0000c7a0: 6c64 2d78 6c5f 6d73 2c2e 646a 616e 676f  ld-xl_ms,.django
+0000c7b0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000c7c0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000c7d0: 656c 642d 7873 5f6d 6520 2e66 6965 6c64  eld-xs_me .field
+0000c7e0: 2d78 735f 6d65 2c2e 646a 616e 676f 636d  -xs_me,.djangocm
+0000c7f0: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
+0000c800: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
+0000c810: 642d 7873 5f6d 6520 2e66 6965 6c64 2d78  d-xs_me .field-x
+0000c820: 735f 6d73 2c2e 646a 616e 676f 636d 732d  s_ms,.djangocms-
+0000c830: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000c840: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000c850: 7873 5f6d 6520 2e66 6965 6c64 2d78 786c  xs_me .field-xxl
+0000c860: 5f6d 652c 2e64 6a61 6e67 6f63 6d73 2d66  _me,.djangocms-f
+0000c870: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000c880: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000c890: 735f 6d65 202e 6669 656c 642d 7878 6c5f  s_me .field-xxl_
+0000c8a0: 6d73 2c2e 646a 616e 676f 636d 732d 6672  ms,.djangocms-fr
+0000c8b0: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+0000c8c0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000c8d0: 5f6d 7320 2e66 6965 6c64 2d6c 675f 6d65  _ms .field-lg_me
+0000c8e0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000c8f0: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000c900: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
+0000c910: 7320 2e66 6965 6c64 2d6c 675f 6d73 2c2e  s .field-lg_ms,.
+0000c920: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000c930: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000c940: 726f 772e 6669 656c 642d 7873 5f6d 7320  row.field-xs_ms 
+0000c950: 2e66 6965 6c64 2d6d 645f 6d65 2c2e 646a  .field-md_me,.dj
+0000c960: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000c970: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000c980: 772e 6669 656c 642d 7873 5f6d 7320 2e66  w.field-xs_ms .f
+0000c990: 6965 6c64 2d6d 645f 6d73 2c2e 646a 616e  ield-md_ms,.djan
+0000c9a0: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
+0000c9b0: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
+0000c9c0: 6669 656c 642d 7873 5f6d 7320 2e66 6965  field-xs_ms .fie
+0000c9d0: 6c64 2d73 6d5f 6d65 2c2e 646a 616e 676f  ld-sm_me,.django
+0000c9e0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000c9f0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000ca00: 656c 642d 7873 5f6d 7320 2e66 6965 6c64  eld-xs_ms .field
+0000ca10: 2d73 6d5f 6d73 2c2e 646a 616e 676f 636d  -sm_ms,.djangocm
+0000ca20: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
+0000ca30: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
+0000ca40: 642d 7873 5f6d 7320 2e66 6965 6c64 2d78  d-xs_ms .field-x
+0000ca50: 6c5f 6d65 2c2e 646a 616e 676f 636d 732d  l_me,.djangocms-
+0000ca60: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000ca70: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000ca80: 7873 5f6d 7320 2e66 6965 6c64 2d78 6c5f  xs_ms .field-xl_
+0000ca90: 6d73 2c2e 646a 616e 676f 636d 732d 6672  ms,.djangocms-fr
+0000caa0: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+0000cab0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000cac0: 5f6d 7320 2e66 6965 6c64 2d78 735f 6d65  _ms .field-xs_me
+0000cad0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000cae0: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000caf0: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
+0000cb00: 7320 2e66 6965 6c64 2d78 735f 6d73 2c2e  s .field-xs_ms,.
+0000cb10: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000cb20: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000cb30: 726f 772e 6669 656c 642d 7873 5f6d 7320  row.field-xs_ms 
+0000cb40: 2e66 6965 6c64 2d78 786c 5f6d 652c 2e64  .field-xxl_me,.d
+0000cb50: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000cb60: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000cb70: 6f77 2e66 6965 6c64 2d78 735f 6d73 202e  ow.field-xs_ms .
+0000cb80: 6669 656c 642d 7878 6c5f 6d73 2c2e 646a  field-xxl_ms,.dj
+0000cb90: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000cba0: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000cbb0: 772e 6669 656c 642d 7873 5f6f 6666 7365  w.field-xs_offse
+0000cbc0: 7420 2e66 6965 6c64 2d6c 675f 6d65 2c2e  t .field-lg_me,.
+0000cbd0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000cbe0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000cbf0: 726f 772e 6669 656c 642d 7873 5f6f 6666  row.field-xs_off
+0000cc00: 7365 7420 2e66 6965 6c64 2d6c 675f 6d73  set .field-lg_ms
+0000cc10: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000cc20: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000cc30: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
+0000cc40: 6666 7365 7420 2e66 6965 6c64 2d6d 645f  ffset .field-md_
+0000cc50: 6d65 2c2e 646a 616e 676f 636d 732d 6672  me,.djangocms-fr
+0000cc60: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+0000cc70: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000cc80: 5f6f 6666 7365 7420 2e66 6965 6c64 2d6d  _offset .field-m
+0000cc90: 645f 6d73 2c2e 646a 616e 676f 636d 732d  d_ms,.djangocms-
+0000cca0: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000ccb0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000ccc0: 7873 5f6f 6666 7365 7420 2e66 6965 6c64  xs_offset .field
+0000ccd0: 2d73 6d5f 6d65 2c2e 646a 616e 676f 636d  -sm_me,.djangocm
+0000cce0: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
+0000ccf0: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
+0000cd00: 642d 7873 5f6f 6666 7365 7420 2e66 6965  d-xs_offset .fie
+0000cd10: 6c64 2d73 6d5f 6d73 2c2e 646a 616e 676f  ld-sm_ms,.django
+0000cd20: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000cd30: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000cd40: 656c 642d 7873 5f6f 6666 7365 7420 2e66  eld-xs_offset .f
+0000cd50: 6965 6c64 2d78 6c5f 6d65 2c2e 646a 616e  ield-xl_me,.djan
+0000cd60: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
+0000cd70: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
+0000cd80: 6669 656c 642d 7873 5f6f 6666 7365 7420  field-xs_offset 
+0000cd90: 2e66 6965 6c64 2d78 6c5f 6d73 2c2e 646a  .field-xl_ms,.dj
+0000cda0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000cdb0: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000cdc0: 772e 6669 656c 642d 7873 5f6f 6666 7365  w.field-xs_offse
+0000cdd0: 7420 2e66 6965 6c64 2d78 735f 6d65 2c2e  t .field-xs_me,.
+0000cde0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000cdf0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000ce00: 726f 772e 6669 656c 642d 7873 5f6f 6666  row.field-xs_off
+0000ce10: 7365 7420 2e66 6965 6c64 2d78 735f 6d73  set .field-xs_ms
+0000ce20: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000ce30: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000ce40: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
+0000ce50: 6666 7365 7420 2e66 6965 6c64 2d78 786c  ffset .field-xxl
+0000ce60: 5f6d 652c 2e64 6a61 6e67 6f63 6d73 2d66  _me,.djangocms-f
+0000ce70: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000ce80: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000ce90: 735f 6f66 6673 6574 202e 6669 656c 642d  s_offset .field-
+0000cea0: 7878 6c5f 6d73 2c2e 646a 616e 676f 636d  xxl_ms,.djangocm
+0000ceb0: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
+0000cec0: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
+0000ced0: 642d 7873 5f6f 7264 6572 202e 6669 656c  d-xs_order .fiel
+0000cee0: 642d 6c67 5f6d 652c 2e64 6a61 6e67 6f63  d-lg_me,.djangoc
+0000cef0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000cf00: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000cf10: 6c64 2d78 735f 6f72 6465 7220 2e66 6965  ld-xs_order .fie
+0000cf20: 6c64 2d6c 675f 6d73 2c2e 646a 616e 676f  ld-lg_ms,.django
+0000cf30: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000cf40: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000cf50: 656c 642d 7873 5f6f 7264 6572 202e 6669  eld-xs_order .fi
+0000cf60: 656c 642d 6d64 5f6d 652c 2e64 6a61 6e67  eld-md_me,.djang
+0000cf70: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000cf80: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000cf90: 6965 6c64 2d78 735f 6f72 6465 7220 2e66  ield-xs_order .f
+0000cfa0: 6965 6c64 2d6d 645f 6d73 2c2e 646a 616e  ield-md_ms,.djan
+0000cfb0: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
+0000cfc0: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
+0000cfd0: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
+0000cfe0: 6669 656c 642d 736d 5f6d 652c 2e64 6a61  field-sm_me,.dja
+0000cff0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000d000: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000d010: 2e66 6965 6c64 2d78 735f 6f72 6465 7220  .field-xs_order 
+0000d020: 2e66 6965 6c64 2d73 6d5f 6d73 2c2e 646a  .field-sm_ms,.dj
+0000d030: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000d040: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000d050: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
+0000d060: 202e 6669 656c 642d 786c 5f6d 652c 2e64   .field-xl_me,.d
+0000d070: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000d080: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000d090: 6f77 2e66 6965 6c64 2d78 735f 6f72 6465  ow.field-xs_orde
+0000d0a0: 7220 2e66 6965 6c64 2d78 6c5f 6d73 2c2e  r .field-xl_ms,.
+0000d0b0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000d0c0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000d0d0: 726f 772e 6669 656c 642d 7873 5f6f 7264  row.field-xs_ord
+0000d0e0: 6572 202e 6669 656c 642d 7873 5f6d 652c  er .field-xs_me,
+0000d0f0: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000d100: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000d110: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f72  -row.field-xs_or
+0000d120: 6465 7220 2e66 6965 6c64 2d78 735f 6d73  der .field-xs_ms
+0000d130: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000d140: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000d150: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
+0000d160: 7264 6572 202e 6669 656c 642d 7878 6c5f  rder .field-xxl_
+0000d170: 6d65 2c2e 646a 616e 676f 636d 732d 6672  me,.djangocms-fr
+0000d180: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+0000d190: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000d1a0: 5f6f 7264 6572 202e 6669 656c 642d 7878  _order .field-xx
+0000d1b0: 6c5f 6d73 2c2e 646a 616e 676f 636d 732d  l_ms,.djangocms-
+0000d1c0: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
+0000d1d0: 726d 2d72 6f77 2e66 6965 6c64 2d72 6f77  rm-row.field-row
+0000d1e0: 5f63 6f6c 735f 7873 202e 6669 656c 642d  _cols_xs .field-
+0000d1f0: 6c67 5f6d 652c 2e64 6a61 6e67 6f63 6d73  lg_me,.djangocms
+0000d200: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+0000d210: 6f72 6d2d 726f 772e 6669 656c 642d 726f  orm-row.field-ro
+0000d220: 775f 636f 6c73 5f78 7320 2e66 6965 6c64  w_cols_xs .field
+0000d230: 2d6c 675f 6d73 2c2e 646a 616e 676f 636d  -lg_ms,.djangocm
+0000d240: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
+0000d250: 666f 726d 2d72 6f77 2e66 6965 6c64 2d72  form-row.field-r
+0000d260: 6f77 5f63 6f6c 735f 7873 202e 6669 656c  ow_cols_xs .fiel
+0000d270: 642d 6d64 5f6d 652c 2e64 6a61 6e67 6f63  d-md_me,.djangoc
+0000d280: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+0000d290: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000d2a0: 726f 775f 636f 6c73 5f78 7320 2e66 6965  row_cols_xs .fie
+0000d2b0: 6c64 2d6d 645f 6d73 2c2e 646a 616e 676f  ld-md_ms,.django
+0000d2c0: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
+0000d2d0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000d2e0: 2d72 6f77 5f63 6f6c 735f 7873 202e 6669  -row_cols_xs .fi
+0000d2f0: 656c 642d 736d 5f6d 652c 2e64 6a61 6e67  eld-sm_me,.djang
+0000d300: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+0000d310: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+0000d320: 642d 726f 775f 636f 6c73 5f78 7320 2e66  d-row_cols_xs .f
+0000d330: 6965 6c64 2d73 6d5f 6d73 2c2e 646a 616e  ield-sm_ms,.djan
+0000d340: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
+0000d350: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
+0000d360: 6c64 2d72 6f77 5f63 6f6c 735f 7873 202e  ld-row_cols_xs .
+0000d370: 6669 656c 642d 786c 5f6d 652c 2e64 6a61  field-xl_me,.dja
+0000d380: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000d390: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
+0000d3a0: 656c 642d 726f 775f 636f 6c73 5f78 7320  eld-row_cols_xs 
+0000d3b0: 2e66 6965 6c64 2d78 6c5f 6d73 2c2e 646a  .field-xl_ms,.dj
+0000d3c0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000d3d0: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
+0000d3e0: 6965 6c64 2d72 6f77 5f63 6f6c 735f 7873  ield-row_cols_xs
+0000d3f0: 202e 6669 656c 642d 7873 5f6d 652c 2e64   .field-xs_me,.d
+0000d400: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000d410: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+0000d420: 6669 656c 642d 726f 775f 636f 6c73 5f78  field-row_cols_x
+0000d430: 7320 2e66 6965 6c64 2d78 735f 6d73 2c2e  s .field-xs_ms,.
+0000d440: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000d450: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
+0000d460: 2e66 6965 6c64 2d72 6f77 5f63 6f6c 735f  .field-row_cols_
+0000d470: 7873 202e 6669 656c 642d 7878 6c5f 6d65  xs .field-xxl_me
+0000d480: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000d490: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
+0000d4a0: 6f77 2e66 6965 6c64 2d72 6f77 5f63 6f6c  ow.field-row_col
+0000d4b0: 735f 7873 202e 6669 656c 642d 7878 6c5f  s_xs .field-xxl_
+0000d4c0: 6d73 7b74 6578 742d 616c 6967 6e3a 7374  ms{text-align:st
+0000d4d0: 6172 747d 2e64 6a61 6e67 6f63 6d73 2d66  art}.djangocms-f
+0000d4e0: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000d4f0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000d500: 735f 636f 6c20 2e66 6965 6c64 2d6c 675f  s_col .field-lg_
+0000d510: 6d65 206c 6162 656c 2c2e 646a 616e 676f  me label,.django
+0000d520: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000d530: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000d540: 656c 642d 7873 5f63 6f6c 202e 6669 656c  eld-xs_col .fiel
+0000d550: 642d 6c67 5f6d 7320 6c61 6265 6c2c 2e64  d-lg_ms label,.d
+0000d560: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000d570: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000d580: 6f77 2e66 6965 6c64 2d78 735f 636f 6c20  ow.field-xs_col 
+0000d590: 2e66 6965 6c64 2d6d 645f 6d65 206c 6162  .field-md_me lab
+0000d5a0: 656c 2c2e 646a 616e 676f 636d 732d 6672  el,.djangocms-fr
+0000d5b0: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+0000d5c0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000d5d0: 5f63 6f6c 202e 6669 656c 642d 6d64 5f6d  _col .field-md_m
+0000d5e0: 7320 6c61 6265 6c2c 2e64 6a61 6e67 6f63  s label,.djangoc
+0000d5f0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000d600: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000d610: 6c64 2d78 735f 636f 6c20 2e66 6965 6c64  ld-xs_col .field
+0000d620: 2d73 6d5f 6d65 206c 6162 656c 2c2e 646a  -sm_me label,.dj
+0000d630: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000d640: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000d650: 772e 6669 656c 642d 7873 5f63 6f6c 202e  w.field-xs_col .
+0000d660: 6669 656c 642d 736d 5f6d 7320 6c61 6265  field-sm_ms labe
+0000d670: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
+0000d680: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000d690: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000d6a0: 636f 6c20 2e66 6965 6c64 2d78 6c5f 6d65  col .field-xl_me
+0000d6b0: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
+0000d6c0: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
+0000d6d0: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
+0000d6e0: 642d 7873 5f63 6f6c 202e 6669 656c 642d  d-xs_col .field-
+0000d6f0: 786c 5f6d 7320 6c61 6265 6c2c 2e64 6a61  xl_ms label,.dja
+0000d700: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000d710: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000d720: 2e66 6965 6c64 2d78 735f 636f 6c20 2e66  .field-xs_col .f
+0000d730: 6965 6c64 2d78 735f 6d65 206c 6162 656c  ield-xs_me label
+0000d740: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000d750: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000d760: 6d2d 726f 772e 6669 656c 642d 7873 5f63  m-row.field-xs_c
+0000d770: 6f6c 202e 6669 656c 642d 7873 5f6d 7320  ol .field-xs_ms 
+0000d780: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000d790: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000d7a0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000d7b0: 2d78 735f 636f 6c20 2e66 6965 6c64 2d78  -xs_col .field-x
+0000d7c0: 786c 5f6d 6520 6c61 6265 6c2c 2e64 6a61  xl_me label,.dja
+0000d7d0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000d7e0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000d7f0: 2e66 6965 6c64 2d78 735f 636f 6c20 2e66  .field-xs_col .f
+0000d800: 6965 6c64 2d78 786c 5f6d 7320 6c61 6265  ield-xxl_ms labe
+0000d810: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
+0000d820: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000d830: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000d840: 6d65 202e 6669 656c 642d 6c67 5f6d 6520  me .field-lg_me 
+0000d850: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000d860: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000d870: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000d880: 2d78 735f 6d65 202e 6669 656c 642d 6c67  -xs_me .field-lg
+0000d890: 5f6d 7320 6c61 6265 6c2c 2e64 6a61 6e67  _ms label,.djang
+0000d8a0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000d8b0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000d8c0: 6965 6c64 2d78 735f 6d65 202e 6669 656c  ield-xs_me .fiel
+0000d8d0: 642d 6d64 5f6d 6520 6c61 6265 6c2c 2e64  d-md_me label,.d
+0000d8e0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000d8f0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000d900: 6f77 2e66 6965 6c64 2d78 735f 6d65 202e  ow.field-xs_me .
+0000d910: 6669 656c 642d 6d64 5f6d 7320 6c61 6265  field-md_ms labe
+0000d920: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
+0000d930: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000d940: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000d950: 6d65 202e 6669 656c 642d 736d 5f6d 6520  me .field-sm_me 
+0000d960: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000d970: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000d980: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000d990: 2d78 735f 6d65 202e 6669 656c 642d 736d  -xs_me .field-sm
+0000d9a0: 5f6d 7320 6c61 6265 6c2c 2e64 6a61 6e67  _ms label,.djang
+0000d9b0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000d9c0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000d9d0: 6965 6c64 2d78 735f 6d65 202e 6669 656c  ield-xs_me .fiel
+0000d9e0: 642d 786c 5f6d 6520 6c61 6265 6c2c 2e64  d-xl_me label,.d
+0000d9f0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000da00: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000da10: 6f77 2e66 6965 6c64 2d78 735f 6d65 202e  ow.field-xs_me .
+0000da20: 6669 656c 642d 786c 5f6d 7320 6c61 6265  field-xl_ms labe
+0000da30: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
+0000da40: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000da50: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000da60: 6d65 202e 6669 656c 642d 7873 5f6d 6520  me .field-xs_me 
+0000da70: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000da80: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000da90: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000daa0: 2d78 735f 6d65 202e 6669 656c 642d 7873  -xs_me .field-xs
+0000dab0: 5f6d 7320 6c61 6265 6c2c 2e64 6a61 6e67  _ms label,.djang
+0000dac0: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000dad0: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000dae0: 6965 6c64 2d78 735f 6d65 202e 6669 656c  ield-xs_me .fiel
+0000daf0: 642d 7878 6c5f 6d65 206c 6162 656c 2c2e  d-xxl_me label,.
+0000db00: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000db10: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000db20: 726f 772e 6669 656c 642d 7873 5f6d 6520  row.field-xs_me 
+0000db30: 2e66 6965 6c64 2d78 786c 5f6d 7320 6c61  .field-xxl_ms la
+0000db40: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
+0000db50: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000db60: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000db70: 735f 6d73 202e 6669 656c 642d 6c67 5f6d  s_ms .field-lg_m
+0000db80: 6520 6c61 6265 6c2c 2e64 6a61 6e67 6f63  e label,.djangoc
+0000db90: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000dba0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000dbb0: 6c64 2d78 735f 6d73 202e 6669 656c 642d  ld-xs_ms .field-
+0000dbc0: 6c67 5f6d 7320 6c61 6265 6c2c 2e64 6a61  lg_ms label,.dja
+0000dbd0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000dbe0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000dbf0: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
+0000dc00: 656c 642d 6d64 5f6d 6520 6c61 6265 6c2c  eld-md_me label,
+0000dc10: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000dc20: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000dc30: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d73  -row.field-xs_ms
+0000dc40: 202e 6669 656c 642d 6d64 5f6d 7320 6c61   .field-md_ms la
+0000dc50: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
+0000dc60: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000dc70: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000dc80: 735f 6d73 202e 6669 656c 642d 736d 5f6d  s_ms .field-sm_m
+0000dc90: 6520 6c61 6265 6c2c 2e64 6a61 6e67 6f63  e label,.djangoc
+0000dca0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000dcb0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000dcc0: 6c64 2d78 735f 6d73 202e 6669 656c 642d  ld-xs_ms .field-
+0000dcd0: 736d 5f6d 7320 6c61 6265 6c2c 2e64 6a61  sm_ms label,.dja
+0000dce0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000dcf0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000dd00: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
+0000dd10: 656c 642d 786c 5f6d 6520 6c61 6265 6c2c  eld-xl_me label,
+0000dd20: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000dd30: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000dd40: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d73  -row.field-xs_ms
+0000dd50: 202e 6669 656c 642d 786c 5f6d 7320 6c61   .field-xl_ms la
+0000dd60: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
+0000dd70: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000dd80: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000dd90: 735f 6d73 202e 6669 656c 642d 7873 5f6d  s_ms .field-xs_m
+0000dda0: 6520 6c61 6265 6c2c 2e64 6a61 6e67 6f63  e label,.djangoc
+0000ddb0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000ddc0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000ddd0: 6c64 2d78 735f 6d73 202e 6669 656c 642d  ld-xs_ms .field-
+0000dde0: 7873 5f6d 7320 6c61 6265 6c2c 2e64 6a61  xs_ms label,.dja
+0000ddf0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000de00: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000de10: 2e66 6965 6c64 2d78 735f 6d73 202e 6669  .field-xs_ms .fi
+0000de20: 656c 642d 7878 6c5f 6d65 206c 6162 656c  eld-xxl_me label
+0000de30: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000de40: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000de50: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
+0000de60: 7320 2e66 6965 6c64 2d78 786c 5f6d 7320  s .field-xxl_ms 
+0000de70: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000de80: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000de90: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000dea0: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
+0000deb0: 642d 6c67 5f6d 6520 6c61 6265 6c2c 2e64  d-lg_me label,.d
+0000dec0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000ded0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000dee0: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
+0000def0: 6574 202e 6669 656c 642d 6c67 5f6d 7320  et .field-lg_ms 
+0000df00: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000df10: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000df20: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000df30: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
+0000df40: 642d 6d64 5f6d 6520 6c61 6265 6c2c 2e64  d-md_me label,.d
+0000df50: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000df60: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000df70: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
+0000df80: 6574 202e 6669 656c 642d 6d64 5f6d 7320  et .field-md_ms 
+0000df90: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000dfa0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000dfb0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000dfc0: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
+0000dfd0: 642d 736d 5f6d 6520 6c61 6265 6c2c 2e64  d-sm_me label,.d
+0000dfe0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000dff0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000e000: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
+0000e010: 6574 202e 6669 656c 642d 736d 5f6d 7320  et .field-sm_ms 
+0000e020: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000e030: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000e040: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000e050: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
+0000e060: 642d 786c 5f6d 6520 6c61 6265 6c2c 2e64  d-xl_me label,.d
+0000e070: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000e080: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000e090: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
+0000e0a0: 6574 202e 6669 656c 642d 786c 5f6d 7320  et .field-xl_ms 
+0000e0b0: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000e0c0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000e0d0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000e0e0: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
+0000e0f0: 642d 7873 5f6d 6520 6c61 6265 6c2c 2e64  d-xs_me label,.d
+0000e100: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000e110: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000e120: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
+0000e130: 6574 202e 6669 656c 642d 7873 5f6d 7320  et .field-xs_ms 
+0000e140: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000e150: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000e160: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000e170: 2d78 735f 6f66 6673 6574 202e 6669 656c  -xs_offset .fiel
+0000e180: 642d 7878 6c5f 6d65 206c 6162 656c 2c2e  d-xxl_me label,.
+0000e190: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000e1a0: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000e1b0: 726f 772e 6669 656c 642d 7873 5f6f 6666  row.field-xs_off
+0000e1c0: 7365 7420 2e66 6965 6c64 2d78 786c 5f6d  set .field-xxl_m
+0000e1d0: 7320 6c61 6265 6c2c 2e64 6a61 6e67 6f63  s label,.djangoc
+0000e1e0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000e1f0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000e200: 6c64 2d78 735f 6f72 6465 7220 2e66 6965  ld-xs_order .fie
+0000e210: 6c64 2d6c 675f 6d65 206c 6162 656c 2c2e  ld-lg_me label,.
+0000e220: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000e230: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000e240: 726f 772e 6669 656c 642d 7873 5f6f 7264  row.field-xs_ord
+0000e250: 6572 202e 6669 656c 642d 6c67 5f6d 7320  er .field-lg_ms 
+0000e260: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000e270: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000e280: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000e290: 2d78 735f 6f72 6465 7220 2e66 6965 6c64  -xs_order .field
+0000e2a0: 2d6d 645f 6d65 206c 6162 656c 2c2e 646a  -md_me label,.dj
+0000e2b0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000e2c0: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000e2d0: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
+0000e2e0: 202e 6669 656c 642d 6d64 5f6d 7320 6c61   .field-md_ms la
+0000e2f0: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
+0000e300: 726f 6e74 656e 642d 636f 6c75 6d6e 202e  rontend-column .
+0000e310: 666f 726d 2d72 6f77 2e66 6965 6c64 2d78  form-row.field-x
+0000e320: 735f 6f72 6465 7220 2e66 6965 6c64 2d73  s_order .field-s
+0000e330: 6d5f 6d65 206c 6162 656c 2c2e 646a 616e  m_me label,.djan
+0000e340: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
+0000e350: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
+0000e360: 6669 656c 642d 7873 5f6f 7264 6572 202e  field-xs_order .
+0000e370: 6669 656c 642d 736d 5f6d 7320 6c61 6265  field-sm_ms labe
+0000e380: 6c2c 2e64 6a61 6e67 6f63 6d73 2d66 726f  l,.djangocms-fro
+0000e390: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000e3a0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000e3b0: 6f72 6465 7220 2e66 6965 6c64 2d78 6c5f  order .field-xl_
+0000e3c0: 6d65 206c 6162 656c 2c2e 646a 616e 676f  me label,.django
+0000e3d0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000e3e0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000e3f0: 656c 642d 7873 5f6f 7264 6572 202e 6669  eld-xs_order .fi
+0000e400: 656c 642d 786c 5f6d 7320 6c61 6265 6c2c  eld-xl_ms label,
+0000e410: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000e420: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000e430: 2d72 6f77 2e66 6965 6c64 2d78 735f 6f72  -row.field-xs_or
+0000e440: 6465 7220 2e66 6965 6c64 2d78 735f 6d65  der .field-xs_me
+0000e450: 206c 6162 656c 2c2e 646a 616e 676f 636d   label,.djangocm
+0000e460: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
+0000e470: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
+0000e480: 642d 7873 5f6f 7264 6572 202e 6669 656c  d-xs_order .fiel
+0000e490: 642d 7873 5f6d 7320 6c61 6265 6c2c 2e64  d-xs_ms label,.d
+0000e4a0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000e4b0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000e4c0: 6f77 2e66 6965 6c64 2d78 735f 6f72 6465  ow.field-xs_orde
+0000e4d0: 7220 2e66 6965 6c64 2d78 786c 5f6d 6520  r .field-xxl_me 
+0000e4e0: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000e4f0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000e500: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000e510: 2d78 735f 6f72 6465 7220 2e66 6965 6c64  -xs_order .field
+0000e520: 2d78 786c 5f6d 7320 6c61 6265 6c2c 2e64  -xxl_ms label,.d
+0000e530: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000e540: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+0000e550: 6669 656c 642d 726f 775f 636f 6c73 5f78  field-row_cols_x
+0000e560: 7320 2e66 6965 6c64 2d6c 675f 6d65 206c  s .field-lg_me l
+0000e570: 6162 656c 2c2e 646a 616e 676f 636d 732d  abel,.djangocms-
+0000e580: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
+0000e590: 726d 2d72 6f77 2e66 6965 6c64 2d72 6f77  rm-row.field-row
+0000e5a0: 5f63 6f6c 735f 7873 202e 6669 656c 642d  _cols_xs .field-
+0000e5b0: 6c67 5f6d 7320 6c61 6265 6c2c 2e64 6a61  lg_ms label,.dja
+0000e5c0: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000e5d0: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
+0000e5e0: 656c 642d 726f 775f 636f 6c73 5f78 7320  eld-row_cols_xs 
+0000e5f0: 2e66 6965 6c64 2d6d 645f 6d65 206c 6162  .field-md_me lab
+0000e600: 656c 2c2e 646a 616e 676f 636d 732d 6672  el,.djangocms-fr
+0000e610: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
+0000e620: 2d72 6f77 2e66 6965 6c64 2d72 6f77 5f63  -row.field-row_c
+0000e630: 6f6c 735f 7873 202e 6669 656c 642d 6d64  ols_xs .field-md
+0000e640: 5f6d 7320 6c61 6265 6c2c 2e64 6a61 6e67  _ms label,.djang
+0000e650: 6f63 6d73 2d66 726f 6e74 656e 642d 726f  ocms-frontend-ro
+0000e660: 7720 2e66 6f72 6d2d 726f 772e 6669 656c  w .form-row.fiel
+0000e670: 642d 726f 775f 636f 6c73 5f78 7320 2e66  d-row_cols_xs .f
+0000e680: 6965 6c64 2d73 6d5f 6d65 206c 6162 656c  ield-sm_me label
+0000e690: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000e6a0: 7465 6e64 2d72 6f77 202e 666f 726d 2d72  tend-row .form-r
+0000e6b0: 6f77 2e66 6965 6c64 2d72 6f77 5f63 6f6c  ow.field-row_col
+0000e6c0: 735f 7873 202e 6669 656c 642d 736d 5f6d  s_xs .field-sm_m
+0000e6d0: 7320 6c61 6265 6c2c 2e64 6a61 6e67 6f63  s label,.djangoc
+0000e6e0: 6d73 2d66 726f 6e74 656e 642d 726f 7720  ms-frontend-row 
+0000e6f0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000e700: 726f 775f 636f 6c73 5f78 7320 2e66 6965  row_cols_xs .fie
+0000e710: 6c64 2d78 6c5f 6d65 206c 6162 656c 2c2e  ld-xl_me label,.
+0000e720: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000e730: 6e64 2d72 6f77 202e 666f 726d 2d72 6f77  nd-row .form-row
+0000e740: 2e66 6965 6c64 2d72 6f77 5f63 6f6c 735f  .field-row_cols_
+0000e750: 7873 202e 6669 656c 642d 786c 5f6d 7320  xs .field-xl_ms 
+0000e760: 6c61 6265 6c2c 2e64 6a61 6e67 6f63 6d73  label,.djangocms
+0000e770: 2d66 726f 6e74 656e 642d 726f 7720 2e66  -frontend-row .f
+0000e780: 6f72 6d2d 726f 772e 6669 656c 642d 726f  orm-row.field-ro
+0000e790: 775f 636f 6c73 5f78 7320 2e66 6965 6c64  w_cols_xs .field
+0000e7a0: 2d78 735f 6d65 206c 6162 656c 2c2e 646a  -xs_me label,.dj
+0000e7b0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000e7c0: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
+0000e7d0: 6965 6c64 2d72 6f77 5f63 6f6c 735f 7873  ield-row_cols_xs
+0000e7e0: 202e 6669 656c 642d 7873 5f6d 7320 6c61   .field-xs_ms la
+0000e7f0: 6265 6c2c 2e64 6a61 6e67 6f63 6d73 2d66  bel,.djangocms-f
+0000e800: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
+0000e810: 6d2d 726f 772e 6669 656c 642d 726f 775f  m-row.field-row_
+0000e820: 636f 6c73 5f78 7320 2e66 6965 6c64 2d78  cols_xs .field-x
+0000e830: 786c 5f6d 6520 6c61 6265 6c2c 2e64 6a61  xl_me label,.dja
+0000e840: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000e850: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
+0000e860: 656c 642d 726f 775f 636f 6c73 5f78 7320  eld-row_cols_xs 
+0000e870: 2e66 6965 6c64 2d78 786c 5f6d 7320 6c61  .field-xxl_ms la
+0000e880: 6265 6c7b 696e 7365 742d 696e 6c69 6e65  bel{inset-inline
+0000e890: 2d73 7461 7274 3a33 3070 783b 696e 7365  -start:30px;inse
+0000e8a0: 742d 626c 6f63 6b2d 7374 6172 743a 3134  t-block-start:14
+0000e8b0: 7078 7d2e 646a 616e 676f 636d 732d 6672  px}.djangocms-fr
+0000e8c0: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+0000e8d0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000e8e0: 5f63 6f6c 202e 6669 656c 642d 6c67 5f6d  _col .field-lg_m
+0000e8f0: 6520 696e 7075 742c 2e64 6a61 6e67 6f63  e input,.djangoc
+0000e900: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000e910: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000e920: 6c64 2d78 735f 636f 6c20 2e66 6965 6c64  ld-xs_col .field
+0000e930: 2d6c 675f 6d73 2069 6e70 7574 2c2e 646a  -lg_ms input,.dj
+0000e940: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000e950: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000e960: 772e 6669 656c 642d 7873 5f63 6f6c 202e  w.field-xs_col .
+0000e970: 6669 656c 642d 6d64 5f6d 6520 696e 7075  field-md_me inpu
+0000e980: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
+0000e990: 6e74 656e 642d 636f 6c75 6d6e 202e 666f  ntend-column .fo
+0000e9a0: 726d 2d72 6f77 2e66 6965 6c64 2d78 735f  rm-row.field-xs_
+0000e9b0: 636f 6c20 2e66 6965 6c64 2d6d 645f 6d73  col .field-md_ms
+0000e9c0: 2069 6e70 7574 2c2e 646a 616e 676f 636d   input,.djangocm
+0000e9d0: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
+0000e9e0: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
+0000e9f0: 642d 7873 5f63 6f6c 202e 6669 656c 642d  d-xs_col .field-
+0000ea00: 736d 5f6d 6520 696e 7075 742c 2e64 6a61  sm_me input,.dja
+0000ea10: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000ea20: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000ea30: 2e66 6965 6c64 2d78 735f 636f 6c20 2e66  .field-xs_col .f
+0000ea40: 6965 6c64 2d73 6d5f 6d73 2069 6e70 7574  ield-sm_ms input
+0000ea50: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000ea60: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000ea70: 6d2d 726f 772e 6669 656c 642d 7873 5f63  m-row.field-xs_c
+0000ea80: 6f6c 202e 6669 656c 642d 786c 5f6d 6520  ol .field-xl_me 
+0000ea90: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
+0000eaa0: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000eab0: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000eac0: 2d78 735f 636f 6c20 2e66 6965 6c64 2d78  -xs_col .field-x
+0000ead0: 6c5f 6d73 2069 6e70 7574 2c2e 646a 616e  l_ms input,.djan
+0000eae0: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
+0000eaf0: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
+0000eb00: 6669 656c 642d 7873 5f63 6f6c 202e 6669  field-xs_col .fi
+0000eb10: 656c 642d 7873 5f6d 6520 696e 7075 742c  eld-xs_me input,
+0000eb20: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000eb30: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000eb40: 2d72 6f77 2e66 6965 6c64 2d78 735f 636f  -row.field-xs_co
+0000eb50: 6c20 2e66 6965 6c64 2d78 735f 6d73 2069  l .field-xs_ms i
+0000eb60: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
+0000eb70: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000eb80: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000eb90: 7873 5f63 6f6c 202e 6669 656c 642d 7878  xs_col .field-xx
+0000eba0: 6c5f 6d65 2069 6e70 7574 2c2e 646a 616e  l_me input,.djan
+0000ebb0: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
+0000ebc0: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
+0000ebd0: 6669 656c 642d 7873 5f63 6f6c 202e 6669  field-xs_col .fi
+0000ebe0: 656c 642d 7878 6c5f 6d73 2069 6e70 7574  eld-xxl_ms input
+0000ebf0: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000ec00: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000ec10: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
+0000ec20: 6520 2e66 6965 6c64 2d6c 675f 6d65 2069  e .field-lg_me i
+0000ec30: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
+0000ec40: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000ec50: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000ec60: 7873 5f6d 6520 2e66 6965 6c64 2d6c 675f  xs_me .field-lg_
+0000ec70: 6d73 2069 6e70 7574 2c2e 646a 616e 676f  ms input,.django
+0000ec80: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000ec90: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000eca0: 656c 642d 7873 5f6d 6520 2e66 6965 6c64  eld-xs_me .field
+0000ecb0: 2d6d 645f 6d65 2069 6e70 7574 2c2e 646a  -md_me input,.dj
+0000ecc0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000ecd0: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000ece0: 772e 6669 656c 642d 7873 5f6d 6520 2e66  w.field-xs_me .f
+0000ecf0: 6965 6c64 2d6d 645f 6d73 2069 6e70 7574  ield-md_ms input
+0000ed00: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000ed10: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000ed20: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
+0000ed30: 6520 2e66 6965 6c64 2d73 6d5f 6d65 2069  e .field-sm_me i
+0000ed40: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
+0000ed50: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000ed60: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000ed70: 7873 5f6d 6520 2e66 6965 6c64 2d73 6d5f  xs_me .field-sm_
+0000ed80: 6d73 2069 6e70 7574 2c2e 646a 616e 676f  ms input,.django
+0000ed90: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000eda0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000edb0: 656c 642d 7873 5f6d 6520 2e66 6965 6c64  eld-xs_me .field
+0000edc0: 2d78 6c5f 6d65 2069 6e70 7574 2c2e 646a  -xl_me input,.dj
+0000edd0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000ede0: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000edf0: 772e 6669 656c 642d 7873 5f6d 6520 2e66  w.field-xs_me .f
+0000ee00: 6965 6c64 2d78 6c5f 6d73 2069 6e70 7574  ield-xl_ms input
+0000ee10: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000ee20: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000ee30: 6d2d 726f 772e 6669 656c 642d 7873 5f6d  m-row.field-xs_m
+0000ee40: 6520 2e66 6965 6c64 2d78 735f 6d65 2069  e .field-xs_me i
+0000ee50: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
+0000ee60: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000ee70: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000ee80: 7873 5f6d 6520 2e66 6965 6c64 2d78 735f  xs_me .field-xs_
+0000ee90: 6d73 2069 6e70 7574 2c2e 646a 616e 676f  ms input,.django
+0000eea0: 636d 732d 6672 6f6e 7465 6e64 2d63 6f6c  cms-frontend-col
+0000eeb0: 756d 6e20 2e66 6f72 6d2d 726f 772e 6669  umn .form-row.fi
+0000eec0: 656c 642d 7873 5f6d 6520 2e66 6965 6c64  eld-xs_me .field
+0000eed0: 2d78 786c 5f6d 6520 696e 7075 742c 2e64  -xxl_me input,.d
+0000eee0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000eef0: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000ef00: 6f77 2e66 6965 6c64 2d78 735f 6d65 202e  ow.field-xs_me .
+0000ef10: 6669 656c 642d 7878 6c5f 6d73 2069 6e70  field-xxl_ms inp
+0000ef20: 7574 2c2e 646a 616e 676f 636d 732d 6672  ut,.djangocms-fr
+0000ef30: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+0000ef40: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000ef50: 5f6d 7320 2e66 6965 6c64 2d6c 675f 6d65  _ms .field-lg_me
+0000ef60: 2069 6e70 7574 2c2e 646a 616e 676f 636d   input,.djangocm
+0000ef70: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
+0000ef80: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
+0000ef90: 642d 7873 5f6d 7320 2e66 6965 6c64 2d6c  d-xs_ms .field-l
+0000efa0: 675f 6d73 2069 6e70 7574 2c2e 646a 616e  g_ms input,.djan
+0000efb0: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
+0000efc0: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
+0000efd0: 6669 656c 642d 7873 5f6d 7320 2e66 6965  field-xs_ms .fie
+0000efe0: 6c64 2d6d 645f 6d65 2069 6e70 7574 2c2e  ld-md_me input,.
+0000eff0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000f000: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000f010: 726f 772e 6669 656c 642d 7873 5f6d 7320  row.field-xs_ms 
+0000f020: 2e66 6965 6c64 2d6d 645f 6d73 2069 6e70  .field-md_ms inp
+0000f030: 7574 2c2e 646a 616e 676f 636d 732d 6672  ut,.djangocms-fr
+0000f040: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+0000f050: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000f060: 5f6d 7320 2e66 6965 6c64 2d73 6d5f 6d65  _ms .field-sm_me
+0000f070: 2069 6e70 7574 2c2e 646a 616e 676f 636d   input,.djangocm
+0000f080: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
+0000f090: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
+0000f0a0: 642d 7873 5f6d 7320 2e66 6965 6c64 2d73  d-xs_ms .field-s
+0000f0b0: 6d5f 6d73 2069 6e70 7574 2c2e 646a 616e  m_ms input,.djan
+0000f0c0: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
+0000f0d0: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
+0000f0e0: 6669 656c 642d 7873 5f6d 7320 2e66 6965  field-xs_ms .fie
+0000f0f0: 6c64 2d78 6c5f 6d65 2069 6e70 7574 2c2e  ld-xl_me input,.
+0000f100: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000f110: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000f120: 726f 772e 6669 656c 642d 7873 5f6d 7320  row.field-xs_ms 
+0000f130: 2e66 6965 6c64 2d78 6c5f 6d73 2069 6e70  .field-xl_ms inp
+0000f140: 7574 2c2e 646a 616e 676f 636d 732d 6672  ut,.djangocms-fr
+0000f150: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+0000f160: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000f170: 5f6d 7320 2e66 6965 6c64 2d78 735f 6d65  _ms .field-xs_me
+0000f180: 2069 6e70 7574 2c2e 646a 616e 676f 636d   input,.djangocm
+0000f190: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
+0000f1a0: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
+0000f1b0: 642d 7873 5f6d 7320 2e66 6965 6c64 2d78  d-xs_ms .field-x
+0000f1c0: 735f 6d73 2069 6e70 7574 2c2e 646a 616e  s_ms input,.djan
+0000f1d0: 676f 636d 732d 6672 6f6e 7465 6e64 2d63  gocms-frontend-c
+0000f1e0: 6f6c 756d 6e20 2e66 6f72 6d2d 726f 772e  olumn .form-row.
+0000f1f0: 6669 656c 642d 7873 5f6d 7320 2e66 6965  field-xs_ms .fie
+0000f200: 6c64 2d78 786c 5f6d 6520 696e 7075 742c  ld-xxl_me input,
+0000f210: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000f220: 656e 642d 636f 6c75 6d6e 202e 666f 726d  end-column .form
+0000f230: 2d72 6f77 2e66 6965 6c64 2d78 735f 6d73  -row.field-xs_ms
+0000f240: 202e 6669 656c 642d 7878 6c5f 6d73 2069   .field-xxl_ms i
+0000f250: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
+0000f260: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000f270: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000f280: 7873 5f6f 6666 7365 7420 2e66 6965 6c64  xs_offset .field
+0000f290: 2d6c 675f 6d65 2069 6e70 7574 2c2e 646a  -lg_me input,.dj
+0000f2a0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000f2b0: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000f2c0: 772e 6669 656c 642d 7873 5f6f 6666 7365  w.field-xs_offse
+0000f2d0: 7420 2e66 6965 6c64 2d6c 675f 6d73 2069  t .field-lg_ms i
+0000f2e0: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
+0000f2f0: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000f300: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000f310: 7873 5f6f 6666 7365 7420 2e66 6965 6c64  xs_offset .field
+0000f320: 2d6d 645f 6d65 2069 6e70 7574 2c2e 646a  -md_me input,.dj
+0000f330: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000f340: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000f350: 772e 6669 656c 642d 7873 5f6f 6666 7365  w.field-xs_offse
+0000f360: 7420 2e66 6965 6c64 2d6d 645f 6d73 2069  t .field-md_ms i
+0000f370: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
+0000f380: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000f390: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000f3a0: 7873 5f6f 6666 7365 7420 2e66 6965 6c64  xs_offset .field
+0000f3b0: 2d73 6d5f 6d65 2069 6e70 7574 2c2e 646a  -sm_me input,.dj
+0000f3c0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000f3d0: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000f3e0: 772e 6669 656c 642d 7873 5f6f 6666 7365  w.field-xs_offse
+0000f3f0: 7420 2e66 6965 6c64 2d73 6d5f 6d73 2069  t .field-sm_ms i
+0000f400: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
+0000f410: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000f420: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000f430: 7873 5f6f 6666 7365 7420 2e66 6965 6c64  xs_offset .field
+0000f440: 2d78 6c5f 6d65 2069 6e70 7574 2c2e 646a  -xl_me input,.dj
+0000f450: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000f460: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000f470: 772e 6669 656c 642d 7873 5f6f 6666 7365  w.field-xs_offse
+0000f480: 7420 2e66 6965 6c64 2d78 6c5f 6d73 2069  t .field-xl_ms i
+0000f490: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
+0000f4a0: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000f4b0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000f4c0: 7873 5f6f 6666 7365 7420 2e66 6965 6c64  xs_offset .field
+0000f4d0: 2d78 735f 6d65 2069 6e70 7574 2c2e 646a  -xs_me input,.dj
+0000f4e0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000f4f0: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000f500: 772e 6669 656c 642d 7873 5f6f 6666 7365  w.field-xs_offse
+0000f510: 7420 2e66 6965 6c64 2d78 735f 6d73 2069  t .field-xs_ms i
+0000f520: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
+0000f530: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000f540: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000f550: 7873 5f6f 6666 7365 7420 2e66 6965 6c64  xs_offset .field
+0000f560: 2d78 786c 5f6d 6520 696e 7075 742c 2e64  -xxl_me input,.d
+0000f570: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000f580: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000f590: 6f77 2e66 6965 6c64 2d78 735f 6f66 6673  ow.field-xs_offs
+0000f5a0: 6574 202e 6669 656c 642d 7878 6c5f 6d73  et .field-xxl_ms
+0000f5b0: 2069 6e70 7574 2c2e 646a 616e 676f 636d   input,.djangocm
+0000f5c0: 732d 6672 6f6e 7465 6e64 2d63 6f6c 756d  s-frontend-colum
+0000f5d0: 6e20 2e66 6f72 6d2d 726f 772e 6669 656c  n .form-row.fiel
+0000f5e0: 642d 7873 5f6f 7264 6572 202e 6669 656c  d-xs_order .fiel
+0000f5f0: 642d 6c67 5f6d 6520 696e 7075 742c 2e64  d-lg_me input,.d
+0000f600: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000f610: 642d 636f 6c75 6d6e 202e 666f 726d 2d72  d-column .form-r
+0000f620: 6f77 2e66 6965 6c64 2d78 735f 6f72 6465  ow.field-xs_orde
+0000f630: 7220 2e66 6965 6c64 2d6c 675f 6d73 2069  r .field-lg_ms i
+0000f640: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
+0000f650: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000f660: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000f670: 7873 5f6f 7264 6572 202e 6669 656c 642d  xs_order .field-
+0000f680: 6d64 5f6d 6520 696e 7075 742c 2e64 6a61  md_me input,.dja
+0000f690: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000f6a0: 636f 6c75 6d6e 202e 666f 726d 2d72 6f77  column .form-row
+0000f6b0: 2e66 6965 6c64 2d78 735f 6f72 6465 7220  .field-xs_order 
+0000f6c0: 2e66 6965 6c64 2d6d 645f 6d73 2069 6e70  .field-md_ms inp
+0000f6d0: 7574 2c2e 646a 616e 676f 636d 732d 6672  ut,.djangocms-fr
+0000f6e0: 6f6e 7465 6e64 2d63 6f6c 756d 6e20 2e66  ontend-column .f
+0000f6f0: 6f72 6d2d 726f 772e 6669 656c 642d 7873  orm-row.field-xs
+0000f700: 5f6f 7264 6572 202e 6669 656c 642d 736d  _order .field-sm
+0000f710: 5f6d 6520 696e 7075 742c 2e64 6a61 6e67  _me input,.djang
+0000f720: 6f63 6d73 2d66 726f 6e74 656e 642d 636f  ocms-frontend-co
+0000f730: 6c75 6d6e 202e 666f 726d 2d72 6f77 2e66  lumn .form-row.f
+0000f740: 6965 6c64 2d78 735f 6f72 6465 7220 2e66  ield-xs_order .f
+0000f750: 6965 6c64 2d73 6d5f 6d73 2069 6e70 7574  ield-sm_ms input
+0000f760: 2c2e 646a 616e 676f 636d 732d 6672 6f6e  ,.djangocms-fron
+0000f770: 7465 6e64 2d63 6f6c 756d 6e20 2e66 6f72  tend-column .for
+0000f780: 6d2d 726f 772e 6669 656c 642d 7873 5f6f  m-row.field-xs_o
+0000f790: 7264 6572 202e 6669 656c 642d 786c 5f6d  rder .field-xl_m
+0000f7a0: 6520 696e 7075 742c 2e64 6a61 6e67 6f63  e input,.djangoc
+0000f7b0: 6d73 2d66 726f 6e74 656e 642d 636f 6c75  ms-frontend-colu
+0000f7c0: 6d6e 202e 666f 726d 2d72 6f77 2e66 6965  mn .form-row.fie
+0000f7d0: 6c64 2d78 735f 6f72 6465 7220 2e66 6965  ld-xs_order .fie
+0000f7e0: 6c64 2d78 6c5f 6d73 2069 6e70 7574 2c2e  ld-xl_ms input,.
+0000f7f0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+0000f800: 6e64 2d63 6f6c 756d 6e20 2e66 6f72 6d2d  nd-column .form-
+0000f810: 726f 772e 6669 656c 642d 7873 5f6f 7264  row.field-xs_ord
+0000f820: 6572 202e 6669 656c 642d 7873 5f6d 6520  er .field-xs_me 
+0000f830: 696e 7075 742c 2e64 6a61 6e67 6f63 6d73  input,.djangocms
+0000f840: 2d66 726f 6e74 656e 642d 636f 6c75 6d6e  -frontend-column
+0000f850: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000f860: 2d78 735f 6f72 6465 7220 2e66 6965 6c64  -xs_order .field
+0000f870: 2d78 735f 6d73 2069 6e70 7574 2c2e 646a  -xs_ms input,.dj
+0000f880: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000f890: 2d63 6f6c 756d 6e20 2e66 6f72 6d2d 726f  -column .form-ro
+0000f8a0: 772e 6669 656c 642d 7873 5f6f 7264 6572  w.field-xs_order
+0000f8b0: 202e 6669 656c 642d 7878 6c5f 6d65 2069   .field-xxl_me i
+0000f8c0: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
+0000f8d0: 6672 6f6e 7465 6e64 2d63 6f6c 756d 6e20  frontend-column 
+0000f8e0: 2e66 6f72 6d2d 726f 772e 6669 656c 642d  .form-row.field-
+0000f8f0: 7873 5f6f 7264 6572 202e 6669 656c 642d  xs_order .field-
+0000f900: 7878 6c5f 6d73 2069 6e70 7574 2c2e 646a  xxl_ms input,.dj
+0000f910: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+0000f920: 2d72 6f77 202e 666f 726d 2d72 6f77 2e66  -row .form-row.f
+0000f930: 6965 6c64 2d72 6f77 5f63 6f6c 735f 7873  ield-row_cols_xs
+0000f940: 202e 6669 656c 642d 6c67 5f6d 6520 696e   .field-lg_me in
+0000f950: 7075 742c 2e64 6a61 6e67 6f63 6d73 2d66  put,.djangocms-f
+0000f960: 726f 6e74 656e 642d 726f 7720 2e66 6f72  rontend-row .for
+0000f970: 6d2d 726f 772e 6669 656c 642d 726f 775f  m-row.field-row_
+0000f980: 636f 6c73 5f78 7320 2e66 6965 6c64 2d6c  cols_xs .field-l
+0000f990: 675f 6d73 2069 6e70 7574 2c2e 646a 616e  g_ms input,.djan
+0000f9a0: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
+0000f9b0: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
+0000f9c0: 6c64 2d72 6f77 5f63 6f6c 735f 7873 202e  ld-row_cols_xs .
+0000f9d0: 6669 656c 642d 6d64 5f6d 6520 696e 7075  field-md_me inpu
+0000f9e0: 742c 2e64 6a61 6e67 6f63 6d73 2d66 726f  t,.djangocms-fro
+0000f9f0: 6e74 656e 642d 726f 7720 2e66 6f72 6d2d  ntend-row .form-
+0000fa00: 726f 772e 6669 656c 642d 726f 775f 636f  row.field-row_co
+0000fa10: 6c73 5f78 7320 2e66 6965 6c64 2d6d 645f  ls_xs .field-md_
+0000fa20: 6d73 2069 6e70 7574 2c2e 646a 616e 676f  ms input,.django
+0000fa30: 636d 732d 6672 6f6e 7465 6e64 2d72 6f77  cms-frontend-row
+0000fa40: 202e 666f 726d 2d72 6f77 2e66 6965 6c64   .form-row.field
+0000fa50: 2d72 6f77 5f63 6f6c 735f 7873 202e 6669  -row_cols_xs .fi
+0000fa60: 656c 642d 736d 5f6d 6520 696e 7075 742c  eld-sm_me input,
+0000fa70: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+0000fa80: 656e 642d 726f 7720 2e66 6f72 6d2d 726f  end-row .form-ro
+0000fa90: 772e 6669 656c 642d 726f 775f 636f 6c73  w.field-row_cols
+0000faa0: 5f78 7320 2e66 6965 6c64 2d73 6d5f 6d73  _xs .field-sm_ms
+0000fab0: 2069 6e70 7574 2c2e 646a 616e 676f 636d   input,.djangocm
+0000fac0: 732d 6672 6f6e 7465 6e64 2d72 6f77 202e  s-frontend-row .
+0000fad0: 666f 726d 2d72 6f77 2e66 6965 6c64 2d72  form-row.field-r
+0000fae0: 6f77 5f63 6f6c 735f 7873 202e 6669 656c  ow_cols_xs .fiel
+0000faf0: 642d 786c 5f6d 6520 696e 7075 742c 2e64  d-xl_me input,.d
+0000fb00: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000fb10: 642d 726f 7720 2e66 6f72 6d2d 726f 772e  d-row .form-row.
+0000fb20: 6669 656c 642d 726f 775f 636f 6c73 5f78  field-row_cols_x
+0000fb30: 7320 2e66 6965 6c64 2d78 6c5f 6d73 2069  s .field-xl_ms i
+0000fb40: 6e70 7574 2c2e 646a 616e 676f 636d 732d  nput,.djangocms-
+0000fb50: 6672 6f6e 7465 6e64 2d72 6f77 202e 666f  frontend-row .fo
+0000fb60: 726d 2d72 6f77 2e66 6965 6c64 2d72 6f77  rm-row.field-row
+0000fb70: 5f63 6f6c 735f 7873 202e 6669 656c 642d  _cols_xs .field-
+0000fb80: 7873 5f6d 6520 696e 7075 742c 2e64 6a61  xs_me input,.dja
+0000fb90: 6e67 6f63 6d73 2d66 726f 6e74 656e 642d  ngocms-frontend-
+0000fba0: 726f 7720 2e66 6f72 6d2d 726f 772e 6669  row .form-row.fi
+0000fbb0: 656c 642d 726f 775f 636f 6c73 5f78 7320  eld-row_cols_xs 
+0000fbc0: 2e66 6965 6c64 2d78 735f 6d73 2069 6e70  .field-xs_ms inp
+0000fbd0: 7574 2c2e 646a 616e 676f 636d 732d 6672  ut,.djangocms-fr
+0000fbe0: 6f6e 7465 6e64 2d72 6f77 202e 666f 726d  ontend-row .form
+0000fbf0: 2d72 6f77 2e66 6965 6c64 2d72 6f77 5f63  -row.field-row_c
+0000fc00: 6f6c 735f 7873 202e 6669 656c 642d 7878  ols_xs .field-xx
+0000fc10: 6c5f 6d65 2069 6e70 7574 2c2e 646a 616e  l_me input,.djan
+0000fc20: 676f 636d 732d 6672 6f6e 7465 6e64 2d72  gocms-frontend-r
+0000fc30: 6f77 202e 666f 726d 2d72 6f77 2e66 6965  ow .form-row.fie
+0000fc40: 6c64 2d72 6f77 5f63 6f6c 735f 7873 202e  ld-row_cols_xs .
+0000fc50: 6669 656c 642d 7878 6c5f 6d73 2069 6e70  field-xxl_ms inp
+0000fc60: 7574 7b70 6f73 6974 696f 6e3a 7265 6c61  ut{position:rela
+0000fc70: 7469 7665 3b62 6f78 2d73 697a 696e 673a  tive;box-sizing:
+0000fc80: 626f 7264 6572 2d62 6f78 3b74 6f70 3a2d  border-box;top:-
+0000fc90: 3370 787d 2e67 7269 642d 7265 7365 747b  3px}.grid-reset{
+0000fca0: 706f 7369 7469 6f6e 3a61 6273 6f6c 7574  position:absolut
+0000fcb0: 653b 696e 7365 742d 696e 6c69 6e65 2d65  e;inset-inline-e
+0000fcc0: 6e64 3a35 7078 3b69 6e73 6574 2d62 6c6f  nd:5px;inset-blo
+0000fcd0: 636b 2d73 7461 7274 3a30 7d2e 6963 6f6e  ck-start:0}.icon
+0000fce0: 2d74 6865 6164 7b74 6578 742d 616c 6967  -thead{text-alig
+0000fcf0: 6e3a 6365 6e74 6572 3b6d 6172 6769 6e2d  n:center;margin-
+0000fd00: 626f 7474 6f6d 3a31 3570 787d 2e69 636f  bottom:15px}.ico
+0000fd10: 6e2d 7468 6561 6420 2e69 636f 6e7b 666f  n-thead .icon{fo
+0000fd20: 6e74 2d73 697a 653a 3330 7078 7d2e 6963  nt-size:30px}.ic
+0000fd30: 6f6e 2d74 6865 6164 202e 6963 6f6e 2d73  on-thead .icon-s
+0000fd40: 697a 652d 736d 7b74 7261 6e73 666f 726d  ize-sm{transform
+0000fd50: 3a72 6f74 6174 6528 3930 6465 6729 7d2e  :rotate(90deg)}.
+0000fd60: 6963 6f6e 2d74 6974 6c65 7b64 6973 706c  icon-title{displ
+0000fd70: 6179 3a62 6c6f 636b 3b66 6f6e 742d 7369  ay:block;font-si
+0000fd80: 7a65 3a31 3270 783b 636f 6c6f 723a 2339  ze:12px;color:#9
+0000fd90: 3939 3b70 6164 6469 6e67 3a35 7078 2030  99;padding:5px 0
+0000fda0: 2030 7d2e 646a 616e 676f 636d 732d 6672   0}.djangocms-fr
+0000fdb0: 6f6e 7465 6e64 2d70 7265 7669 6577 7b70  ontend-preview{p
+0000fdc0: 6f73 6974 696f 6e3a 6669 7865 643b 696e  osition:fixed;in
+0000fdd0: 7365 742d 626c 6f63 6b2d 7374 6172 743a  set-block-start:
+0000fde0: 303b 696e 7365 742d 696e 6c69 6e65 2d65  0;inset-inline-e
+0000fdf0: 6e64 3a30 3b7a 2d69 6e64 6578 3a31 303b  nd:0;z-index:10;
+0000fe00: 7465 7874 2d61 6c69 676e 3a63 656e 7465  text-align:cente
+0000fe10: 723b 626f 7264 6572 2d72 6164 6975 733a  r;border-radius:
+0000fe20: 3020 3020 3020 3370 783b 7061 6464 696e  0 0 0 3px;paddin
+0000fe30: 673a 3130 7078 2032 3070 7820 3237 7078  g:10px 20px 27px
+0000fe40: 3b62 6f72 6465 723a 3170 7820 736f 6c69  ;border:1px soli
+0000fe50: 6420 7661 7228 2d2d 6463 612d 6772 6179  d var(--dca-gray
+0000fe60: 2c76 6172 282d 2d68 6169 726c 696e 652d  ,var(--hairline-
+0000fe70: 636f 6c6f 722c 2363 6363 2929 3b62 6f72  color,#ccc));bor
+0000fe80: 6465 722d 626c 6f63 6b2d 7374 6172 743a  der-block-start:
+0000fe90: 6e6f 6e65 3b62 6f72 6465 722d 696e 6c69  none;border-inli
+0000fea0: 6e65 2d65 6e64 3a6e 6f6e 653b 6261 636b  ne-end:none;back
+0000feb0: 6772 6f75 6e64 3a76 6172 282d 2d62 6f64  ground:var(--bod
+0000fec0: 792d 6267 2c23 6666 6629 7d40 6d65 6469  y-bg,#fff)}@medi
+0000fed0: 6120 2870 7265 6665 7273 2d63 6f6c 6f72  a (prefers-color
+0000fee0: 2d73 6368 656d 653a 6461 726b 297b 2e64  -scheme:dark){.d
+0000fef0: 6a61 6e67 6f63 6d73 2d66 726f 6e74 656e  jangocms-fronten
+0000ff00: 642d 7072 6576 6965 777b 6261 636b 6772  d-preview{backgr
+0000ff10: 6f75 6e64 3a76 6172 282d 2d62 6f64 792d  ound:var(--body-
+0000ff20: 6267 2c23 3030 3029 7d7d 2e64 6a61 6e67  bg,#000)}}.djang
+0000ff30: 6f63 6d73 2d66 726f 6e74 656e 642d 7072  ocms-frontend-pr
+0000ff40: 6576 6965 7720 6832 7b66 6f6e 742d 7369  eview h2{font-si
+0000ff50: 7a65 3a31 3470 783b 6d69 6e2d 7769 6474  ze:14px;min-widt
+0000ff60: 683a 3135 3070 783b 6d61 7267 696e 3a30  h:150px;margin:0
+0000ff70: 2030 2031 3270 787d 2e64 6a61 6e67 6f63   0 12px}.djangoc
+0000ff80: 6d73 2d66 726f 6e74 656e 642d 7072 6576  ms-frontend-prev
+0000ff90: 6965 7720 2e62 342d 7072 6576 6965 777b  iew .b4-preview{
+0000ffa0: 6d61 7267 696e 3a30 2030 202d 3135 7078  margin:0 0 -15px
+0000ffb0: 7d2e 646a 616e 676f 636d 732d 6672 6f6e  }.djangocms-fron
+0000ffc0: 7465 6e64 2d70 7265 7669 6577 202e 6234  tend-preview .b4
+0000ffd0: 2d63 6c6f 7365 7b70 6f73 6974 696f 6e3a  -close{position:
+0000ffe0: 6162 736f 6c75 7465 3b69 6e73 6574 2d69  absolute;inset-i
+0000fff0: 6e6c 696e 652d 656e 643a 3130 7078 3b69  nline-end:10px;i
+00010000: 6e73 6574 2d62 6c6f 636b 2d73 7461 7274  nset-block-start
+00010010: 3a38 7078 3b7a 2d69 6e64 6578 3a31 3030  :8px;z-index:100
+00010020: 3b64 6973 706c 6179 3a62 6c6f 636b 3b63  ;display:block;c
+00010030: 6f6c 6f72 3a23 3565 3565 3565 3b66 6f6e  olor:#5e5e5e;fon
+00010040: 742d 7369 7a65 3a31 3270 783b 6c69 6e65  t-size:12px;line
+00010050: 2d68 6569 6768 743a 3230 7078 3b66 6f6e  -height:20px;fon
+00010060: 742d 7765 6967 6874 3a37 3030 3b74 6578  t-weight:700;tex
+00010070: 742d 7472 616e 7366 6f72 6d3a 7570 7065  t-transform:uppe
+00010080: 7263 6173 653b 7769 6474 683a 3230 7078  rcase;width:20px
+00010090: 3b68 6569 6768 743a 3230 7078 3b62 6f72  ;height:20px;bor
+000100a0: 6465 722d 7261 6469 7573 3a33 7078 3b62  der-radius:3px;b
+000100b0: 6163 6b67 726f 756e 643a 2364 6464 7d2e  ackground:#ddd}.
+000100c0: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
+000100d0: 6e64 2d70 7265 7669 6577 202e 6234 2d63  nd-preview .b4-c
+000100e0: 6c6f 7365 3a68 6f76 6572 7b63 6f6c 6f72  lose:hover{color
+000100f0: 3a23 6666 6621 696d 706f 7274 616e 743b  :#fff!important;
+00010100: 7465 7874 2d64 6563 6f72 6174 696f 6e3a  text-decoration:
+00010110: 6e6f 6e65 3b62 6163 6b67 726f 756e 643a  none;background:
+00010120: 2330 6266 7d2e 646a 616e 676f 636d 732d  #0bf}.djangocms-
+00010130: 6672 6f6e 7465 6e64 2d70 7265 7669 6577  frontend-preview
+00010140: 202e 6274 6e3e 7370 616e 7b76 6572 7469   .btn>span{verti
+00010150: 6361 6c2d 616c 6967 6e3a 6d69 6464 6c65  cal-align:middle
+00010160: 7d2e 646a 616e 676f 636d 732d 6672 6f6e  }.djangocms-fron
+00010170: 7465 6e64 2d70 7265 7669 6577 202e 6274  tend-preview .bt
+00010180: 6e3e 7370 616e 3e2e 6963 6f6e 7b76 6572  n>span>.icon{ver
+00010190: 7469 6361 6c2d 616c 6967 6e3a 6d69 6464  tical-align:midd
+000101a0: 6c65 7d2e 646a 616e 676f 636d 732d 6672  le}.djangocms-fr
+000101b0: 6f6e 7465 6e64 2d70 7265 7669 6577 202e  ontend-preview .
+000101c0: 6274 6e3e 7370 616e 2073 7667 2c2e 646a  btn>span svg,.dj
+000101d0: 616e 676f 636d 732d 6672 6f6e 7465 6e64  angocms-frontend
+000101e0: 2d70 7265 7669 6577 202e 6274 6e3e 7370  -preview .btn>sp
+000101f0: 616e 2075 7365 7b66 696c 6c3a 6375 7272  an use{fill:curr
+00010200: 656e 7443 6f6c 6f72 7d2e 646a 616e 676f  entColor}.django
+00010210: 636d 732d 6672 6f6e 7465 6e64 2d62 6c6f  cms-frontend-blo
+00010220: 636b 7175 6f74 6520 7465 7874 6172 6561  ckquote textarea
+00010230: 7b68 6569 6768 743a 3131 3070 787d 2369  {height:110px}#i
+00010240: 645f 6c69 6e6b 5f74 7970 657b 7061 6464  d_link_type{padd
+00010250: 696e 673a 303b 6d61 7267 696e 3a30 3b62  ing:0;margin:0;b
+00010260: 6f72 6465 723a 6e6f 6e65 7d23 6964 5f6c  order:none}#id_l
+00010270: 696e 6b5f 7479 7065 206c 697b 7061 6464  ink_type li{padd
+00010280: 696e 673a 303b 6d61 7267 696e 3a30 2031  ing:0;margin:0 1
+00010290: 3570 7820 3570 7820 303b 626f 7264 6572  5px 5px 0;border
+000102a0: 3a6e 6f6e 657d 2369 645f 6c69 6e6b 5f74  :none}#id_link_t
+000102b0: 7970 6520 6c61 6265 6c20 696e 7075 747b  ype label input{
+000102c0: 706f 7369 7469 6f6e 3a72 656c 6174 6976  position:relativ
+000102d0: 653b 746f 703a 2d34 7078 7d61 5b64 6174  e;top:-4px}a[dat
+000102e0: 612d 706b 5d7b 706f 7369 7469 6f6e 3a72  a-pk]{position:r
+000102f0: 656c 6174 6976 657d 615b 6461 7461 2d70  elative}a[data-p
+00010300: 6b5d 3a61 6674 6572 7b63 6f6e 7465 6e74  k]:after{content
+00010310: 3a61 7474 7228 6461 7461 2d70 6b29 3b76  :attr(data-pk);v
+00010320: 6973 6962 696c 6974 793a 6869 6464 656e  isibility:hidden
+00010330: 3b77 6964 7468 3a61 7574 6f3b 666f 6e74  ;width:auto;font
+00010340: 2d77 6569 6768 743a 3430 303b 666f 6e74  -weight:400;font
+00010350: 2d73 697a 653a 3830 253b 6261 636b 6772  -size:80%;backgr
+00010360: 6f75 6e64 2d63 6f6c 6f72 3a76 6172 282d  ound-color:var(-
+00010370: 2d64 6361 2d77 6869 7465 2c76 6172 282d  -dca-white,var(-
+00010380: 2d62 6f64 792d 6267 2c23 6666 6629 293b  -body-bg,#fff));
+00010390: 636f 6c6f 723a 7661 7228 2d2d 6463 612d  color:var(--dca-
+000103a0: 6772 6179 2c76 6172 282d 2d62 6f64 792d  gray,var(--body-
+000103b0: 6667 2c23 3333 3329 293b 626f 7264 6572  fg,#333));border
+000103c0: 3a73 6f6c 6964 2031 7078 2076 6172 282d  :solid 1px var(-
+000103d0: 2d64 6361 2d67 7261 792c 7661 7228 2d2d  -dca-gray,var(--
+000103e0: 626f 6479 2d66 672c 2333 3333 2929 3b74  body-fg,#333));t
+000103f0: 6578 742d 616c 6967 6e3a 6365 6e74 6572  ext-align:center
+00010400: 3b70 6164 6469 6e67 3a35 7078 2031 3070  ;padding:5px 10p
+00010410: 783b 706f 7369 7469 6f6e 3a61 6273 6f6c  x;position:absol
+00010420: 7574 653b 7a2d 696e 6465 783a 313b 746f  ute;z-index:1;to
+00010430: 703a 3131 3025 3b69 6e73 6574 2d69 6e6c  p:110%;inset-inl
+00010440: 696e 652d 7374 6172 743a 3530 253b 6d61  ine-start:50%;ma
+00010450: 7267 696e 2d69 6e6c 696e 652d 7374 6172  rgin-inline-star
+00010460: 743a 2d35 3025 7d61 5b64 6174 612d 706b  t:-50%}a[data-pk
+00010470: 5d3a 686f 7665 723a 6166 7465 727b 7669  ]:hover:after{vi
+00010480: 7369 6269 6c69 7479 3a76 6973 6962 6c65  sibility:visible
+00010490: 7d2e 646a 616e 676f 636d 732d 6164 6d69  }.djangocms-admi
+000104a0: 6e2d 7374 796c 6520 2e66 6f72 6d2d 726f  n-style .form-ro
+000104b0: 772e 6669 656c 642d 706c 7567 696e 5f74  w.field-plugin_t
+000104c0: 6974 6c65 2069 6e70 7574 5b6e 616d 653d  itle input[name=
+000104d0: 706c 7567 696e 5f74 6974 6c65 5f30 5d7b  plugin_title_0]{
+000104e0: 6d61 7267 696e 2d62 6f74 746f 6d3a 2e35  margin-bottom:.5
+000104f0: 656d 2169 6d70 6f72 7461 6e74 7d2e 646a  em!important}.dj
+00010500: 616e 676f 636d 732d 6164 6d69 6e2d 7374  angocms-admin-st
+00010510: 796c 6520 2e66 6f72 6d2d 726f 772e 6669  yle .form-row.fi
+00010520: 656c 642d 706c 7567 696e 5f74 6974 6c65  eld-plugin_title
+00010530: 2069 6e70 7574 5b6e 616d 653d 706c 7567   input[name=plug
+00010540: 696e 5f74 6974 6c65 5f31 5d7b 7769 6474  in_title_1]{widt
+00010550: 683a 6361 6c63 2831 3030 2520 2d20 3265  h:calc(100% - 2e
+00010560: 6d29 2169 6d70 6f72 7461 6e74 7d62 6f64  m)!important}bod
+00010570: 793a 6e6f 7428 2e64 6a61 6e67 6f63 6d73  y:not(.djangocms
+00010580: 2d61 646d 696e 2d73 7479 6c65 2920 2e66  -admin-style) .f
+00010590: 6f72 6d2d 726f 772e 6669 656c 642d 706c  orm-row.field-pl
+000105a0: 7567 696e 5f74 6974 6c65 2069 6e70 7574  ugin_title input
+000105b0: 5b6e 616d 653d 706c 7567 696e 5f74 6974  [name=plugin_tit
+000105c0: 6c65 5f31 5d7b 7769 6474 683a 6361 6c63  le_1]{width:calc
+000105d0: 2831 3030 2520 2d20 3230 3070 7820 2d20  (100% - 200px - 
+000105e0: 3165 6d29 2169 6d70 6f72 7461 6e74 3b6d  1em)!important;m
+000105f0: 6172 6769 6e2d 696e 6c69 6e65 2d73 7461  argin-inline-sta
+00010600: 7274 3a31 656d 7d2e 6672 6f6e 7465 6e64  rt:1em}.frontend
+00010610: 2d69 636f 6e2d 7069 636b 6572 7b74 6578  -icon-picker{tex
+00010620: 742d 616c 6967 6e3a 6365 6e74 6572 3b64  t-align:center;d
+00010630: 6973 706c 6179 3a69 6e6c 696e 652d 626c  isplay:inline-bl
+00010640: 6f63 6b7d 2e66 726f 6e74 656e 642d 6963  ock}.frontend-ic
+00010650: 6f6e 2d70 6963 6b65 7220 2e69 636f 6e2d  on-picker .icon-
+00010660: 636f 6e74 6169 6e65 727b 706f 7369 7469  container{positi
+00010670: 6f6e 3a72 656c 6174 6976 653b 6d61 7267  on:relative;marg
+00010680: 696e 3a2e 3565 6d20 6175 746f 3b77 6964  in:.5em auto;wid
+00010690: 7468 3a37 656d 3b68 6569 6768 743a 3765  th:7em;height:7e
+000106a0: 6d3b 626f 7264 6572 3a31 7078 2076 6172  m;border:1px var
+000106b0: 282d 2d64 6361 2d67 7261 792d 6c69 6768  (--dca-gray-ligh
+000106c0: 742c 7661 7228 2d2d 626f 7264 6572 2d63  t,var(--border-c
+000106d0: 6f6c 6f72 2c23 6433 6433 6433 2929 2073  olor,#d3d3d3)) s
+000106e0: 6f6c 6964 3b74 7261 6e73 6974 696f 6e3a  olid;transition:
+000106f0: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
+00010700: 202e 3135 732c 636f 6c6f 7220 2e31 3573   .15s,color .15s
+00010710: 7d2e 6672 6f6e 7465 6e64 2d69 636f 6e2d  }.frontend-icon-
+00010720: 7069 636b 6572 202e 6963 6f6e 2d63 6f6e  picker .icon-con
+00010730: 7461 696e 6572 202e 6963 6f6e 2d70 7265  tainer .icon-pre
+00010740: 7669 6577 7b77 6964 7468 3a37 656d 3b68  view{width:7em;h
+00010750: 6569 6768 743a 3765 6d3b 6469 7370 6c61  eight:7em;displa
+00010760: 793a 2d6d 732d 666c 6578 626f 783b 6469  y:-ms-flexbox;di
+00010770: 7370 6c61 793a 666c 6578 3b2d 6d73 2d66  splay:flex;-ms-f
+00010780: 6c65 782d 6469 7265 6374 696f 6e3a 636f  lex-direction:co
+00010790: 6c75 6d6e 3b66 6c65 782d 6469 7265 6374  lumn;flex-direct
+000107a0: 696f 6e3a 636f 6c75 6d6e 3b2d 6d73 2d66  ion:column;-ms-f
+000107b0: 6c65 782d 7061 636b 3a63 656e 7465 723b  lex-pack:center;
+000107c0: 6a75 7374 6966 792d 636f 6e74 656e 743a  justify-content:
+000107d0: 6365 6e74 6572 7d2e 6672 6f6e 7465 6e64  center}.frontend
+000107e0: 2d69 636f 6e2d 7069 636b 6572 202e 6963  -icon-picker .ic
+000107f0: 6f6e 2d63 6f6e 7461 696e 6572 202e 6963  on-container .ic
+00010800: 6f6e 2d70 7265 7669 6577 202e 6963 6f6e  on-preview .icon
+00010810: 2d62 6f78 7b66 6f6e 742d 7369 7a65 3a35  -box{font-size:5
+00010820: 3030 253b 6c69 6e65 2d68 6569 6768 743a  00%;line-height:
+00010830: 312e 333b 6d61 7267 696e 3a30 3b74 6578  1.3;margin:0;tex
+00010840: 742d 616c 6967 6e3a 6365 6e74 6572 7d2e  t-align:center}.
+00010850: 6672 6f6e 7465 6e64 2d69 636f 6e2d 7069  frontend-icon-pi
+00010860: 636b 6572 202e 6963 6f6e 2d63 6f6e 7461  cker .icon-conta
+00010870: 696e 6572 202e 6963 6f6e 2d70 7265 7669  iner .icon-previ
+00010880: 6577 202e 6963 6f6e 2d62 6f78 2069 2c2e  ew .icon-box i,.
+00010890: 6672 6f6e 7465 6e64 2d69 636f 6e2d 7069  frontend-icon-pi
+000108a0: 636b 6572 202e 6963 6f6e 2d63 6f6e 7461  cker .icon-conta
+000108b0: 696e 6572 202e 6963 6f6e 2d70 7265 7669  iner .icon-previ
+000108c0: 6577 202e 6963 6f6e 2d62 6f78 2073 7061  ew .icon-box spa
+000108d0: 6e7b 666f 6e74 2d73 697a 653a 756e 7365  n{font-size:unse
+000108e0: 747d 2e66 726f 6e74 656e 642d 6963 6f6e  t}.frontend-icon
+000108f0: 2d70 6963 6b65 7220 2e69 636f 6e2d 636f  -picker .icon-co
+00010900: 6e74 6169 6e65 7220 2e69 636f 6e2d 7072  ntainer .icon-pr
+00010910: 6576 6965 7720 2e65 6d70 7479 2d62 6f78  eview .empty-box
+00010920: 7b74 6578 742d 616c 6967 6e3a 6365 6e74  {text-align:cent
+00010930: 6572 3b6f 7665 7266 6c6f 773a 6869 6464  er;overflow:hidd
+00010940: 656e 3b74 6578 742d 6f76 6572 666c 6f77  en;text-overflow
+00010950: 3a65 6c6c 6970 7369 733b 6c69 6e65 2d68  :ellipsis;line-h
+00010960: 6569 6768 743a 313b 666f 6e74 2d73 697a  eight:1;font-siz
+00010970: 653a 3130 3025 7d2e 6672 6f6e 7465 6e64  e:100%}.frontend
+00010980: 2d69 636f 6e2d 7069 636b 6572 202e 6963  -icon-picker .ic
+00010990: 6f6e 2d63 6f6e 7461 696e 6572 202e 6963  on-container .ic
+000109a0: 6f6e 2d70 7265 7669 6577 202e 656d 7074  on-preview .empt
+000109b0: 792d 626f 782e 6869 6464 656e 7b64 6973  y-box.hidden{dis
+000109c0: 706c 6179 3a6e 6f6e 657d 2e66 726f 6e74  play:none}.front
+000109d0: 656e 642d 6963 6f6e 2d70 6963 6b65 7220  end-icon-picker 
+000109e0: 2e69 636f 6e2d 636f 6e74 6169 6e65 7220  .icon-container 
+000109f0: 2e69 636f 6e2d 7072 6576 6965 773a 686f  .icon-preview:ho
+00010a00: 7665 727b 6261 636b 6772 6f75 6e64 3a76  ver{background:v
+00010a10: 6172 282d 2d64 6361 2d67 7261 792d 6c69  ar(--dca-gray-li
+00010a20: 6768 742c 7661 7228 2d2d 626f 7264 6572  ght,var(--border
+00010a30: 2d63 6f6c 6f72 2c23 6433 6433 6433 2929  -color,#d3d3d3))
+00010a40: 3b63 7572 736f 723a 706f 696e 7465 727d  ;cursor:pointer}
+00010a50: 2e66 726f 6e74 656e 642d 6963 6f6e 2d70  .frontend-icon-p
+00010a60: 6963 6b65 7220 2e69 636f 6e2d 636f 6e74  icker .icon-cont
+00010a70: 6169 6e65 7220 2e69 636f 6e2d 636c 6f73  ainer .icon-clos
+00010a80: 652d 696e 6469 6361 746f 727b 6469 7370  e-indicator{disp
+00010a90: 6c61 793a 626c 6f63 6b3b 626f 7264 6572  lay:block;border
+00010aa0: 2d72 6164 6975 733a 3530 253b 636f 6c6f  -radius:50%;colo
+00010ab0: 723a 7661 7228 2d2d 6463 612d 626c 6163  r:var(--dca-blac
+00010ac0: 6b2c 7661 7228 2d2d 626f 6479 2d66 672c  k,var(--body-fg,
+00010ad0: 2330 3030 2929 3b62 6163 6b67 726f 756e  #000));backgroun
+00010ae0: 642d 636f 6c6f 723a 7661 7228 2d2d 6463  d-color:var(--dc
+00010af0: 612d 7768 6974 652c 7661 7228 2d2d 626f  a-white,var(--bo
+00010b00: 6479 2d62 672c 2366 6666 2929 3b70 6164  dy-bg,#fff));pad
+00010b10: 6469 6e67 3a2e 3372 656d 3b62 6f72 6465  ding:.3rem;borde
+00010b20: 723a 3170 7820 736f 6c69 6420 7661 7228  r:1px solid var(
+00010b30: 2d2d 6463 612d 626c 6163 6b2c 7661 7228  --dca-black,var(
+00010b40: 2d2d 626f 6479 2d66 672c 2330 3030 2929  --body-fg,#000))
+00010b50: 3b74 7261 6e73 666f 726d 3a74 7261 6e73  ;transform:trans
+00010b60: 6c61 7465 282d 3530 252c 2d35 3025 293b  late(-50%,-50%);
+00010b70: 746f 703a 303b 696e 7365 742d 696e 6c69  top:0;inset-inli
+00010b80: 6e65 2d73 7461 7274 3a31 3030 253b 7769  ne-start:100%;wi
+00010b90: 6474 683a 2e36 656d 3b68 6569 6768 743a  dth:.6em;height:
+00010ba0: 2e36 656d 3b6c 696e 652d 6865 6967 6874  .6em;line-height
+00010bb0: 3a2e 3565 6d3b 706f 7369 7469 6f6e 3a61  :.5em;position:a
+00010bc0: 6273 6f6c 7574 653b 7472 616e 7369 7469  bsolute;transiti
+00010bd0: 6f6e 3a62 6163 6b67 726f 756e 642d 636f  on:background-co
+00010be0: 6c6f 7220 2e31 3573 7d2e 6672 6f6e 7465  lor .15s}.fronte
+00010bf0: 6e64 2d69 636f 6e2d 7069 636b 6572 202e  nd-icon-picker .
+00010c00: 6963 6f6e 2d63 6f6e 7461 696e 6572 202e  icon-container .
+00010c10: 6963 6f6e 2d63 6c6f 7365 2d69 6e64 6963  icon-close-indic
+00010c20: 6174 6f72 3a62 6566 6f72 657b 636f 6e74  ator:before{cont
+00010c30: 656e 743a 22c3 9722 7d2e 6672 6f6e 7465  ent:".."}.fronte
+00010c40: 6e64 2d69 636f 6e2d 7069 636b 6572 202e  nd-icon-picker .
+00010c50: 6963 6f6e 2d63 6f6e 7461 696e 6572 202e  icon-container .
+00010c60: 6963 6f6e 2d63 6c6f 7365 2d69 6e64 6963  icon-close-indic
+00010c70: 6174 6f72 3a68 6f76 6572 7b62 6163 6b67  ator:hover{backg
+00010c80: 726f 756e 643a 7661 7228 2d2d 6465 6c65  round:var(--dele
+00010c90: 7465 2d62 7574 746f 6e2d 6267 2c72 6564  te-button-bg,red
+00010ca0: 293b 636f 6c6f 723a 7661 7228 2d2d 6465  );color:var(--de
+00010cb0: 6c65 7465 2d62 7574 746f 6e2d 6667 2c23  lete-button-fg,#
+00010cc0: 6666 6629 3b63 7572 736f 723a 706f 696e  fff);cursor:poin
+00010cd0: 7465 727d 2e75 6970 2d6d 6f64 616c 7b70  ter}.uip-modal{p
+00010ce0: 6f73 6974 696f 6e3a 6669 7865 643b 6865  osition:fixed;he
+00010cf0: 6967 6874 3a31 3030 253b 7769 6474 683a  ight:100%;width:
+00010d00: 3130 3025 3b69 6e73 6574 2d62 6c6f 636b  100%;inset-block
+00010d10: 2d65 6e64 3a30 3b69 6e73 6574 2d69 6e6c  -end:0;inset-inl
+00010d20: 696e 652d 7374 6172 743a 303b 6261 636b  ine-start:0;back
+00010d30: 6772 6f75 6e64 2d63 6f6c 6f72 3a72 6762  ground-color:rgb
+00010d40: 6128 302c 302c 302c 2e38 293b 7a2d 696e  a(0,0,0,.8);z-in
+00010d50: 6465 783a 3939 3939 3b2d 7765 626b 6974  dex:9999;-webkit
+00010d60: 2d75 7365 722d 7365 6c65 6374 3a6e 6f6e  -user-select:non
+00010d70: 653b 2d6d 732d 7573 6572 2d73 656c 6563  e;-ms-user-selec
+00010d80: 743a 6e6f 6e65 3b75 7365 722d 7365 6c65  t:none;user-sele
+00010d90: 6374 3a6e 6f6e 653b 6469 7370 6c61 793a  ct:none;display:
+00010da0: 2d6d 732d 666c 6578 626f 783b 6469 7370  -ms-flexbox;disp
+00010db0: 6c61 793a 666c 6578 3b2d 6d73 2d66 6c65  lay:flex;-ms-fle
+00010dc0: 782d 616c 6967 6e3a 6365 6e74 6572 3b61  x-align:center;a
+00010dd0: 6c69 676e 2d69 7465 6d73 3a63 656e 7465  lign-items:cente
+00010de0: 727d 2e75 6970 2d6d 6f64 616c 202a 2c2e  r}.uip-modal *,.
+00010df0: 7569 702d 6d6f 6461 6c20 3a61 6674 6572  uip-modal :after
+00010e00: 2c2e 7569 702d 6d6f 6461 6c20 3a62 6566  ,.uip-modal :bef
+00010e10: 6f72 657b 626f 782d 7369 7a69 6e67 3a62  ore{box-sizing:b
+00010e20: 6f72 6465 722d 626f 787d 2e75 6970 2d6d  order-box}.uip-m
+00010e30: 6f64 616c 2e75 6970 2d63 6c6f 7365 7b6f  odal.uip-close{o
+00010e40: 7061 6369 7479 3a30 3b76 6973 6962 696c  pacity:0;visibil
+00010e50: 6974 793a 6869 6464 656e 3b74 7261 6e73  ity:hidden;trans
+00010e60: 6974 696f 6e3a 616c 6c20 2e34 7320 6561  ition:all .4s ea
+00010e70: 7365 2d69 6e2d 6f75 747d 2e75 6970 2d6d  se-in-out}.uip-m
+00010e80: 6f64 616c 2e75 6970 2d6f 7065 6e7b 6f70  odal.uip-open{op
+00010e90: 6163 6974 793a 313b 7669 7369 6269 6c69  acity:1;visibili
+00010ea0: 7479 3a76 6973 6962 6c65 3b74 7261 6e73  ty:visible;trans
+00010eb0: 6974 696f 6e3a 616c 6c20 2e34 7320 6561  ition:all .4s ea
+00010ec0: 7365 2d69 6e2d 6f75 747d 2e75 6970 2d6d  se-in-out}.uip-m
+00010ed0: 6f64 616c 202e 7569 702d 6d6f 6461 6c2d  odal .uip-modal-
+00010ee0: 2d63 6f6e 7465 6e74 7b70 6f73 6974 696f  -content{positio
+00010ef0: 6e3a 6162 736f 6c75 7465 3b62 6f72 6465  n:absolute;borde
+00010f00: 722d 7261 6469 7573 3a33 7078 3b62 6f78  r-radius:3px;box
+00010f10: 2d73 6861 646f 773a 3270 7820 3870 7820  -shadow:2px 8px 
+00010f20: 3233 7078 2033 7078 2072 6762 6128 302c  23px 3px rgba(0,
+00010f30: 302c 302c 2e32 293b 6f76 6572 666c 6f77  0,0,.2);overflow
+00010f40: 3a68 6964 6465 6e3b 666f 6e74 2d66 616d  :hidden;font-fam
+00010f50: 696c 793a 526f 626f 746f 2c41 7269 616c  ily:Roboto,Arial
+00010f60: 2c48 656c 7665 7469 6361 2c56 6572 6461  ,Helvetica,Verda
+00010f70: 6e61 2c73 616e 732d 7365 7269 663b 6261  na,sans-serif;ba
+00010f80: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a76  ckground-color:v
+00010f90: 6172 282d 2d64 6361 2d67 7261 792d 6c69  ar(--dca-gray-li
+00010fa0: 6768 7465 7374 2c76 6172 282d 2d64 6172  ghtest,var(--dar
+00010fb0: 6b65 6e65 642d 6267 2c23 6638 6638 6638  kened-bg,#f8f8f8
+00010fc0: 2929 3b77 6964 7468 3a31 3030 253b 6d61  ));width:100%;ma
+00010fd0: 7267 696e 3a61 7574 6f3b 6c65 6674 3a30  rgin:auto;left:0
+00010fe0: 3b72 6967 6874 3a30 3b6d 6172 6769 6e2d  ;right:0;margin-
+00010ff0: 626f 7474 6f6d 3a32 656d 7d2e 7569 702d  bottom:2em}.uip-
+00011000: 6d6f 6461 6c20 2e75 6970 2d6d 6f64 616c  modal .uip-modal
+00011010: 2d2d 636f 6e74 656e 7420 2e75 6970 2d6d  --content .uip-m
+00011020: 6f64 616c 2d2d 6865 6164 6572 7b70 6164  odal--header{pad
+00011030: 6469 6e67 3a31 3570 7820 3135 7078 3b62  ding:15px 15px;b
+00011040: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
+00011050: 7661 7228 2d2d 6463 612d 7768 6974 652c  var(--dca-white,
+00011060: 7661 7228 2d2d 6267 2d63 6f6c 6f72 2c23  var(--bg-color,#
+00011070: 6666 6629 293b 626f 782d 7368 6164 6f77  fff));box-shadow
+00011080: 3a30 2030 2038 7078 2072 6762 6128 302c  :0 0 8px rgba(0,
+00011090: 302c 302c 2e31 293b 706f 7369 7469 6f6e  0,0,.1);position
+000110a0: 3a72 656c 6174 6976 653b 7a2d 696e 6465  :relative;z-inde
+000110b0: 783a 313b 666f 6e74 2d73 697a 653a 3135  x:1;font-size:15
+000110c0: 7078 3b63 6f6c 6f72 3a76 6172 282d 2d64  px;color:var(--d
+000110d0: 6361 2d67 7261 792c 7661 7228 2d2d 626f  ca-gray,var(--bo
+000110e0: 6479 2d71 7569 6574 2d63 6f6c 6f72 2c23  dy-quiet-color,#
+000110f0: 3636 3629 293b 666f 6e74 2d77 6569 6768  666));font-weigh
+00011100: 743a 3530 303b 6469 7370 6c61 793a 2d6d  t:500;display:-m
+00011110: 732d 666c 6578 626f 783b 6469 7370 6c61  s-flexbox;displa
+00011120: 793a 666c 6578 3b2d 6d73 2d66 6c65 782d  y:flex;-ms-flex-
+00011130: 616c 6967 6e3a 6365 6e74 6572 3b61 6c69  align:center;ali
+00011140: 676e 2d69 7465 6d73 3a63 656e 7465 723b  gn-items:center;
+00011150: 2d6d 732d 666c 6578 2d70 6163 6b3a 6a75  -ms-flex-pack:ju
+00011160: 7374 6966 793b 6a75 7374 6966 792d 636f  stify;justify-co
+00011170: 6e74 656e 743a 7370 6163 652d 6265 7477  ntent:space-betw
+00011180: 6565 6e7d 2e75 6970 2d6d 6f64 616c 202e  een}.uip-modal .
+00011190: 7569 702d 6d6f 6461 6c2d 2d63 6f6e 7465  uip-modal--conte
+000111a0: 6e74 202e 7569 702d 6d6f 6461 6c2d 2d68  nt .uip-modal--h
+000111b0: 6561 6465 7220 2e75 6970 2d6d 6f64 616c  eader .uip-modal
+000111c0: 2d2d 6865 6164 6572 2d6c 6f67 6f2d 7469  --header-logo-ti
+000111d0: 746c 657b 7061 6464 696e 672d 746f 703a  tle{padding-top:
+000111e0: 3270 783b 6c69 6e65 2d68 6569 6768 743a  2px;line-height:
+000111f0: 313b 7465 7874 2d74 7261 6e73 666f 726d  1;text-transform
+00011200: 3a75 7070 6572 6361 7365 3b66 6f6e 742d  :uppercase;font-
+00011210: 7765 6967 6874 3a37 3030 3b63 7572 736f  weight:700;curso
+00011220: 723a 706f 696e 7465 727d 2e75 6970 2d6d  r:pointer}.uip-m
+00011230: 6f64 616c 202e 7569 702d 6d6f 6461 6c2d  odal .uip-modal-
+00011240: 2d63 6f6e 7465 6e74 202e 7569 702d 6d6f  -content .uip-mo
+00011250: 6461 6c2d 2d68 6561 6465 7220 2e75 6970  dal--header .uip
+00011260: 2d6d 6f64 616c 2d2d 6865 6164 6572 2d63  -modal--header-c
+00011270: 6c6f 7365 2d62 746e 7b63 7572 736f 723a  lose-btn{cursor:
+00011280: 706f 696e 7465 727d 2e75 6970 2d6d 6f64  pointer}.uip-mod
+00011290: 616c 202e 7569 702d 6d6f 6461 6c2d 2d63  al .uip-modal--c
+000112a0: 6f6e 7465 6e74 202e 7569 702d 6d6f 6461  ontent .uip-moda
+000112b0: 6c2d 2d62 6f64 797b 666f 6e74 2d73 697a  l--body{font-siz
+000112c0: 653a 3132 7078 3b6c 696e 652d 6865 6967  e:12px;line-heig
+000112d0: 6874 3a31 2e35 3b62 6f78 2d73 697a 696e  ht:1.5;box-sizin
+000112e0: 673a 626f 7264 6572 2d62 6f78 3b70 6164  g:border-box;pad
+000112f0: 6469 6e67 3a30 3b68 6569 6768 743a 3730  ding:0;height:70
+00011300: 7668 3b64 6973 706c 6179 3a2d 6d73 2d66  vh;display:-ms-f
+00011310: 6c65 7862 6f78 3b64 6973 706c 6179 3a66  lexbox;display:f
+00011320: 6c65 783b 6d69 6e2d 6865 6967 6874 3a35  lex;min-height:5
+00011330: 3070 783b 6d61 782d 6865 6967 6874 3a38  0px;max-height:8
+00011340: 3576 683b 6f76 6572 666c 6f77 3a61 7574  5vh;overflow:aut
+00011350: 6f7d 2e75 6970 2d6d 6f64 616c 202e 7569  o}.uip-modal .ui
+00011360: 702d 6d6f 6461 6c2d 2d63 6f6e 7465 6e74  p-modal--content
+00011370: 202e 7569 702d 6d6f 6461 6c2d 2d62 6f64   .uip-modal--bod
+00011380: 7920 2e75 6970 2d6d 6f64 616c 2d2d 7369  y .uip-modal--si
+00011390: 6465 6261 727b 2d6d 732d 666c 6578 2d6e  debar{-ms-flex-n
+000113a0: 6567 6174 6976 653a 303b 666c 6578 2d73  egative:0;flex-s
+000113b0: 6872 696e 6b3a 303b 6d61 782d 7769 6474  hrink:0;max-widt
+000113c0: 683a 3235 257d 2e75 6970 2d6d 6f64 616c  h:25%}.uip-modal
+000113d0: 202e 7569 702d 6d6f 6461 6c2d 2d63 6f6e   .uip-modal--con
+000113e0: 7465 6e74 202e 7569 702d 6d6f 6461 6c2d  tent .uip-modal-
+000113f0: 2d62 6f64 7920 2e75 6970 2d6d 6f64 616c  -body .uip-modal
+00011400: 2d2d 7369 6465 6261 7220 2e75 6970 2d6d  --sidebar .uip-m
+00011410: 6f64 616c 2d2d 7369 6465 6261 722d 7461  odal--sidebar-ta
+00011420: 6273 7b6d 6172 6769 6e2d 746f 703a 3330  bs{margin-top:30
+00011430: 7078 7d2e 7569 702d 6d6f 6461 6c20 2e75  px}.uip-modal .u
+00011440: 6970 2d6d 6f64 616c 2d2d 636f 6e74 656e  ip-modal--conten
+00011450: 7420 2e75 6970 2d6d 6f64 616c 2d2d 626f  t .uip-modal--bo
+00011460: 6479 202e 7569 702d 6d6f 6461 6c2d 2d73  dy .uip-modal--s
+00011470: 6964 6562 6172 202e 7569 702d 6d6f 6461  idebar .uip-moda
+00011480: 6c2d 2d73 6964 6562 6172 2d74 6162 7320  l--sidebar-tabs 
+00011490: 2e75 6970 2d6d 6f64 616c 2d2d 7369 6465  .uip-modal--side
+000114a0: 6261 722d 7461 622d 6974 656d 7b70 6164  bar-tab-item{pad
+000114b0: 6469 6e67 3a31 3570 783b 666f 6e74 2d73  ding:15px;font-s
+000114c0: 697a 653a 3134 7078 3b63 6f6c 6f72 3a76  ize:14px;color:v
+000114d0: 6172 282d 2d64 6361 2d67 7261 792c 7661  ar(--dca-gray,va
+000114e0: 7228 2d2d 626f 6479 2d71 7569 6574 2d63  r(--body-quiet-c
+000114f0: 6f6c 6f72 2c23 3636 3629 293b 7465 7874  olor,#666));text
+00011500: 2d61 6c69 676e 3a73 7461 7274 3b63 7572  -align:start;cur
+00011510: 736f 723a 706f 696e 7465 723b 706f 7369  sor:pointer;posi
+00011520: 7469 6f6e 3a72 656c 6174 6976 653b 6469  tion:relative;di
+00011530: 7370 6c61 793a 2d6d 732d 666c 6578 626f  splay:-ms-flexbo
+00011540: 783b 6469 7370 6c61 793a 666c 6578 3b2d  x;display:flex;-
+00011550: 6d73 2d66 6c65 782d 616c 6967 6e3a 6365  ms-flex-align:ce
+00011560: 6e74 6572 3b61 6c69 676e 2d69 7465 6d73  nter;align-items
+00011570: 3a63 656e 7465 723b 7465 7874 2d74 7261  :center;text-tra
+00011580: 6e73 666f 726d 3a63 6170 6974 616c 697a  nsform:capitaliz
+00011590: 657d 2e75 6970 2d6d 6f64 616c 202e 7569  e}.uip-modal .ui
+000115a0: 702d 6d6f 6461 6c2d 2d63 6f6e 7465 6e74  p-modal--content
+000115b0: 202e 7569 702d 6d6f 6461 6c2d 2d62 6f64   .uip-modal--bod
+000115c0: 7920 2e75 6970 2d6d 6f64 616c 2d2d 7369  y .uip-modal--si
+000115d0: 6465 6261 7220 2e75 6970 2d6d 6f64 616c  debar .uip-modal
+000115e0: 2d2d 7369 6465 6261 722d 7461 6273 202e  --sidebar-tabs .
+000115f0: 7569 702d 6d6f 6461 6c2d 2d73 6964 6562  uip-modal--sideb
+00011600: 6172 2d74 6162 2d69 7465 6d20 697b 666f  ar-tab-item i{fo
+00011610: 6e74 2d73 697a 653a 3230 7078 3b70 6164  nt-size:20px;pad
+00011620: 6469 6e67 2d69 6e6c 696e 652d 656e 643a  ding-inline-end:
+00011630: 3135 7078 3b63 6f6c 6f72 3a76 6172 282d  15px;color:var(-
+00011640: 2d64 6361 2d67 7261 792d 6c69 6768 7465  -dca-gray-lighte
+00011650: 722c 7661 7228 2d2d 626f 7264 6572 2d63  r,var(--border-c
+00011660: 6f6c 6f72 2c23 6363 6329 297d 2e75 6970  olor,#ccc))}.uip
+00011670: 2d6d 6f64 616c 202e 7569 702d 6d6f 6461  -modal .uip-moda
+00011680: 6c2d 2d63 6f6e 7465 6e74 202e 7569 702d  l--content .uip-
+00011690: 6d6f 6461 6c2d 2d62 6f64 7920 2e75 6970  modal--body .uip
+000116a0: 2d6d 6f64 616c 2d2d 7369 6465 6261 7220  -modal--sidebar 
+000116b0: 2e75 6970 2d6d 6f64 616c 2d2d 7369 6465  .uip-modal--side
+000116c0: 6261 722d 7461 6273 202e 7569 702d 6d6f  bar-tabs .uip-mo
+000116d0: 6461 6c2d 2d73 6964 6562 6172 2d74 6162  dal--sidebar-tab
+000116e0: 2d69 7465 6d20 696d 677b 7061 6464 696e  -item img{paddin
+000116f0: 672d 696e 6c69 6e65 2d65 6e64 3a31 3570  g-inline-end:15p
+00011700: 787d 2e75 6970 2d6d 6f64 616c 202e 7569  x}.uip-modal .ui
+00011710: 702d 6d6f 6461 6c2d 2d63 6f6e 7465 6e74  p-modal--content
+00011720: 202e 7569 702d 6d6f 6461 6c2d 2d62 6f64   .uip-modal--bod
+00011730: 7920 2e75 6970 2d6d 6f64 616c 2d2d 7369  y .uip-modal--si
+00011740: 6465 6261 7220 2e75 6970 2d6d 6f64 616c  debar .uip-modal
+00011750: 2d2d 7369 6465 6261 722d 7461 6273 202e  --sidebar-tabs .
+00011760: 7569 702d 6d6f 6461 6c2d 2d73 6964 6562  uip-modal--sideb
+00011770: 6172 2d74 6162 2d69 7465 6d2e 756e 6976  ar-tab-item.univ
+00011780: 6572 7361 6c2d 6163 7469 7665 7b62 6163  ersal-active{bac
+00011790: 6b67 726f 756e 642d 636f 6c6f 723a 7661  kground-color:va
+000117a0: 7228 2d2d 6463 612d 7768 6974 652c 7661  r(--dca-white,va
+000117b0: 7228 2d2d 6267 2d63 6f6c 6f72 2c23 6666  r(--bg-color,#ff
+000117c0: 6629 293b 626f 782d 7368 6164 6f77 3a30  f));box-shadow:0
+000117d0: 2036 7078 2032 3070 7820 3020 7267 6261   6px 20px 0 rgba
+000117e0: 2830 2c30 2c30 2c2e 3129 7d2e 7569 702d  (0,0,0,.1)}.uip-
+000117f0: 6d6f 6461 6c20 2e75 6970 2d6d 6f64 616c  modal .uip-modal
+00011800: 2d2d 636f 6e74 656e 7420 2e75 6970 2d6d  --content .uip-m
+00011810: 6f64 616c 2d2d 626f 6479 202e 7569 702d  odal--body .uip-
+00011820: 6d6f 6461 6c2d 2d73 6964 6562 6172 202e  modal--sidebar .
+00011830: 7569 702d 6d6f 6461 6c2d 2d73 6964 6562  uip-modal--sideb
+00011840: 6172 2d74 6162 7320 2e75 6970 2d6d 6f64  ar-tabs .uip-mod
+00011850: 616c 2d2d 7369 6465 6261 722d 7461 622d  al--sidebar-tab-
+00011860: 6974 656d 2e75 6e69 7665 7273 616c 2d61  item.universal-a
+00011870: 6374 6976 653a 6166 7465 727b 636f 6e74  ctive:after{cont
+00011880: 656e 743a 2222 3b70 6f73 6974 696f 6e3a  ent:"";position:
+00011890: 6162 736f 6c75 7465 3b68 6569 6768 743a  absolute;height:
+000118a0: 3130 3025 3b77 6964 7468 3a35 7078 3b69  100%;width:5px;i
+000118b0: 6e73 6574 2d62 6c6f 636b 2d73 7461 7274  nset-block-start
+000118c0: 3a30 3b69 6e73 6574 2d69 6e6c 696e 652d  :0;inset-inline-
+000118d0: 7374 6172 743a 303b 6261 636b 6772 6f75  start:0;backgrou
+000118e0: 6e64 2d63 6f6c 6f72 3a23 3062 667d 2e75  nd-color:#0bf}.u
+000118f0: 6970 2d6d 6f64 616c 202e 7569 702d 6d6f  ip-modal .uip-mo
+00011900: 6461 6c2d 2d63 6f6e 7465 6e74 202e 7569  dal--content .ui
+00011910: 702d 6d6f 6461 6c2d 2d62 6f64 7920 2e75  p-modal--body .u
+00011920: 6970 2d6d 6f64 616c 2d2d 7369 6465 6261  ip-modal--sideba
+00011930: 7220 2e75 6970 2d6d 6f64 616c 2d2d 7369  r .uip-modal--si
+00011940: 6465 6261 722d 7461 6273 202e 7569 702d  debar-tabs .uip-
+00011950: 6d6f 6461 6c2d 2d73 6964 6562 6172 2d74  modal--sidebar-t
+00011960: 6162 2d69 7465 6d2e 756e 6976 6572 7361  ab-item.universa
+00011970: 6c2d 6163 7469 7665 2069 7b63 6f6c 6f72  l-active i{color
+00011980: 3a23 3062 667d 2e75 6970 2d6d 6f64 616c  :#0bf}.uip-modal
+00011990: 202e 7569 702d 6d6f 6461 6c2d 2d63 6f6e   .uip-modal--con
+000119a0: 7465 6e74 202e 7569 702d 6d6f 6461 6c2d  tent .uip-modal-
+000119b0: 2d62 6f64 7920 2e75 6970 2d6d 6f64 616c  -body .uip-modal
+000119c0: 2d2d 7369 6465 6261 7220 2e75 6970 2d6d  --sidebar .uip-m
+000119d0: 6f64 616c 2d2d 7369 6465 6261 722d 7461  odal--sidebar-ta
+000119e0: 6273 202e 7569 702d 6d6f 6461 6c2d 2d73  bs .uip-modal--s
+000119f0: 6964 6562 6172 2d74 6162 2d69 7465 6d3a  idebar-tab-item:
+00011a00: 6f6e 6c79 2d63 6869 6c64 7b64 6973 706c  only-child{displ
+00011a10: 6179 3a6e 6f6e 657d 2e75 6970 2d6d 6f64  ay:none}.uip-mod
+00011a20: 616c 202e 7569 702d 6d6f 6461 6c2d 2d63  al .uip-modal--c
+00011a30: 6f6e 7465 6e74 202e 7569 702d 6d6f 6461  ontent .uip-moda
+00011a40: 6c2d 2d62 6f64 7920 2e75 6970 2d6d 6f64  l--body .uip-mod
+00011a50: 616c 2d2d 6963 6f6e 2d70 7265 7669 6577  al--icon-preview
+00011a60: 2d77 7261 707b 6469 7370 6c61 793a 2d6d  -wrap{display:-m
+00011a70: 732d 666c 6578 626f 783b 6469 7370 6c61  s-flexbox;displa
+00011a80: 793a 666c 6578 3b2d 6d73 2d66 6c65 782d  y:flex;-ms-flex-
+00011a90: 6469 7265 6374 696f 6e3a 636f 6c75 6d6e  direction:column
+00011aa0: 3b66 6c65 782d 6469 7265 6374 696f 6e3a  ;flex-direction:
+00011ab0: 636f 6c75 6d6e 3b70 6164 6469 6e67 3a33  column;padding:3
+00011ac0: 3070 7820 3830 7078 2030 3b77 6964 7468  0px 80px 0;width
+00011ad0: 3a31 3030 257d 2e75 6970 2d6d 6f64 616c  :100%}.uip-modal
+00011ae0: 202e 7569 702d 6d6f 6461 6c2d 2d63 6f6e   .uip-modal--con
+00011af0: 7465 6e74 202e 7569 702d 6d6f 6461 6c2d  tent .uip-modal-
+00011b00: 2d62 6f64 7920 2e75 6970 2d6d 6f64 616c  -body .uip-modal
+00011b10: 2d2d 6963 6f6e 2d70 7265 7669 6577 2d77  --icon-preview-w
+00011b20: 7261 7020 2e75 6970 2d6d 6f64 616c 2d2d  rap .uip-modal--
+00011b30: 6963 6f6e 2d70 7265 7669 6577 2d69 6e6e  icon-preview-inn
+00011b40: 6572 7b6f 7665 7266 6c6f 773a 6175 746f  er{overflow:auto
+00011b50: 3b6d 6172 6769 6e3a 3235 7078 202d 3135  ;margin:25px -15
+00011b60: 7078 2030 3b70 6164 6469 6e67 3a30 2031  px 0;padding:0 1
+00011b70: 3570 7820 3135 7078 7d2e 7569 702d 6d6f  5px 15px}.uip-mo
+00011b80: 6461 6c20 2e75 6970 2d6d 6f64 616c 2d2d  dal .uip-modal--
+00011b90: 636f 6e74 656e 7420 2e75 6970 2d6d 6f64  content .uip-mod
+00011ba0: 616c 2d2d 626f 6479 202e 7569 702d 6d6f  al--body .uip-mo
+00011bb0: 6461 6c2d 2d69 636f 6e2d 7072 6576 6965  dal--icon-previe
+00011bc0: 772d 7772 6170 202e 7569 702d 6d6f 6461  w-wrap .uip-moda
+00011bd0: 6c2d 2d69 636f 6e2d 7072 6576 6965 772d  l--icon-preview-
+00011be0: 696e 6e65 7220 2e75 6970 2d6d 6f64 616c  inner .uip-modal
+00011bf0: 2d2d 6963 6f6e 2d70 7265 7669 6577 7b64  --icon-preview{d
+00011c00: 6973 706c 6179 3a2d 6d73 2d67 7269 643b  isplay:-ms-grid;
+00011c10: 6469 7370 6c61 793a 6772 6964 3b67 7269  display:grid;gri
+00011c20: 642d 6761 703a 3230 7078 3b6d 6172 6769  d-gap:20px;margi
+00011c30: 6e3a 3230 7078 2030 7d2e 7569 702d 6d6f  n:20px 0}.uip-mo
+00011c40: 6461 6c20 2e75 6970 2d6d 6f64 616c 2d2d  dal .uip-modal--
+00011c50: 636f 6e74 656e 7420 2e75 6970 2d6d 6f64  content .uip-mod
+00011c60: 616c 2d2d 626f 6479 202e 7569 702d 6d6f  al--body .uip-mo
+00011c70: 6461 6c2d 2d69 636f 6e2d 7072 6576 6965  dal--icon-previe
+00011c80: 772d 7772 6170 202e 7569 702d 6d6f 6461  w-wrap .uip-moda
+00011c90: 6c2d 2d69 636f 6e2d 7072 6576 6965 772d  l--icon-preview-
+00011ca0: 696e 6e65 7220 2e75 6970 2d6d 6f64 616c  inner .uip-modal
+00011cb0: 2d2d 6963 6f6e 2d70 7265 7669 6577 202e  --icon-preview .
+00011cc0: 7569 702d 6963 6f6e 2d69 7465 6d7b 706f  uip-icon-item{po
+00011cd0: 7369 7469 6f6e 3a72 656c 6174 6976 653b  sition:relative;
+00011ce0: 7061 6464 696e 673a 3130 7078 3b62 6163  padding:10px;bac
+00011cf0: 6b67 726f 756e 642d 636f 6c6f 723a 7661  kground-color:va
+00011d00: 7228 2d2d 6463 612d 7768 6974 652c 7661  r(--dca-white,va
+00011d10: 7228 2d2d 6267 2d63 6f6c 6f72 2c23 6666  r(--bg-color,#ff
+00011d20: 6629 293b 626f 782d 7368 6164 6f77 3a30  f));box-shadow:0
+00011d30: 2031 7078 2031 3270 7820 7267 6261 2830   1px 12px rgba(0
+00011d40: 2c30 2c30 2c2e 3035 293b 626f 7264 6572  ,0,0,.05);border
+00011d50: 2d72 6164 6975 733a 3370 783b 6375 7273  -radius:3px;curs
+00011d60: 6f72 3a70 6f69 6e74 6572 3b74 7261 6e73  or:pointer;trans
+00011d70: 6974 696f 6e3a 616c 6c20 2e33 733b 6f76  ition:all .3s;ov
+00011d80: 6572 666c 6f77 3a68 6964 6465 6e7d 2e75  erflow:hidden}.u
+00011d90: 6970 2d6d 6f64 616c 202e 7569 702d 6d6f  ip-modal .uip-mo
+00011da0: 6461 6c2d 2d63 6f6e 7465 6e74 202e 7569  dal--content .ui
+00011db0: 702d 6d6f 6461 6c2d 2d62 6f64 7920 2e75  p-modal--body .u
+00011dc0: 6970 2d6d 6f64 616c 2d2d 6963 6f6e 2d70  ip-modal--icon-p
+00011dd0: 7265 7669 6577 2d77 7261 7020 2e75 6970  review-wrap .uip
+00011de0: 2d6d 6f64 616c 2d2d 6963 6f6e 2d70 7265  -modal--icon-pre
+00011df0: 7669 6577 2d69 6e6e 6572 202e 7569 702d  view-inner .uip-
+00011e00: 6d6f 6461 6c2d 2d69 636f 6e2d 7072 6576  modal--icon-prev
+00011e10: 6965 7720 2e75 6970 2d69 636f 6e2d 6974  iew .uip-icon-it
+00011e20: 656d 3a68 6f76 6572 7b62 6f78 2d73 6861  em:hover{box-sha
+00011e30: 646f 773a 3020 3170 7820 3134 7078 2072  dow:0 1px 14px r
+00011e40: 6762 6128 302c 302c 302c 2e31 3629 7d2e  gba(0,0,0,.16)}.
+00011e50: 7569 702d 6d6f 6461 6c20 2e75 6970 2d6d  uip-modal .uip-m
+00011e60: 6f64 616c 2d2d 636f 6e74 656e 7420 2e75  odal--content .u
+00011e70: 6970 2d6d 6f64 616c 2d2d 626f 6479 202e  ip-modal--body .
+00011e80: 7569 702d 6d6f 6461 6c2d 2d69 636f 6e2d  uip-modal--icon-
+00011e90: 7072 6576 6965 772d 7772 6170 202e 7569  preview-wrap .ui
+00011ea0: 702d 6d6f 6461 6c2d 2d69 636f 6e2d 7072  p-modal--icon-pr
+00011eb0: 6576 6965 772d 696e 6e65 7220 2e75 6970  eview-inner .uip
+00011ec0: 2d6d 6f64 616c 2d2d 6963 6f6e 2d70 7265  -modal--icon-pre
+00011ed0: 7669 6577 202e 7569 702d 6963 6f6e 2d69  view .uip-icon-i
+00011ee0: 7465 6d2e 756e 6976 6572 7361 6c2d 7365  tem.universal-se
+00011ef0: 6c65 6374 6564 7b62 6f78 2d73 6861 646f  lected{box-shado
+00011f00: 773a 3020 3170 7820 3132 7078 2072 6762  w:0 1px 12px rgb
+00011f10: 6128 302c 302c 302c 2e30 3529 2c30 2030  a(0,0,0,.05),0 0
+00011f20: 2030 2033 7078 2023 3062 667d 2e75 6970   0 3px #0bf}.uip
+00011f30: 2d6d 6f64 616c 202e 7569 702d 6d6f 6461  -modal .uip-moda
+00011f40: 6c2d 2d63 6f6e 7465 6e74 202e 7569 702d  l--content .uip-
+00011f50: 6d6f 6461 6c2d 2d62 6f64 7920 2e75 6970  modal--body .uip
+00011f60: 2d6d 6f64 616c 2d2d 6963 6f6e 2d70 7265  -modal--icon-pre
+00011f70: 7669 6577 2d77 7261 7020 2e75 6970 2d6d  view-wrap .uip-m
+00011f80: 6f64 616c 2d2d 6963 6f6e 2d70 7265 7669  odal--icon-previ
+00011f90: 6577 2d69 6e6e 6572 202e 7569 702d 6d6f  ew-inner .uip-mo
+00011fa0: 6461 6c2d 2d69 636f 6e2d 7072 6576 6965  dal--icon-previe
+00011fb0: 7720 2e75 6970 2d69 636f 6e2d 6974 656d  w .uip-icon-item
+00011fc0: 202e 7569 702d 6963 6f6e 2d69 7465 6d2d   .uip-icon-item-
+00011fd0: 696e 6e65 727b 6469 7370 6c61 793a 2d6d  inner{display:-m
+00011fe0: 732d 666c 6578 626f 783b 6469 7370 6c61  s-flexbox;displa
+00011ff0: 793a 666c 6578 3b2d 6d73 2d66 6c65 782d  y:flex;-ms-flex-
+00012000: 6469 7265 6374 696f 6e3a 636f 6c75 6d6e  direction:column
+00012010: 3b66 6c65 782d 6469 7265 6374 696f 6e3a  ;flex-direction:
+00012020: 636f 6c75 6d6e 3b2d 6d73 2d66 6c65 782d  column;-ms-flex-
+00012030: 616c 6967 6e3a 6365 6e74 6572 3b61 6c69  align:center;ali
+00012040: 676e 2d69 7465 6d73 3a63 656e 7465 723b  gn-items:center;
+00012050: 7061 6464 696e 673a 3170 787d 2e75 6970  padding:1px}.uip
+00012060: 2d6d 6f64 616c 202e 7569 702d 6d6f 6461  -modal .uip-moda
+00012070: 6c2d 2d63 6f6e 7465 6e74 202e 7569 702d  l--content .uip-
+00012080: 6d6f 6461 6c2d 2d62 6f64 7920 2e75 6970  modal--body .uip
+00012090: 2d6d 6f64 616c 2d2d 6963 6f6e 2d70 7265  -modal--icon-pre
+000120a0: 7669 6577 2d77 7261 7020 2e75 6970 2d6d  view-wrap .uip-m
+000120b0: 6f64 616c 2d2d 6963 6f6e 2d70 7265 7669  odal--icon-previ
+000120c0: 6577 2d69 6e6e 6572 202e 7569 702d 6d6f  ew-inner .uip-mo
+000120d0: 6461 6c2d 2d69 636f 6e2d 7072 6576 6965  dal--icon-previe
+000120e0: 7720 2e75 6970 2d69 636f 6e2d 6974 656d  w .uip-icon-item
+000120f0: 202e 7569 702d 6963 6f6e 2d69 7465 6d2d   .uip-icon-item-
+00012100: 696e 6e65 7220 2e75 6970 2d69 636f 6e2d  inner .uip-icon-
+00012110: 6974 656d 5f5f 6963 6f6e 2c2e 7569 702d  item__icon,.uip-
+00012120: 6d6f 6461 6c20 2e75 6970 2d6d 6f64 616c  modal .uip-modal
+00012130: 2d2d 636f 6e74 656e 7420 2e75 6970 2d6d  --content .uip-m
+00012140: 6f64 616c 2d2d 626f 6479 202e 7569 702d  odal--body .uip-
+00012150: 6d6f 6461 6c2d 2d69 636f 6e2d 7072 6576  modal--icon-prev
+00012160: 6965 772d 7772 6170 202e 7569 702d 6d6f  iew-wrap .uip-mo
+00012170: 6461 6c2d 2d69 636f 6e2d 7072 6576 6965  dal--icon-previe
+00012180: 772d 696e 6e65 7220 2e75 6970 2d6d 6f64  w-inner .uip-mod
+00012190: 616c 2d2d 6963 6f6e 2d70 7265 7669 6577  al--icon-preview
+000121a0: 202e 7569 702d 6963 6f6e 2d69 7465 6d20   .uip-icon-item 
+000121b0: 2e75 6970 2d69 636f 6e2d 6974 656d 2d69  .uip-icon-item-i
+000121c0: 6e6e 6572 2069 7b66 6f6e 742d 7369 7a65  nner i{font-size
+000121d0: 3a32 3570 783b 636f 6c6f 723a 7661 7228  :25px;color:var(
+000121e0: 2d2d 6463 612d 6772 6179 2d64 6172 6b65  --dca-gray-darke
+000121f0: 7374 2c76 6172 282d 2d62 6f64 792d 6667  st,var(--body-fg
+00012200: 2c23 3333 3329 297d 2e75 6970 2d6d 6f64  ,#333))}.uip-mod
+00012210: 616c 202e 7569 702d 6d6f 6461 6c2d 2d63  al .uip-modal--c
+00012220: 6f6e 7465 6e74 202e 7569 702d 6d6f 6461  ontent .uip-moda
+00012230: 6c2d 2d62 6f64 7920 2e75 6970 2d6d 6f64  l--body .uip-mod
+00012240: 616c 2d2d 6963 6f6e 2d70 7265 7669 6577  al--icon-preview
+00012250: 2d77 7261 7020 2e75 6970 2d6d 6f64 616c  -wrap .uip-modal
+00012260: 2d2d 6963 6f6e 2d70 7265 7669 6577 2d69  --icon-preview-i
+00012270: 6e6e 6572 202e 7569 702d 6d6f 6461 6c2d  nner .uip-modal-
+00012280: 2d69 636f 6e2d 7072 6576 6965 7720 2e75  -icon-preview .u
+00012290: 6970 2d69 636f 6e2d 6974 656d 202e 7569  ip-icon-item .ui
+000122a0: 702d 6963 6f6e 2d69 7465 6d2d 696e 6e65  p-icon-item-inne
+000122b0: 7220 2e75 6970 2d69 636f 6e2d 6974 656d  r .uip-icon-item
+000122c0: 2d6e 616d 657b 636f 6c6f 723a 7661 7228  -name{color:var(
+000122d0: 2d2d 6463 612d 6772 6179 2c76 6172 282d  --dca-gray,var(-
+000122e0: 2d62 6f64 792d 7175 6965 742d 636f 6c6f  -body-quiet-colo
+000122f0: 722c 2336 3636 2929 3b66 6f6e 742d 7369  r,#666));font-si
+00012300: 7a65 3a31 3170 783b 7061 6464 696e 673a  ze:11px;padding:
+00012310: 3133 7078 2030 2030 3b6d 6178 2d77 6964  13px 0 0;max-wid
+00012320: 7468 3a31 3030 253b 7768 6974 652d 7370  th:100%;white-sp
+00012330: 6163 653a 6e6f 7772 6170 3b74 6578 742d  ace:nowrap;text-
+00012340: 6f76 6572 666c 6f77 3a65 6c6c 6970 7369  overflow:ellipsi
+00012350: 733b 6f76 6572 666c 6f77 3a68 6964 6465  s;overflow:hidde
+00012360: 6e3b 7465 7874 2d74 7261 6e73 666f 726d  n;text-transform
+00012370: 3a63 6170 6974 616c 697a 657d 2e75 6970  :capitalize}.uip
+00012380: 2d6d 6f64 616c 202e 7569 702d 6d6f 6461  -modal .uip-moda
+00012390: 6c2d 2d63 6f6e 7465 6e74 202e 7569 702d  l--content .uip-
+000123a0: 6d6f 6461 6c2d 2d62 6f64 7920 2e75 6970  modal--body .uip
+000123b0: 2d6d 6f64 616c 2d2d 6963 6f6e 2d70 7265  -modal--icon-pre
+000123c0: 7669 6577 2d77 7261 7020 2e75 6970 2d6d  view-wrap .uip-m
+000123d0: 6f64 616c 2d2d 6963 6f6e 2d73 6561 7263  odal--icon-searc
+000123e0: 687b 706f 7369 7469 6f6e 3a72 656c 6174  h{position:relat
+000123f0: 6976 657d 2e75 6970 2d6d 6f64 616c 202e  ive}.uip-modal .
+00012400: 7569 702d 6d6f 6461 6c2d 2d63 6f6e 7465  uip-modal--conte
+00012410: 6e74 202e 7569 702d 6d6f 6461 6c2d 2d62  nt .uip-modal--b
+00012420: 6f64 7920 2e75 6970 2d6d 6f64 616c 2d2d  ody .uip-modal--
+00012430: 6963 6f6e 2d70 7265 7669 6577 2d77 7261  icon-preview-wra
+00012440: 7020 2e75 6970 2d6d 6f64 616c 2d2d 6963  p .uip-modal--ic
+00012450: 6f6e 2d73 6561 7263 6820 696e 7075 747b  on-search input{
+00012460: 7769 6474 683a 3130 3025 3b70 6164 6469  width:100%;paddi
+00012470: 6e67 3a38 7078 2031 3570 783b 6261 636b  ng:8px 15px;back
+00012480: 6772 6f75 6e64 2d63 6f6c 6f72 3a76 6172  ground-color:var
+00012490: 282d 2d64 6361 2d77 6869 7465 2c76 6172  (--dca-white,var
+000124a0: 282d 2d62 672d 636f 6c6f 722c 2366 6666  (--bg-color,#fff
+000124b0: 2929 3b62 6f72 6465 723a 6e6f 6e65 7d2e  ));border:none}.
+000124c0: 7569 702d 6d6f 6461 6c20 2e75 6970 2d6d  uip-modal .uip-m
+000124d0: 6f64 616c 2d2d 636f 6e74 656e 7420 2e75  odal--content .u
+000124e0: 6970 2d6d 6f64 616c 2d2d 626f 6479 202e  ip-modal--body .
+000124f0: 7569 702d 6d6f 6461 6c2d 2d69 636f 6e2d  uip-modal--icon-
+00012500: 7072 6576 6965 772d 7772 6170 202e 7569  preview-wrap .ui
+00012510: 702d 6d6f 6461 6c2d 2d69 636f 6e2d 7365  p-modal--icon-se
+00012520: 6172 6368 2069 6e70 7574 3a2d 6d73 2d69  arch input:-ms-i
+00012530: 6e70 7574 2d70 6c61 6365 686f 6c64 6572  nput-placeholder
+00012540: 7b66 6f6e 742d 7374 796c 653a 6974 616c  {font-style:ital
+00012550: 6963 7d2e 7569 702d 6d6f 6461 6c20 2e75  ic}.uip-modal .u
+00012560: 6970 2d6d 6f64 616c 2d2d 636f 6e74 656e  ip-modal--conten
+00012570: 7420 2e75 6970 2d6d 6f64 616c 2d2d 626f  t .uip-modal--bo
+00012580: 6479 202e 7569 702d 6d6f 6461 6c2d 2d69  dy .uip-modal--i
+00012590: 636f 6e2d 7072 6576 6965 772d 7772 6170  con-preview-wrap
+000125a0: 202e 7569 702d 6d6f 6461 6c2d 2d69 636f   .uip-modal--ico
+000125b0: 6e2d 7365 6172 6368 2069 6e70 7574 3a3a  n-search input::
+000125c0: 706c 6163 6568 6f6c 6465 727b 666f 6e74  placeholder{font
+000125d0: 2d73 7479 6c65 3a69 7461 6c69 637d 2e75  -style:italic}.u
+000125e0: 6970 2d6d 6f64 616c 202e 7569 702d 6d6f  ip-modal .uip-mo
+000125f0: 6461 6c2d 2d63 6f6e 7465 6e74 202e 7569  dal--content .ui
+00012600: 702d 6d6f 6461 6c2d 2d62 6f64 7920 2e75  p-modal--body .u
+00012610: 6970 2d6d 6f64 616c 2d2d 6963 6f6e 2d70  ip-modal--icon-p
+00012620: 7265 7669 6577 2d77 7261 7020 2e75 6970  review-wrap .uip
+00012630: 2d6d 6f64 616c 2d2d 6963 6f6e 2d73 6561  -modal--icon-sea
+00012640: 7263 6820 696d 677b 706f 7369 7469 6f6e  rch img{position
+00012650: 3a61 6273 6f6c 7574 653b 746f 703a 3530  :absolute;top:50
+00012660: 253b 7472 616e 7366 6f72 6d3a 7472 616e  %;transform:tran
+00012670: 736c 6174 6559 282d 3530 2529 3b69 6e73  slateY(-50%);ins
+00012680: 6574 2d69 6e6c 696e 652d 656e 643a 3130  et-inline-end:10
+00012690: 7078 7d2e 7569 702d 6d6f 6461 6c20 2e75  px}.uip-modal .u
+000126a0: 6970 2d6d 6f64 616c 2d2d 666f 6f74 6572  ip-modal--footer
+000126b0: 7b62 6f72 6465 722d 746f 703a 3170 7820  {border-top:1px 
+000126c0: 736f 6c69 6420 7661 7228 2d2d 6463 612d  solid var(--dca-
+000126d0: 6772 6179 2d6c 6967 6874 6572 2c76 6172  gray-lighter,var
+000126e0: 282d 2d62 6f72 6465 722d 636f 6c6f 722c  (--border-color,
+000126f0: 2363 6363 2929 3b74 6578 742d 616c 6967  #ccc));text-alig
+00012700: 6e3a 6365 6e74 6572 3b62 6163 6b67 726f  n:center;backgro
+00012710: 756e 642d 636f 6c6f 723a 7661 7228 2d2d  und-color:var(--
+00012720: 6463 612d 7768 6974 652c 7661 7228 2d2d  dca-white,var(--
+00012730: 6267 2d63 6f6c 6f72 2c23 6666 6629 293b  bg-color,#fff));
+00012740: 626f 7264 6572 3a6e 6f6e 653b 6469 7370  border:none;disp
+00012750: 6c61 793a 6e6f 6e65 3b2d 6d73 2d66 6c65  lay:none;-ms-fle
+00012760: 782d 7061 636b 3a65 6e64 3b6a 7573 7469  x-pack:end;justi
+00012770: 6679 2d63 6f6e 7465 6e74 3a66 6c65 782d  fy-content:flex-
+00012780: 656e 643b 7061 6464 696e 673a 3570 783b  end;padding:5px;
+00012790: 626f 782d 7368 6164 6f77 3a30 2030 2038  box-shadow:0 0 8
+000127a0: 7078 2072 6762 6128 302c 302c 302c 2e31  px rgba(0,0,0,.1
+000127b0: 293b 706f 7369 7469 6f6e 3a72 656c 6174  );position:relat
+000127c0: 6976 653b 6469 7370 6c61 793a 2d6d 732d  ive;display:-ms-
+000127d0: 666c 6578 626f 783b 6469 7370 6c61 793a  flexbox;display:
+000127e0: 666c 6578 7d2e 7569 702d 6d6f 6461 6c20  flex}.uip-modal 
+000127f0: 2e75 6970 2d6d 6f64 616c 2d2d 666f 6f74  .uip-modal--foot
+00012800: 6572 2062 7574 746f 6e2e 7569 702d 696e  er button.uip-in
+00012810: 7365 7274 2d69 636f 6e2d 6275 7474 6f6e  sert-icon-button
+00012820: 7b70 6164 6469 6e67 3a31 3070 7820 3335  {padding:10px 35
+00012830: 7078 2169 6d70 6f72 7461 6e74 3b63 6f6c  px!important;col
+00012840: 6f72 3a76 6172 282d 2d64 6361 2d77 6869  or:var(--dca-whi
+00012850: 7465 2c76 6172 282d 2d62 672d 636f 6c6f  te,var(--bg-colo
+00012860: 722c 2366 6666 2929 2169 6d70 6f72 7461  r,#fff))!importa
+00012870: 6e74 3b62 6163 6b67 726f 756e 642d 636f  nt;background-co
+00012880: 6c6f 723a 2330 6266 2169 6d70 6f72 7461  lor:#0bf!importa
+00012890: 6e74 3b62 6f72 6465 723a 6e6f 6e65 3b63  nt;border:none;c
+000128a0: 7572 736f 723a 706f 696e 7465 723b 6f75  ursor:pointer;ou
+000128b0: 746c 696e 653a 307d 2e75 6970 2d6d 6f64  tline:0}.uip-mod
+000128c0: 616c 202e 7569 702d 6d6f 6461 6c2d 2d66  al .uip-modal--f
+000128d0: 6f6f 7465 7220 2e75 6e69 7665 7273 616c  ooter .universal
+000128e0: 2d62 7574 746f 6e7b 6865 6967 6874 3a34  -button{height:4
+000128f0: 3070 783b 6d61 7267 696e 2d69 6e6c 696e  0px;margin-inlin
+00012900: 652d 7374 6172 743a 3570 787d 2e75 6970  e-start:5px}.uip
+00012910: 2d6d 6f64 616c 202e 7569 702d 6d6f 6461  -modal .uip-moda
+00012920: 6c2d 2d66 6f6f 7465 7220 2e75 6e69 7665  l--footer .unive
+00012930: 7273 616c 2d62 7574 746f 6e2d 7375 6363  rsal-button-succ
+00012940: 6573 737b 7061 6464 696e 673a 3132 7078  ess{padding:12px
+00012950: 2033 3670 783b 636f 6c6f 723a 7661 7228   36px;color:var(
+00012960: 2d2d 6463 612d 7768 6974 652c 7661 7228  --dca-white,var(
+00012970: 2d2d 6267 2d63 6f6c 6f72 2c23 6666 6629  --bg-color,#fff)
+00012980: 293b 7769 6474 683a 696e 6974 6961 6c7d  );width:initial}
+00012990: 2e75 6970 2d6d 6f64 616c 202e 7569 702d  .uip-modal .uip-
+000129a0: 6d6f 6461 6c2d 2d66 6f6f 7465 7220 2e75  modal--footer .u
+000129b0: 6e69 7665 7273 616c 2d62 7574 746f 6e2d  niversal-button-
+000129c0: 7375 6363 6573 733a 686f 7665 727b 6261  success:hover{ba
+000129d0: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a23  ckground-color:#
+000129e0: 3062 667d 406d 6564 6961 2028 6d69 6e2d  0bf}@media (min-
+000129f0: 7769 6474 683a 3134 3430 7078 297b 626f  width:1440px){bo
+00012a00: 6479 3a6e 6f74 282e 636d 732d 6164 6d69  dy:not(.cms-admi
+00012a10: 6e2d 6d6f 6461 6c29 202e 7569 702d 6d6f  n-modal) .uip-mo
+00012a20: 6461 6c20 2e75 6970 2d6d 6f64 616c 2d2d  dal .uip-modal--
+00012a30: 636f 6e74 656e 747b 6d61 782d 7769 6474  content{max-widt
+00012a40: 683a 3132 3030 7078 7d7d 406d 6564 6961  h:1200px}}@media
+00012a50: 2028 6d61 782d 7769 6474 683a 3134 3339   (max-width:1439
+00012a60: 7078 297b 626f 6479 3a6e 6f74 282e 636d  px){body:not(.cm
+00012a70: 732d 6164 6d69 6e2d 6d6f 6461 6c29 202e  s-admin-modal) .
+00012a80: 7569 702d 6d6f 6461 6c20 2e75 6970 2d6d  uip-modal .uip-m
+00012a90: 6f64 616c 2d2d 636f 6e74 656e 747b 6d61  odal--content{ma
+00012aa0: 782d 7769 6474 683a 3939 3070 787d 2e75  x-width:990px}.u
+00012ab0: 6970 2d6d 6f64 616c 2d2d 6963 6f6e 2d70  ip-modal--icon-p
+00012ac0: 7265 7669 6577 2d77 7261 707b 7061 6464  review-wrap{padd
+00012ad0: 696e 673a 3330 7078 2035 3070 7820 307d  ing:30px 50px 0}
+00012ae0: 7d40 6d65 6469 6120 286d 6178 2d77 6964  }@media (max-wid
+00012af0: 7468 3a31 3032 3370 7829 7b62 6f64 793a  th:1023px){body:
+00012b00: 6e6f 7428 2e63 6d73 2d61 646d 696e 2d6d  not(.cms-admin-m
+00012b10: 6f64 616c 2920 2e75 6970 2d6d 6f64 616c  odal) .uip-modal
+00012b20: 202e 7569 702d 6d6f 6461 6c2d 2d63 6f6e   .uip-modal--con
+00012b30: 7465 6e74 7b6d 6178 2d77 6964 7468 3a37  tent{max-width:7
+00012b40: 3430 7078 7d7d 406d 6564 6961 2028 6d61  40px}}@media (ma
+00012b50: 782d 7769 6474 683a 3736 3770 7829 7b2e  x-width:767px){.
+00012b60: 7569 702d 6d6f 6461 6c2d 2d69 636f 6e2d  uip-modal--icon-
+00012b70: 7072 6576 6965 772d 7772 6170 7b70 6164  preview-wrap{pad
+00012b80: 6469 6e67 3a31 3570 7821 696d 706f 7274  ding:15px!import
+00012b90: 616e 747d 2e75 6970 2d6d 6f64 616c 2d2d  ant}.uip-modal--
+00012ba0: 7369 6465 6261 727b 6469 7370 6c61 793a  sidebar{display:
+00012bb0: 6e6f 6e65 7d7d 406d 6564 6961 2028 6d69  none}}@media (mi
+00012bc0: 6e2d 7769 6474 683a 3134 3430 7078 297b  n-width:1440px){
+00012bd0: 2e75 6970 2d6d 6f64 616c 2d2d 6963 6f6e  .uip-modal--icon
+00012be0: 2d70 7265 7669 6577 7b2d 6d73 2d67 7269  -preview{-ms-gri
+00012bf0: 642d 636f 6c75 6d6e 733a 2831 6672 295b  d-columns:(1fr)[
+00012c00: 375d 3b67 7269 642d 7465 6d70 6c61 7465  7];grid-template
+00012c10: 2d63 6f6c 756d 6e73 3a72 6570 6561 7428  -columns:repeat(
+00012c20: 372c 3166 7229 7d7d 406d 6564 6961 2028  7,1fr)}}@media (
+00012c30: 6d61 782d 7769 6474 683a 3134 3339 7078  max-width:1439px
+00012c40: 297b 2e75 6970 2d6d 6f64 616c 2d2d 6963  ){.uip-modal--ic
+00012c50: 6f6e 2d70 7265 7669 6577 7b2d 6d73 2d67  on-preview{-ms-g
+00012c60: 7269 642d 636f 6c75 6d6e 733a 2831 6672  rid-columns:(1fr
+00012c70: 295b 365d 3b67 7269 642d 7465 6d70 6c61  )[6];grid-templa
+00012c80: 7465 2d63 6f6c 756d 6e73 3a72 6570 6561  te-columns:repea
+00012c90: 7428 362c 3166 7229 7d7d 406d 6564 6961  t(6,1fr)}}@media
+00012ca0: 2028 6d61 782d 7769 6474 683a 3130 3234   (max-width:1024
+00012cb0: 7078 297b 2e75 6970 2d6d 6f64 616c 2d2d  px){.uip-modal--
+00012cc0: 6963 6f6e 2d70 7265 7669 6577 7b2d 6d73  icon-preview{-ms
+00012cd0: 2d67 7269 642d 636f 6c75 6d6e 733a 2831  -grid-columns:(1
+00012ce0: 6672 295b 355d 3b67 7269 642d 7465 6d70  fr)[5];grid-temp
+00012cf0: 6c61 7465 2d63 6f6c 756d 6e73 3a72 6570  late-columns:rep
+00012d00: 6561 7428 352c 3166 7229 7d7d 406d 6564  eat(5,1fr)}}@med
+00012d10: 6961 2028 6d61 782d 7769 6474 683a 3736  ia (max-width:76
+00012d20: 3770 7829 7b2e 7569 702d 6d6f 6461 6c2d  7px){.uip-modal-
+00012d30: 2d69 636f 6e2d 7072 6576 6965 777b 2d6d  -icon-preview{-m
+00012d40: 732d 6772 6964 2d63 6f6c 756d 6e73 3a28  s-grid-columns:(
+00012d50: 3166 7229 5b34 5d3b 6772 6964 2d74 656d  1fr)[4];grid-tem
+00012d60: 706c 6174 652d 636f 6c75 6d6e 733a 7265  plate-columns:re
+00012d70: 7065 6174 2834 2c31 6672 297d 7d40 6d65  peat(4,1fr)}}@me
+00012d80: 6469 6120 286d 6178 2d77 6964 7468 3a34  dia (max-width:4
+00012d90: 3739 7078 297b 2e75 6970 2d6d 6f64 616c  79px){.uip-modal
+00012da0: 2d2d 6963 6f6e 2d70 7265 7669 6577 7b2d  --icon-preview{-
+00012db0: 6d73 2d67 7269 642d 636f 6c75 6d6e 733a  ms-grid-columns:
+00012dc0: 2831 6672 295b 335d 3b67 7269 642d 7465  (1fr)[3];grid-te
+00012dd0: 6d70 6c61 7465 2d63 6f6c 756d 6e73 3a72  mplate-columns:r
+00012de0: 6570 6561 7428 332c 3166 7229 7d7d 406d  epeat(3,1fr)}}@m
+00012df0: 6564 6961 2028 6d61 782d 7769 6474 683a  edia (max-width:
+00012e00: 3134 3339 7078 297b 2e75 6970 2d6d 6f64  1439px){.uip-mod
+00012e10: 616c 2d2d 7369 6465 6261 722d 7461 622d  al--sidebar-tab-
+00012e20: 6974 656d 7b70 6164 6469 6e67 3a31 3570  item{padding:15p
+00012e30: 7820 3135 7078 2031 3570 7820 3235 7078  x 15px 15px 25px
+00012e40: 3b66 6f6e 742d 7369 7a65 3a31 3170 787d  ;font-size:11px}
+00012e50: 2e75 6970 2d6d 6f64 616c 2d2d 7369 6465  .uip-modal--side
+00012e60: 6261 722d 7461 622d 6974 656d 2069 7b66  bar-tab-item i{f
+00012e70: 6f6e 742d 7369 7a65 3a31 3570 787d 7d40  ont-size:15px}}@
+00012e80: 6d65 6469 6120 286d 6178 2d77 6964 7468  media (max-width
+00012e90: 3a31 3032 3470 7829 7b2e 7569 702d 6d6f  :1024px){.uip-mo
+00012ea0: 6461 6c2d 2d73 6964 6562 6172 2d74 6162  dal--sidebar-tab
+00012eb0: 2d69 7465 6d20 692c 2e75 6970 2d6d 6f64  -item i,.uip-mod
+00012ec0: 616c 2d2d 7369 6465 6261 722d 7461 622d  al--sidebar-tab-
+00012ed0: 6974 656d 2069 6d67 7b64 6973 706c 6179  item img{display
+00012ee0: 3a6e 6f6e 657d 7d2e 7372 2d6f 6e6c 797b  :none}}.sr-only{
+00012ef0: 706f 7369 7469 6f6e 3a61 6273 6f6c 7574  position:absolut
+00012f00: 6521 696d 706f 7274 616e 743b 7769 6474  e!important;widt
+00012f10: 683a 3170 7821 696d 706f 7274 616e 743b  h:1px!important;
+00012f20: 6865 6967 6874 3a31 7078 2169 6d70 6f72  height:1px!impor
+00012f30: 7461 6e74 3b70 6164 6469 6e67 3a30 2169  tant;padding:0!i
+00012f40: 6d70 6f72 7461 6e74 3b6d 6172 6769 6e3a  mportant;margin:
+00012f50: 2d31 7078 2169 6d70 6f72 7461 6e74 3b6f  -1px!important;o
+00012f60: 7665 7266 6c6f 773a 6869 6464 656e 2169  verflow:hidden!i
+00012f70: 6d70 6f72 7461 6e74 3b63 6c69 703a 7265  mportant;clip:re
+00012f80: 6374 2830 2c30 2c30 2c30 2921 696d 706f  ct(0,0,0,0)!impo
+00012f90: 7274 616e 743b 7768 6974 652d 7370 6163  rtant;white-spac
+00012fa0: 653a 6e6f 7772 6170 2169 6d70 6f72 7461  e:nowrap!importa
+00012fb0: 6e74 3b62 6f72 6465 723a 3021 696d 706f  nt;border:0!impo
+00012fc0: 7274 616e 747d 756c 2e6e 6176 7b6d 6172  rtant}ul.nav{mar
+00012fd0: 6769 6e2d 626f 7474 6f6d 3a31 656d 7d75  gin-bottom:1em}u
+00012fe0: 6c2e 6e61 763e 6c69 2e6e 6176 2d69 7465  l.nav>li.nav-ite
+00012ff0: 6d7b 6c69 7374 2d73 7479 6c65 2d74 7970  m{list-style-typ
+00013000: 653a 6e6f 6e65 3b70 6164 6469 6e67 3a69  e:none;padding:i
+00013010: 6e68 6572 6974 7d2e 636f 6c4d 2075 6c3a  nherit}.colM ul:
+00013020: 6e6f 7428 2e6f 626a 6563 742d 746f 6f6c  not(.object-tool
+00013030: 7329 2e6e 6176 7b6d 6172 6769 6e2d 746f  s).nav{margin-to
+00013040: 703a 303b 6d61 7267 696e 2d62 6f74 746f  p:0;margin-botto
+00013050: 6d3a 3230 7078 7d75 6c2e 6e61 7620 2e6e  m:20px}ul.nav .n
+00013060: 6176 2d69 7465 6d7b 6d61 7267 696e 2d69  av-item{margin-i
+00013070: 6e6c 696e 652d 656e 643a 3172 656d 7d75  nline-end:1rem}u
+00013080: 6c2e 6e61 7620 2e6e 6176 2d6c 696e 6b7b  l.nav .nav-link{
+00013090: 706f 7369 7469 6f6e 3a72 656c 6174 6976  position:relativ
+000130a0: 653b 7465 7874 2d64 6563 6f72 6174 696f  e;text-decoratio
+000130b0: 6e3a 6e6f 6e65 7d75 6c2e 6e61 7620 2e6e  n:none}ul.nav .n
+000130c0: 6176 2d6c 696e 6b20 7370 616e 2e69 6e64  av-link span.ind
+000130d0: 6963 6174 6f72 7b64 6973 706c 6179 3a6e  icator{display:n
+000130e0: 6f6e 653b 626f 7264 6572 2d72 6164 6975  one;border-radiu
+000130f0: 733a 3530 253b 7061 6464 696e 673a 2e35  s:50%;padding:.5
+00013100: 7265 6d3b 626f 7264 6572 3a31 7078 2073  rem;border:1px s
+00013110: 6f6c 6964 2076 6172 282d 2d64 6361 2d77  olid var(--dca-w
+00013120: 6869 7465 2c76 6172 282d 2d62 6f64 792d  hite,var(--body-
+00013130: 6267 2c23 6666 6629 293b 7472 616e 7366  bg,#fff));transf
+00013140: 6f72 6d3a 7472 616e 736c 6174 6528 2d35  orm:translate(-5
+00013150: 3025 2c2d 3530 2529 3b69 6e73 6574 2d62  0%,-50%);inset-b
+00013160: 6c6f 636b 2d73 7461 7274 3a30 3b69 6e73  lock-start:0;ins
+00013170: 6574 2d69 6e6c 696e 652d 7374 6172 743a  et-inline-start:
+00013180: 3130 3025 3b70 6f73 6974 696f 6e3a 6162  100%;position:ab
+00013190: 736f 6c75 7465 7d75 6c2e 6e61 7620 2e6e  solute}ul.nav .n
+000131a0: 6176 2d6c 696e 6b20 7370 616e 2e69 6e64  av-link span.ind
+000131b0: 6963 6174 6f72 2e65 7272 6f72 7b62 6163  icator.error{bac
+000131c0: 6b67 726f 756e 642d 636f 6c6f 723a 7661  kground-color:va
+000131d0: 7228 2d2d 6273 2d64 616e 6765 7229 7d75  r(--bs-danger)}u
+000131e0: 6c2e 6e61 7620 2e6e 6176 2d6c 696e 6b20  l.nav .nav-link 
+000131f0: 7370 616e 2e69 6e64 6963 6174 6f72 2e61  span.indicator.a
+00013200: 7474 7269 6275 7465 737b 6261 636b 6772  ttributes{backgr
+00013210: 6f75 6e64 2d63 6f6c 6f72 3a76 6172 282d  ound-color:var(-
+00013220: 2d62 732d 696e 666f 293b 6469 7370 6c61  -bs-info);displa
+00013230: 793a 626c 6f63 6b7d 756c 2e6e 6176 202e  y:block}ul.nav .
+00013240: 6e61 762d 6c69 6e6b 2e65 7272 6f72 3e73  nav-link.error>s
+00013250: 7061 6e2e 696e 6469 6361 746f 727b 6469  pan.indicator{di
+00013260: 7370 6c61 793a 626c 6f63 6b7d 756c 2e6e  splay:block}ul.n
+00013270: 6176 2e6e 6176 2d70 696c 6c73 202e 6e61  av.nav-pills .na
+00013280: 762d 6c69 6e6b 3a6e 6f74 282e 6163 7469  v-link:not(.acti
+00013290: 7665 297b 626f 7264 6572 2d73 7479 6c65  ve){border-style
+000132a0: 3a73 6f6c 6964 3b62 6f72 6465 722d 7769  :solid;border-wi
+000132b0: 6474 683a 3170 787d 626f 6479 3a6e 6f74  dth:1px}body:not
+000132c0: 282e 646a 616e 676f 636d 732d 6164 6d69  (.djangocms-admi
+000132d0: 6e2d 7374 796c 6529 2075 6c2e 646a 616e  n-style) ul.djan
+000132e0: 676f 636d 732d 6672 6f6e 7465 6e64 2e6e  gocms-frontend.n
+000132f0: 6176 2d74 6162 732b 6469 762e 7461 622d  av-tabs+div.tab-
+00013300: 636f 6e74 656e 7420 2e74 6162 2d70 616e  content .tab-pan
+00013310: 657b 626f 7264 6572 2d6c 6566 742d 7374  e{border-left-st
+00013320: 796c 653a 736f 6c69 643b 626f 7264 6572  yle:solid;border
+00013330: 2d62 6f74 746f 6d2d 7374 796c 653a 736f  -bottom-style:so
+00013340: 6c69 643b 626f 7264 6572 2d72 6967 6874  lid;border-right
+00013350: 2d73 7479 6c65 3a73 6f6c 6964 3b62 6f72  -style:solid;bor
+00013360: 6465 722d 6c65 6674 2d63 6f6c 6f72 3a76  der-left-color:v
+00013370: 6172 282d 2d68 6169 726c 696e 652d 636f  ar(--hairline-co
+00013380: 6c6f 7229 3b62 6f72 6465 722d 626f 7474  lor);border-bott
+00013390: 6f6d 2d63 6f6c 6f72 3a76 6172 282d 2d68  om-color:var(--h
+000133a0: 6169 726c 696e 652d 636f 6c6f 7229 3b62  airline-color);b
+000133b0: 6f72 6465 722d 7269 6768 742d 636f 6c6f  order-right-colo
+000133c0: 723a 7661 7228 2d2d 6861 6972 6c69 6e65  r:var(--hairline
+000133d0: 2d63 6f6c 6f72 293b 626f 7264 6572 2d77  -color);border-w
+000133e0: 6964 7468 3a31 7078 7d62 6f64 793a 6e6f  idth:1px}body:no
+000133f0: 7428 2e64 6a61 6e67 6f63 6d73 2d61 646d  t(.djangocms-adm
+00013400: 696e 2d73 7479 6c65 2920 756c 2e64 6a61  in-style) ul.dja
+00013410: 6e67 6f63 6d73 2d66 726f 6e74 656e 642e  ngocms-frontend.
+00013420: 6e61 762d 7461 6273 2b64 6976 2e74 6162  nav-tabs+div.tab
+00013430: 2d63 6f6e 7465 6e74 202e 7461 622d 7061  -content .tab-pa
+00013440: 6e65 2066 6965 6c64 7365 743a 6c61 7374  ne fieldset:last
+00013450: 2d63 6869 6c64 7b6d 6172 6769 6e2d 626f  -child{margin-bo
+00013460: 7474 6f6d 3a30 7d64 6976 2e74 6162 2d70  ttom:0}div.tab-p
+00013470: 6b7b 2d6d 732d 666c 6578 2d69 7465 6d2d  k{-ms-flex-item-
+00013480: 616c 6967 6e3a 6365 6e74 6572 3b2d 6d73  align:center;-ms
+00013490: 2d67 7269 642d 726f 772d 616c 6967 6e3a  -grid-row-align:
+000134a0: 6365 6e74 6572 3b61 6c69 676e 2d73 656c  center;align-sel
+000134b0: 663a 6365 6e74 6572 3b63 6f6c 6f72 3a76  f:center;color:v
+000134c0: 6172 282d 2d64 6361 2d67 7261 792d 6461  ar(--dca-gray-da
+000134d0: 726b 6572 2c76 6172 282d 2d62 6f64 792d  rker,var(--body-
+000134e0: 6667 2c23 3333 3329 293b 666f 6e74 2d73  fg,#333));font-s
+000134f0: 697a 653a 3830 253b 6d61 7267 696e 2d69  ize:80%;margin-i
+00013500: 6e6c 696e 652d 7374 6172 743a 6175 746f  nline-start:auto
+00013510: 7d2e 646a 616e 676f 636d 732d 6164 6d69  }.djangocms-admi
+00013520: 6e2d 7374 796c 6520 2e63 6f6c 4d20 756c  n-style .colM ul
+00013530: 2e6e 6176 3a6e 6f74 282e 6f62 6a65 6374  .nav:not(.object
+00013540: 2d74 6f6f 6c73 293a 6e6f 7428 2e6d 6573  -tools):not(.mes
+00013550: 7361 6765 6c69 7374 297b 6d61 7267 696e  sagelist){margin
+00013560: 2d74 6f70 3a30 7d2e 646a 616e 676f 636d  -top:0}.djangocm
+00013570: 732d 6164 6d69 6e2d 7374 796c 6520 2e63  s-admin-style .c
+00013580: 6f6c 4d20 756c 2e6e 6176 3a6e 6f74 282e  olM ul.nav:not(.
+00013590: 6f62 6a65 6374 2d74 6f6f 6c73 293a 6e6f  object-tools):no
+000135a0: 7428 2e6d 6573 7361 6765 6c69 7374 2920  t(.messagelist) 
+000135b0: 6c69 2e6e 6176 2d69 7465 6d7b 626f 7264  li.nav-item{bord
+000135c0: 6572 2d74 6f70 3a6e 6f6e 657d 696e 7075  er-top:none}inpu
+000135d0: 745b 7479 7065 3d6e 756d 6265 725d 2e61  t[type=number].a
+000135e0: 7574 6f2d 6669 656c 642b 7370 616e 7b64  uto-field+span{d
+000135f0: 6973 706c 6179 3a6e 6f6e 653b 706f 7369  isplay:none;posi
+00013600: 7469 6f6e 3a61 6273 6f6c 7574 653b 696e  tion:absolute;in
+00013610: 7365 742d 626c 6f63 6b2d 656e 643a 303b  set-block-end:0;
+00013620: 696e 7365 742d 696e 6c69 6e65 2d65 6e64  inset-inline-end
+00013630: 3a30 3b74 6578 742d 616c 6967 6e3a 656e  :0;text-align:en
+00013640: 643b 6d61 7267 696e 2d69 6e6c 696e 652d  d;margin-inline-
+00013650: 656e 643a 3331 7078 3b6d 6172 6769 6e2d  end:31px;margin-
+00013660: 626c 6f63 6b2d 656e 643a 3233 7078 3b63  block-end:23px;c
+00013670: 7572 736f 723a 706f 696e 7465 727d 626f  ursor:pointer}bo
+00013680: 6479 3a6e 6f74 282e 646a 616e 676f 636d  dy:not(.djangocm
+00013690: 732d 6164 6d69 6e2d 7374 796c 6529 2069  s-admin-style) i
+000136a0: 6e70 7574 5b74 7970 653d 6e75 6d62 6572  nput[type=number
+000136b0: 5d2e 6175 746f 2d66 6965 6c64 2b73 7061  ].auto-field+spa
+000136c0: 6e7b 6d61 7267 696e 2d62 6f74 746f 6d3a  n{margin-bottom:
+000136d0: 3233 7078 7d40 6d65 6469 6120 286d 6178  23px}@media (max
+000136e0: 2d77 6964 7468 3a31 3032 3470 7829 7b62  -width:1024px){b
+000136f0: 6f64 793a 6e6f 7428 2e64 6a61 6e67 6f63  ody:not(.djangoc
+00013700: 6d73 2d61 646d 696e 2d73 7479 6c65 2920  ms-admin-style) 
+00013710: 696e 7075 745b 7479 7065 3d6e 756d 6265  input[type=numbe
+00013720: 725d 2e61 7574 6f2d 6669 656c 642b 7370  r].auto-field+sp
+00013730: 616e 7b6d 6172 6769 6e2d 626f 7474 6f6d  an{margin-bottom
+00013740: 3a32 3470 787d 7d69 6e70 7574 5b74 7970  :24px}}input[typ
+00013750: 653d 6e75 6d62 6572 5d2e 6175 746f 2d66  e=number].auto-f
+00013760: 6965 6c64 2b73 7061 6e3a 6166 7465 727b  ield+span:after{
+00013770: 636f 6e74 656e 743a 2261 7574 6f22 7d69  content:"auto"}i
+00013780: 6e70 7574 5b74 7970 653d 6e75 6d62 6572  nput[type=number
+00013790: 5d2e 6175 746f 2d66 6965 6c64 2e61 7574  ].auto-field.aut
+000137a0: 6f7b 636f 6c6f 723a 7661 7228 2d2d 6463  o{color:var(--dc
+000137b0: 612d 7768 6974 652c 7661 7228 2d2d 626f  a-white,var(--bo
+000137c0: 6479 2d62 672c 2366 6666 2929 3b63 6172  dy-bg,#fff));car
+000137d0: 6574 2d63 6f6c 6f72 3a76 6172 282d 2d64  et-color:var(--d
+000137e0: 6361 2d62 6c61 636b 2c76 6172 282d 2d62  ca-black,var(--b
+000137f0: 6f64 792d 6667 2c23 3030 3029 297d 696e  ody-fg,#000))}in
+00013800: 7075 745b 7479 7065 3d6e 756d 6265 725d  put[type=number]
+00013810: 2e61 7574 6f2d 6669 656c 642e 6175 746f  .auto-field.auto
+00013820: 2b73 7061 6e7b 6469 7370 6c61 793a 626c  +span{display:bl
+00013830: 6f63 6b7d                                ock}
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/css/base.css.map` & `djangocms_frontend-1.3.2/djangocms_frontend/static/djangocms_frontend/css/base.css.map`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/css/button_group.css` & `djangocms_frontend-1.3.2/djangocms_frontend/static/djangocms_frontend/css/button_group.css`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map` & `djangocms_frontend-1.3.2/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/js/auto_input.js` & `djangocms_frontend-1.3.2/djangocms_frontend/static/djangocms_frontend/js/auto_input.js`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js` & `djangocms_frontend-1.3.2/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js` & `djangocms_frontend-1.3.2/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js` & `djangocms_frontend-1.3.2/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/js/django_select2.js` & `djangocms_frontend-1.3.2/djangocms_frontend/static/djangocms_frontend/js/django_select2.js`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/templates/bootstrap5/base.html` & `djangocms_frontend-1.3.2/djangocms_frontend/templates/bootstrap5/base.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/templates/bootstrap5/menu.html` & `djangocms_frontend-1.3.2/djangocms_frontend/templates/bootstrap5/menu.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html` & `djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/deprecated.html` & `djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend/admin/deprecated.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html` & `djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html` & `djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html` & `djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html` & `djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html` & `djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend.html` & `djangocms_frontend-1.3.2/djangocms_frontend/templates/djangocms_frontend.html`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend/templatetags/frontend.py` & `djangocms_frontend-1.3.2/djangocms_frontend/templatetags/frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 
 @register.simple_tag
 def get_attributes(attribute_field, *add_classes):
     """Joins a list of classes with an attributes field and returns all html attributes"""
     additional_classes = set()
     for classes in add_classes:
         if classes:
-            additional_classes.update(
-                classes.split() if isinstance(classes, str) else classes
-            )
+            additional_classes.update(classes.split() if isinstance(classes, str) else classes)
     attrs = []
     if attribute_field:
         for key, val in attribute_field.items():
             if key.lower() == "class":
                 val = " ".join(additional_classes.union(set(val.split())))
             if val:
                 attrs.append(f'{key}="{conditional_escape(val)}"')
@@ -85,17 +83,15 @@
             if as_json
             else plugin.get(item, "")
         )
     framework_info = context.get("framework_info", {})  # already available
     if not framework_info:
         content_type_id = context.get("content_type_id", None)
         if content_type_id:  # Get from content_type
-            model_name = (
-                ContentType.objects.get(id=content_type_id).model_class().__name__
-            )
+            model_name = ContentType.objects.get(id=content_type_id).model_class().__name__
             framework_info = settings.FRAMEWORK_PLUGIN_INFO.get(model_name, {})
             context["framework_info"] = framework_info  # and store
     return (
         mark_safe(json.dumps(framework_info.get(item, ""), cls=LazyEncoder))
         if as_json
         else framework_info.get(item, "")
     )
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend.egg-info/PKG-INFO` & `djangocms_frontend-1.3.2/djangocms_frontend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-frontend
-Version: 1.3.1
+Version: 1.3.2
 Summary: Adds abstract User Interface items as plugins to django CMS.
 Home-page: https://github.com/django-cms/djangocms-frontend
 Author: fsbraun
 Author-email: fsbraun@gmx.de
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `djangocms_frontend-1.3.1/djangocms_frontend.egg-info/SOURCES.txt` & `djangocms_frontend-1.3.2/djangocms_frontend.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,14 @@
 djangocms_frontend/contrib/link/__init__.py
 djangocms_frontend/contrib/link/apps.py
 djangocms_frontend/contrib/link/cms_plugins.py
 djangocms_frontend/contrib/link/constants.py
 djangocms_frontend/contrib/link/forms.py
 djangocms_frontend/contrib/link/helpers.py
 djangocms_frontend/contrib/link/models.py
-djangocms_frontend/contrib/link/urls.py
 djangocms_frontend/contrib/link/views.py
 djangocms_frontend/contrib/link/frameworks/__init__.py
 djangocms_frontend/contrib/link/frameworks/bootstrap5.py
 djangocms_frontend/contrib/link/migrations/0001_initial.py
 djangocms_frontend/contrib/link/migrations/__init__.py
 djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg
 djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/link.html
```

### Comparing `djangocms_frontend-1.3.1/pyproject.toml` & `djangocms_frontend-1.3.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 
 [tool.ruff]
 exclude = [
     ".env",
     ".venv",
     "**/migrations/**",
 ]
-ignore = [
+lint.ignore = [
     "E501",  # line too long
     "F403",  # 'from module import *' used; unable to detect undefined names
     "E701",  # multiple statements on one line (colon)
     "F401",  # module imported but unused
 ]
 line-length = 119
-select = [
+lint.select = [
     "I",
     "E",
     "F",
     "W",
 ]
```

### Comparing `djangocms_frontend-1.3.1/setup.py` & `djangocms_frontend-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/accordion/test_models.py` & `djangocms_frontend-1.3.2/tests/accordion/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/accordion/test_plugins.py` & `djangocms_frontend-1.3.2/tests/accordion/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/alert/test_plugins.py` & `djangocms_frontend-1.3.2/tests/alert/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/badge/test_plugins.py` & `djangocms_frontend-1.3.2/tests/badge/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/card/test_models.py` & `djangocms_frontend-1.3.2/tests/card/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/card/test_plugins.py` & `djangocms_frontend-1.3.2/tests/card/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/carousel/test_models.py` & `djangocms_frontend-1.3.2/tests/carousel/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/carousel/test_plugins.py` & `djangocms_frontend-1.3.2/tests/carousel/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/collapse/test_models.py` & `djangocms_frontend-1.3.2/tests/collapse/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/collapse/test_plugins.py` & `djangocms_frontend-1.3.2/tests/collapse/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/content/test_models.py` & `djangocms_frontend-1.3.2/tests/content/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/content/test_plugins.py` & `djangocms_frontend-1.3.2/tests/content/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/fixtures.py` & `djangocms_frontend-1.3.2/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/grid/test_models.py` & `djangocms_frontend-1.3.2/tests/grid/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/grid/test_plugins.py` & `djangocms_frontend-1.3.2/tests/grid/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/helpers.py` & `djangocms_frontend-1.3.2/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/icon/test_models.py` & `djangocms_frontend-1.3.2/tests/icon/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/icon/test_plugins.py` & `djangocms_frontend-1.3.2/tests/icon/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/image/test_drag_n_drop.py` & `djangocms_frontend-1.3.2/tests/image/test_drag_n_drop.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/image/test_plugins.py` & `djangocms_frontend-1.3.2/tests/image/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/jumbotron/test_plugins.py` & `djangocms_frontend-1.3.2/tests/jumbotron/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/link/test_plugins.py` & `djangocms_frontend-1.3.2/tests/link/test_plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,16 +115,16 @@
             or ('class="btn-outline-primary btn"' in response.content.decode("utf-8")),
             f'Cound not find class="btn btn-outline-primary" in {response.content.decode("utf-8")}',
         )
 
     def test_smart_link_field(self):
         slf = SmartLinkField()
         choices = get_choices(None)
-        self.assertEqual("example.com", choices[0][0])  # Site name
-        self.assertIn(("2-1", "home"), choices[0][1])
+        self.assertEqual("example.com", choices[1][0])  # Site name
+        self.assertIn(("2-1", "home"), choices[1][1])
 
         cleaned = slf.clean("2-1")
         self.assertEqual(dict(model="cms.page", pk=1), cleaned)
 
         self.assertEqual(slf.prepare_value("blabla"), "")
         self.assertEqual(slf.prepare_value(dict(model="cms.page", pk=1)), "2-1")
         self.assertEqual(slf.prepare_value(self.home), "2-1")
```

### Comparing `djangocms_frontend-1.3.1/tests/listgroup/test_models.py` & `djangocms_frontend-1.3.2/tests/listgroup/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/listgroup/test_plugins.py` & `djangocms_frontend-1.3.2/tests/listgroup/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/media/test_models.py` & `djangocms_frontend-1.3.2/tests/media/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/media/test_plugins.py` & `djangocms_frontend-1.3.2/tests/media/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/navigation/test_models.py` & `djangocms_frontend-1.3.2/tests/navigation/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/navigation/test_plugins.py` & `djangocms_frontend-1.3.2/tests/navigation/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/tabs/test_models.py` & `djangocms_frontend-1.3.2/tests/tabs/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/tabs/test_plugins.py` & `djangocms_frontend-1.3.2/tests/tabs/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/test_constants.py` & `djangocms_frontend-1.3.2/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/test_fields.py` & `djangocms_frontend-1.3.2/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/test_helpers.py` & `djangocms_frontend-1.3.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/test_migrations.py` & `djangocms_frontend-1.3.2/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/test_settings.py` & `djangocms_frontend-1.3.2/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/utilities/test_models.py` & `djangocms_frontend-1.3.2/tests/utilities/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms_frontend-1.3.1/tests/utilities/test_plugins.py` & `djangocms_frontend-1.3.2/tests/utilities/test_plugins.py`

 * *Files identical despite different names*


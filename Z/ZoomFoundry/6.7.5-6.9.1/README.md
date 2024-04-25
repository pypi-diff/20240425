# Comparing `tmp/ZoomFoundry-6.7.5.tar.gz` & `tmp/ZoomFoundry-6.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ZoomFoundry-6.7.5.tar", last modified: Fri Sep 25 05:43:15 2020, max compression
+gzip compressed data, was "dist/ZoomFoundry-6.9.1.tar", last modified: Wed Oct  7 21:07:38 2020, max compression
```

## Comparing `ZoomFoundry-6.7.5.tar` & `ZoomFoundry-6.9.1.tar`

### file list

```diff
@@ -1,498 +1,499 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/
--rw-r--r--   0 root         (0) root         (0)     2860 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1522 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      223 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9361 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6781 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:14.000000 ZoomFoundry-6.7.5/ZoomFoundry.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9361 2020-09-25 05:43:13.000000 ZoomFoundry-6.7.5/ZoomFoundry.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    18518 2020-09-25 05:43:14.000000 ZoomFoundry-6.7.5/ZoomFoundry.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-09-25 05:43:13.000000 ZoomFoundry-6.7.5/ZoomFoundry.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2020-09-25 05:43:13.000000 ZoomFoundry-6.7.5/ZoomFoundry.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      127 2020-09-25 05:43:13.000000 ZoomFoundry-6.7.5/ZoomFoundry.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2020-09-25 05:43:13.000000 ZoomFoundry-6.7.5/ZoomFoundry.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      231 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1836 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/
--rw-r--r--   0 root         (0) root         (0)     1020 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1196 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/__main__.py
--rw-r--r--   0 root         (0) root         (0)       22 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:14.000000 ZoomFoundry-6.7.5/zoom/_assets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:14.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:14.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/apps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/apps/basic/
--rw-r--r--   0 root         (0) root         (0)      123 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/apps/basic/app.py
--rw-r--r--   0 root         (0) root         (0)       60 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/apps/basic/config.ini
--rw-r--r--   0 root         (0) root         (0)      564 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/apps/basic/index.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:14.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/instances/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:14.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/instances/basic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/instances/basic/apps/
--rw-r--r--   0 root         (0) root         (0)       69 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/instances/basic/apps/default.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:14.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/instances/basic/sites/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/instances/basic/sites/localhost/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/instances/basic/sites/localhost/.gitinclude
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/instances/basic/themes/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/instances/basic/themes/.gitinclude
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:14.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/sites/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/sites/basic/
--rw-r--r--   0 root         (0) root         (0)     3944 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/sites/basic/site.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:14.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/
--rw-r--r--   0 root         (0) root         (0)       73 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/README.md
--rw-r--r--   0 root         (0) root         (0)      131 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/content.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/css/
--rw-r--r--   0 root         (0) root         (0)      653 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/css/buttons.css
--rw-r--r--   0 root         (0) root         (0)      357 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/css/components.css
--rw-r--r--   0 root         (0) root         (0)      649 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/css/containers.css
--rw-r--r--   0 root         (0) root         (0)     1552 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/css/content.css
--rw-r--r--   0 root         (0) root         (0)      840 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/css/flags.css
--rw-r--r--   0 root         (0) root         (0)      576 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/css/guide.css
--rw-r--r--   0 root         (0) root         (0)     3846 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/css/navigation.css
--rw-r--r--   0 root         (0) root         (0)      540 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/css/pricebox.css
--rw-r--r--   0 root         (0) root         (0)       91 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/css/print.css
--rw-r--r--   0 root         (0) root         (0)     2299 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/css/social.css
--rw-r--r--   0 root         (0) root         (0)       43 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/css/style.css
--rw-r--r--   0 root         (0) root         (0)     9538 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/css/widget.css
--rw-r--r--   0 root         (0) root         (0)      131 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/default.html
--rw-r--r--   0 root         (0) root         (0)      131 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/templates/
--rw-r--r--   0 root         (0) root         (0)     2039 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/templates/body.html
--rw-r--r--   0 root         (0) root         (0)      705 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/templates/head.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/
--rw-r--r--   0 root         (0) root         (0)      263 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/about.md
--rw-r--r--   0 root         (0) root         (0)      251 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/app.py
--rw-r--r--   0 root         (0) root         (0)     1420 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/apps.py
--rw-r--r--   0 root         (0) root         (0)       33 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/config.ini
--rw-r--r--   0 root         (0) root         (0)     1302 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/database.py
--rw-r--r--   0 root         (0) root         (0)      109 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/fields.py
--rw-r--r--   0 root         (0) root         (0)     7280 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/groups.py
--rw-r--r--   0 root         (0) root         (0)    16101 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/index.py
--rw-r--r--   0 root         (0) root         (0)     2082 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/jobs.py
--rw-r--r--   0 root         (0) root         (0)     2709 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/mail.py
--rw-r--r--   0 root         (0) root         (0)     8930 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/model.py
--rw-r--r--   0 root         (0) root         (0)      331 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/reset.md
--rw-r--r--   0 root         (0) root         (0)      183 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/test_format.py
--rw-r--r--   0 root         (0) root         (0)     7499 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/users.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/views/
--rw-r--r--   0 root         (0) root         (0)      247 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/views/index_page_layout_view.css
--rw-r--r--   0 root         (0) root         (0)      276 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/views/index_page_layout_view.html
--rw-r--r--   0 root         (0) root         (0)      571 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/views/metric_view.css
--rw-r--r--   0 root         (0) root         (0)      199 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/views/metric_view.html
--rw-r--r--   0 root         (0) root         (0)       29 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/views/metric_view.name.html
--rw-r--r--   0 root         (0) root         (0)       94 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/views/metric_view.red.css
--rw-r--r--   0 root         (0) root         (0)       77 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/views/metrics_view.html
--rw-r--r--   0 root         (0) root         (0)      485 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/views/panel_view.css
--rw-r--r--   0 root         (0) root         (0)      155 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/views/panel_view.html
--rw-r--r--   0 root         (0) root         (0)      107 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/views/panel_view.js
--rw-r--r--   0 root         (0) root         (0)       55 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/views/test_view.html
--rw-r--r--   0 root         (0) root         (0)     1416 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/views.py
--rw-r--r--   0 root         (0) root         (0)      440 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/welcome.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/api/
--rw-r--r--   0 root         (0) root         (0)       68 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/api/app.py
--rw-r--r--   0 root         (0) root         (0)       41 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/api/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/
--rw-r--r--   0 root         (0) root         (0)     2435 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/app.py
--rw-r--r--   0 root         (0) root         (0)       27 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/config.ini
--rw-r--r--   0 root         (0) root         (0)       56 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/contact.md
--rw-r--r--   0 root         (0) root         (0)     8541 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/files.py
--rw-r--r--   0 root         (0) root         (0)     6102 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/images.py
--rw-r--r--   0 root         (0) root         (0)      119 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/index.md
--rw-r--r--   0 root         (0) root         (0)     1997 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/index.py
--rw-r--r--   0 root         (0) root         (0)     3185 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/pages.py
--rw-r--r--   0 root         (0) root         (0)      434 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/snippets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/static/
--rw-r--r--   0 root         (0) root         (0)     1827 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/static/file-manager.css
--rw-r--r--   0 root         (0) root         (0)     5322 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/static/file-manager.js
--rw-r--r--   0 root         (0) root         (0)     1642 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/static/markdown-linker.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/views/
--rw-r--r--   0 root         (0) root         (0)      828 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/views/file-manager.html
--rw-r--r--   0 root         (0) root         (0)      971 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/views/images.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/forgot/
--rw-r--r--   0 root         (0) root         (0)      494 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/forgot/activate.md
--rw-r--r--   0 root         (0) root         (0)       72 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/forgot/app.py
--rw-r--r--   0 root         (0) root         (0)      171 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/forgot/complete.md
--rw-r--r--   0 root         (0) root         (0)       20 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/forgot/config.ini
--rw-r--r--   0 root         (0) root         (0)      365 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/forgot/expired.md
--rw-r--r--   0 root         (0) root         (0)      199 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/forgot/index.md
--rw-r--r--   0 root         (0) root         (0)     2345 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/forgot/index.py
--rw-r--r--   0 root         (0) root         (0)     3370 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/forgot/model.py
--rw-r--r--   0 root         (0) root         (0)      228 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/forgot/reset.md
--rw-r--r--   0 root         (0) root         (0)      239 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/forgot/step2.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/hello/
--rw-r--r--   0 root         (0) root         (0)      532 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/hello/app.py
--rw-r--r--   0 root         (0) root         (0)       25 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/hello/background.py
--rw-r--r--   0 root         (0) root         (0)      239 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/hello/packages.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/home/
--rw-r--r--   0 root         (0) root         (0)     1612 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/home/app.py
--rw-r--r--   0 root         (0) root         (0)       42 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/home/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/icons/
--rw-r--r--   0 root         (0) root         (0)       84 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/icons/app.py
--rw-r--r--   0 root         (0) root         (0)       59 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/icons/config.ini
--rw-r--r--   0 root         (0) root         (0)   213349 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/icons/icons.html
--rw-r--r--   0 root         (0) root         (0)      638 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/icons/index.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/login/
--rw-r--r--   0 root         (0) root         (0)       53 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/login/app.py
--rw-r--r--   0 root         (0) root         (0)       40 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/login/config.ini
--rw-r--r--   0 root         (0) root         (0)     3093 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/login/index.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/login/views/
--rw-r--r--   0 root         (0) root         (0)       36 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/login/views/forgot_password.css
--rw-r--r--   0 root         (0) root         (0)       80 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/login/views/forgot_password.pug
--rw-r--r--   0 root         (0) root         (0)       94 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/login/views/login_form.css
--rw-r--r--   0 root         (0) root         (0)     1043 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/login/views/login_form.html
--rw-r--r--   0 root         (0) root         (0)      105 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/login/views/remember_me.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/logout/
--rw-r--r--   0 root         (0) root         (0)      821 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/logout/app.py
--rw-r--r--   0 root         (0) root         (0)       40 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/logout/config.ini
--rw-r--r--   0 root         (0) root         (0)      101 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/packages.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/ping/
--rw-r--r--   0 root         (0) root         (0)       81 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/ping/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/register/
--rw-r--r--   0 root         (0) root         (0)      255 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/register/activate.html
--rw-r--r--   0 root         (0) root         (0)      264 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/register/already_registered.md
--rw-r--r--   0 root         (0) root         (0)       53 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/register/app.py
--rw-r--r--   0 root         (0) root         (0)      307 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/register/expired.md
--rw-r--r--   0 root         (0) root         (0)     2640 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/register/index.py
--rw-r--r--   0 root         (0) root         (0)     7014 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/register/model.py
--rw-r--r--   0 root         (0) root         (0)      306 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/register/name_taken.md
--rw-r--r--   0 root         (0) root         (0)      268 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/register/register_complete.md
--rw-r--r--   0 root         (0) root         (0)      997 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/register/registration.html
--rw-r--r--   0 root         (0) root         (0)      319 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/register/step2.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/
--rw-r--r--   0 root         (0) root         (0)      217 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/about.md
--rw-r--r--   0 root         (0) root         (0)     1628 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/alerts.py
--rw-r--r--   0 root         (0) root         (0)      293 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/app.py
--rw-r--r--   0 root         (0) root         (0)     1212 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/background.py
--rw-r--r--   0 root         (0) root         (0)      648 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/collection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/components/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/components/widgets_layout/
--rw-r--r--   0 root         (0) root         (0)      122 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/components/widgets_layout/__init__.py
--rw-r--r--   0 root         (0) root         (0)       44 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/components/widgets_layout/widgets_layout.pug
--rw-r--r--   0 root         (0) root         (0)      124 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/components/widgets_layout/widgets_layout.sass
--rw-r--r--   0 root         (0) root         (0)     1128 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/components.py
--rw-r--r--   0 root         (0) root         (0)       75 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/config.ini
--rw-r--r--   0 root         (0) root         (0)     6824 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/fields.py
--rw-r--r--   0 root         (0) root         (0)     1043 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/flags.py
--rw-r--r--   0 root         (0) root         (0)     1451 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/index.py
--rw-r--r--   0 root         (0) root         (0)       71 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/model.py
--rw-r--r--   0 root         (0) root         (0)     2459 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/parts.py
--rw-r--r--   0 root         (0) root         (0)     1156 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/responses.py
--rw-r--r--   0 root         (0) root         (0)     4682 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/sample.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/static/
--rw-r--r--   0 root         (0) root         (0)       37 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/static/test.css
--rw-r--r--   0 root         (0) root         (0)       21 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/static/test.js
--rw-r--r--   0 root         (0) root         (0)       24 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/static/test.json
--rw-r--r--   0 root         (0) root         (0)      792 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/widgets/
--rw-r--r--   0 root         (0) root         (0)     2070 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)       32 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/widgets/cards.pug
--rw-r--r--   0 root         (0) root         (0)      243 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/widgets/cards.sass
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/settings/
--rw-r--r--   0 root         (0) root         (0)      164 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/settings/about.md
--rw-r--r--   0 root         (0) root         (0)       88 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/settings/app.py
--rw-r--r--   0 root         (0) root         (0)       36 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/settings/config.ini
--rw-r--r--   0 root         (0) root         (0)     3898 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/settings/index.py
--rw-r--r--   0 root         (0) root         (0)     2521 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/settings/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/storage/
--rw-r--r--   0 root         (0) root         (0)      203 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/storage/about.md
--rw-r--r--   0 root         (0) root         (0)       91 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/storage/app.py
--rw-r--r--   0 root         (0) root         (0)       76 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/storage/config.ini
--rw-r--r--   0 root         (0) root         (0)     4077 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/standard_apps/storage/index.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:14.000000 ZoomFoundry-6.7.5/zoom/_assets/web/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:14.000000 ZoomFoundry-6.7.5/zoom/_assets/web/sites/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/sites/default/
--rw-r--r--   0 root         (0) root         (0)     3760 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/sites/default/site.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/sites/localhost/
--rw-r--r--   0 root         (0) root         (0)       95 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/sites/localhost/site.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:14.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/
--rw-r--r--   0 root         (0) root         (0)      356 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/_partials/
--rw-r--r--   0 root         (0) root         (0)      228 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/_partials/footer.pug
--rw-r--r--   0 root         (0) root         (0)      516 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/_partials/head.pug
--rw-r--r--   0 root         (0) root         (0)       76 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/_partials/layout.pug
--rw-r--r--   0 root         (0) root         (0)      502 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/_partials/nav.pug
--rw-r--r--   0 root         (0) root         (0)      186 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/_partials/tail.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/
--rw-r--r--   0 root         (0) root         (0)      761 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/buttons.css
--rw-r--r--   0 root         (0) root         (0)      249 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/buttons.css.map
--rw-r--r--   0 root         (0) root         (0)      234 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/components.css
--rw-r--r--   0 root         (0) root         (0)      165 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/components.css.map
--rw-r--r--   0 root         (0) root         (0)       45 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/containers.css
--rw-r--r--   0 root         (0) root         (0)       91 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/containers.css.map
--rw-r--r--   0 root         (0) root         (0)     1981 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/content.css
--rw-r--r--   0 root         (0) root         (0)      629 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/content.css.map
--rw-r--r--   0 root         (0) root         (0)     1000 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/flags.css
--rw-r--r--   0 root         (0) root         (0)      259 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/flags.css.map
--rw-r--r--   0 root         (0) root         (0)     4745 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/navigation.css
--rw-r--r--   0 root         (0) root         (0)     1276 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/navigation.css.map
--rw-r--r--   0 root         (0) root         (0)      233 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/print.css
--rw-r--r--   0 root         (0) root         (0)      141 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/print.css.map
--rw-r--r--   0 root         (0) root         (0)     2680 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/social.css
--rw-r--r--   0 root         (0) root         (0)      560 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/social.css.map
--rw-r--r--   0 root         (0) root         (0)      911 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/style.css
--rw-r--r--   0 root         (0) root         (0)      428 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/style.css.map
--rw-r--r--   0 root         (0) root         (0)    11649 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/widget.css
--rw-r--r--   0 root         (0) root         (0)     2689 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/widget.css.map
--rw-r--r--   0 root         (0) root         (0)      223 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/default.pug
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/images/
--rw-r--r--   0 root         (0) root         (0)    10713 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/images/android-chrome-192x192.png
--rw-r--r--   0 root         (0) root         (0)    25739 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/images/android-chrome-512x512.png
--rw-r--r--   0 root         (0) root         (0)     9614 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/images/apple-touch-icon.png
--rw-r--r--   0 root         (0) root         (0)     9614 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/images/banner-logo.png
--rw-r--r--   0 root         (0) root         (0)     9614 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/images/email-logo.png
--rw-r--r--   0 root         (0) root         (0)      769 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/images/favicon-16x16.png
--rw-r--r--   0 root         (0) root         (0)     1548 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/images/favicon-32x32.png
--rw-r--r--   0 root         (0) root         (0)    15406 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/images/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:14.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/src/sass/
--rw-r--r--   0 root         (0) root         (0)      636 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/src/sass/buttons.sass
--rw-r--r--   0 root         (0) root         (0)      160 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/src/sass/components.sass
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/src/sass/containers.sass
--rw-r--r--   0 root         (0) root         (0)     1720 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/src/sass/content.sass
--rw-r--r--   0 root         (0) root         (0)      904 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/src/sass/flags.sass
--rw-r--r--   0 root         (0) root         (0)     4541 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/src/sass/navigation.sass
--rw-r--r--   0 root         (0) root         (0)      175 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/src/sass/print.sass
--rw-r--r--   0 root         (0) root         (0)     2061 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/src/sass/social.sass
--rw-r--r--   0 root         (0) root         (0)      879 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/src/sass/style.sass
--rw-r--r--   0 root         (0) root         (0)    10940 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/src/sass/widget.sass
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/
--rw-r--r--   0 root         (0) root         (0)       49 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/index.wsgi
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:14.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/
--rw-r--r--   0 root         (0) root         (0)     1131 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:14.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/bootstrap4.5/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/bootstrap4.5/css/
--rw-r--r--   0 root         (0) root         (0)   160403 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/bootstrap4.5/css/bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   646432 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/bootstrap4.5/css/bootstrap.min.css.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/bootstrap4.5/js/
--rw-r--r--   0 root         (0) root         (0)    81084 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/bootstrap4.5/js/bootstrap.bundle.min.js
--rw-r--r--   0 root         (0) root         (0)   315300 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/bootstrap4.5/js/bootstrap.bundle.min.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/css/
--rw-r--r--   0 root         (0) root         (0)    26132 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap-theme.css
--rw-r--r--   0 root         (0) root         (0)    47706 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap-theme.css.map
--rw-r--r--   0 root         (0) root         (0)    23409 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap-theme.min.css
--rw-r--r--   0 root         (0) root         (0)    25648 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap-theme.min.css.map
--rw-r--r--   0 root         (0) root         (0)   146010 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap.css
--rw-r--r--   0 root         (0) root         (0)   389287 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap.css.map
--rw-r--r--   0 root         (0) root         (0)   121200 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)   542194 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap.min.css.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/fonts/
--rw-r--r--   0 root         (0) root         (0)    20127 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 root         (0) root         (0)   108738 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 root         (0) root         (0)    45404 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 root         (0) root         (0)    23424 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 root         (0) root         (0)    18028 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/js/
--rw-r--r--   0 root         (0) root         (0)    69707 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/js/bootstrap.js
--rw-r--r--   0 root         (0) root         (0)    37045 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/js/bootstrap.min.js
--rw-r--r--   0 root         (0) root         (0)      484 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/js/npm.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/chosen/
--rw-r--r--   0 root         (0) root         (0)     1215 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/chosen/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      538 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/chosen/chosen-sprite.png
--rw-r--r--   0 root         (0) root         (0)      738 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/chosen/chosen-sprite@2x.png
--rw-r--r--   0 root         (0) root         (0)    29121 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/chosen/chosen.jquery.min.js
--rw-r--r--   0 root         (0) root         (0)    10220 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/chosen/chosen.min.css
--rw-r--r--   0 root         (0) root         (0)      240 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/cookieconsent.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/dropzone/
--rw-r--r--   0 root         (0) root         (0)     1150 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/dropzone/LICENSE
--rw-r--r--   0 root         (0) root         (0)      751 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/dropzone/basic.min.css
--rw-r--r--   0 root         (0) root         (0)    33689 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/dropzone/dropzone-amd-module.min.js
--rw-r--r--   0 root         (0) root         (0)     9717 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/dropzone/dropzone.min.css
--rw-r--r--   0 root         (0) root         (0)    33588 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/dropzone/dropzone.min.js
--rw-r--r--   0 root         (0) root         (0)       70 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/dropzone.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:14.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/fontawesome4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/fontawesome4/css/
--rw-r--r--   0 root         (0) root         (0)    37414 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/fontawesome4/css/font-awesome.css
--rw-r--r--   0 root         (0) root         (0)    31000 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/fontawesome4/css/font-awesome.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/fontawesome4/fonts/
--rw-r--r--   0 root         (0) root         (0)   165742 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/fontawesome4/fonts/fontawesome-webfont.eot
--rw-r--r--   0 root         (0) root         (0)   444379 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/fontawesome4/fonts/fontawesome-webfont.svg
--rw-r--r--   0 root         (0) root         (0)   165548 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/fontawesome4/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 root         (0) root         (0)    98024 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/fontawesome4/fonts/fontawesome-webfont.woff
--rw-r--r--   0 root         (0) root         (0)    77160 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/fontawesome4/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 root         (0) root         (0)      202 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/fouc.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/
--rw-r--r--   0 root         (0) root         (0)     1987 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/checkmark.png
--rw-r--r--   0 root         (0) root         (0)      251 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/delete.png
--rw-r--r--   0 root         (0) root         (0)      276 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/down_arrow_blue.png
--rw-r--r--   0 root         (0) root         (0)     1133 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/down_arrow_red.png
--rw-r--r--   0 root         (0) root         (0)     6006 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/favicon.ico
--rw-r--r--   0 root         (0) root         (0)      699 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/follow-off.png
--rw-r--r--   0 root         (0) root         (0)      655 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/follow-on.png
--rw-r--r--   0 root         (0) root         (0)      381 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/heart-off.png
--rw-r--r--   0 root         (0) root         (0)      333 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/heart-on.png
--rw-r--r--   0 root         (0) root         (0)      360 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/mail-off.png
--rw-r--r--   0 root         (0) root         (0)      286 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/mail-on.png
--rw-r--r--   0 root         (0) root         (0)     9546 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/no_image.png
--rw-r--r--   0 root         (0) root         (0)     3350 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/no_photo.png
--rw-r--r--   0 root         (0) root         (0)    10829 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/progress.gif
--rw-r--r--   0 root         (0) root         (0)      251 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/remove.png
--rw-r--r--   0 root         (0) root         (0)      400 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/remove_filter.png
--rw-r--r--   0 root         (0) root         (0)      398 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/remove_filter_hover.png
--rw-r--r--   0 root         (0) root         (0)     2098 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/secure.png
--rw-r--r--   0 root         (0) root         (0)     1067 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/settings.png
--rw-r--r--   0 root         (0) root         (0)     1297 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/settings2.png
--rw-r--r--   0 root         (0) root         (0)     8544 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/social-icons-small.png
--rw-r--r--   0 root         (0) root         (0)    10440 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/social-icons.png
--rw-r--r--   0 root         (0) root         (0)       42 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/spacer.gif
--rw-r--r--   0 root         (0) root         (0)      625 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/star-off.png
--rw-r--r--   0 root         (0) root         (0)      872 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/star-on.png
--rw-r--r--   0 root         (0) root         (0)     3485 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/star_empty.png
--rw-r--r--   0 root         (0) root         (0)     3459 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/star_full.png
--rw-r--r--   0 root         (0) root         (0)     3491 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/star_half_full.png
--rw-r--r--   0 root         (0) root         (0)     1449 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/thumbs-down-off.png
--rw-r--r--   0 root         (0) root         (0)     1547 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/thumbs-down.png
--rw-r--r--   0 root         (0) root         (0)     1460 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/thumbs-up-off.png
--rw-r--r--   0 root         (0) root         (0)     1569 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/thumbs-up.png
--rw-r--r--   0 root         (0) root         (0)      286 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/trash.png
--rw-r--r--   0 root         (0) root         (0)      302 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/up_arrow_blue.png
--rw-r--r--   0 root         (0) root         (0)     5344 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images-field.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery/
--rw-r--r--   0 root         (0) root         (0)    86596 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery/jquery.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/
--rw-r--r--   0 root         (0) root         (0)   253669 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/jquery-ui.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:14.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/
--rw-r--r--   0 root         (0) root         (0)      393 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-r--r--   0 root         (0) root         (0)      265 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0 root         (0) root         (0)      323 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
--rw-r--r--   0 root         (0) root         (0)      324 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0 root         (0) root         (0)      390 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0 root         (0) root         (0)      325 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0 root         (0) root         (0)     7025 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-icons_222222_256x240.png
--rw-r--r--   0 root         (0) root         (0)     4676 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0 root         (0) root         (0)     7090 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-icons_454545_256x240.png
--rw-r--r--   0 root         (0) root         (0)     7111 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-icons_888888_256x240.png
--rw-r--r--   0 root         (0) root         (0)     4676 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0 root         (0) root         (0)    36536 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/jquery-ui.css
--rw-r--r--   0 root         (0) root         (0)    31286 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/jquery-ui.min.css
--rw-r--r--   0 root         (0) root         (0)    17882 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/theme.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui-touch-punch/
--rw-r--r--   0 root         (0) root         (0)     5074 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui-touch-punch/jquery.ui.touch-punch.js
--rw-r--r--   0 root         (0) root         (0)     1291 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui-touch-punch/jquery.ui.touch-punch.min.js
--rw-r--r--   0 root         (0) root         (0)     1127 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/spin.js
--rw-r--r--   0 root         (0) root         (0)      102 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/test.js
--rw-r--r--   0 root         (0) root         (0)     1282 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/zoom.js
--rw-r--r--   0 root         (0) root         (0)       78 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/alerts.py
--rw-r--r--   0 root         (0) root         (0)    23768 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/apps.py
--rw-r--r--   0 root         (0) root         (0)       52 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/audit.py
--rw-r--r--   0 root         (0) root         (0)      604 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/auditing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/auth/
--rw-r--r--   0 root         (0) root         (0)     1969 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9822 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/background.py
--rw-r--r--   0 root         (0) root         (0)     8524 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/browse.py
--rw-r--r--   0 root         (0) root         (0)     3169 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/buckets.py
--rw-r--r--   0 root         (0) root         (0)     3088 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/cache.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/cli/
--rw-r--r--   0 root         (0) root         (0)      154 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1273 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/cli/assign.py
--rw-r--r--   0 root         (0) root         (0)     8058 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/cli/common.py
--rw-r--r--   0 root         (0) root         (0)    12144 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/cli/database.py
--rw-r--r--   0 root         (0) root         (0)     4661 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/cli/describe.py
--rw-r--r--   0 root         (0) root         (0)     3154 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/cli/init.py
--rw-r--r--   0 root         (0) root         (0)     2759 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/cli/main.py
--rw-r--r--   0 root         (0) root         (0)     3082 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/cli/new.py
--rw-r--r--   0 root         (0) root         (0)     2670 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/cli/run.py
--rw-r--r--   0 root         (0) root         (0)     2273 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/cli/serve.py
--rw-r--r--   0 root         (0) root         (0)      885 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/cli/setups.py
--rw-r--r--   0 root         (0) root         (0)     7382 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/cli/utils.py
--rw-r--r--   0 root         (0) root         (0)    29613 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/collect.py
--rw-r--r--   0 root         (0) root         (0)    11582 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/component.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/components/
--rw-r--r--   0 root         (0) root         (0)     5492 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/components/apps/
--rw-r--r--   0 root         (0) root         (0)      215 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/components/apps/__init__.py
--rw-r--r--   0 root         (0) root         (0)      257 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/components/apps/app_menu_item.html
--rw-r--r--   0 root         (0) root         (0)    10132 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/components/flags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/components/instances/
--rw-r--r--   0 root         (0) root         (0)      550 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/components/instances/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/components/instances/instance.css
--rw-r--r--   0 root         (0) root         (0)     1031 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/components/instances/instance.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/components/views/
--rw-r--r--   0 root         (0) root         (0)      243 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/components/views/header_bar.html
--rw-r--r--   0 root         (0) root         (0)     4458 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/config.py
--rw-r--r--   0 root         (0) root         (0)      160 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/context.py
--rw-r--r--   0 root         (0) root         (0)     3077 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/cookies.py
--rw-r--r--   0 root         (0) root         (0)    23822 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/database.py
--rw-r--r--   0 root         (0) root         (0)      729 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    97261 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/fields.py
--rw-r--r--   0 root         (0) root         (0)     4540 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/fill.py
--rw-r--r--   0 root         (0) root         (0)     5048 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/forms.py
--rw-r--r--   0 root         (0) root         (0)    10144 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/helpers.py
--rw-r--r--   0 root         (0) root         (0)     5226 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/html.py
--rw-r--r--   0 root         (0) root         (0)     1784 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/impersonation.py
--rw-r--r--   0 root         (0) root         (0)     4907 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/instances.py
--rw-r--r--   0 root         (0) root         (0)     1837 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/jsonz.py
--rw-r--r--   0 root         (0) root         (0)     2209 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/logging.py
--rw-r--r--   0 root         (0) root         (0)    13828 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/mail.py
--rw-r--r--   0 root         (0) root         (0)    23554 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/middleware.py
--rw-r--r--   0 root         (0) root         (0)    12261 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/migrations.py
--rw-r--r--   0 root         (0) root         (0)    19267 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/models.py
--rw-r--r--   0 root         (0) root         (0)    11265 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/mvc.py
--rw-r--r--   0 root         (0) root         (0)     7386 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/packages.py
--rw-r--r--   0 root         (0) root         (0)     6105 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/page.py
--rw-r--r--   0 root         (0) root         (0)     5233 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/profiler.py
--rw-r--r--   0 root         (0) root         (0)    17875 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/queues.py
--rw-r--r--   0 root         (0) root         (0)    26462 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/records.py
--rw-r--r--   0 root         (0) root         (0)     3807 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/render.py
--rw-r--r--   0 root         (0) root         (0)    10560 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/request.py
--rw-r--r--   0 root         (0) root         (0)    15023 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/response.py
--rw-r--r--   0 root         (0) root         (0)     4624 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/server.py
--rw-r--r--   0 root         (0) root         (0)     1088 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/services.py
--rw-r--r--   0 root         (0) root         (0)     6231 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/session.py
--rw-r--r--   0 root         (0) root         (0)     4338 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/settings.py
--rw-r--r--   0 root         (0) root         (0)    13207 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/site.py
--rw-r--r--   0 root         (0) root         (0)     3079 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/sites.py
--rw-r--r--   0 root         (0) root         (0)     1453 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/snippets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/sql/
--rw-r--r--   0 root         (0) root         (0)      343 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/sql/create_test_tables_sqlite3.sql
--rw-r--r--   0 root         (0) root         (0)      130 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/sql/create_testuser.sql
--rw-r--r--   0 root         (0) root         (0)       89 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/sql/create_zoomuser.sql
--rw-r--r--   0 root         (0) root         (0)      312 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/sql/get_recent_users.sql
--rw-r--r--   0 root         (0) root         (0)      133 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/sql/last_seen_patch_mysql.sql
--rw-r--r--   0 root         (0) root         (0)     6417 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/sql/setup_mysql.sql
--rw-r--r--   0 root         (0) root         (0)     5950 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/sql/setup_sqlite3g.sql
--rw-r--r--   0 root         (0) root         (0)     7979 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/sqltools.py
--rw-r--r--   0 root         (0) root         (0)    28070 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/store.py
--rw-r--r--   0 root         (0) root         (0)     1987 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/templates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/testing/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/testing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9619 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/testing/apptest.py
--rw-r--r--   0 root         (0) root         (0)      269 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/testing/common.py
--rw-r--r--   0 root         (0) root         (0)    10792 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/testing/webtest.py
--rw-r--r--   0 root         (0) root         (0)    19401 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/tools.py
--rw-r--r--   0 root         (0) root         (0)    20739 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/users.py
--rw-r--r--   0 root         (0) root         (0)    27946 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/utils.py
--rw-r--r--   0 root         (0) root         (0)    13271 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/views/
--rw-r--r--   0 root         (0) root         (0)      120 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/views/clear_search.html
--rw-r--r--   0 root         (0) root         (0)      112 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/views/field.html
--rw-r--r--   0 root         (0) root         (0)      425 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/views/google_tracker.html
--rw-r--r--   0 root         (0) root         (0)      159 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/views/hint.html
--rw-r--r--   0 root         (0) root         (0)      403 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/views/page_header.html
--rw-r--r--   0 root         (0) root         (0)      331 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/views/search_box.html
--rw-r--r--   0 root         (0) root         (0)      579 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/views/system_pulldown_menu.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/widgets/cards/
--rw-r--r--   0 root         (0) root         (0)      799 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/widgets/cards/__init__.py
--rw-r--r--   0 root         (0) root         (0)      618 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/widgets/cards/card.sass
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/widgets/charts/
--rw-r--r--   0 root         (0) root         (0)     1774 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/widgets/charts/__init__.py
--rw-r--r--   0 root         (0) root         (0)      401 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/widgets/charts/chart_widget.css
--rw-r--r--   0 root         (0) root         (0)      269 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/widgets/charts/chart_widget.html
--rw-r--r--   0 root         (0) root         (0)     1583 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/widgets/charts/chart_widget.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/widgets/metrics/
--rw-r--r--   0 root         (0) root         (0)     1641 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/widgets/metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)      405 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/widgets/metrics/metric_widget.css
--rw-r--r--   0 root         (0) root         (0)      277 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/widgets/metrics/metric_widget.html
--rw-r--r--   0 root         (0) root         (0)     1523 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/widgets/metrics/metric_widget.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-25 05:43:15.000000 ZoomFoundry-6.7.5/zoom/widgets/progress/
--rw-r--r--   0 root         (0) root         (0)      638 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/widgets/progress/__init__.py
--rw-r--r--   0 root         (0) root         (0)      276 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/widgets/progress/progress_widget.pug
--rw-r--r--   0 root         (0) root         (0)      822 2020-09-25 05:43:12.000000 ZoomFoundry-6.7.5/zoom/widgets/progress/progress_widget.sass
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:38.000000 ZoomFoundry-6.9.1/
+-rw-r--r--   0 root         (0) root         (0)     2968 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1522 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      223 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9361 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6781 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/ZoomFoundry.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9361 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/ZoomFoundry.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18569 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/ZoomFoundry.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/ZoomFoundry.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/ZoomFoundry.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/ZoomFoundry.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/ZoomFoundry.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      231 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2020-10-07 21:07:38.000000 ZoomFoundry-6.9.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1880 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/
+-rw-r--r--   0 root         (0) root         (0)     1020 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1196 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/__main__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/apps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/apps/basic/
+-rw-r--r--   0 root         (0) root         (0)      123 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/apps/basic/app.py
+-rw-r--r--   0 root         (0) root         (0)       60 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/apps/basic/config.ini
+-rw-r--r--   0 root         (0) root         (0)      564 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/apps/basic/index.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/instances/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/instances/basic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/instances/basic/apps/
+-rw-r--r--   0 root         (0) root         (0)       69 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/instances/basic/apps/default.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/instances/basic/sites/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/instances/basic/sites/localhost/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/instances/basic/sites/localhost/.gitinclude
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/instances/basic/themes/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/instances/basic/themes/.gitinclude
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/sites/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/sites/basic/
+-rw-r--r--   0 root         (0) root         (0)     3944 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/sites/basic/site.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/
+-rw-r--r--   0 root         (0) root         (0)       73 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/README.md
+-rw-r--r--   0 root         (0) root         (0)      131 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/content.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/css/
+-rw-r--r--   0 root         (0) root         (0)      653 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/css/buttons.css
+-rw-r--r--   0 root         (0) root         (0)      357 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/css/components.css
+-rw-r--r--   0 root         (0) root         (0)      649 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/css/containers.css
+-rw-r--r--   0 root         (0) root         (0)     1552 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/css/content.css
+-rw-r--r--   0 root         (0) root         (0)      840 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/css/flags.css
+-rw-r--r--   0 root         (0) root         (0)      576 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/css/guide.css
+-rw-r--r--   0 root         (0) root         (0)     3846 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/css/navigation.css
+-rw-r--r--   0 root         (0) root         (0)      540 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/css/pricebox.css
+-rw-r--r--   0 root         (0) root         (0)       91 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/css/print.css
+-rw-r--r--   0 root         (0) root         (0)     2299 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/css/social.css
+-rw-r--r--   0 root         (0) root         (0)       43 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/css/style.css
+-rw-r--r--   0 root         (0) root         (0)     9538 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/css/widget.css
+-rw-r--r--   0 root         (0) root         (0)      131 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/default.html
+-rw-r--r--   0 root         (0) root         (0)      131 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/templates/
+-rw-r--r--   0 root         (0) root         (0)     2039 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/templates/body.html
+-rw-r--r--   0 root         (0) root         (0)      705 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/templates/head.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/
+-rw-r--r--   0 root         (0) root         (0)      263 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/about.md
+-rw-r--r--   0 root         (0) root         (0)      251 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/app.py
+-rw-r--r--   0 root         (0) root         (0)     1420 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/apps.py
+-rw-r--r--   0 root         (0) root         (0)       33 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/config.ini
+-rw-r--r--   0 root         (0) root         (0)     1302 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/database.py
+-rw-r--r--   0 root         (0) root         (0)      109 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/fields.py
+-rw-r--r--   0 root         (0) root         (0)     7280 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/groups.py
+-rw-r--r--   0 root         (0) root         (0)    16101 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/index.py
+-rw-r--r--   0 root         (0) root         (0)     2082 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/jobs.py
+-rw-r--r--   0 root         (0) root         (0)     2709 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/mail.py
+-rw-r--r--   0 root         (0) root         (0)     8930 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/model.py
+-rw-r--r--   0 root         (0) root         (0)      331 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/reset.md
+-rw-r--r--   0 root         (0) root         (0)      183 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/test_format.py
+-rw-r--r--   0 root         (0) root         (0)     7499 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/users.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/views/
+-rw-r--r--   0 root         (0) root         (0)      247 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/views/index_page_layout_view.css
+-rw-r--r--   0 root         (0) root         (0)      276 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/views/index_page_layout_view.html
+-rw-r--r--   0 root         (0) root         (0)      571 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/views/metric_view.css
+-rw-r--r--   0 root         (0) root         (0)      199 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/views/metric_view.html
+-rw-r--r--   0 root         (0) root         (0)       29 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/views/metric_view.name.html
+-rw-r--r--   0 root         (0) root         (0)       94 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/views/metric_view.red.css
+-rw-r--r--   0 root         (0) root         (0)       77 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/views/metrics_view.html
+-rw-r--r--   0 root         (0) root         (0)      485 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/views/panel_view.css
+-rw-r--r--   0 root         (0) root         (0)      155 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/views/panel_view.html
+-rw-r--r--   0 root         (0) root         (0)      107 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/views/panel_view.js
+-rw-r--r--   0 root         (0) root         (0)       55 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/views/test_view.html
+-rw-r--r--   0 root         (0) root         (0)     1416 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/views.py
+-rw-r--r--   0 root         (0) root         (0)      440 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/welcome.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/api/
+-rw-r--r--   0 root         (0) root         (0)       68 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/api/app.py
+-rw-r--r--   0 root         (0) root         (0)       41 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/api/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/
+-rw-r--r--   0 root         (0) root         (0)     2435 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/app.py
+-rw-r--r--   0 root         (0) root         (0)       27 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/config.ini
+-rw-r--r--   0 root         (0) root         (0)       56 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/contact.md
+-rw-r--r--   0 root         (0) root         (0)     8541 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/files.py
+-rw-r--r--   0 root         (0) root         (0)     6102 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/images.py
+-rw-r--r--   0 root         (0) root         (0)      119 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/index.md
+-rw-r--r--   0 root         (0) root         (0)     1997 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/index.py
+-rw-r--r--   0 root         (0) root         (0)     3185 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/pages.py
+-rw-r--r--   0 root         (0) root         (0)      434 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/snippets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/static/
+-rw-r--r--   0 root         (0) root         (0)     1827 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/static/file-manager.css
+-rw-r--r--   0 root         (0) root         (0)     5322 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/static/file-manager.js
+-rw-r--r--   0 root         (0) root         (0)     1642 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/static/markdown-linker.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/views/
+-rw-r--r--   0 root         (0) root         (0)      828 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/views/file-manager.html
+-rw-r--r--   0 root         (0) root         (0)      971 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/views/images.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/forgot/
+-rw-r--r--   0 root         (0) root         (0)      494 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/forgot/activate.md
+-rw-r--r--   0 root         (0) root         (0)       72 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/forgot/app.py
+-rw-r--r--   0 root         (0) root         (0)      171 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/forgot/complete.md
+-rw-r--r--   0 root         (0) root         (0)       20 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/forgot/config.ini
+-rw-r--r--   0 root         (0) root         (0)      365 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/forgot/expired.md
+-rw-r--r--   0 root         (0) root         (0)      199 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/forgot/index.md
+-rw-r--r--   0 root         (0) root         (0)     2345 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/forgot/index.py
+-rw-r--r--   0 root         (0) root         (0)     3370 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/forgot/model.py
+-rw-r--r--   0 root         (0) root         (0)      228 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/forgot/reset.md
+-rw-r--r--   0 root         (0) root         (0)      239 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/forgot/step2.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/hello/
+-rw-r--r--   0 root         (0) root         (0)      532 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/hello/app.py
+-rw-r--r--   0 root         (0) root         (0)       25 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/hello/background.py
+-rw-r--r--   0 root         (0) root         (0)      239 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/hello/packages.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/home/
+-rw-r--r--   0 root         (0) root         (0)     1612 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/home/app.py
+-rw-r--r--   0 root         (0) root         (0)       42 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/home/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/icons/
+-rw-r--r--   0 root         (0) root         (0)       84 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/icons/app.py
+-rw-r--r--   0 root         (0) root         (0)       59 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/icons/config.ini
+-rw-r--r--   0 root         (0) root         (0)   213349 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/icons/icons.html
+-rw-r--r--   0 root         (0) root         (0)      638 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/icons/index.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/login/
+-rw-r--r--   0 root         (0) root         (0)       53 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/login/app.py
+-rw-r--r--   0 root         (0) root         (0)       40 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/login/config.ini
+-rw-r--r--   0 root         (0) root         (0)     3093 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/login/index.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/login/views/
+-rw-r--r--   0 root         (0) root         (0)       36 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/login/views/forgot_password.css
+-rw-r--r--   0 root         (0) root         (0)       80 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/login/views/forgot_password.pug
+-rw-r--r--   0 root         (0) root         (0)       94 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/login/views/login_form.css
+-rw-r--r--   0 root         (0) root         (0)     1043 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/login/views/login_form.html
+-rw-r--r--   0 root         (0) root         (0)      105 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/login/views/remember_me.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/logout/
+-rw-r--r--   0 root         (0) root         (0)      821 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/logout/app.py
+-rw-r--r--   0 root         (0) root         (0)       40 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/logout/config.ini
+-rw-r--r--   0 root         (0) root         (0)      101 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/packages.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/ping/
+-rw-r--r--   0 root         (0) root         (0)       81 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/ping/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/register/
+-rw-r--r--   0 root         (0) root         (0)      255 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/register/activate.html
+-rw-r--r--   0 root         (0) root         (0)      264 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/register/already_registered.md
+-rw-r--r--   0 root         (0) root         (0)       53 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/register/app.py
+-rw-r--r--   0 root         (0) root         (0)      307 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/register/expired.md
+-rw-r--r--   0 root         (0) root         (0)     2640 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/register/index.py
+-rw-r--r--   0 root         (0) root         (0)     7014 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/register/model.py
+-rw-r--r--   0 root         (0) root         (0)      306 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/register/name_taken.md
+-rw-r--r--   0 root         (0) root         (0)      268 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/register/register_complete.md
+-rw-r--r--   0 root         (0) root         (0)      997 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/register/registration.html
+-rw-r--r--   0 root         (0) root         (0)      319 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/register/step2.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/
+-rw-r--r--   0 root         (0) root         (0)      217 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/about.md
+-rw-r--r--   0 root         (0) root         (0)     1628 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/alerts.py
+-rw-r--r--   0 root         (0) root         (0)      293 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/app.py
+-rw-r--r--   0 root         (0) root         (0)     1212 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/background.py
+-rw-r--r--   0 root         (0) root         (0)      648 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/collection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/components/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/components/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/components/widgets_layout/
+-rw-r--r--   0 root         (0) root         (0)      122 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/components/widgets_layout/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       44 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/components/widgets_layout/widgets_layout.pug
+-rw-r--r--   0 root         (0) root         (0)      124 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/components/widgets_layout/widgets_layout.sass
+-rw-r--r--   0 root         (0) root         (0)     1128 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/components.py
+-rw-r--r--   0 root         (0) root         (0)       75 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/config.ini
+-rw-r--r--   0 root         (0) root         (0)     6886 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/fields.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/flags.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/index.py
+-rw-r--r--   0 root         (0) root         (0)       71 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/model.py
+-rw-r--r--   0 root         (0) root         (0)     2459 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/parts.py
+-rw-r--r--   0 root         (0) root         (0)     1156 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/responses.py
+-rw-r--r--   0 root         (0) root         (0)     4682 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/sample.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/static/
+-rw-r--r--   0 root         (0) root         (0)       37 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/static/test.css
+-rw-r--r--   0 root         (0) root         (0)       21 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/static/test.js
+-rw-r--r--   0 root         (0) root         (0)       24 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/static/test.json
+-rw-r--r--   0 root         (0) root         (0)      792 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/widgets/
+-rw-r--r--   0 root         (0) root         (0)     2070 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       32 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/widgets/cards.pug
+-rw-r--r--   0 root         (0) root         (0)      243 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/widgets/cards.sass
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/settings/
+-rw-r--r--   0 root         (0) root         (0)      164 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/settings/about.md
+-rw-r--r--   0 root         (0) root         (0)       88 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/settings/app.py
+-rw-r--r--   0 root         (0) root         (0)       36 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/settings/config.ini
+-rw-r--r--   0 root         (0) root         (0)     3898 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/settings/index.py
+-rw-r--r--   0 root         (0) root         (0)     2521 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/settings/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/storage/
+-rw-r--r--   0 root         (0) root         (0)      203 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/storage/about.md
+-rw-r--r--   0 root         (0) root         (0)       91 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/storage/app.py
+-rw-r--r--   0 root         (0) root         (0)       76 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/storage/config.ini
+-rw-r--r--   0 root         (0) root         (0)     4077 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/standard_apps/storage/index.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/sites/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/sites/default/
+-rw-r--r--   0 root         (0) root         (0)     3760 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/sites/default/site.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/sites/localhost/
+-rw-r--r--   0 root         (0) root         (0)       95 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/sites/localhost/site.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/
+-rw-r--r--   0 root         (0) root         (0)      356 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/_partials/
+-rw-r--r--   0 root         (0) root         (0)      228 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/_partials/footer.pug
+-rw-r--r--   0 root         (0) root         (0)      516 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/_partials/head.pug
+-rw-r--r--   0 root         (0) root         (0)       76 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/_partials/layout.pug
+-rw-r--r--   0 root         (0) root         (0)      502 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/_partials/nav.pug
+-rw-r--r--   0 root         (0) root         (0)      186 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/_partials/tail.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/
+-rw-r--r--   0 root         (0) root         (0)      761 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/buttons.css
+-rw-r--r--   0 root         (0) root         (0)      249 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/buttons.css.map
+-rw-r--r--   0 root         (0) root         (0)      234 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/components.css
+-rw-r--r--   0 root         (0) root         (0)      165 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/components.css.map
+-rw-r--r--   0 root         (0) root         (0)       45 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/containers.css
+-rw-r--r--   0 root         (0) root         (0)       91 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/containers.css.map
+-rw-r--r--   0 root         (0) root         (0)     1981 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/content.css
+-rw-r--r--   0 root         (0) root         (0)      629 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/content.css.map
+-rw-r--r--   0 root         (0) root         (0)     1000 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/flags.css
+-rw-r--r--   0 root         (0) root         (0)      259 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/flags.css.map
+-rw-r--r--   0 root         (0) root         (0)     4745 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/navigation.css
+-rw-r--r--   0 root         (0) root         (0)     1276 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/navigation.css.map
+-rw-r--r--   0 root         (0) root         (0)      233 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/print.css
+-rw-r--r--   0 root         (0) root         (0)      141 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/print.css.map
+-rw-r--r--   0 root         (0) root         (0)     2680 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/social.css
+-rw-r--r--   0 root         (0) root         (0)      560 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/social.css.map
+-rw-r--r--   0 root         (0) root         (0)      911 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/style.css
+-rw-r--r--   0 root         (0) root         (0)      428 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/style.css.map
+-rw-r--r--   0 root         (0) root         (0)    11649 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/widget.css
+-rw-r--r--   0 root         (0) root         (0)     2689 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/widget.css.map
+-rw-r--r--   0 root         (0) root         (0)      223 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/default.pug
+-rw-r--r--   0 root         (0) root         (0)      241 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/email_template.pug
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/images/
+-rw-r--r--   0 root         (0) root         (0)    10713 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/images/android-chrome-192x192.png
+-rw-r--r--   0 root         (0) root         (0)    25739 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/images/android-chrome-512x512.png
+-rw-r--r--   0 root         (0) root         (0)     9614 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/images/apple-touch-icon.png
+-rw-r--r--   0 root         (0) root         (0)     9614 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/images/banner-logo.png
+-rw-r--r--   0 root         (0) root         (0)     9614 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/images/email-logo.png
+-rw-r--r--   0 root         (0) root         (0)      769 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/images/favicon-16x16.png
+-rw-r--r--   0 root         (0) root         (0)     1548 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/images/favicon-32x32.png
+-rw-r--r--   0 root         (0) root         (0)    15406 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/images/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/src/sass/
+-rw-r--r--   0 root         (0) root         (0)      636 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/src/sass/buttons.sass
+-rw-r--r--   0 root         (0) root         (0)      160 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/src/sass/components.sass
+-rw-r--r--   0 root         (0) root         (0)        0 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/src/sass/containers.sass
+-rw-r--r--   0 root         (0) root         (0)     1720 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/src/sass/content.sass
+-rw-r--r--   0 root         (0) root         (0)      904 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/src/sass/flags.sass
+-rw-r--r--   0 root         (0) root         (0)     4541 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/src/sass/navigation.sass
+-rw-r--r--   0 root         (0) root         (0)      175 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/src/sass/print.sass
+-rw-r--r--   0 root         (0) root         (0)     2061 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/src/sass/social.sass
+-rw-r--r--   0 root         (0) root         (0)      879 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/src/sass/style.sass
+-rw-r--r--   0 root         (0) root         (0)    10940 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/src/sass/widget.sass
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/
+-rw-r--r--   0 root         (0) root         (0)       49 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/index.wsgi
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/
+-rw-r--r--   0 root         (0) root         (0)     1131 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/bootstrap4.5/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/bootstrap4.5/css/
+-rw-r--r--   0 root         (0) root         (0)   160403 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/bootstrap4.5/css/bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   646432 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/bootstrap4.5/css/bootstrap.min.css.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/bootstrap4.5/js/
+-rw-r--r--   0 root         (0) root         (0)    81084 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/bootstrap4.5/js/bootstrap.bundle.min.js
+-rw-r--r--   0 root         (0) root         (0)   315300 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/bootstrap4.5/js/bootstrap.bundle.min.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/css/
+-rw-r--r--   0 root         (0) root         (0)    26132 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap-theme.css
+-rw-r--r--   0 root         (0) root         (0)    47706 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap-theme.css.map
+-rw-r--r--   0 root         (0) root         (0)    23409 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap-theme.min.css
+-rw-r--r--   0 root         (0) root         (0)    25648 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap-theme.min.css.map
+-rw-r--r--   0 root         (0) root         (0)   146010 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap.css
+-rw-r--r--   0 root         (0) root         (0)   389287 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0 root         (0) root         (0)   121200 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)   542194 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap.min.css.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/fonts/
+-rw-r--r--   0 root         (0) root         (0)    20127 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 root         (0) root         (0)   108738 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 root         (0) root         (0)    45404 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 root         (0) root         (0)    23424 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 root         (0) root         (0)    18028 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/js/
+-rw-r--r--   0 root         (0) root         (0)    69707 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/js/bootstrap.js
+-rw-r--r--   0 root         (0) root         (0)    37045 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0 root         (0) root         (0)      484 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/js/npm.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/chosen/
+-rw-r--r--   0 root         (0) root         (0)     1215 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/chosen/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      538 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/chosen/chosen-sprite.png
+-rw-r--r--   0 root         (0) root         (0)      738 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/chosen/chosen-sprite@2x.png
+-rw-r--r--   0 root         (0) root         (0)    29121 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/chosen/chosen.jquery.min.js
+-rw-r--r--   0 root         (0) root         (0)    10220 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/chosen/chosen.min.css
+-rw-r--r--   0 root         (0) root         (0)      240 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/cookieconsent.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/dropzone/
+-rw-r--r--   0 root         (0) root         (0)     1150 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/dropzone/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      751 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/dropzone/basic.min.css
+-rw-r--r--   0 root         (0) root         (0)    33689 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/dropzone/dropzone-amd-module.min.js
+-rw-r--r--   0 root         (0) root         (0)     9717 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/dropzone/dropzone.min.css
+-rw-r--r--   0 root         (0) root         (0)    33588 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/dropzone/dropzone.min.js
+-rw-r--r--   0 root         (0) root         (0)       70 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/dropzone.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/fontawesome4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/fontawesome4/css/
+-rw-r--r--   0 root         (0) root         (0)    37414 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/fontawesome4/css/font-awesome.css
+-rw-r--r--   0 root         (0) root         (0)    31000 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/fontawesome4/css/font-awesome.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/fontawesome4/fonts/
+-rw-r--r--   0 root         (0) root         (0)   165742 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/fontawesome4/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 root         (0) root         (0)   444379 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/fontawesome4/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 root         (0) root         (0)   165548 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/fontawesome4/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 root         (0) root         (0)    98024 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/fontawesome4/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 root         (0) root         (0)    77160 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/fontawesome4/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 root         (0) root         (0)      202 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/fouc.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/
+-rw-r--r--   0 root         (0) root         (0)     1987 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/checkmark.png
+-rw-r--r--   0 root         (0) root         (0)      251 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/delete.png
+-rw-r--r--   0 root         (0) root         (0)      276 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/down_arrow_blue.png
+-rw-r--r--   0 root         (0) root         (0)     1133 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/down_arrow_red.png
+-rw-r--r--   0 root         (0) root         (0)     6006 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)      699 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/follow-off.png
+-rw-r--r--   0 root         (0) root         (0)      655 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/follow-on.png
+-rw-r--r--   0 root         (0) root         (0)      381 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/heart-off.png
+-rw-r--r--   0 root         (0) root         (0)      333 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/heart-on.png
+-rw-r--r--   0 root         (0) root         (0)      360 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/mail-off.png
+-rw-r--r--   0 root         (0) root         (0)      286 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/mail-on.png
+-rw-r--r--   0 root         (0) root         (0)     9546 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/no_image.png
+-rw-r--r--   0 root         (0) root         (0)     3350 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/no_photo.png
+-rw-r--r--   0 root         (0) root         (0)    10829 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/progress.gif
+-rw-r--r--   0 root         (0) root         (0)      251 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/remove.png
+-rw-r--r--   0 root         (0) root         (0)      400 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/remove_filter.png
+-rw-r--r--   0 root         (0) root         (0)      398 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/remove_filter_hover.png
+-rw-r--r--   0 root         (0) root         (0)     2098 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/secure.png
+-rw-r--r--   0 root         (0) root         (0)     1067 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/settings.png
+-rw-r--r--   0 root         (0) root         (0)     1297 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/settings2.png
+-rw-r--r--   0 root         (0) root         (0)     8544 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/social-icons-small.png
+-rw-r--r--   0 root         (0) root         (0)    10440 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/social-icons.png
+-rw-r--r--   0 root         (0) root         (0)       42 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/spacer.gif
+-rw-r--r--   0 root         (0) root         (0)      625 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/star-off.png
+-rw-r--r--   0 root         (0) root         (0)      872 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/star-on.png
+-rw-r--r--   0 root         (0) root         (0)     3485 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/star_empty.png
+-rw-r--r--   0 root         (0) root         (0)     3459 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/star_full.png
+-rw-r--r--   0 root         (0) root         (0)     3491 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/star_half_full.png
+-rw-r--r--   0 root         (0) root         (0)     1449 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/thumbs-down-off.png
+-rw-r--r--   0 root         (0) root         (0)     1547 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/thumbs-down.png
+-rw-r--r--   0 root         (0) root         (0)     1460 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/thumbs-up-off.png
+-rw-r--r--   0 root         (0) root         (0)     1569 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/thumbs-up.png
+-rw-r--r--   0 root         (0) root         (0)      286 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/trash.png
+-rw-r--r--   0 root         (0) root         (0)      302 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/up_arrow_blue.png
+-rw-r--r--   0 root         (0) root         (0)     5344 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images-field.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery/
+-rw-r--r--   0 root         (0) root         (0)    86596 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery/jquery.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/
+-rw-r--r--   0 root         (0) root         (0)   253669 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/jquery-ui.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/
+-rw-r--r--   0 root         (0) root         (0)      393 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-r--r--   0 root         (0) root         (0)      265 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0 root         (0) root         (0)      323 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
+-rw-r--r--   0 root         (0) root         (0)      324 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0 root         (0) root         (0)      390 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0 root         (0) root         (0)      325 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0 root         (0) root         (0)     7025 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-icons_222222_256x240.png
+-rw-r--r--   0 root         (0) root         (0)     4676 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-icons_2e83ff_256x240.png
+-rw-r--r--   0 root         (0) root         (0)     7090 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-icons_454545_256x240.png
+-rw-r--r--   0 root         (0) root         (0)     7111 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-icons_888888_256x240.png
+-rw-r--r--   0 root         (0) root         (0)     4676 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0 root         (0) root         (0)    36536 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/jquery-ui.css
+-rw-r--r--   0 root         (0) root         (0)    31286 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/jquery-ui.min.css
+-rw-r--r--   0 root         (0) root         (0)    17882 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/theme.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui-touch-punch/
+-rw-r--r--   0 root         (0) root         (0)     5074 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui-touch-punch/jquery.ui.touch-punch.js
+-rw-r--r--   0 root         (0) root         (0)     1291 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui-touch-punch/jquery.ui.touch-punch.min.js
+-rw-r--r--   0 root         (0) root         (0)     1127 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/spin.js
+-rw-r--r--   0 root         (0) root         (0)      102 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/test.js
+-rw-r--r--   0 root         (0) root         (0)     1282 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/zoom.js
+-rw-r--r--   0 root         (0) root         (0)       78 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/alerts.py
+-rw-r--r--   0 root         (0) root         (0)    23768 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/apps.py
+-rw-r--r--   0 root         (0) root         (0)       52 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/audit.py
+-rw-r--r--   0 root         (0) root         (0)      604 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/auditing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/auth/
+-rw-r--r--   0 root         (0) root         (0)     1982 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9822 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/background.py
+-rw-r--r--   0 root         (0) root         (0)     8524 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/browse.py
+-rw-r--r--   0 root         (0) root         (0)     3169 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/buckets.py
+-rw-r--r--   0 root         (0) root         (0)     3088 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/cache.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/cli/
+-rw-r--r--   0 root         (0) root         (0)      154 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/cli/assign.py
+-rw-r--r--   0 root         (0) root         (0)     8058 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/cli/common.py
+-rw-r--r--   0 root         (0) root         (0)    12144 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/cli/database.py
+-rw-r--r--   0 root         (0) root         (0)     4661 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/cli/describe.py
+-rw-r--r--   0 root         (0) root         (0)     3154 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/cli/init.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/cli/main.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/cli/new.py
+-rw-r--r--   0 root         (0) root         (0)     2670 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/cli/run.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/cli/serve.py
+-rw-r--r--   0 root         (0) root         (0)      885 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/cli/setups.py
+-rw-r--r--   0 root         (0) root         (0)     7382 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/cli/utils.py
+-rw-r--r--   0 root         (0) root         (0)    29613 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/collect.py
+-rw-r--r--   0 root         (0) root         (0)    11582 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/component.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/components/
+-rw-r--r--   0 root         (0) root         (0)     5492 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/components/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/components/apps/
+-rw-r--r--   0 root         (0) root         (0)      215 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/components/apps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      257 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/components/apps/app_menu_item.html
+-rw-r--r--   0 root         (0) root         (0)    10132 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/components/flags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/components/instances/
+-rw-r--r--   0 root         (0) root         (0)      550 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/components/instances/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/components/instances/instance.css
+-rw-r--r--   0 root         (0) root         (0)     1031 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/components/instances/instance.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/components/views/
+-rw-r--r--   0 root         (0) root         (0)      243 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/components/views/header_bar.html
+-rw-r--r--   0 root         (0) root         (0)     4458 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/config.py
+-rw-r--r--   0 root         (0) root         (0)      160 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/context.py
+-rw-r--r--   0 root         (0) root         (0)     3077 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/cookies.py
+-rw-r--r--   0 root         (0) root         (0)    23822 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/database.py
+-rw-r--r--   0 root         (0) root         (0)      729 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    97396 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/fields.py
+-rw-r--r--   0 root         (0) root         (0)     4540 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/fill.py
+-rw-r--r--   0 root         (0) root         (0)     5048 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/forms.py
+-rw-r--r--   0 root         (0) root         (0)    10144 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     5226 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/html.py
+-rw-r--r--   0 root         (0) root         (0)     1784 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/impersonation.py
+-rw-r--r--   0 root         (0) root         (0)     4907 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/instances.py
+-rw-r--r--   0 root         (0) root         (0)     1837 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/jsonz.py
+-rw-r--r--   0 root         (0) root         (0)     2209 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/logging.py
+-rw-r--r--   0 root         (0) root         (0)    13546 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/mail.py
+-rw-r--r--   0 root         (0) root         (0)    23554 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/middleware.py
+-rw-r--r--   0 root         (0) root         (0)    12261 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/migrations.py
+-rw-r--r--   0 root         (0) root         (0)    19267 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/models.py
+-rw-r--r--   0 root         (0) root         (0)    11265 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/mvc.py
+-rw-r--r--   0 root         (0) root         (0)     7386 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/packages.py
+-rw-r--r--   0 root         (0) root         (0)     6105 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/page.py
+-rw-r--r--   0 root         (0) root         (0)     5233 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/profiler.py
+-rw-r--r--   0 root         (0) root         (0)    17875 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/queues.py
+-rw-r--r--   0 root         (0) root         (0)    26462 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/records.py
+-rw-r--r--   0 root         (0) root         (0)     3807 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/render.py
+-rw-r--r--   0 root         (0) root         (0)    10560 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/request.py
+-rw-r--r--   0 root         (0) root         (0)    15023 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/response.py
+-rw-r--r--   0 root         (0) root         (0)     4624 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/server.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/services.py
+-rw-r--r--   0 root         (0) root         (0)     6231 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/session.py
+-rw-r--r--   0 root         (0) root         (0)     4338 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/settings.py
+-rw-r--r--   0 root         (0) root         (0)    13207 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/site.py
+-rw-r--r--   0 root         (0) root         (0)     3079 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/sites.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/snippets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/sql/
+-rw-r--r--   0 root         (0) root         (0)      343 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/sql/create_test_tables_sqlite3.sql
+-rw-r--r--   0 root         (0) root         (0)      130 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/sql/create_testuser.sql
+-rw-r--r--   0 root         (0) root         (0)       89 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/sql/create_zoomuser.sql
+-rw-r--r--   0 root         (0) root         (0)      312 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/sql/get_recent_users.sql
+-rw-r--r--   0 root         (0) root         (0)      133 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/sql/last_seen_patch_mysql.sql
+-rw-r--r--   0 root         (0) root         (0)     6417 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/sql/setup_mysql.sql
+-rw-r--r--   0 root         (0) root         (0)     5950 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/sql/setup_sqlite3g.sql
+-rw-r--r--   0 root         (0) root         (0)     7979 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/sqltools.py
+-rw-r--r--   0 root         (0) root         (0)    28070 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/store.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/templates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/testing/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/testing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9619 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/testing/apptest.py
+-rw-r--r--   0 root         (0) root         (0)      269 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/testing/common.py
+-rw-r--r--   0 root         (0) root         (0)    10792 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/testing/webtest.py
+-rw-r--r--   0 root         (0) root         (0)    19396 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/tools.py
+-rw-r--r--   0 root         (0) root         (0)    20739 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/users.py
+-rw-r--r--   0 root         (0) root         (0)    27946 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/utils.py
+-rw-r--r--   0 root         (0) root         (0)    13271 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/views/
+-rw-r--r--   0 root         (0) root         (0)      120 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/views/clear_search.html
+-rw-r--r--   0 root         (0) root         (0)      112 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/views/field.html
+-rw-r--r--   0 root         (0) root         (0)      425 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/views/google_tracker.html
+-rw-r--r--   0 root         (0) root         (0)      159 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/views/hint.html
+-rw-r--r--   0 root         (0) root         (0)      403 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/views/page_header.html
+-rw-r--r--   0 root         (0) root         (0)      331 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/views/search_box.html
+-rw-r--r--   0 root         (0) root         (0)      579 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/views/system_pulldown_menu.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/widgets/cards/
+-rw-r--r--   0 root         (0) root         (0)      799 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/widgets/cards/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      618 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/widgets/cards/card.sass
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/widgets/charts/
+-rw-r--r--   0 root         (0) root         (0)     1774 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/widgets/charts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      401 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/widgets/charts/chart_widget.css
+-rw-r--r--   0 root         (0) root         (0)      269 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/widgets/charts/chart_widget.html
+-rw-r--r--   0 root         (0) root         (0)     1583 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/widgets/charts/chart_widget.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/widgets/metrics/
+-rw-r--r--   0 root         (0) root         (0)     1641 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/widgets/metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      405 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/widgets/metrics/metric_widget.css
+-rw-r--r--   0 root         (0) root         (0)      277 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/widgets/metrics/metric_widget.html
+-rw-r--r--   0 root         (0) root         (0)     1523 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/widgets/metrics/metric_widget.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-07 21:07:37.000000 ZoomFoundry-6.9.1/zoom/widgets/progress/
+-rw-r--r--   0 root         (0) root         (0)      638 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/widgets/progress/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      276 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/widgets/progress/progress_widget.pug
+-rw-r--r--   0 root         (0) root         (0)      822 2020-10-07 21:07:36.000000 ZoomFoundry-6.9.1/zoom/widgets/progress/progress_widget.sass
```

### Comparing `ZoomFoundry-6.7.5/CHANGELOG.md` & `ZoomFoundry-6.9.1/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 ### Added
 
+## [6.9.0] - 2020-10-07
+- add email template support
+- add TimezoneField
+- update bcrypt support to latest
+
 ## [6.8.0] - 2020-08-30
 - add partial response
 - add cards
 - add progress widget
 - add metric widget
 - update chosen package to latest version 1.8.7
```

### Comparing `ZoomFoundry-6.7.5/LICENSE` & `ZoomFoundry-6.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/PKG-INFO` & `ZoomFoundry-6.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZoomFoundry
-Version: 6.7.5
+Version: 6.9.1
 Summary: A dynamic Web Framework that promotes modularity and rapid prototyping
 Home-page: https://github.com/dsilabs/zoom
 Author: DSI Labs
 Author-email: support@dsilabs.ca
 License: UNKNOWN
 Description: # README
```

### Comparing `ZoomFoundry-6.7.5/README.md` & `ZoomFoundry-6.9.1/README.md`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/ZoomFoundry.egg-info/PKG-INFO` & `ZoomFoundry-6.9.1/ZoomFoundry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZoomFoundry
-Version: 6.7.5
+Version: 6.9.1
 Summary: A dynamic Web Framework that promotes modularity and rapid prototyping
 Home-page: https://github.com/dsilabs/zoom
 Author: DSI Labs
 Author-email: support@dsilabs.ca
 License: UNKNOWN
 Description: # README
```

### Comparing `ZoomFoundry-6.7.5/ZoomFoundry.egg-info/SOURCES.txt` & `ZoomFoundry-6.9.1/ZoomFoundry.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -207,14 +207,15 @@
 zoom/_assets/standard_apps/storage/app.py
 zoom/_assets/standard_apps/storage/config.ini
 zoom/_assets/standard_apps/storage/index.py
 zoom/_assets/web/sites/default/site.ini
 zoom/_assets/web/sites/localhost/site.ini
 zoom/_assets/web/themes/default/README.md
 zoom/_assets/web/themes/default/default.pug
+zoom/_assets/web/themes/default/email_template.pug
 zoom/_assets/web/themes/default/_partials/footer.pug
 zoom/_assets/web/themes/default/_partials/head.pug
 zoom/_assets/web/themes/default/_partials/layout.pug
 zoom/_assets/web/themes/default/_partials/nav.pug
 zoom/_assets/web/themes/default/_partials/tail.pug
 zoom/_assets/web/themes/default/css/buttons.css
 zoom/_assets/web/themes/default/css/buttons.css.map
```

### Comparing `ZoomFoundry-6.7.5/setup.py` & `ZoomFoundry-6.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,17 @@
     'markdown>=2.6.1',
     'Pillow>=1.0',
     'faker',
     'docopt',
     'werkzeug',
     'croniter',
     'pypugjs>=5.9.1',
-    'libsass>=0.19.4'
+    'libsass>=0.19.4',
+    'pytz==2020.1',
+    'pytzdata==2019.3'
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 about = {}
 with open(os.path.join(here, 'zoom', '__version__.py'), 'r', encoding='utf-8') as f:
     exec(f.read(), about)
```

### Comparing `ZoomFoundry-6.7.5/zoom/__init__.py` & `ZoomFoundry-6.9.1/zoom/__init__.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/__main__.py` & `ZoomFoundry-6.9.1/zoom/__main__.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/boilerplates/apps/basic/index.py` & `ZoomFoundry-6.9.1/zoom/_assets/boilerplates/apps/basic/index.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/boilerplates/sites/basic/site.ini` & `ZoomFoundry-6.9.1/zoom/_assets/boilerplates/sites/basic/site.ini`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/css/buttons.css` & `ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/css/buttons.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/css/containers.css` & `ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/css/containers.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/css/content.css` & `ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/css/content.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/css/flags.css` & `ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/css/flags.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/css/guide.css` & `ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/css/guide.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/css/navigation.css` & `ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/css/navigation.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/css/pricebox.css` & `ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/css/pricebox.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/css/social.css` & `ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/css/social.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/css/widget.css` & `ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/css/widget.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/templates/body.html` & `ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/templates/body.html`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/boilerplates/themes/basic/templates/head.html` & `ZoomFoundry-6.9.1/zoom/_assets/boilerplates/themes/basic/templates/head.html`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/apps.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/apps.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/database.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/database.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/groups.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/groups.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/index.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/index.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/jobs.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/jobs.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/mail.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/mail.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/model.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/model.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/users.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/users.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/views/metric_view.css` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/views/metric_view.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/admin/views.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/admin/views.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/app.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/app.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/files.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/files.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/images.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/images.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/index.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/index.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/pages.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/pages.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/static/file-manager.css` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/static/file-manager.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/static/file-manager.js` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/static/file-manager.js`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/static/markdown-linker.js` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/static/markdown-linker.js`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/views/file-manager.html` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/views/file-manager.html`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/content/views/images.css` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/content/views/images.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/forgot/index.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/forgot/index.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/forgot/model.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/forgot/model.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/hello/app.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/hello/app.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/home/app.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/home/app.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/icons/icons.html` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/icons/icons.html`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/icons/index.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/icons/index.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/login/index.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/login/index.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/login/views/login_form.html` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/login/views/login_form.html`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/logout/app.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/logout/app.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/register/index.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/register/index.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/register/model.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/register/model.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/register/registration.html` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/register/registration.html`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/alerts.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/alerts.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/background.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/background.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/collection.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/collection.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/components.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/components.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/fields.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     MoneyField('Amount', hint='test hint'),
     MoneyField('Placeholder', placeholder=100, hint='test hint'),
     MoneyField('Foreign Amount', symbol='£', hint='test hint'),
     DateField('Date', hint='test hint'),
     DateField('Min Max Date', min=date1, max=date2, hint='test hint'),
     DateField('Formatted Date', format='%Y-%m-%d (%A)', hint='test hint'),
     BirthdateField('Birth Date', hint='test hint'),
+    TimezoneField('Timezone'),
     CheckboxesField(
         'Select', values=['One', 'Two', 'Three'], hint='test hint'),
     CheckboxField('Publish', hint='test hint'),
     RadioField('Radio', values=['One', 'Two', 'Three'], hint='test hint'),
     PulldownField(
         'Pulldown', options=['One', 'Two', 'Three'], hint='test hint'),
     ChosenSelectField(
@@ -81,14 +82,15 @@
     twitter='dsilabs',
     web='https://www.dsilabs.ca',
     password='mypass',
     number_of_things=123,
     count=456,
     size=1.2345,
     decimal=Decimal('1234132.234'),
+    timezone='Canada/Pacific',
     amount=Decimal('12341232.32432'),
     foreign_amount=Decimal('121232.432'),
     date=datetime.date(2015, 4, 1),
     min_max_date=datetime.date(2015, 4, 2),
     formatted_date=datetime.date(2015, 4, 3),
     birth_date=datetime.date(2073, 2, 4),
     select='One',
```

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/flags.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/flags.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/index.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/index.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/parts.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/parts.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/responses.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/responses.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/sample.md` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/sample.md`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/tools.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/tools.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/sample/widgets/__init__.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/sample/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/settings/index.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/settings/index.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/settings/model.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/settings/model.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/standard_apps/storage/index.py` & `ZoomFoundry-6.9.1/zoom/_assets/standard_apps/storage/index.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/sites/default/site.ini` & `ZoomFoundry-6.9.1/zoom/_assets/web/sites/default/site.ini`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/_partials/head.pug` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/_partials/head.pug`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/buttons.css` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/buttons.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/content.css` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/content.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/content.css.map` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/content.css.map`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/flags.css` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/flags.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/navigation.css` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/navigation.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/navigation.css.map` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/navigation.css.map`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/social.css` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/social.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/social.css.map` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/social.css.map`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/style.css` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/style.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/widget.css` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/widget.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/css/widget.css.map` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/css/widget.css.map`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/images/android-chrome-192x192.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/images/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/images/android-chrome-512x512.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/images/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/images/apple-touch-icon.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/images/banner-logo.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/images/banner-logo.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/images/email-logo.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/images/email-logo.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/images/favicon-16x16.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/images/favicon-32x32.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/images/favicon.ico` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/src/sass/buttons.sass` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/src/sass/buttons.sass`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/src/sass/content.sass` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/src/sass/content.sass`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/src/sass/flags.sass` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/src/sass/flags.sass`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/src/sass/navigation.sass` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/src/sass/navigation.sass`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/src/sass/social.sass` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/src/sass/social.sass`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/src/sass/style.sass` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/src/sass/style.sass`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/themes/default/src/sass/widget.sass` & `ZoomFoundry-6.9.1/zoom/_assets/web/themes/default/src/sass/widget.sass`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/LICENSE` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/LICENSE`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/bootstrap4.5/css/bootstrap.min.css` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/bootstrap4.5/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/bootstrap4.5/css/bootstrap.min.css.map` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/bootstrap4.5/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/bootstrap4.5/js/bootstrap.bundle.min.js` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/bootstrap4.5/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/bootstrap4.5/js/bootstrap.bundle.min.js.map` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/bootstrap4.5/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap-theme.css` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap-theme.css.map` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap-theme.min.css` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap-theme.min.css.map` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap.css` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap.css.map` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap.min.css` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap.min.css.map` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/fonts/glyphicons-halflings-regular.eot` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/fonts/glyphicons-halflings-regular.svg` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/fonts/glyphicons-halflings-regular.ttf` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/fonts/glyphicons-halflings-regular.woff` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/fonts/glyphicons-halflings-regular.woff2` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/js/bootstrap.js` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/bootstrap/js/bootstrap.min.js` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/chosen/LICENSE.md` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/chosen/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/chosen/chosen-sprite.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/chosen/chosen-sprite.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/chosen/chosen-sprite@2x.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/chosen/chosen-sprite@2x.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/chosen/chosen.jquery.min.js` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/chosen/chosen.jquery.min.js`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/chosen/chosen.min.css` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/chosen/chosen.min.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/dropzone/LICENSE` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/dropzone/LICENSE`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/dropzone/basic.min.css` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/dropzone/basic.min.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/dropzone/dropzone-amd-module.min.js` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/dropzone/dropzone-amd-module.min.js`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/dropzone/dropzone.min.css` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/dropzone/dropzone.min.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/dropzone/dropzone.min.js` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/dropzone/dropzone.min.js`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/fontawesome4/css/font-awesome.css` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/fontawesome4/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/fontawesome4/css/font-awesome.min.css` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/fontawesome4/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/fontawesome4/fonts/fontawesome-webfont.eot` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/fontawesome4/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/fontawesome4/fonts/fontawesome-webfont.svg` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/fontawesome4/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/fontawesome4/fonts/fontawesome-webfont.ttf` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/fontawesome4/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/fontawesome4/fonts/fontawesome-webfont.woff` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/fontawesome4/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/fontawesome4/fonts/fontawesome-webfont.woff2` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/fontawesome4/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/checkmark.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/checkmark.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/down_arrow_red.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/down_arrow_red.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/favicon.ico` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/follow-off.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/follow-off.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/follow-on.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/follow-on.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/no_image.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/no_image.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/no_photo.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/no_photo.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/progress.gif` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/progress.gif`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/secure.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/secure.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/settings.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/settings.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/settings2.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/settings2.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/social-icons-small.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/social-icons-small.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/social-icons.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/social-icons.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/star-off.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/star-off.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/star-on.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/star-on.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/star_empty.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/star_empty.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/star_full.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/star_full.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/star_half_full.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/star_half_full.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/thumbs-down-off.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/thumbs-down-off.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/thumbs-down.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/thumbs-down.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/thumbs-up-off.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/thumbs-up-off.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images/thumbs-up.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images/thumbs-up.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/images-field.js` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/images-field.js`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery/jquery.min.js` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/jquery-ui.min.js` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-icons_222222_256x240.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-icons_2e83ff_256x240.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-icons_454545_256x240.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-icons_888888_256x240.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-icons_cd0a0a_256x240.png` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/jquery-ui.css` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/jquery-ui.min.css` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/theme.css` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui/themes/smoothness/theme.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui-touch-punch/jquery.ui.touch-punch.js` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui-touch-punch/jquery.ui.touch-punch.js`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/jquery-ui-touch-punch/jquery.ui.touch-punch.min.js` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/jquery-ui-touch-punch/jquery.ui.touch-punch.min.js`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/spin.js` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/spin.js`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/_assets/web/www/static/zoom/zoom.js` & `ZoomFoundry-6.9.1/zoom/_assets/web/www/static/zoom/zoom.js`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/apps.py` & `ZoomFoundry-6.9.1/zoom/apps.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/auditing.py` & `ZoomFoundry-6.9.1/zoom/auditing.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/auth/__init__.py` & `ZoomFoundry-6.9.1/zoom/auth/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,26 +43,28 @@
     context = get_context()
     return context.encrypt(password)
 
 
 def validate_password(password, stored_password_hash):
     """validate a password and return the best hash
 
-    >>> hash = '$bcrypt-sha256$2a,14$q4iT8GFWNrwfYDIMKaYI0e$KVxn8PWpzKbOgE/qfwG.IVhRIx.Pma6'
+    >>> hash = '$bcrypt-sha256$v=2,t=2b,r=14$v1UwNPTDgX5pEusaU5XKXe$y0C3DuzSGp/vuV5UYPrSqzT8HfjCqxS'
     >>> validate_password('admin', hash)
     (True, None)
 
     >>> validate_password('admin1', hash)
     (False, None)
 
     >>> valid, hash = validate_password('mypass', '6f8c114b58f2ce9e')
     >>> valid
     True
-    >>> len(hash) == 75 and hash.startswith('$bcrypt')
+    >>> hash.startswith('$bcrypt')
     True
+    >>> len(hash)
+    83
 
     >>> new_hash = hash_password('adminpw')
     >>> validate_password('adminpw', new_hash)
     (True, None)
 
     Validates the supplied password to see if it matches the stored password
     based one of the accepted algorithms and also returns a hash based on the
```

### Comparing `ZoomFoundry-6.7.5/zoom/background.py` & `ZoomFoundry-6.9.1/zoom/background.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/browse.py` & `ZoomFoundry-6.9.1/zoom/browse.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/buckets.py` & `ZoomFoundry-6.9.1/zoom/buckets.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/cache.py` & `ZoomFoundry-6.9.1/zoom/cache.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/cli/assign.py` & `ZoomFoundry-6.9.1/zoom/cli/assign.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/cli/common.py` & `ZoomFoundry-6.9.1/zoom/cli/common.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/cli/database.py` & `ZoomFoundry-6.9.1/zoom/cli/database.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/cli/describe.py` & `ZoomFoundry-6.9.1/zoom/cli/describe.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/cli/init.py` & `ZoomFoundry-6.9.1/zoom/cli/init.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/cli/main.py` & `ZoomFoundry-6.9.1/zoom/cli/main.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/cli/new.py` & `ZoomFoundry-6.9.1/zoom/cli/new.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/cli/run.py` & `ZoomFoundry-6.9.1/zoom/cli/run.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/cli/serve.py` & `ZoomFoundry-6.9.1/zoom/cli/serve.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/cli/setups.py` & `ZoomFoundry-6.9.1/zoom/cli/setups.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/cli/utils.py` & `ZoomFoundry-6.9.1/zoom/cli/utils.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/collect.py` & `ZoomFoundry-6.9.1/zoom/collect.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/component.py` & `ZoomFoundry-6.9.1/zoom/component.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/components/__init__.py` & `ZoomFoundry-6.9.1/zoom/components/__init__.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/components/flags.py` & `ZoomFoundry-6.9.1/zoom/components/flags.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/components/instances/__init__.py` & `ZoomFoundry-6.9.1/zoom/components/instances/__init__.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/components/instances/instance.css` & `ZoomFoundry-6.9.1/zoom/components/instances/instance.css`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/components/instances/instance.html` & `ZoomFoundry-6.9.1/zoom/components/instances/instance.html`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/config.py` & `ZoomFoundry-6.9.1/zoom/config.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/cookies.py` & `ZoomFoundry-6.9.1/zoom/cookies.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/database.py` & `ZoomFoundry-6.9.1/zoom/database.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/exceptions.py` & `ZoomFoundry-6.9.1/zoom/exceptions.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/fields.py` & `ZoomFoundry-6.9.1/zoom/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1769,14 +1769,15 @@
                         changeMonth: true,
                         changeYear: true,
                         yearRange: '-120:+00'
                     });
             """
         )
 
+
 class CheckboxesField(Field):
     """Checkboxes field.
 
     >>> cb = CheckboxesField('Select', value='One', values=['One','Two','Three'], hint='test hint')
     >>> print(cb.widget())
     <ul class="checkbox_field">
     <li><input checked class="checkbox_field" type="checkbox" id="select" name="select" value="One" /><div>One</div></li>
@@ -2234,14 +2235,22 @@
     select_layout = '<select data-placeholder="{place}" class="{classed}" name="{name}" id="{name}">\n'
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         zoom.requires('chosen')
 
 
+class TimezoneField(ChosenSelectField):
+
+    @property
+    def options(self):
+        import pytz
+        return pytz.all_timezones
+
+
 class MultiselectField(TextField):
     """Multiselect Field
 
     >>> MultiselectField('Type',value='One',options=['One','Two']).display_value()
     'One'
 
     >>> f = MultiselectField('Type', default='One', options=['One','Two'])
```

### Comparing `ZoomFoundry-6.7.5/zoom/fill.py` & `ZoomFoundry-6.9.1/zoom/fill.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/forms.py` & `ZoomFoundry-6.9.1/zoom/forms.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/helpers.py` & `ZoomFoundry-6.9.1/zoom/helpers.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/html.py` & `ZoomFoundry-6.9.1/zoom/html.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/impersonation.py` & `ZoomFoundry-6.9.1/zoom/impersonation.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/instances.py` & `ZoomFoundry-6.9.1/zoom/instances.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/jsonz.py` & `ZoomFoundry-6.9.1/zoom/jsonz.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/logging.py` & `ZoomFoundry-6.9.1/zoom/logging.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/mail.py` & `ZoomFoundry-6.9.1/zoom/mail.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from email.utils import formataddr
 
 import zoom
 from zoom.context import context
 from zoom.store import EntityStore
 from zoom.tools import ensure_listy, now
 from zoom.utils import Record
+from zoom.tools import get_template
 
 
 __all__ = (
     'send',
     'send_as',
     'deliver',
     'Attachment',
@@ -38,37 +39,14 @@
 
 
 class SystemMail(Record):
     """system message"""
     pass
 
 
-BODY_TPL = """
-<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.0 Transitional//EN">
-<HTML>
-<BODY>
-<table width="100%">
- <tr>
-  <td align="left">
-  <img src="{logo_url}" alt="banner logo">
-  </td>
- </tr>
- <tr>
-  <td align="left">
-    <font face="helvetica,arial,freesans,clean,sans-serif" size="2">
-    {message}
-    </font>
-  </td>
- </tr>
-</table>
-</BODY>
-</HTML>
-"""
-
-
 class Attachment(object):
     """Email attachment
 
     provide either a pathname, or a filename and a pathname, or if sending
     directly a filename and a file-like object.
 
     """
@@ -101,15 +79,16 @@
 
 def get_mail_store(site):
     """returns the mail store"""
     return EntityStore(site.db, SystemMail)
 
 
 def format_as_html(text, logo_url):
-    return BODY_TPL.format(logo_url=logo_url, message=text)
+    template = get_template('email_template')
+    return template.format(logo_url=logo_url, message=text)
 
 
 def display_email_address(email):
     """Make a formatted address (eg: "User Name <username@somewhere.net>"),
        from a tuple (Display name, email address) or a list of tuples.
        If the parameter is a string, it is returned.
```

### Comparing `ZoomFoundry-6.7.5/zoom/middleware.py` & `ZoomFoundry-6.9.1/zoom/middleware.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/migrations.py` & `ZoomFoundry-6.9.1/zoom/migrations.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/models.py` & `ZoomFoundry-6.9.1/zoom/models.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/mvc.py` & `ZoomFoundry-6.9.1/zoom/mvc.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/packages.py` & `ZoomFoundry-6.9.1/zoom/packages.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/page.py` & `ZoomFoundry-6.9.1/zoom/page.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/profiler.py` & `ZoomFoundry-6.9.1/zoom/profiler.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/queues.py` & `ZoomFoundry-6.9.1/zoom/queues.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/records.py` & `ZoomFoundry-6.9.1/zoom/records.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/render.py` & `ZoomFoundry-6.9.1/zoom/render.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/request.py` & `ZoomFoundry-6.9.1/zoom/request.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/response.py` & `ZoomFoundry-6.9.1/zoom/response.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/server.py` & `ZoomFoundry-6.9.1/zoom/server.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/services.py` & `ZoomFoundry-6.9.1/zoom/services.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/session.py` & `ZoomFoundry-6.9.1/zoom/session.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/settings.py` & `ZoomFoundry-6.9.1/zoom/settings.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/site.py` & `ZoomFoundry-6.9.1/zoom/site.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/sites.py` & `ZoomFoundry-6.9.1/zoom/sites.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/snippets.py` & `ZoomFoundry-6.9.1/zoom/snippets.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/sql/setup_mysql.sql` & `ZoomFoundry-6.9.1/zoom/sql/setup_mysql.sql`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/sql/setup_sqlite3g.sql` & `ZoomFoundry-6.9.1/zoom/sql/setup_sqlite3g.sql`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/sqltools.py` & `ZoomFoundry-6.9.1/zoom/sqltools.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/store.py` & `ZoomFoundry-6.9.1/zoom/store.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/templates.py` & `ZoomFoundry-6.9.1/zoom/templates.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/testing/apptest.py` & `ZoomFoundry-6.9.1/zoom/testing/apptest.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/testing/webtest.py` & `ZoomFoundry-6.9.1/zoom/testing/webtest.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/tools.py` & `ZoomFoundry-6.9.1/zoom/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -639,15 +639,15 @@
             'Unable to use specified template path.  '
             'Templates are located in theme folders.'
         )
 
     return site.templates.setdefault(name, load_template_file(name, default))
 
 def get_template(template_name='default', theme='default'):
-    """Get site page template"""
+    """Get site template"""
 
     logger = logging.getLogger(__name__)
     path = zoom.system.site.themes_path
     isfile = os.path.isfile
 
     pathname = os.path.realpath(
         os.path.join(path, theme, template_name + '.html')
```

### Comparing `ZoomFoundry-6.7.5/zoom/users.py` & `ZoomFoundry-6.9.1/zoom/users.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/utils.py` & `ZoomFoundry-6.9.1/zoom/utils.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/validators.py` & `ZoomFoundry-6.9.1/zoom/validators.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/views/system_pulldown_menu.html` & `ZoomFoundry-6.9.1/zoom/views/system_pulldown_menu.html`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/widgets/cards/__init__.py` & `ZoomFoundry-6.9.1/zoom/widgets/cards/__init__.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/widgets/cards/card.sass` & `ZoomFoundry-6.9.1/zoom/widgets/cards/card.sass`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/widgets/charts/__init__.py` & `ZoomFoundry-6.9.1/zoom/widgets/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/widgets/charts/chart_widget.js` & `ZoomFoundry-6.9.1/zoom/widgets/charts/chart_widget.js`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/widgets/metrics/__init__.py` & `ZoomFoundry-6.9.1/zoom/widgets/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/widgets/metrics/metric_widget.js` & `ZoomFoundry-6.9.1/zoom/widgets/metrics/metric_widget.js`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/widgets/progress/__init__.py` & `ZoomFoundry-6.9.1/zoom/widgets/progress/__init__.py`

 * *Files identical despite different names*

### Comparing `ZoomFoundry-6.7.5/zoom/widgets/progress/progress_widget.sass` & `ZoomFoundry-6.9.1/zoom/widgets/progress/progress_widget.sass`

 * *Files identical despite different names*


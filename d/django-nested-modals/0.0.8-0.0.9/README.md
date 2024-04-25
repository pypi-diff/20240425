# Comparing `tmp/django-nested-modals-0.0.8.tar.gz` & `tmp/django-nested-modals-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\django-nested-modals-0.0.8.tar", last modified: Mon Aug 23 12:15:37 2021, max compression
+gzip compressed data, was "dist\django-nested-modals-0.0.9.tar", last modified: Tue Aug 24 16:21:41 2021, max compression
```

## Comparing `django-nested-modals-0.0.8.tar` & `django-nested-modals-0.0.9.tar`

### file list

```diff
@@ -1,213 +1,215 @@
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.531165 django-nested-modals-0.0.8/
--rw-rw-rw-   0        0        0       72 2021-06-03 13:39:20.000000 django-nested-modals-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1263 2021-08-23 12:15:37.530158 django-nested-modals-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.174023 django-nested-modals-0.0.8/django_modals/
--rw-rw-rw-   0        0        0        0 2021-06-21 15:23:22.000000 django-nested-modals-0.0.8/django_modals/__init__.py
--rw-rw-rw-   0        0        0       98 2021-07-01 09:32:15.000000 django-nested-modals-0.0.8/django_modals/apps.py
--rw-rw-rw-   0        0        0     2499 2021-08-09 11:57:29.000000 django-nested-modals-0.0.8/django_modals/datatables.py
--rw-rw-rw-   0        0        0     6194 2021-08-02 17:00:45.000000 django-nested-modals-0.0.8/django_modals/fields.py
--rw-rw-rw-   0        0        0     1825 2021-08-01 09:36:32.000000 django-nested-modals-0.0.8/django_modals/form_helpers.py
--rw-rw-rw-   0        0        0     7604 2021-08-01 14:38:03.000000 django-nested-modals-0.0.8/django_modals/forms.py
--rw-rw-rw-   0        0        0     4640 2021-08-23 11:13:46.000000 django-nested-modals-0.0.8/django_modals/helper.py
--rw-rw-rw-   0        0        0     1100 2021-08-19 13:02:38.000000 django-nested-modals-0.0.8/django_modals/includes.py
--rw-rw-rw-   0        0        0    21795 2021-08-19 14:11:48.000000 django-nested-modals-0.0.8/django_modals/modals.py
--rw-rw-rw-   0        0        0     2340 2021-07-31 15:38:45.000000 django-nested-modals-0.0.8/django_modals/processes.py
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.019562 django-nested-modals-0.0.8/django_modals/static/
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.020562 django-nested-modals-0.0.8/django_modals/static/django_modals/
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.243576 django-nested-modals-0.0.8/django_modals/static/django_modals/css/
--rw-rw-rw-   0        0        0     2795 2021-08-09 12:48:23.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/css/bootstrap4-toggle.min.css
--rw-rw-rw-   0        0        0    11635 2021-08-17 13:16:24.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/css/modals.css
--rw-rw-rw-   0        0        0    14966 2020-01-28 05:01:22.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/css/select2.min.css
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.020562 django-nested-modals-0.0.8/django_modals/static/django_modals/jquery_ui_limited/
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.253684 django-nested-modals-0.0.8/django_modals/static/django_modals/jquery_ui_limited/css/
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.264244 django-nested-modals-0.0.8/django_modals/static/django_modals/jquery_ui_limited/css/images/
--rw-rw-rw-   0        0        0     7090 2021-08-19 09:53:36.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_444444_256x240.png
--rw-rw-rw-   0        0        0     7074 2021-08-19 09:53:36.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_555555_256x240.png
--rw-rw-rw-   0        0        0     4618 2021-08-19 09:53:36.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_777620_256x240.png
--rw-rw-rw-   0        0        0     7111 2021-08-19 09:53:36.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_777777_256x240.png
--rw-rw-rw-   0        0        0     4618 2021-08-19 09:53:36.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_cc0000_256x240.png
--rw-rw-rw-   0        0        0     6487 2021-08-19 09:53:36.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_ffffff_256x240.png
--rw-rw-rw-   0        0        0    19140 2021-08-19 09:53:36.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/jquery_ui_limited/css/jquery-ui.min.css
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.299785 django-nested-modals-0.0.8/django_modals/static/django_modals/jquery_ui_limited/js/
--rw-rw-rw-   0        0        0    66564 2021-08-19 09:53:36.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/jquery_ui_limited/js/jquery-ui.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.450768 django-nested-modals-0.0.8/django_modals/static/django_modals/js/
--rw-rw-rw-   0        0        0     4431 2021-08-09 12:48:59.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/js/bootstrap4-toggle.min.js
--rw-rw-rw-   0        0        0    14414 2021-08-03 21:02:23.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/js/modals.js
--rw-rw-rw-   0        0        0     7635 2021-07-20 13:30:05.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/js/modals.min.js
--rw-rw-rw-   0        0        0    70891 2020-01-28 05:01:22.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/js/select2.min.js
--rw-rw-rw-   0        0        0     2902 2021-07-23 12:59:56.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/js/widget_select2.js
--rw-rw-rw-   0        0        0     1316 2021-07-20 13:30:05.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/js/widget_select2.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.535780 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/
--rw-rw-rw-   0        0        0     3561 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/jquery.tinymce.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.542780 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/langs/
--rw-rw-rw-   0        0        0      151 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/langs/readme.md
--rw-rw-rw-   0        0        0    26441 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/license.txt
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.033562 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.559780 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/advlist/
--rw-rw-rw-   0        0        0     2226 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/advlist/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.575289 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/anchor/
--rw-rw-rw-   0        0        0     1446 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/anchor/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.584801 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/autolink/
--rw-rw-rw-   0        0        0     2127 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/autolink/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.618548 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/autoresize/
--rw-rw-rw-   0        0        0     2074 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/autoresize/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.628562 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/autosave/
--rw-rw-rw-   0        0        0     2856 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/autosave/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.643115 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/bbcode/
--rw-rw-rw-   0        0        0     2850 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/bbcode/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.654655 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/charmap/
--rw-rw-rw-   0        0        0     8601 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/charmap/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.662196 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/code/
--rw-rw-rw-   0        0        0     1024 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/code/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.676740 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/codesample/
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.681805 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/codesample/css/
--rw-rw-rw-   0        0        0     2334 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/codesample/css/prism.css
--rw-rw-rw-   0        0        0    19350 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/codesample/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.697792 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/colorpicker/
--rw-rw-rw-   0        0        0     1349 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/colorpicker/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.706793 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/contextmenu/
--rw-rw-rw-   0        0        0     1824 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/contextmenu/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.716794 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/directionality/
--rw-rw-rw-   0        0        0      857 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/directionality/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.725794 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/emoticons/
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.743334 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/emoticons/img/
--rw-rw-rw-   0        0        0      354 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-cool.gif
--rw-rw-rw-   0        0        0      329 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-cry.gif
--rw-rw-rw-   0        0        0      331 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-embarassed.gif
--rw-rw-rw-   0        0        0      342 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-foot-in-mouth.gif
--rw-rw-rw-   0        0        0      340 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-frown.gif
--rw-rw-rw-   0        0        0      336 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-innocent.gif
--rw-rw-rw-   0        0        0      338 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-kiss.gif
--rw-rw-rw-   0        0        0      343 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-laughing.gif
--rw-rw-rw-   0        0        0      321 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-money-mouth.gif
--rw-rw-rw-   0        0        0      323 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-sealed.gif
--rw-rw-rw-   0        0        0      344 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-smile.gif
--rw-rw-rw-   0        0        0      338 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-surprised.gif
--rw-rw-rw-   0        0        0      328 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-tongue-out.gif
--rw-rw-rw-   0        0        0      337 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-undecided.gif
--rw-rw-rw-   0        0        0      350 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-wink.gif
--rw-rw-rw-   0        0        0      336 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-yell.gif
--rw-rw-rw-   0        0        0     1071 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/emoticons/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.757352 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/fullpage/
--rw-rw-rw-   0        0        0     7168 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/fullpage/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.767351 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/fullscreen/
--rw-rw-rw-   0        0        0     2184 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/fullscreen/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.785351 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/help/
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.786352 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/help/img/
--rw-rw-rw-   0        0        0    13208 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/help/img/logo.png
--rw-rw-rw-   0        0        0     8179 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/help/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.794152 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/hr/
--rw-rw-rw-   0        0        0      428 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/hr/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.818508 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/image/
--rw-rw-rw-   0        0        0    15852 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/image/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.841201 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/imagetools/
--rw-rw-rw-   0        0        0    32354 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/imagetools/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.852199 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/importcss/
--rw-rw-rw-   0        0        0     3131 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/importcss/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.864209 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/insertdatetime/
--rw-rw-rw-   0        0        0     2633 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/insertdatetime/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.874200 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/legacyoutput/
--rw-rw-rw-   0        0        0     3402 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/legacyoutput/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.886199 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/link/
--rw-rw-rw-   0        0        0     8940 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/link/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.909199 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/lists/
--rw-rw-rw-   0        0        0    26968 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/lists/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.931890 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/media/
--rw-rw-rw-   0        0        0    16576 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/media/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.942881 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/nonbreaking/
--rw-rw-rw-   0        0        0     1012 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/nonbreaking/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.953906 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/noneditable/
--rw-rw-rw-   0        0        0     1540 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/noneditable/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.991727 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/pagebreak/
--rw-rw-rw-   0        0        0     1436 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/pagebreak/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.020234 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/paste/
--rw-rw-rw-   0        0        0    30837 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/paste/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.034254 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/preview/
--rw-rw-rw-   0        0        0     2044 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/preview/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.042255 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/print/
--rw-rw-rw-   0        0        0      465 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/print/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.049254 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/save/
--rw-rw-rw-   0        0        0     1426 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/save/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.061765 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/searchreplace/
--rw-rw-rw-   0        0        0     7352 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/searchreplace/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.073769 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/spellchecker/
--rw-rw-rw-   0        0        0    10308 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/spellchecker/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.082903 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/tabfocus/
--rw-rw-rw-   0        0        0     1614 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/tabfocus/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.118491 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/table/
--rw-rw-rw-   0        0        0   118578 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/table/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.133490 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/template/
--rw-rw-rw-   0        0        0     5191 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/template/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.144492 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/textcolor/
--rw-rw-rw-   0        0        0     4927 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/textcolor/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.157496 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/textpattern/
--rw-rw-rw-   0        0        0     7405 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/textpattern/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.167489 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/toc/
--rw-rw-rw-   0        0        0     2941 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/toc/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.177490 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/visualblocks/
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.207490 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/visualblocks/css/
--rw-rw-rw-   0        0        0     5473 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/visualblocks/css/visualblocks.css
--rw-rw-rw-   0        0        0     1691 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/visualblocks/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.219489 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/visualchars/
--rw-rw-rw-   0        0        0     5321 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/visualchars/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.248488 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/wordcount/
--rw-rw-rw-   0        0        0    12035 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/wordcount/plugin.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.033562 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.273224 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/
--rw-rw-rw-   0        0        0     3611 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/content.inline.min.css
--rw-rw-rw-   0        0        0     4017 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/content.min.css
--rw-rw-rw-   0        0        0      234 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/content.mobile.min.css
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.337156 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/
--rw-rw-rw-   0        0        0     4624 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce-mobile.woff
--rw-rw-rw-   0        0        0     9492 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce-small.eot
--rw-rw-rw-   0        0        0    24727 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce-small.svg
--rw-rw-rw-   0        0        0     9304 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce-small.ttf
--rw-rw-rw-   0        0        0     9380 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce-small.woff
--rw-rw-rw-   0        0        0    18912 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce.eot
--rw-rw-rw-   0        0        0    46373 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce.svg
--rw-rw-rw-   0        0        0    18748 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce.ttf
--rw-rw-rw-   0        0        0    18824 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce.woff
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.341156 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/img/
--rw-rw-rw-   0        0        0       53 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/img/anchor.gif
--rw-rw-rw-   0        0        0     2608 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/img/loader.gif
--rw-rw-rw-   0        0        0      152 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/img/object.gif
--rw-rw-rw-   0        0        0       43 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/img/trans.gif
--rw-rw-rw-   0        0        0    44049 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/skin.min.css
--rw-rw-rw-   0        0        0    27895 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/skin.mobile.min.css
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.040561 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/themes/
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.364927 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/themes/inlite/
--rw-rw-rw-   0        0        0   131875 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/themes/inlite/theme.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.405614 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/themes/mobile/
--rw-rw-rw-   0        0        0   164139 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/themes/mobile/theme.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.437731 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/themes/modern/
--rw-rw-rw-   0        0        0   130746 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/themes/modern/theme.min.js
--rw-rw-rw-   0        0        0   365570 2020-07-13 03:26:08.000000 django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/tinymce.min.js
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:36.041561 django-nested-modals-0.0.8/django_modals/templates/
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.454089 django-nested-modals-0.0.8/django_modals/templates/django_modals/
--rw-rw-rw-   0        0        0      842 2021-08-19 13:14:16.000000 django-nested-modals-0.0.8/django_modals/templates/django_modals/base.html
--rw-rw-rw-   0        0        0      487 2021-08-19 14:08:41.000000 django-nested-modals-0.0.8/django_modals/templates/django_modals/blank_page_form.html
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.459060 django-nested-modals-0.0.8/django_modals/templates/django_modals/fields/
--rw-rw-rw-   0        0        0     1668 2021-07-14 11:22:32.000000 django-nested-modals-0.0.8/django_modals/templates/django_modals/fields/label_checkbox.html
--rw-rw-rw-   0        0        0     1831 2021-08-17 12:38:25.000000 django-nested-modals-0.0.8/django_modals/templates/django_modals/modal_base.html
--rw-rw-rw-   0        0        0      151 2021-07-01 15:20:26.000000 django-nested-modals-0.0.8/django_modals/templates/django_modals/multi_form.html
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.496636 django-nested-modals-0.0.8/django_modals/templates/django_modals/widgets/
--rw-rw-rw-   0        0        0      498 2021-07-20 14:25:48.000000 django-nested-modals-0.0.8/django_modals/templates/django_modals/widgets/datepicker.html
--rw-rw-rw-   0        0        0     1120 2021-07-23 13:02:27.000000 django-nested-modals-0.0.8/django_modals/templates/django_modals/widgets/select2.html
--rw-rw-rw-   0        0        0      472 2021-07-20 14:25:48.000000 django-nested-modals-0.0.8/django_modals/templates/django_modals/widgets/tinymce.html
--rw-rw-rw-   0        0        0      459 2021-07-14 07:45:40.000000 django-nested-modals-0.0.8/django_modals/templates/django_modals/widgets/toggle.html
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.498636 django-nested-modals-0.0.8/django_modals/templatetags/
--rw-rw-rw-   0        0        0        0 2020-04-22 08:24:59.000000 django-nested-modals-0.0.8/django_modals/templatetags/__init__.py
--rw-rw-rw-   0        0        0      868 2021-08-19 13:08:56.000000 django-nested-modals-0.0.8/django_modals/templatetags/modal_tags.py
--rw-rw-rw-   0        0        0      754 2021-08-09 14:15:53.000000 django-nested-modals-0.0.8/django_modals/url_helper.py
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.512636 django-nested-modals-0.0.8/django_modals/widgets/
--rw-rw-rw-   0        0        0      311 2021-07-27 08:26:14.000000 django-nested-modals-0.0.8/django_modals/widgets/jquery_datepicker.py
--rw-rw-rw-   0        0        0     2763 2021-08-01 10:14:13.000000 django-nested-modals-0.0.8/django_modals/widgets/select2.py
--rw-rw-rw-   0        0        0      449 2021-08-01 12:59:19.000000 django-nested-modals-0.0.8/django_modals/widgets/widgets.py
-drwxrwxrwx   0        0        0        0 2021-08-23 12:15:37.529183 django-nested-modals-0.0.8/django_nested_modals.egg-info/
--rw-rw-rw-   0        0        0     1263 2021-08-23 12:15:35.000000 django-nested-modals-0.0.8/django_nested_modals.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9054 2021-08-23 12:15:35.000000 django-nested-modals-0.0.8/django_nested_modals.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-08-23 12:15:35.000000 django-nested-modals-0.0.8/django_nested_modals.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2021-08-23 12:15:35.000000 django-nested-modals-0.0.8/django_nested_modals.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2021-08-23 12:15:35.000000 django-nested-modals-0.0.8/django_nested_modals.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-08-23 12:15:37.531165 django-nested-modals-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      749 2021-08-23 12:14:46.000000 django-nested-modals-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.766106 django-nested-modals-0.0.9/
+-rw-rw-rw-   0        0        0       72 2021-06-03 13:39:20.000000 django-nested-modals-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1263 2021-08-24 16:21:41.764509 django-nested-modals-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:40.926974 django-nested-modals-0.0.9/django_modals/
+-rw-rw-rw-   0        0        0        0 2021-06-21 15:23:22.000000 django-nested-modals-0.0.9/django_modals/__init__.py
+-rw-rw-rw-   0        0        0       98 2021-07-01 09:32:15.000000 django-nested-modals-0.0.9/django_modals/apps.py
+-rw-rw-rw-   0        0        0     2499 2021-08-09 11:57:29.000000 django-nested-modals-0.0.9/django_modals/datatables.py
+-rw-rw-rw-   0        0        0     6194 2021-08-02 17:00:45.000000 django-nested-modals-0.0.9/django_modals/fields.py
+-rw-rw-rw-   0        0        0     1825 2021-08-01 09:36:32.000000 django-nested-modals-0.0.9/django_modals/form_helpers.py
+-rw-rw-rw-   0        0        0     7604 2021-08-01 14:38:03.000000 django-nested-modals-0.0.9/django_modals/forms.py
+-rw-rw-rw-   0        0        0     4640 2021-08-23 11:13:46.000000 django-nested-modals-0.0.9/django_modals/helper.py
+-rw-rw-rw-   0        0        0     1136 2021-08-24 12:47:29.000000 django-nested-modals-0.0.9/django_modals/includes.py
+-rw-rw-rw-   0        0        0    21795 2021-08-19 14:11:48.000000 django-nested-modals-0.0.9/django_modals/modals.py
+-rw-rw-rw-   0        0        0     2340 2021-07-31 15:38:45.000000 django-nested-modals-0.0.9/django_modals/processes.py
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:40.877751 django-nested-modals-0.0.9/django_modals/static/
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:40.879752 django-nested-modals-0.0.9/django_modals/static/django_modals/
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:40.952570 django-nested-modals-0.0.9/django_modals/static/django_modals/css/
+-rw-rw-rw-   0        0        0     2795 2021-08-09 12:48:23.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/css/bootstrap4-toggle.min.css
+-rw-rw-rw-   0        0        0    11635 2021-08-17 13:16:24.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/css/modals.css
+-rw-rw-rw-   0        0        0    14966 2020-01-28 05:01:22.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/css/select2.min.css
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:40.878753 django-nested-modals-0.0.9/django_modals/static/django_modals/jquery_ui_limited/
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:40.963579 django-nested-modals-0.0.9/django_modals/static/django_modals/jquery_ui_limited/css/
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:40.971571 django-nested-modals-0.0.9/django_modals/static/django_modals/jquery_ui_limited/css/images/
+-rw-rw-rw-   0        0        0     7090 2021-08-19 09:53:36.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_444444_256x240.png
+-rw-rw-rw-   0        0        0     7074 2021-08-19 09:53:36.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_555555_256x240.png
+-rw-rw-rw-   0        0        0     4618 2021-08-19 09:53:36.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_777620_256x240.png
+-rw-rw-rw-   0        0        0     7111 2021-08-19 09:53:36.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_777777_256x240.png
+-rw-rw-rw-   0        0        0     4618 2021-08-19 09:53:36.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_cc0000_256x240.png
+-rw-rw-rw-   0        0        0     6487 2021-08-19 09:53:36.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_ffffff_256x240.png
+-rw-rw-rw-   0        0        0    19140 2021-08-19 09:53:36.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/jquery_ui_limited/css/jquery-ui.min.css
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:40.996572 django-nested-modals-0.0.9/django_modals/static/django_modals/jquery_ui_limited/js/
+-rw-rw-rw-   0        0        0    66564 2021-08-19 09:53:36.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/jquery_ui_limited/js/jquery-ui.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.073578 django-nested-modals-0.0.9/django_modals/static/django_modals/js/
+-rw-rw-rw-   0        0        0     4431 2021-08-09 12:48:59.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/js/bootstrap4-toggle.min.js
+-rw-rw-rw-   0        0        0    14414 2021-08-03 21:02:23.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/js/modals.js
+-rw-rw-rw-   0        0        0     7635 2021-07-20 13:30:05.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/js/modals.min.js
+-rw-rw-rw-   0        0        0    16152 2021-08-24 12:51:42.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/js/modals_legacy.js
+-rw-rw-rw-   0        0        0    70891 2020-01-28 05:01:22.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/js/select2.min.js
+-rw-rw-rw-   0        0        0     2918 2021-08-24 12:59:41.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/js/widget_select2.js
+-rw-rw-rw-   0        0        0     1316 2021-07-20 13:30:05.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/js/widget_select2.min.js
+-rw-rw-rw-   0        0        0     2508 2021-08-24 12:55:59.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/js/widget_select2_legacy.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.132670 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/
+-rw-rw-rw-   0        0        0     3561 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/jquery.tinymce.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.134779 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/langs/
+-rw-rw-rw-   0        0        0      151 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/langs/readme.md
+-rw-rw-rw-   0        0        0    26441 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/license.txt
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:40.893755 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.136340 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/advlist/
+-rw-rw-rw-   0        0        0     2226 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/advlist/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.144918 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/anchor/
+-rw-rw-rw-   0        0        0     1446 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/anchor/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.145918 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/autolink/
+-rw-rw-rw-   0        0        0     2127 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/autolink/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.154512 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/autoresize/
+-rw-rw-rw-   0        0        0     2074 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/autoresize/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.157514 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/autosave/
+-rw-rw-rw-   0        0        0     2856 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/autosave/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.158512 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/bbcode/
+-rw-rw-rw-   0        0        0     2850 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/bbcode/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.168513 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/charmap/
+-rw-rw-rw-   0        0        0     8601 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/charmap/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.175513 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/code/
+-rw-rw-rw-   0        0        0     1024 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/code/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.189565 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/codesample/
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.195354 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/codesample/css/
+-rw-rw-rw-   0        0        0     2334 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/codesample/css/prism.css
+-rw-rw-rw-   0        0        0    19350 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/codesample/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.202359 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/colorpicker/
+-rw-rw-rw-   0        0        0     1349 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/colorpicker/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.214205 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/contextmenu/
+-rw-rw-rw-   0        0        0     1824 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/contextmenu/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.222166 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/directionality/
+-rw-rw-rw-   0        0        0      857 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/directionality/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.223825 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/emoticons/
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.239723 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/emoticons/img/
+-rw-rw-rw-   0        0        0      354 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-cool.gif
+-rw-rw-rw-   0        0        0      329 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-cry.gif
+-rw-rw-rw-   0        0        0      331 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-embarassed.gif
+-rw-rw-rw-   0        0        0      342 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-foot-in-mouth.gif
+-rw-rw-rw-   0        0        0      340 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-frown.gif
+-rw-rw-rw-   0        0        0      336 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-innocent.gif
+-rw-rw-rw-   0        0        0      338 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-kiss.gif
+-rw-rw-rw-   0        0        0      343 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-laughing.gif
+-rw-rw-rw-   0        0        0      321 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-money-mouth.gif
+-rw-rw-rw-   0        0        0      323 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-sealed.gif
+-rw-rw-rw-   0        0        0      344 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-smile.gif
+-rw-rw-rw-   0        0        0      338 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-surprised.gif
+-rw-rw-rw-   0        0        0      328 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-tongue-out.gif
+-rw-rw-rw-   0        0        0      337 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-undecided.gif
+-rw-rw-rw-   0        0        0      350 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-wink.gif
+-rw-rw-rw-   0        0        0      336 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/emoticons/img/smiley-yell.gif
+-rw-rw-rw-   0        0        0     1071 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/emoticons/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.250326 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/fullpage/
+-rw-rw-rw-   0        0        0     7168 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/fullpage/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.252327 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/fullscreen/
+-rw-rw-rw-   0        0        0     2184 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/fullscreen/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.253327 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/help/
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.254327 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/help/img/
+-rw-rw-rw-   0        0        0    13208 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/help/img/logo.png
+-rw-rw-rw-   0        0        0     8179 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/help/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.255328 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/hr/
+-rw-rw-rw-   0        0        0      428 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/hr/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.269668 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/image/
+-rw-rw-rw-   0        0        0    15852 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/image/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.285504 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/imagetools/
+-rw-rw-rw-   0        0        0    32354 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/imagetools/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.287756 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/importcss/
+-rw-rw-rw-   0        0        0     3131 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/importcss/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.289781 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/insertdatetime/
+-rw-rw-rw-   0        0        0     2633 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/insertdatetime/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.298783 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/legacyoutput/
+-rw-rw-rw-   0        0        0     3402 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/legacyoutput/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.313346 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/link/
+-rw-rw-rw-   0        0        0     8940 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/link/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.331798 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/lists/
+-rw-rw-rw-   0        0        0    26968 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/lists/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.345546 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/media/
+-rw-rw-rw-   0        0        0    16576 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/media/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.347541 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/nonbreaking/
+-rw-rw-rw-   0        0        0     1012 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/nonbreaking/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.351177 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/noneditable/
+-rw-rw-rw-   0        0        0     1540 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/noneditable/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.353176 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/pagebreak/
+-rw-rw-rw-   0        0        0     1436 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/pagebreak/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.367368 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/paste/
+-rw-rw-rw-   0        0        0    30837 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/paste/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.368981 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/preview/
+-rw-rw-rw-   0        0        0     2044 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/preview/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.371059 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/print/
+-rw-rw-rw-   0        0        0      465 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/print/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.379096 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/save/
+-rw-rw-rw-   0        0        0     1426 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/save/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.382509 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/searchreplace/
+-rw-rw-rw-   0        0        0     7352 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/searchreplace/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.402756 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/spellchecker/
+-rw-rw-rw-   0        0        0    10308 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/spellchecker/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.404753 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/tabfocus/
+-rw-rw-rw-   0        0        0     1614 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/tabfocus/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.439480 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/table/
+-rw-rw-rw-   0        0        0   118578 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/table/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.441059 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/template/
+-rw-rw-rw-   0        0        0     5191 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/template/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.443085 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/textcolor/
+-rw-rw-rw-   0        0        0     4927 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/textcolor/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.445084 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/textpattern/
+-rw-rw-rw-   0        0        0     7405 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/textpattern/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.454087 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/toc/
+-rw-rw-rw-   0        0        0     2941 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/toc/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.466329 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/visualblocks/
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.495767 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/visualblocks/css/
+-rw-rw-rw-   0        0        0     5473 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/visualblocks/css/visualblocks.css
+-rw-rw-rw-   0        0        0     1691 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/visualblocks/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.497772 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/visualchars/
+-rw-rw-rw-   0        0        0     5321 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/visualchars/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.519764 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/wordcount/
+-rw-rw-rw-   0        0        0    12035 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/wordcount/plugin.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:40.894751 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.545764 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/
+-rw-rw-rw-   0        0        0     3611 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/content.inline.min.css
+-rw-rw-rw-   0        0        0     4017 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/content.min.css
+-rw-rw-rw-   0        0        0      234 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/content.mobile.min.css
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.605579 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/
+-rw-rw-rw-   0        0        0     4624 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce-mobile.woff
+-rw-rw-rw-   0        0        0     9492 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce-small.eot
+-rw-rw-rw-   0        0        0    24727 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce-small.svg
+-rw-rw-rw-   0        0        0     9304 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce-small.ttf
+-rw-rw-rw-   0        0        0     9380 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce-small.woff
+-rw-rw-rw-   0        0        0    18912 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce.eot
+-rw-rw-rw-   0        0        0    46373 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce.svg
+-rw-rw-rw-   0        0        0    18748 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce.ttf
+-rw-rw-rw-   0        0        0    18824 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce.woff
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.613582 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/img/
+-rw-rw-rw-   0        0        0       53 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/img/anchor.gif
+-rw-rw-rw-   0        0        0     2608 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/img/loader.gif
+-rw-rw-rw-   0        0        0      152 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/img/object.gif
+-rw-rw-rw-   0        0        0       43 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/img/trans.gif
+-rw-rw-rw-   0        0        0    44049 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/skin.min.css
+-rw-rw-rw-   0        0        0    27895 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/skin.mobile.min.css
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:40.896752 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/themes/
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.636591 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/themes/inlite/
+-rw-rw-rw-   0        0        0   131875 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/themes/inlite/theme.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.676580 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/themes/mobile/
+-rw-rw-rw-   0        0        0   164139 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/themes/mobile/theme.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.710578 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/themes/modern/
+-rw-rw-rw-   0        0        0   130746 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/themes/modern/theme.min.js
+-rw-rw-rw-   0        0        0   365570 2020-07-13 03:26:08.000000 django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/tinymce.min.js
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:40.896752 django-nested-modals-0.0.9/django_modals/templates/
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.725578 django-nested-modals-0.0.9/django_modals/templates/django_modals/
+-rw-rw-rw-   0        0        0      842 2021-08-19 13:14:16.000000 django-nested-modals-0.0.9/django_modals/templates/django_modals/base.html
+-rw-rw-rw-   0        0        0      487 2021-08-19 14:08:41.000000 django-nested-modals-0.0.9/django_modals/templates/django_modals/blank_page_form.html
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.729578 django-nested-modals-0.0.9/django_modals/templates/django_modals/fields/
+-rw-rw-rw-   0        0        0     1668 2021-07-14 11:22:32.000000 django-nested-modals-0.0.9/django_modals/templates/django_modals/fields/label_checkbox.html
+-rw-rw-rw-   0        0        0     1831 2021-08-17 12:38:25.000000 django-nested-modals-0.0.9/django_modals/templates/django_modals/modal_base.html
+-rw-rw-rw-   0        0        0      151 2021-07-01 15:20:26.000000 django-nested-modals-0.0.9/django_modals/templates/django_modals/multi_form.html
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.735579 django-nested-modals-0.0.9/django_modals/templates/django_modals/widgets/
+-rw-rw-rw-   0        0        0      498 2021-07-20 14:25:48.000000 django-nested-modals-0.0.9/django_modals/templates/django_modals/widgets/datepicker.html
+-rw-rw-rw-   0        0        0     1120 2021-07-23 13:02:27.000000 django-nested-modals-0.0.9/django_modals/templates/django_modals/widgets/select2.html
+-rw-rw-rw-   0        0        0      472 2021-07-20 14:25:48.000000 django-nested-modals-0.0.9/django_modals/templates/django_modals/widgets/tinymce.html
+-rw-rw-rw-   0        0        0      459 2021-07-14 07:45:40.000000 django-nested-modals-0.0.9/django_modals/templates/django_modals/widgets/toggle.html
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.741578 django-nested-modals-0.0.9/django_modals/templatetags/
+-rw-rw-rw-   0        0        0        0 2020-04-22 08:24:59.000000 django-nested-modals-0.0.9/django_modals/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      868 2021-08-19 13:08:56.000000 django-nested-modals-0.0.9/django_modals/templatetags/modal_tags.py
+-rw-rw-rw-   0        0        0      754 2021-08-09 14:15:53.000000 django-nested-modals-0.0.9/django_modals/url_helper.py
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.746583 django-nested-modals-0.0.9/django_modals/widgets/
+-rw-rw-rw-   0        0        0      311 2021-07-27 08:26:14.000000 django-nested-modals-0.0.9/django_modals/widgets/jquery_datepicker.py
+-rw-rw-rw-   0        0        0     2763 2021-08-01 10:14:13.000000 django-nested-modals-0.0.9/django_modals/widgets/select2.py
+-rw-rw-rw-   0        0        0      449 2021-08-01 12:59:19.000000 django-nested-modals-0.0.9/django_modals/widgets/widgets.py
+drwxrwxrwx   0        0        0        0 2021-08-24 16:21:41.762533 django-nested-modals-0.0.9/django_nested_modals.egg-info/
+-rw-rw-rw-   0        0        0     1263 2021-08-24 16:21:40.000000 django-nested-modals-0.0.9/django_nested_modals.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9172 2021-08-24 16:21:40.000000 django-nested-modals-0.0.9/django_nested_modals.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-08-24 16:21:40.000000 django-nested-modals-0.0.9/django_nested_modals.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2021-08-24 16:21:40.000000 django-nested-modals-0.0.9/django_nested_modals.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2021-08-24 16:21:40.000000 django-nested-modals-0.0.9/django_nested_modals.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-08-24 16:21:41.766106 django-nested-modals-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      749 2021-08-24 16:20:29.000000 django-nested-modals-0.0.9/setup.py
```

### Comparing `django-nested-modals-0.0.8/PKG-INFO` & `django-nested-modals-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-nested-modals
-Version: 0.0.8
+Version: 0.0.9
 Summary: Django app to implement Bootstrap nested modals
 Home-page: https://github.com/jonesim/django-modals
 Author: Ian Jones
 License: UNKNOWN
 Description: [![PyPI version](https://badge.fury.io/py/django-nested-modals.svg)](https://badge.fury.io/py/django-nested-modals)
         
         Add to installed apps in settings
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-nested-modals Version: 0.0.8 Summary: Django
+Metadata-Version: 2.1 Name: django-nested-modals Version: 0.0.9 Summary: Django
 app to implement Bootstrap nested modals Home-page: https://github.com/jonesim/
 django-modals Author: Ian Jones License: UNKNOWN Description: [![PyPI version]
 (https://badge.fury.io/py/django-nested-modals.svg)](https://badge.fury.io/py/
 django-nested-modals) Add to installed apps in settings `'bootstrap_modals',`
 Add to template
 ####See django_examples for example usage Types of redirect Existing modal
 sends ajax command return self.command_response(ajax_modal_replace
```

### Comparing `django-nested-modals-0.0.8/django_modals/datatables.py` & `django-nested-modals-0.0.9/django_modals/datatables.py`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/fields.py` & `django-nested-modals-0.0.9/django_modals/fields.py`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/form_helpers.py` & `django-nested-modals-0.0.9/django_modals/form_helpers.py`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/forms.py` & `django-nested-modals-0.0.9/django_modals/forms.py`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/helper.py` & `django-nested-modals-0.0.9/django_modals/helper.py`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/includes.py` & `django-nested-modals-0.0.9/django_modals/includes.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     js_filename = 'ajax_helpers.js'
     js_path = ''
 
 
 class Modals(SourceBase):
     static_path = 'django_modals/'
     filename = 'modals'
+    legacy_js = 'modals_legacy.js'
 
 
 class Toggle(SourceBase):
     static_path = 'django_modals/'
     cdn_path = 'cdn.jsdelivr.net/gh/gitbrent/bootstrap4-toggle@3.6.1/'
     filename = 'bootstrap4-toggle.min'
```

### Comparing `django-nested-modals-0.0.8/django_modals/modals.py` & `django-nested-modals-0.0.9/django_modals/modals.py`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/processes.py` & `django-nested-modals-0.0.9/django_modals/processes.py`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/css/bootstrap4-toggle.min.css` & `django-nested-modals-0.0.9/django_modals/static/django_modals/css/bootstrap4-toggle.min.css`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/css/modals.css` & `django-nested-modals-0.0.9/django_modals/static/django_modals/css/modals.css`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/css/select2.min.css` & `django-nested-modals-0.0.9/django_modals/static/django_modals/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_444444_256x240.png` & `django-nested-modals-0.0.9/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_555555_256x240.png` & `django-nested-modals-0.0.9/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_777620_256x240.png` & `django-nested-modals-0.0.9/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_777777_256x240.png` & `django-nested-modals-0.0.9/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_cc0000_256x240.png` & `django-nested-modals-0.0.9/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_ffffff_256x240.png` & `django-nested-modals-0.0.9/django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/jquery_ui_limited/css/jquery-ui.min.css` & `django-nested-modals-0.0.9/django_modals/static/django_modals/jquery_ui_limited/css/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/jquery_ui_limited/js/jquery-ui.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/jquery_ui_limited/js/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/js/bootstrap4-toggle.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/js/bootstrap4-toggle.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/js/modals.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/js/modals.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/js/modals.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/js/modals.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/js/select2.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/js/widget_select2.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/js/widget_select2.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -17,18 +17,18 @@
         }
         var modal_url = django_modal.modal_div().attr("data-url");
         var select2_params = {
             theme: "bootstrap4",
             dropdownParent: modal_container,
             allowClear: true,
             placeholder: placeholder
-        }
+        };
 
         if (data !== undefined) {
-            select2_params.data = data
+            select2_params.data = data;
         }
 
         if (data !== undefined || ajax) {
             select2_params.templateSelection = function(text) {
                 return $("<span>" + text.text + "</span>");
             };
             select2_params.templateResult = function(text) {
@@ -75,11 +75,11 @@
         }
         select_element.select2(select2_params);
         $(".select2-selection__rendered").hover(function() {
             $(this).removeAttr("title");
         });
     }
     return {
-        initselect2,
-        modal
+        initselect2: initselect2,
+        modal: modal
     };
 }();
```

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/js/widget_select2.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/js/widget_select2.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/jquery.tinymce.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/jquery.tinymce.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/license.txt` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/license.txt`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/advlist/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/advlist/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/anchor/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/anchor/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/autolink/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/autolink/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/autoresize/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/autoresize/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/autosave/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/autosave/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/bbcode/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/bbcode/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/charmap/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/charmap/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/code/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/code/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/codesample/css/prism.css` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/codesample/css/prism.css`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/codesample/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/codesample/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/colorpicker/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/colorpicker/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/contextmenu/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/contextmenu/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/directionality/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/directionality/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/emoticons/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/emoticons/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/fullpage/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/fullpage/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/fullscreen/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/fullscreen/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/help/img/logo.png` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/help/img/logo.png`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/help/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/help/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/image/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/image/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/imagetools/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/imagetools/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/importcss/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/importcss/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/insertdatetime/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/insertdatetime/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/legacyoutput/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/legacyoutput/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/link/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/link/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/lists/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/lists/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/media/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/media/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/nonbreaking/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/nonbreaking/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/noneditable/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/noneditable/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/pagebreak/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/pagebreak/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/paste/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/paste/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/preview/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/preview/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/save/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/save/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/searchreplace/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/searchreplace/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/spellchecker/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/spellchecker/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/tabfocus/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/tabfocus/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/table/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/table/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/template/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/template/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/textcolor/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/textcolor/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/textpattern/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/textpattern/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/toc/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/toc/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/visualblocks/css/visualblocks.css` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/visualblocks/css/visualblocks.css`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/visualblocks/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/visualblocks/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/visualchars/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/visualchars/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/plugins/wordcount/plugin.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/plugins/wordcount/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/content.inline.min.css` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/content.inline.min.css`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/content.min.css` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/content.min.css`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce-mobile.woff` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce-mobile.woff`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce-small.eot` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce-small.eot`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce-small.svg` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce-small.svg`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce-small.ttf` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce-small.ttf`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce-small.woff` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce-small.woff`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce.eot` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce.eot`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce.svg` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce.svg`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce.ttf` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce.ttf`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce.woff` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/fonts/tinymce.woff`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/img/loader.gif` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/img/loader.gif`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/skin.min.css` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/skin.min.css`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/skins/lightgray/skin.mobile.min.css` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/skins/lightgray/skin.mobile.min.css`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/themes/inlite/theme.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/themes/inlite/theme.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/themes/mobile/theme.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/themes/mobile/theme.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/themes/modern/theme.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/themes/modern/theme.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/static/django_modals/tinymce/tinymce.min.js` & `django-nested-modals-0.0.9/django_modals/static/django_modals/tinymce/tinymce.min.js`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/templates/django_modals/base.html` & `django-nested-modals-0.0.9/django_modals/templates/django_modals/base.html`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/templates/django_modals/fields/label_checkbox.html` & `django-nested-modals-0.0.9/django_modals/templates/django_modals/fields/label_checkbox.html`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/templates/django_modals/modal_base.html` & `django-nested-modals-0.0.9/django_modals/templates/django_modals/modal_base.html`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/templates/django_modals/widgets/select2.html` & `django-nested-modals-0.0.9/django_modals/templates/django_modals/widgets/select2.html`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/templatetags/modal_tags.py` & `django-nested-modals-0.0.9/django_modals/templatetags/modal_tags.py`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/url_helper.py` & `django-nested-modals-0.0.9/django_modals/url_helper.py`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_modals/widgets/select2.py` & `django-nested-modals-0.0.9/django_modals/widgets/select2.py`

 * *Files identical despite different names*

### Comparing `django-nested-modals-0.0.8/django_nested_modals.egg-info/PKG-INFO` & `django-nested-modals-0.0.9/django_nested_modals.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-nested-modals
-Version: 0.0.8
+Version: 0.0.9
 Summary: Django app to implement Bootstrap nested modals
 Home-page: https://github.com/jonesim/django-modals
 Author: Ian Jones
 License: UNKNOWN
 Description: [![PyPI version](https://badge.fury.io/py/django-nested-modals.svg)](https://badge.fury.io/py/django-nested-modals)
         
         Add to installed apps in settings
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-nested-modals Version: 0.0.8 Summary: Django
+Metadata-Version: 2.1 Name: django-nested-modals Version: 0.0.9 Summary: Django
 app to implement Bootstrap nested modals Home-page: https://github.com/jonesim/
 django-modals Author: Ian Jones License: UNKNOWN Description: [![PyPI version]
 (https://badge.fury.io/py/django-nested-modals.svg)](https://badge.fury.io/py/
 django-nested-modals) Add to installed apps in settings `'bootstrap_modals',`
 Add to template
 ####See django_examples for example usage Types of redirect Existing modal
 sends ajax command return self.command_response(ajax_modal_replace
```

### Comparing `django-nested-modals-0.0.8/django_nested_modals.egg-info/SOURCES.txt` & `django-nested-modals-0.0.9/django_nested_modals.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -21,17 +21,19 @@
 django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_777777_256x240.png
 django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_cc0000_256x240.png
 django_modals/static/django_modals/jquery_ui_limited/css/images/ui-icons_ffffff_256x240.png
 django_modals/static/django_modals/jquery_ui_limited/js/jquery-ui.min.js
 django_modals/static/django_modals/js/bootstrap4-toggle.min.js
 django_modals/static/django_modals/js/modals.js
 django_modals/static/django_modals/js/modals.min.js
+django_modals/static/django_modals/js/modals_legacy.js
 django_modals/static/django_modals/js/select2.min.js
 django_modals/static/django_modals/js/widget_select2.js
 django_modals/static/django_modals/js/widget_select2.min.js
+django_modals/static/django_modals/js/widget_select2_legacy.js
 django_modals/static/django_modals/tinymce/jquery.tinymce.min.js
 django_modals/static/django_modals/tinymce/license.txt
 django_modals/static/django_modals/tinymce/tinymce.min.js
 django_modals/static/django_modals/tinymce/langs/readme.md
 django_modals/static/django_modals/tinymce/plugins/advlist/plugin.min.js
 django_modals/static/django_modals/tinymce/plugins/anchor/plugin.min.js
 django_modals/static/django_modals/tinymce/plugins/autolink/plugin.min.js
```

### Comparing `django-nested-modals-0.0.8/setup.py` & `django-nested-modals-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-nested-modals",
-    version="0.0.8",
+    version="0.0.9",
     author="Ian Jones",
     description="Django app to implement Bootstrap nested modals",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jonesim/django-modals",
     include_package_data = True,
     packages=['django_modals'],
```


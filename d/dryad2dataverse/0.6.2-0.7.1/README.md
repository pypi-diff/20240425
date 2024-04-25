# Comparing `tmp/dryad2dataverse-0.6.2.tar.gz` & `tmp/dryad2dataverse-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dryad2dataverse-0.6.2.tar", last modified: Thu Aug 24 16:57:05 2023, max compression
+gzip compressed data, was "dryad2dataverse-0.7.1.tar", last modified: Thu Apr 25 17:56:07 2024, max compression
```

## Comparing `dryad2dataverse-0.6.2.tar` & `dryad2dataverse-0.7.1.tar`

### file list

```diff
@@ -1,261 +1,261 @@
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.585763 dryad2dataverse-0.6.2/
--rw-r--r--   0 paul       (501) staff       (20)      485 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/.gitignore
--rw-r--r--   0 paul       (501) staff       (20)     3019 2023-08-24 16:57:05.585198 dryad2dataverse-0.6.2/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)     2033 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/README.md
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.143952 dryad2dataverse-0.6.2/docs/
--rw-r--r--   0 paul       (501) staff       (20)      442 2021-11-29 23:23:23.000000 dryad2dataverse-0.6.2/docs/_config.yml
--rw-r--r--   0 paul       (501) staff       (20)    26768 2022-12-07 22:06:06.000000 dryad2dataverse-0.6.2/docs/api_reference.md
--rw-r--r--   0 paul       (501) staff       (20)     5035 2023-05-11 16:15:57.000000 dryad2dataverse-0.6.2/docs/changelog.md
--rw-r--r--   0 paul       (501) staff       (20)     1631 2022-04-14 21:51:21.000000 dryad2dataverse-0.6.2/docs/compiling.md
--rw-r--r--   0 paul       (501) staff       (20)     1152 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/credits.md
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.145008 dryad2dataverse-0.6.2/docs/css/
--rw-r--r--   0 paul       (501) staff       (20)      473 2022-02-04 19:47:46.000000 dryad2dataverse-0.6.2/docs/css/extra.css
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.178513 dryad2dataverse-0.6.2/docs/dbase_structure/
--rw-r--r--   0 paul       (501) staff       (20)    19355 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/anomalies.html
--rw-r--r--   0 paul       (501) staff       (20)        0 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/anomalies.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.110495 dryad2dataverse-0.6.2/docs/dbase_structure/bower/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.101436 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.101219 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.221319 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/css/
--rw-r--r--   0 paul       (501) staff       (20)    26132 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.css
--rw-r--r--   0 paul       (501) staff       (20)    47706 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.css.map
--rw-r--r--   0 paul       (501) staff       (20)    23409 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.min.css
--rw-r--r--   0 paul       (501) staff       (20)    25648 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.min.css.map
--rw-r--r--   0 paul       (501) staff       (20)   146010 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.css
--rw-r--r--   0 paul       (501) staff       (20)   389287 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.css.map
--rw-r--r--   0 paul       (501) staff       (20)   121200 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.min.css
--rw-r--r--   0 paul       (501) staff       (20)   542194 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.min.css.map
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.243032 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/
--rw-r--r--   0 paul       (501) staff       (20)    20127 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 paul       (501) staff       (20)   108738 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 paul       (501) staff       (20)    45404 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 paul       (501) staff       (20)    23424 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 paul       (501) staff       (20)    18028 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.251375 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/js/
--rw-r--r--   0 paul       (501) staff       (20)    69707 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/js/bootstrap.js
--rw-r--r--   0 paul       (501) staff       (20)    37045 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/js/bootstrap.min.js
--rw-r--r--   0 paul       (501) staff       (20)      484 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/js/npm.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.102202 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/plugins/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.254308 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/plugins/fastclick/
--rw-r--r--   0 paul       (501) staff       (20)    25965 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/plugins/fastclick/fastclick.js
--rw-r--r--   0 paul       (501) staff       (20)     8776 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/plugins/fastclick/fastclick.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.255733 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/plugins/jQuery/
--rw-r--r--   0 paul       (501) staff       (20)    85659 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/plugins/jQuery/jquery-2.2.3.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.264155 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/plugins/jQueryUI/
--rw-r--r--   0 paul       (501) staff       (20)   470596 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/plugins/jQueryUI/jquery-ui.js
--rw-r--r--   0 paul       (501) staff       (20)   240427 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/plugins/jQueryUI/jquery-ui.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.275656 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/plugins/slimScroll/
--rw-r--r--   0 paul       (501) staff       (20)    13832 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/plugins/slimScroll/jquery.slimscroll.js
--rw-r--r--   0 paul       (501) staff       (20)     4724 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/plugins/slimScroll/jquery.slimscroll.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.277079 dryad2dataverse-0.6.2/docs/dbase_structure/bower/anchor-js/
--rw-r--r--   0 paul       (501) staff       (20)     5332 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/anchor-js/anchor.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.295220 dryad2dataverse-0.6.2/docs/dbase_structure/bower/codemirror/
--rw-r--r--   0 paul       (501) staff       (20)     8241 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/codemirror/codemirror.css
--rw-r--r--   0 paul       (501) staff       (20)   365757 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/codemirror/codemirror.js
--rw-r--r--   0 paul       (501) staff       (20)    37494 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/codemirror/sql.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.296935 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net/
--rw-r--r--   0 paul       (501) staff       (20)    83268 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net/jquery.dataTables.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.104623 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-bs/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.300453 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-bs/css/
--rw-r--r--   0 paul       (501) staff       (20)     4823 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-bs/css/dataTables.bootstrap.css
--rw-r--r--   0 paul       (501) staff       (20)     4188 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-bs/css/dataTables.bootstrap.min.css
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.302680 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-bs/js/
--rw-r--r--   0 paul       (501) staff       (20)     4559 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-bs/js/dataTables.bootstrap.js
--rw-r--r--   0 paul       (501) staff       (20)     1966 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-bs/js/dataTables.bootstrap.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.324004 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons/
--rw-r--r--   0 paul       (501) staff       (20)     5156 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons/buttons.colVis.js
--rw-r--r--   0 paul       (501) staff       (20)     2704 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons/buttons.colVis.min.js
--rw-r--r--   0 paul       (501) staff       (20)    45617 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons/buttons.flash.js
--rw-r--r--   0 paul       (501) staff       (20)    25454 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons/buttons.flash.min.js
--rw-r--r--   0 paul       (501) staff       (20)    42036 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons/buttons.html5.js
--rw-r--r--   0 paul       (501) staff       (20)    23418 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons/buttons.html5.min.js
--rw-r--r--   0 paul       (501) staff       (20)     4446 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons/buttons.print.js
--rw-r--r--   0 paul       (501) staff       (20)     1950 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons/buttons.print.min.js
--rw-r--r--   0 paul       (501) staff       (20)    40956 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons/dataTables.buttons.js
--rw-r--r--   0 paul       (501) staff       (20)    16520 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons/dataTables.buttons.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.106040 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons-bs/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.327087 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons-bs/css/
--rw-r--r--   0 paul       (501) staff       (20)     3425 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons-bs/css/buttons.bootstrap.css
--rw-r--r--   0 paul       (501) staff       (20)     2867 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons-bs/css/buttons.bootstrap.min.css
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.329554 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons-bs/js/
--rw-r--r--   0 paul       (501) staff       (20)     1400 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons-bs/js/buttons.bootstrap.js
--rw-r--r--   0 paul       (501) staff       (20)      939 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons-bs/js/buttons.bootstrap.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.106936 dryad2dataverse-0.6.2/docs/dbase_structure/bower/font-awesome/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.335343 dryad2dataverse-0.6.2/docs/dbase_structure/bower/font-awesome/css/
--rw-r--r--   0 paul       (501) staff       (20)    37414 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/font-awesome/css/font-awesome.css
--rw-r--r--   0 paul       (501) staff       (20)    21778 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/font-awesome/css/font-awesome.css.map
--rw-r--r--   0 paul       (501) staff       (20)    31000 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/font-awesome/css/font-awesome.min.css
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.369201 dryad2dataverse-0.6.2/docs/dbase_structure/bower/font-awesome/fonts/
--rw-r--r--   0 paul       (501) staff       (20)   134808 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/font-awesome/fonts/FontAwesome.otf
--rw-r--r--   0 paul       (501) staff       (20)   165742 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.eot
--rw-r--r--   0 paul       (501) staff       (20)   444379 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.svg
--rw-r--r--   0 paul       (501) staff       (20)   165548 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 paul       (501) staff       (20)    98024 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.woff
--rw-r--r--   0 paul       (501) staff       (20)    77160 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.372426 dryad2dataverse-0.6.2/docs/dbase_structure/bower/html5shiv/
--rw-r--r--   0 paul       (501) staff       (20)     2730 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/html5shiv/html5shiv.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.108290 dryad2dataverse-0.6.2/docs/dbase_structure/bower/ionicons/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.375346 dryad2dataverse-0.6.2/docs/dbase_structure/bower/ionicons/css/
--rw-r--r--   0 paul       (501) staff       (20)    57193 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/ionicons/css/ionicons.css
--rw-r--r--   0 paul       (501) staff       (20)    51284 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/ionicons/css/ionicons.min.css
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.389346 dryad2dataverse-0.6.2/docs/dbase_structure/bower/ionicons/fonts/
--rw-r--r--   0 paul       (501) staff       (20)   120724 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/ionicons/fonts/ionicons.eot
--rw-r--r--   0 paul       (501) staff       (20)   333834 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/ionicons/fonts/ionicons.svg
--rw-r--r--   0 paul       (501) staff       (20)   188508 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/ionicons/fonts/ionicons.ttf
--rw-r--r--   0 paul       (501) staff       (20)    67904 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/ionicons/fonts/ionicons.woff
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.391471 dryad2dataverse-0.6.2/docs/dbase_structure/bower/jquery/
--rw-r--r--   0 paul       (501) staff       (20)   268039 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/jquery/jquery.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.395980 dryad2dataverse-0.6.2/docs/dbase_structure/bower/js-xlsx/
--rw-r--r--   0 paul       (501) staff       (20)   889680 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/js-xlsx/xlsx.full.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.415152 dryad2dataverse-0.6.2/docs/dbase_structure/bower/pdfmake/
--rw-r--r--   0 paul       (501) staff       (20)   971544 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/pdfmake/pdfmake.min.js
--rw-r--r--   0 paul       (501) staff       (20)   870284 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/pdfmake/vfs_fonts.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.423783 dryad2dataverse-0.6.2/docs/dbase_structure/bower/respond/
--rw-r--r--   0 paul       (501) staff       (20)     4377 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/respond/respond.min.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.428581 dryad2dataverse-0.6.2/docs/dbase_structure/bower/salvattore/
--rw-r--r--   0 paul       (501) staff       (20)     1010 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/salvattore/salvattore.css
--rw-r--r--   0 paul       (501) staff       (20)     7493 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/bower/salvattore/salvattore.min.js
--rw-r--r--   0 paul       (501) staff       (20)     3176 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/column.js
--rw-r--r--   0 paul       (501) staff       (20)    16507 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/columns.html
--rw-r--r--   0 paul       (501) staff       (20)      380 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/constraint.js
--rw-r--r--   0 paul       (501) staff       (20)    15861 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/constraints.html
--rw-r--r--   0 paul       (501) staff       (20)       63 2023-05-03 16:16:07.000000 dryad2dataverse-0.6.2/docs/dbase_structure/deletionOrder.txt
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.111883 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.430815 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/orphans/
--rw-r--r--   0 paul       (501) staff       (20)     1179 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/orphans/orphans.dot
--rw-r--r--   0 paul       (501) staff       (20)     6317 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/orphans/orphans.png
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.435976 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/summary/
--rw-r--r--   0 paul       (501) staff       (20)     5456 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/summary/relationships.real.compact.dot
--rw-r--r--   0 paul       (501) staff       (20)    36361 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/summary/relationships.real.compact.png
--rw-r--r--   0 paul       (501) staff       (20)     8661 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/summary/relationships.real.large.dot
--rw-r--r--   0 paul       (501) staff       (20)    47530 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/summary/relationships.real.large.png
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.466389 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/
--rw-r--r--   0 paul       (501) staff       (20)     2669 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dryadFiles.1degree.dot
--rw-r--r--   0 paul       (501) staff       (20)    17276 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dryadFiles.1degree.png
--rw-r--r--   0 paul       (501) staff       (20)     4823 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dryadFiles.2degrees.dot
--rw-r--r--   0 paul       (501) staff       (20)    43300 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dryadFiles.2degrees.png
--rw-r--r--   0 paul       (501) staff       (20)     6778 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dryadStudy.1degree.dot
--rw-r--r--   0 paul       (501) staff       (20)    47100 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dryadStudy.1degree.png
--rw-r--r--   0 paul       (501) staff       (20)     3965 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dvFiles.1degree.dot
--rw-r--r--   0 paul       (501) staff       (20)    24110 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dvFiles.1degree.png
--rw-r--r--   0 paul       (501) staff       (20)     6134 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dvFiles.2degrees.dot
--rw-r--r--   0 paul       (501) staff       (20)    48156 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dvFiles.2degrees.png
--rw-r--r--   0 paul       (501) staff       (20)     2633 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dvStudy.1degree.dot
--rw-r--r--   0 paul       (501) staff       (20)    15977 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dvStudy.1degree.png
--rw-r--r--   0 paul       (501) staff       (20)     4802 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dvStudy.2degrees.dot
--rw-r--r--   0 paul       (501) staff       (20)    41663 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dvStudy.2degrees.png
--rw-r--r--   0 paul       (501) staff       (20)     3001 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/failed_uploads.1degree.dot
--rw-r--r--   0 paul       (501) staff       (20)    19748 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/failed_uploads.1degree.png
--rw-r--r--   0 paul       (501) staff       (20)     5135 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/failed_uploads.2degrees.dot
--rw-r--r--   0 paul       (501) staff       (20)    44662 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/failed_uploads.2degrees.png
--rw-r--r--   0 paul       (501) staff       (20)     1247 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/lastcheck.1degree.dot
--rw-r--r--   0 paul       (501) staff       (20)     8986 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/lastcheck.1degree.png
--rw-r--r--   0 paul       (501) staff       (20)     4925 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/dryad_dataverse_monitor.sqlite3.%.xml
--rw-r--r--   0 paul       (501) staff       (20)     1411 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/favicon.png
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.112899 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.478705 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/indieflower/
--rw-r--r--   0 paul       (501) staff       (20)    20885 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.eot
--rw-r--r--   0 paul       (501) staff       (20)   133421 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.svg
--rw-r--r--   0 paul       (501) staff       (20)    34336 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.ttf
--rw-r--r--   0 paul       (501) staff       (20)    22020 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.woff
--rw-r--r--   0 paul       (501) staff       (20)    19348 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.woff2
--rw-r--r--   0 paul       (501) staff       (20)      678 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/indieflower/indie-flower.css
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.539431 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/
--rw-r--r--   0 paul       (501) staff       (20)    17228 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.eot
--rw-r--r--   0 paul       (501) staff       (20)    60850 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.svg
--rw-r--r--   0 paul       (501) staff       (20)    37012 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.ttf
--rw-r--r--   0 paul       (501) staff       (20)    18364 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.woff
--rw-r--r--   0 paul       (501) staff       (20)    14588 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.woff2
--rw-r--r--   0 paul       (501) staff       (20)    16121 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.eot
--rw-r--r--   0 paul       (501) staff       (20)    61886 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.svg
--rw-r--r--   0 paul       (501) staff       (20)    34424 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.ttf
--rw-r--r--   0 paul       (501) staff       (20)    17524 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.woff
--rw-r--r--   0 paul       (501) staff       (20)    13856 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.woff2
--rw-r--r--   0 paul       (501) staff       (20)    17220 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.eot
--rw-r--r--   0 paul       (501) staff       (20)    58839 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.svg
--rw-r--r--   0 paul       (501) staff       (20)    36492 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.ttf
--rw-r--r--   0 paul       (501) staff       (20)    18284 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.woff
--rw-r--r--   0 paul       (501) staff       (20)    14508 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.woff2
--rw-r--r--   0 paul       (501) staff       (20)    16137 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.eot
--rw-r--r--   0 paul       (501) staff       (20)    61170 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.svg
--rw-r--r--   0 paul       (501) staff       (20)    34044 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.ttf
--rw-r--r--   0 paul       (501) staff       (20)    17368 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.woff
--rw-r--r--   0 paul       (501) staff       (20)    13688 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.woff2
--rw-r--r--   0 paul       (501) staff       (20)    16896 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.eot
--rw-r--r--   0 paul       (501) staff       (20)    58483 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.svg
--rw-r--r--   0 paul       (501) staff       (20)    36516 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.ttf
--rw-r--r--   0 paul       (501) staff       (20)    18056 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.woff
--rw-r--r--   0 paul       (501) staff       (20)    14440 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.woff2
--rw-r--r--   0 paul       (501) staff       (20)    17231 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.eot
--rw-r--r--   0 paul       (501) staff       (20)    60072 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.svg
--rw-r--r--   0 paul       (501) staff       (20)    36828 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.ttf
--rw-r--r--   0 paul       (501) staff       (20)    18364 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.woff
--rw-r--r--   0 paul       (501) staff       (20)    14624 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.woff2
--rw-r--r--   0 paul       (501) staff       (20)     4561 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro.css
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.543604 dryad2dataverse-0.6.2/docs/dbase_structure/images/
--rw-r--r--   0 paul       (501) staff       (20)     6781 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/images/foreignKey.png
--rw-r--r--   0 paul       (501) staff       (20)     1494 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/images/foreignKeys.png
--rw-r--r--   0 paul       (501) staff       (20)     6781 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/images/primaryKey.png
--rw-r--r--   0 paul       (501) staff       (20)     1494 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/images/primaryKeys.png
--rw-r--r--   0 paul       (501) staff       (20)    19325 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/index.html
--rw-r--r--   0 paul       (501) staff       (20)      147 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/info-html.txt
--rw-r--r--   0 paul       (501) staff       (20)       63 2023-05-03 16:16:07.000000 dryad2dataverse-0.6.2/docs/dbase_structure/insertionOrder.txt
--rw-r--r--   0 paul       (501) staff       (20)     1593 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/main.js
--rw-r--r--   0 paul       (501) staff       (20)     8284 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/orphans.html
--rw-r--r--   0 paul       (501) staff       (20)    10931 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/relationships.html
--rw-r--r--   0 paul       (501) staff       (20)      410 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/relationships.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.545149 dryad2dataverse-0.6.2/docs/dbase_structure/routines/
--rw-r--r--   0 paul       (501) staff       (20)      750 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/routines/routine.js
--rw-r--r--   0 paul       (501) staff       (20)     9154 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/routines.html
--rw-r--r--   0 paul       (501) staff       (20)     2069 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/routines.js
--rw-r--r--   0 paul       (501) staff       (20)     2535 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/schemaSpy.css
--rw-r--r--   0 paul       (501) staff       (20)     1622 2023-05-03 16:15:28.000000 dryad2dataverse-0.6.2/docs/dbase_structure/schemaSpy.js
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.553531 dryad2dataverse-0.6.2/docs/dbase_structure/tables/
--rw-r--r--   0 paul       (501) staff       (20)    15902 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/tables/dryadFiles.html
--rw-r--r--   0 paul       (501) staff       (20)    21507 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/tables/dryadStudy.html
--rw-r--r--   0 paul       (501) staff       (20)    19567 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/tables/dvFiles.html
--rw-r--r--   0 paul       (501) staff       (20)    15866 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/tables/dvStudy.html
--rw-r--r--   0 paul       (501) staff       (20)    16840 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/tables/failed_uploads.html
--rw-r--r--   0 paul       (501) staff       (20)    12927 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/tables/lastcheck.html
--rw-r--r--   0 paul       (501) staff       (20)     1963 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/dbase_structure/tables/table.js
--rw-r--r--   0 paul       (501) staff       (20)     8840 2022-12-07 23:40:02.000000 dryad2dataverse-0.6.2/docs/faq.md
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.555477 dryad2dataverse-0.6.2/docs/images/
--rw-r--r--   0 paul       (501) staff       (20)    30150 2021-11-29 23:23:24.000000 dryad2dataverse-0.6.2/docs/images/dryad2dataverseLogo.png
--rw-r--r--   0 paul       (501) staff       (20)    11191 2021-11-29 23:23:24.000000 dryad2dataverse-0.6.2/docs/images/dryad2dataverseLogo.svg
--rw-r--r--   0 paul       (501) staff       (20)     5538 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/index.md
--rw-r--r--   0 paul       (501) staff       (20)     2518 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/installation.md
--rw-r--r--   0 paul       (501) staff       (20)      473 2022-02-04 19:47:46.000000 dryad2dataverse-0.6.2/docs/other_utils.md
--rw-r--r--   0 paul       (501) staff       (20)     1132 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/pydoc-markdown.yml
--rw-r--r--   0 paul       (501) staff       (20)     5219 2021-11-29 23:23:24.000000 dryad2dataverse-0.6.2/docs/reference.md
--rw-r--r--   0 paul       (501) staff       (20)     8280 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/docs/script.md
--rw-r--r--   0 paul       (501) staff       (20)      294 2021-11-29 23:23:24.000000 dryad2dataverse-0.6.2/docs/track.md
--rw-r--r--   0 paul       (501) staff       (20)     1136 2021-11-29 23:23:24.000000 dryad2dataverse-0.6.2/license.md
--rw-r--r--   0 paul       (501) staff       (20)      705 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/mkdocs.yml
--rw-r--r--   0 paul       (501) staff       (20)     1933 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/pyproject.toml
--rw-r--r--   0 paul       (501) staff       (20)      129 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/requirements.txt
--rw-r--r--   0 paul       (501) staff       (20)       38 2023-08-24 16:57:05.585906 dryad2dataverse-0.6.2/setup.cfg
--rw-r--r--   0 paul       (501) staff       (20)      450 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/setup.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.117227 dryad2dataverse-0.6.2/src/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.571689 dryad2dataverse-0.6.2/src/dryad2dataverse/
--rw-r--r--   0 paul       (501) staff       (20)      712 2023-08-24 16:56:30.000000 dryad2dataverse-0.6.2/src/dryad2dataverse/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)     1429 2023-05-11 15:52:57.000000 dryad2dataverse-0.6.2/src/dryad2dataverse/constants.py
--rw-r--r--   0 paul       (501) staff       (20)     1008 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/src/dryad2dataverse/exceptions.py
--rw-r--r--   0 paul       (501) staff       (20)     1487 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/src/dryad2dataverse/handlers.py
--rw-r--r--   0 paul       (501) staff       (20)    26267 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/src/dryad2dataverse/monitor.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.577930 dryad2dataverse-0.6.2/src/dryad2dataverse/scripts/
--rw-r--r--   0 paul       (501) staff       (20)    26291 2023-08-24 16:56:30.000000 dryad2dataverse-0.6.2/src/dryad2dataverse/scripts/dryadd.py
--rw-r--r--   0 paul       (501) staff       (20)    33476 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/src/dryad2dataverse/serializer.py
--rw-r--r--   0 paul       (501) staff       (20)    34125 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/src/dryad2dataverse/transfer.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.576979 dryad2dataverse-0.6.2/src/dryad2dataverse.egg-info/
--rw-r--r--   0 paul       (501) staff       (20)     3019 2023-08-24 16:57:04.000000 dryad2dataverse-0.6.2/src/dryad2dataverse.egg-info/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)    11378 2023-08-24 16:57:05.000000 dryad2dataverse-0.6.2/src/dryad2dataverse.egg-info/SOURCES.txt
--rw-r--r--   0 paul       (501) staff       (20)        1 2023-08-24 16:57:04.000000 dryad2dataverse-0.6.2/src/dryad2dataverse.egg-info/dependency_links.txt
--rw-r--r--   0 paul       (501) staff       (20)       63 2023-08-24 16:57:04.000000 dryad2dataverse-0.6.2/src/dryad2dataverse.egg-info/entry_points.txt
--rw-r--r--   0 paul       (501) staff       (20)      129 2023-08-24 16:57:04.000000 dryad2dataverse-0.6.2/src/dryad2dataverse.egg-info/requires.txt
--rw-r--r--   0 paul       (501) staff       (20)       16 2023-08-24 16:57:04.000000 dryad2dataverse-0.6.2/src/dryad2dataverse.egg-info/top_level.txt
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-24 16:57:05.584232 dryad2dataverse-0.6.2/tests/
--rw-r--r--   0 paul       (501) staff       (20)        0 2021-09-22 18:45:47.000000 dryad2dataverse-0.6.2/tests/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)     8799 2021-11-29 23:23:24.000000 dryad2dataverse-0.6.2/tests/badURL.json
--rw-r--r--   0 paul       (501) staff       (20)     6281 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/tests/tests_monitor.py
--rw-r--r--   0 paul       (501) staff       (20)    12401 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/tests/tests_serializer.py
--rw-r--r--   0 paul       (501) staff       (20)     2466 2023-05-03 20:42:13.000000 dryad2dataverse-0.6.2/tests/tests_transfer.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:07.941864 dryad2dataverse-0.7.1/
+-rw-r--r--   0 paul       (501) staff       (20)      485 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/.gitignore
+-rw-r--r--   0 paul       (501) staff       (20)     3289 2024-04-25 17:56:07.940171 dryad2dataverse-0.7.1/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)     2033 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/README.md
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.473713 dryad2dataverse-0.7.1/docs/
+-rw-r--r--   0 paul       (501) staff       (20)      442 2021-11-29 23:23:23.000000 dryad2dataverse-0.7.1/docs/_config.yml
+-rw-r--r--   0 paul       (501) staff       (20)    32285 2024-02-29 23:34:53.000000 dryad2dataverse-0.7.1/docs/api_reference.md
+-rw-r--r--   0 paul       (501) staff       (20)     5035 2023-05-11 16:15:57.000000 dryad2dataverse-0.7.1/docs/changelog.md
+-rw-r--r--   0 paul       (501) staff       (20)     1631 2022-04-14 21:51:21.000000 dryad2dataverse-0.7.1/docs/compiling.md
+-rw-r--r--   0 paul       (501) staff       (20)     1152 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/credits.md
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.474485 dryad2dataverse-0.7.1/docs/css/
+-rw-r--r--   0 paul       (501) staff       (20)      473 2022-02-04 19:47:46.000000 dryad2dataverse-0.7.1/docs/css/extra.css
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.533464 dryad2dataverse-0.7.1/docs/dbase_structure/
+-rw-r--r--   0 paul       (501) staff       (20)    19355 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/anomalies.html
+-rw-r--r--   0 paul       (501) staff       (20)        0 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/anomalies.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.383328 dryad2dataverse-0.7.1/docs/dbase_structure/bower/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.373058 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.372644 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.666725 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/
+-rw-r--r--   0 paul       (501) staff       (20)    26132 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.css
+-rw-r--r--   0 paul       (501) staff       (20)    47706 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.css.map
+-rw-r--r--   0 paul       (501) staff       (20)    23409 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.min.css
+-rw-r--r--   0 paul       (501) staff       (20)    25648 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.min.css.map
+-rw-r--r--   0 paul       (501) staff       (20)   146010 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.css
+-rw-r--r--   0 paul       (501) staff       (20)   389287 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0 paul       (501) staff       (20)   121200 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0 paul       (501) staff       (20)   542194 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.min.css.map
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.739515 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/
+-rw-r--r--   0 paul       (501) staff       (20)    20127 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 paul       (501) staff       (20)   108738 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 paul       (501) staff       (20)    45404 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 paul       (501) staff       (20)    23424 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 paul       (501) staff       (20)    18028 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.749548 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/js/
+-rw-r--r--   0 paul       (501) staff       (20)    69707 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/js/bootstrap.js
+-rw-r--r--   0 paul       (501) staff       (20)    37045 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0 paul       (501) staff       (20)      484 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/js/npm.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.374519 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/plugins/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.752877 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/plugins/fastclick/
+-rw-r--r--   0 paul       (501) staff       (20)    25965 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/plugins/fastclick/fastclick.js
+-rw-r--r--   0 paul       (501) staff       (20)     8776 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/plugins/fastclick/fastclick.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.754397 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/plugins/jQuery/
+-rw-r--r--   0 paul       (501) staff       (20)    85659 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/plugins/jQuery/jquery-2.2.3.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.764114 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/plugins/jQueryUI/
+-rw-r--r--   0 paul       (501) staff       (20)   470596 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/plugins/jQueryUI/jquery-ui.js
+-rw-r--r--   0 paul       (501) staff       (20)   240427 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/plugins/jQueryUI/jquery-ui.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.769353 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/plugins/slimScroll/
+-rw-r--r--   0 paul       (501) staff       (20)    13832 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/plugins/slimScroll/jquery.slimscroll.js
+-rw-r--r--   0 paul       (501) staff       (20)     4724 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/plugins/slimScroll/jquery.slimscroll.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.770522 dryad2dataverse-0.7.1/docs/dbase_structure/bower/anchor-js/
+-rw-r--r--   0 paul       (501) staff       (20)     5332 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/anchor-js/anchor.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.779326 dryad2dataverse-0.7.1/docs/dbase_structure/bower/codemirror/
+-rw-r--r--   0 paul       (501) staff       (20)     8241 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/codemirror/codemirror.css
+-rw-r--r--   0 paul       (501) staff       (20)   365757 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/codemirror/codemirror.js
+-rw-r--r--   0 paul       (501) staff       (20)    37494 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/codemirror/sql.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.781186 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net/
+-rw-r--r--   0 paul       (501) staff       (20)    83268 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net/jquery.dataTables.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.376714 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-bs/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.852287 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-bs/css/
+-rw-r--r--   0 paul       (501) staff       (20)     4823 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-bs/css/dataTables.bootstrap.css
+-rw-r--r--   0 paul       (501) staff       (20)     4188 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-bs/css/dataTables.bootstrap.min.css
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.855029 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-bs/js/
+-rw-r--r--   0 paul       (501) staff       (20)     4559 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-bs/js/dataTables.bootstrap.js
+-rw-r--r--   0 paul       (501) staff       (20)     1966 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-bs/js/dataTables.bootstrap.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.871103 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons/
+-rw-r--r--   0 paul       (501) staff       (20)     5156 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.colVis.js
+-rw-r--r--   0 paul       (501) staff       (20)     2704 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.colVis.min.js
+-rw-r--r--   0 paul       (501) staff       (20)    45617 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.flash.js
+-rw-r--r--   0 paul       (501) staff       (20)    25454 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.flash.min.js
+-rw-r--r--   0 paul       (501) staff       (20)    42036 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.html5.js
+-rw-r--r--   0 paul       (501) staff       (20)    23418 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.html5.min.js
+-rw-r--r--   0 paul       (501) staff       (20)     4446 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.print.js
+-rw-r--r--   0 paul       (501) staff       (20)     1950 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.print.min.js
+-rw-r--r--   0 paul       (501) staff       (20)    40956 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons/dataTables.buttons.js
+-rw-r--r--   0 paul       (501) staff       (20)    16520 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons/dataTables.buttons.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.378276 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons-bs/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.874945 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons-bs/css/
+-rw-r--r--   0 paul       (501) staff       (20)     3425 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons-bs/css/buttons.bootstrap.css
+-rw-r--r--   0 paul       (501) staff       (20)     2867 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons-bs/css/buttons.bootstrap.min.css
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.878289 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons-bs/js/
+-rw-r--r--   0 paul       (501) staff       (20)     1400 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons-bs/js/buttons.bootstrap.js
+-rw-r--r--   0 paul       (501) staff       (20)      939 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons-bs/js/buttons.bootstrap.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.379212 dryad2dataverse-0.7.1/docs/dbase_structure/bower/font-awesome/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.882956 dryad2dataverse-0.7.1/docs/dbase_structure/bower/font-awesome/css/
+-rw-r--r--   0 paul       (501) staff       (20)    37414 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/font-awesome/css/font-awesome.css
+-rw-r--r--   0 paul       (501) staff       (20)    21778 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/font-awesome/css/font-awesome.css.map
+-rw-r--r--   0 paul       (501) staff       (20)    31000 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/font-awesome/css/font-awesome.min.css
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.977146 dryad2dataverse-0.7.1/docs/dbase_structure/bower/font-awesome/fonts/
+-rw-r--r--   0 paul       (501) staff       (20)   134808 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/font-awesome/fonts/FontAwesome.otf
+-rw-r--r--   0 paul       (501) staff       (20)   165742 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 paul       (501) staff       (20)   444379 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 paul       (501) staff       (20)   165548 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 paul       (501) staff       (20)    98024 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 paul       (501) staff       (20)    77160 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.981329 dryad2dataverse-0.7.1/docs/dbase_structure/bower/html5shiv/
+-rw-r--r--   0 paul       (501) staff       (20)     2730 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/html5shiv/html5shiv.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.381425 dryad2dataverse-0.7.1/docs/dbase_structure/bower/ionicons/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.988880 dryad2dataverse-0.7.1/docs/dbase_structure/bower/ionicons/css/
+-rw-r--r--   0 paul       (501) staff       (20)    57193 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/ionicons/css/ionicons.css
+-rw-r--r--   0 paul       (501) staff       (20)    51284 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/ionicons/css/ionicons.min.css
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:07.074568 dryad2dataverse-0.7.1/docs/dbase_structure/bower/ionicons/fonts/
+-rw-r--r--   0 paul       (501) staff       (20)   120724 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/ionicons/fonts/ionicons.eot
+-rw-r--r--   0 paul       (501) staff       (20)   333834 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/ionicons/fonts/ionicons.svg
+-rw-r--r--   0 paul       (501) staff       (20)   188508 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/ionicons/fonts/ionicons.ttf
+-rw-r--r--   0 paul       (501) staff       (20)    67904 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/ionicons/fonts/ionicons.woff
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:07.077036 dryad2dataverse-0.7.1/docs/dbase_structure/bower/jquery/
+-rw-r--r--   0 paul       (501) staff       (20)   268039 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/jquery/jquery.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:07.083170 dryad2dataverse-0.7.1/docs/dbase_structure/bower/js-xlsx/
+-rw-r--r--   0 paul       (501) staff       (20)   889680 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/js-xlsx/xlsx.full.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:07.101825 dryad2dataverse-0.7.1/docs/dbase_structure/bower/pdfmake/
+-rw-r--r--   0 paul       (501) staff       (20)   971544 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/pdfmake/pdfmake.min.js
+-rw-r--r--   0 paul       (501) staff       (20)   870284 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/pdfmake/vfs_fonts.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:07.111239 dryad2dataverse-0.7.1/docs/dbase_structure/bower/respond/
+-rw-r--r--   0 paul       (501) staff       (20)     4377 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/respond/respond.min.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:07.114410 dryad2dataverse-0.7.1/docs/dbase_structure/bower/salvattore/
+-rw-r--r--   0 paul       (501) staff       (20)     1010 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/salvattore/salvattore.css
+-rw-r--r--   0 paul       (501) staff       (20)     7493 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/bower/salvattore/salvattore.min.js
+-rw-r--r--   0 paul       (501) staff       (20)     3176 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/column.js
+-rw-r--r--   0 paul       (501) staff       (20)    16507 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/columns.html
+-rw-r--r--   0 paul       (501) staff       (20)      380 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/constraint.js
+-rw-r--r--   0 paul       (501) staff       (20)    15861 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/constraints.html
+-rw-r--r--   0 paul       (501) staff       (20)       63 2023-05-03 16:16:07.000000 dryad2dataverse-0.7.1/docs/dbase_structure/deletionOrder.txt
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.447276 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:07.117274 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/orphans/
+-rw-r--r--   0 paul       (501) staff       (20)     1179 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/orphans/orphans.dot
+-rw-r--r--   0 paul       (501) staff       (20)     6317 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/orphans/orphans.png
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:07.169433 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/summary/
+-rw-r--r--   0 paul       (501) staff       (20)     5456 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/summary/relationships.real.compact.dot
+-rw-r--r--   0 paul       (501) staff       (20)    36361 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/summary/relationships.real.compact.png
+-rw-r--r--   0 paul       (501) staff       (20)     8661 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/summary/relationships.real.large.dot
+-rw-r--r--   0 paul       (501) staff       (20)    47530 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/summary/relationships.real.large.png
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:07.305073 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/
+-rw-r--r--   0 paul       (501) staff       (20)     2669 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dryadFiles.1degree.dot
+-rw-r--r--   0 paul       (501) staff       (20)    17276 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dryadFiles.1degree.png
+-rw-r--r--   0 paul       (501) staff       (20)     4823 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dryadFiles.2degrees.dot
+-rw-r--r--   0 paul       (501) staff       (20)    43300 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dryadFiles.2degrees.png
+-rw-r--r--   0 paul       (501) staff       (20)     6778 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dryadStudy.1degree.dot
+-rw-r--r--   0 paul       (501) staff       (20)    47100 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dryadStudy.1degree.png
+-rw-r--r--   0 paul       (501) staff       (20)     3965 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dvFiles.1degree.dot
+-rw-r--r--   0 paul       (501) staff       (20)    24110 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dvFiles.1degree.png
+-rw-r--r--   0 paul       (501) staff       (20)     6134 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dvFiles.2degrees.dot
+-rw-r--r--   0 paul       (501) staff       (20)    48156 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dvFiles.2degrees.png
+-rw-r--r--   0 paul       (501) staff       (20)     2633 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dvStudy.1degree.dot
+-rw-r--r--   0 paul       (501) staff       (20)    15977 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dvStudy.1degree.png
+-rw-r--r--   0 paul       (501) staff       (20)     4802 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dvStudy.2degrees.dot
+-rw-r--r--   0 paul       (501) staff       (20)    41663 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dvStudy.2degrees.png
+-rw-r--r--   0 paul       (501) staff       (20)     3001 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/failed_uploads.1degree.dot
+-rw-r--r--   0 paul       (501) staff       (20)    19748 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/failed_uploads.1degree.png
+-rw-r--r--   0 paul       (501) staff       (20)     5135 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/failed_uploads.2degrees.dot
+-rw-r--r--   0 paul       (501) staff       (20)    44662 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/failed_uploads.2degrees.png
+-rw-r--r--   0 paul       (501) staff       (20)     1247 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/lastcheck.1degree.dot
+-rw-r--r--   0 paul       (501) staff       (20)     8986 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/lastcheck.1degree.png
+-rw-r--r--   0 paul       (501) staff       (20)     4925 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/dryad_dataverse_monitor.sqlite3.%.xml
+-rw-r--r--   0 paul       (501) staff       (20)     1411 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/favicon.png
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.448235 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:07.392689 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/indieflower/
+-rw-r--r--   0 paul       (501) staff       (20)    20885 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.eot
+-rw-r--r--   0 paul       (501) staff       (20)   133421 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.svg
+-rw-r--r--   0 paul       (501) staff       (20)    34336 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.ttf
+-rw-r--r--   0 paul       (501) staff       (20)    22020 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.woff
+-rw-r--r--   0 paul       (501) staff       (20)    19348 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.woff2
+-rw-r--r--   0 paul       (501) staff       (20)      678 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/indieflower/indie-flower.css
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:07.678572 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/
+-rw-r--r--   0 paul       (501) staff       (20)    17228 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.eot
+-rw-r--r--   0 paul       (501) staff       (20)    60850 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.svg
+-rw-r--r--   0 paul       (501) staff       (20)    37012 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.ttf
+-rw-r--r--   0 paul       (501) staff       (20)    18364 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.woff
+-rw-r--r--   0 paul       (501) staff       (20)    14588 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.woff2
+-rw-r--r--   0 paul       (501) staff       (20)    16121 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.eot
+-rw-r--r--   0 paul       (501) staff       (20)    61886 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.svg
+-rw-r--r--   0 paul       (501) staff       (20)    34424 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.ttf
+-rw-r--r--   0 paul       (501) staff       (20)    17524 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.woff
+-rw-r--r--   0 paul       (501) staff       (20)    13856 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.woff2
+-rw-r--r--   0 paul       (501) staff       (20)    17220 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.eot
+-rw-r--r--   0 paul       (501) staff       (20)    58839 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.svg
+-rw-r--r--   0 paul       (501) staff       (20)    36492 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.ttf
+-rw-r--r--   0 paul       (501) staff       (20)    18284 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.woff
+-rw-r--r--   0 paul       (501) staff       (20)    14508 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.woff2
+-rw-r--r--   0 paul       (501) staff       (20)    16137 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.eot
+-rw-r--r--   0 paul       (501) staff       (20)    61170 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.svg
+-rw-r--r--   0 paul       (501) staff       (20)    34044 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.ttf
+-rw-r--r--   0 paul       (501) staff       (20)    17368 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.woff
+-rw-r--r--   0 paul       (501) staff       (20)    13688 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.woff2
+-rw-r--r--   0 paul       (501) staff       (20)    16896 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.eot
+-rw-r--r--   0 paul       (501) staff       (20)    58483 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.svg
+-rw-r--r--   0 paul       (501) staff       (20)    36516 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.ttf
+-rw-r--r--   0 paul       (501) staff       (20)    18056 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.woff
+-rw-r--r--   0 paul       (501) staff       (20)    14440 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.woff2
+-rw-r--r--   0 paul       (501) staff       (20)    17231 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.eot
+-rw-r--r--   0 paul       (501) staff       (20)    60072 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.svg
+-rw-r--r--   0 paul       (501) staff       (20)    36828 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.ttf
+-rw-r--r--   0 paul       (501) staff       (20)    18364 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.woff
+-rw-r--r--   0 paul       (501) staff       (20)    14624 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.woff2
+-rw-r--r--   0 paul       (501) staff       (20)     4561 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro.css
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:07.685837 dryad2dataverse-0.7.1/docs/dbase_structure/images/
+-rw-r--r--   0 paul       (501) staff       (20)     6781 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/images/foreignKey.png
+-rw-r--r--   0 paul       (501) staff       (20)     1494 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/images/foreignKeys.png
+-rw-r--r--   0 paul       (501) staff       (20)     6781 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/images/primaryKey.png
+-rw-r--r--   0 paul       (501) staff       (20)     1494 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/images/primaryKeys.png
+-rw-r--r--   0 paul       (501) staff       (20)    19325 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/index.html
+-rw-r--r--   0 paul       (501) staff       (20)      147 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/info-html.txt
+-rw-r--r--   0 paul       (501) staff       (20)       63 2023-05-03 16:16:07.000000 dryad2dataverse-0.7.1/docs/dbase_structure/insertionOrder.txt
+-rw-r--r--   0 paul       (501) staff       (20)     1593 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/main.js
+-rw-r--r--   0 paul       (501) staff       (20)     8284 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/orphans.html
+-rw-r--r--   0 paul       (501) staff       (20)    10931 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/relationships.html
+-rw-r--r--   0 paul       (501) staff       (20)      410 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/relationships.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:07.686868 dryad2dataverse-0.7.1/docs/dbase_structure/routines/
+-rw-r--r--   0 paul       (501) staff       (20)      750 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/routines/routine.js
+-rw-r--r--   0 paul       (501) staff       (20)     9154 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/routines.html
+-rw-r--r--   0 paul       (501) staff       (20)     2069 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/routines.js
+-rw-r--r--   0 paul       (501) staff       (20)     2535 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/schemaSpy.css
+-rw-r--r--   0 paul       (501) staff       (20)     1622 2023-05-03 16:15:28.000000 dryad2dataverse-0.7.1/docs/dbase_structure/schemaSpy.js
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:07.800635 dryad2dataverse-0.7.1/docs/dbase_structure/tables/
+-rw-r--r--   0 paul       (501) staff       (20)    15902 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/tables/dryadFiles.html
+-rw-r--r--   0 paul       (501) staff       (20)    21507 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/tables/dryadStudy.html
+-rw-r--r--   0 paul       (501) staff       (20)    19567 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/tables/dvFiles.html
+-rw-r--r--   0 paul       (501) staff       (20)    15866 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/tables/dvStudy.html
+-rw-r--r--   0 paul       (501) staff       (20)    16840 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/tables/failed_uploads.html
+-rw-r--r--   0 paul       (501) staff       (20)    12927 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/tables/lastcheck.html
+-rw-r--r--   0 paul       (501) staff       (20)     1963 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/dbase_structure/tables/table.js
+-rw-r--r--   0 paul       (501) staff       (20)     8840 2022-12-07 23:40:02.000000 dryad2dataverse-0.7.1/docs/faq.md
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:07.804721 dryad2dataverse-0.7.1/docs/images/
+-rw-r--r--   0 paul       (501) staff       (20)    30150 2021-11-29 23:23:24.000000 dryad2dataverse-0.7.1/docs/images/dryad2dataverseLogo.png
+-rw-r--r--   0 paul       (501) staff       (20)    11191 2021-11-29 23:23:24.000000 dryad2dataverse-0.7.1/docs/images/dryad2dataverseLogo.svg
+-rw-r--r--   0 paul       (501) staff       (20)     5538 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/index.md
+-rw-r--r--   0 paul       (501) staff       (20)     2518 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/installation.md
+-rw-r--r--   0 paul       (501) staff       (20)      473 2022-02-04 19:47:46.000000 dryad2dataverse-0.7.1/docs/other_utils.md
+-rw-r--r--   0 paul       (501) staff       (20)     1132 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/pydoc-markdown.yml
+-rw-r--r--   0 paul       (501) staff       (20)     5219 2021-11-29 23:23:24.000000 dryad2dataverse-0.7.1/docs/reference.md
+-rw-r--r--   0 paul       (501) staff       (20)     8280 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/docs/script.md
+-rw-r--r--   0 paul       (501) staff       (20)      294 2021-11-29 23:23:24.000000 dryad2dataverse-0.7.1/docs/track.md
+-rw-r--r--   0 paul       (501) staff       (20)     1136 2021-11-29 23:23:24.000000 dryad2dataverse-0.7.1/license.md
+-rw-r--r--   0 paul       (501) staff       (20)      705 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/mkdocs.yml
+-rw-r--r--   0 paul       (501) staff       (20)     1933 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/pyproject.toml
+-rw-r--r--   0 paul       (501) staff       (20)      150 2024-02-29 23:34:53.000000 dryad2dataverse-0.7.1/requirements.txt
+-rw-r--r--   0 paul       (501) staff       (20)       38 2024-04-25 17:56:07.942162 dryad2dataverse-0.7.1/setup.cfg
+-rw-r--r--   0 paul       (501) staff       (20)      450 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/setup.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:06.451087 dryad2dataverse-0.7.1/src/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:07.815478 dryad2dataverse-0.7.1/src/dryad2dataverse/
+-rw-r--r--   0 paul       (501) staff       (20)      712 2024-04-25 16:39:36.000000 dryad2dataverse-0.7.1/src/dryad2dataverse/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)     1429 2023-05-11 15:52:57.000000 dryad2dataverse-0.7.1/src/dryad2dataverse/constants.py
+-rw-r--r--   0 paul       (501) staff       (20)     1008 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/src/dryad2dataverse/exceptions.py
+-rw-r--r--   0 paul       (501) staff       (20)     1487 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/src/dryad2dataverse/handlers.py
+-rw-r--r--   0 paul       (501) staff       (20)    26267 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/src/dryad2dataverse/monitor.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:07.924576 dryad2dataverse-0.7.1/src/dryad2dataverse/scripts/
+-rw-r--r--   0 paul       (501) staff       (20)    26291 2023-08-24 16:56:30.000000 dryad2dataverse-0.7.1/src/dryad2dataverse/scripts/dryadd.py
+-rw-r--r--   0 paul       (501) staff       (20)    33706 2024-04-25 17:00:10.000000 dryad2dataverse-0.7.1/src/dryad2dataverse/serializer.py
+-rw-r--r--   0 paul       (501) staff       (20)    36233 2024-02-29 23:34:53.000000 dryad2dataverse-0.7.1/src/dryad2dataverse/transfer.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:07.938255 dryad2dataverse-0.7.1/src/dryad2dataverse.egg-info/
+-rw-r--r--   0 paul       (501) staff       (20)     3289 2024-04-25 17:56:06.000000 dryad2dataverse-0.7.1/src/dryad2dataverse.egg-info/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)    11378 2024-04-25 17:56:06.000000 dryad2dataverse-0.7.1/src/dryad2dataverse.egg-info/SOURCES.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2024-04-25 17:56:06.000000 dryad2dataverse-0.7.1/src/dryad2dataverse.egg-info/dependency_links.txt
+-rw-r--r--   0 paul       (501) staff       (20)       63 2024-04-25 17:56:06.000000 dryad2dataverse-0.7.1/src/dryad2dataverse.egg-info/entry_points.txt
+-rw-r--r--   0 paul       (501) staff       (20)      150 2024-04-25 17:56:06.000000 dryad2dataverse-0.7.1/src/dryad2dataverse.egg-info/requires.txt
+-rw-r--r--   0 paul       (501) staff       (20)       16 2024-04-25 17:56:06.000000 dryad2dataverse-0.7.1/src/dryad2dataverse.egg-info/top_level.txt
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2024-04-25 17:56:07.936866 dryad2dataverse-0.7.1/tests/
+-rw-r--r--   0 paul       (501) staff       (20)        0 2021-09-22 18:45:47.000000 dryad2dataverse-0.7.1/tests/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)     8799 2021-11-29 23:23:24.000000 dryad2dataverse-0.7.1/tests/badURL.json
+-rw-r--r--   0 paul       (501) staff       (20)     6281 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/tests/tests_monitor.py
+-rw-r--r--   0 paul       (501) staff       (20)    12401 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/tests/tests_serializer.py
+-rw-r--r--   0 paul       (501) staff       (20)     2466 2023-05-03 20:42:13.000000 dryad2dataverse-0.7.1/tests/tests_transfer.py
```

### Comparing `dryad2dataverse-0.6.2/PKG-INFO` & `dryad2dataverse-0.7.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: dryad2dataverse
-Version: 0.6.2
-Summary: Utility for copying and syncing data from a Dryad data repository to a Dataverse repository
-Author-email: Paul Lesack <paul.lesack@ubc.ca>
-Project-URL: Homepage, https://ubc-library-rc.github.io/dryad2dataverse
-Project-URL: Documentation, https://ubc-library-rc.github.io/dryad2dataverse
-Project-URL: Repository, https://github.com/ubc-library-rc/dryad2dataverse.git
-Project-URL: Tracker, https://github.com/ubc-library-rc/dryad2dataverse/issues
-Keywords: Harvard Dataverse,Dataverse,research data management,data repository,Dryad,datadryad.org,dataverse.org
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Education
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Education
-Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
-Classifier: Topic :: Utilities
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # dryad2dataverse
 
 **dryad2dataverse** is a [Python](https://python.org) package and an associated console line application which allows easier transfer of metadata and data from a Dryad data repository (ie, <https://datadryad.org>) to a [Dataverse](https://dataverse.org/ "Dataverse software main site") repository. Dryad2dataverse is pure Python and should run on any platform which supports Python 3.6 or greater.
 
 Data transfers between repositories require local storage, so not all platforms will be equally suitable.
 
 ## Installing
```

### Comparing `dryad2dataverse-0.6.2/README.md` & `dryad2dataverse-0.7.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: dryad2dataverse
+Version: 0.7.1
+Summary: Utility for copying and syncing data from a Dryad data repository to a Dataverse repository
+Author-email: Paul Lesack <paul.lesack@ubc.ca>
+Project-URL: Homepage, https://ubc-library-rc.github.io/dryad2dataverse
+Project-URL: Documentation, https://ubc-library-rc.github.io/dryad2dataverse
+Project-URL: Repository, https://github.com/ubc-library-rc/dryad2dataverse.git
+Project-URL: Tracker, https://github.com/ubc-library-rc/dryad2dataverse/issues
+Keywords: Harvard Dataverse,Dataverse,research data management,data repository,Dryad,datadryad.org,dataverse.org
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Education
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Education
+Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
+Classifier: Topic :: Utilities
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Requires-Dist: certifi>=2022.12.7
+Requires-Dist: charset-normalizer>=2.0.4
+Requires-Dist: chardet>=3.0.4
+Requires-Dist: idna>=2.10
+Requires-Dist: pycryptodome>=3.20.0
+Requires-Dist: requests>=2.26.0
+Requires-Dist: requests-toolbelt>=0.9.1
+Requires-Dist: urllib3>=1.26.6
+
 # dryad2dataverse
 
 **dryad2dataverse** is a [Python](https://python.org) package and an associated console line application which allows easier transfer of metadata and data from a Dryad data repository (ie, <https://datadryad.org>) to a [Dataverse](https://dataverse.org/ "Dataverse software main site") repository. Dryad2dataverse is pure Python and should run on any platform which supports Python 3.6 or greater.
 
 Data transfers between repositories require local storage, so not all platforms will be equally suitable.
 
 ## Installing
```

### Comparing `dryad2dataverse-0.6.2/docs/api_reference.md` & `dryad2dataverse-0.7.1/docs/api_reference.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 layout: default
 title:  
 nav_order: 15
 ---
 
 # Complete API reference
 
-<a name="dryad2dataverse"></a>
-
 <a id="dryad2dataverse"></a>
 
 ## dryad2dataverse
 
 Dryad to Dataverse utilities. No modules are loaded by default, so
 
 >>> import dryad2dataverse
@@ -275,22 +273,22 @@
 
 **Arguments**:
 
   
   filelist : list
   — List of Dryad file tuples: eg:
   
-  ```
-  [('https://datadryad.org/api/v2/files/385819/download',
-  'GCB_ACG_Mortality_2020.zip',
-  'application/x-zip-compressed', 23787587),
-  ('https://datadryad.org/api/v2/files/385820/download',
-  'Readme_ACG_Mortality.txt',
-  'text/plain', 1350)]
-  ```
+    ```
+    [('https://datadryad.org/api/v2/files/385819/download',
+      'GCB_ACG_Mortality_2020.zip',
+      'application/x-zip-compressed', 23787587),
+     ('https://datadryad.org/api/v2/files/385820/download',
+     'Readme_ACG_Mortality.txt',
+     'text/plain', 1350)]
+     ```
   ----------------------------------------
 
 <a id="dryad2dataverse.monitor.Monitor.get_json_dvfids"></a>
 
 ##### get\_json\_dvfids
 
 ```python
@@ -364,14 +362,20 @@
 
 This module contains the information that configures all the parameters
 required to transfer data from Dryad to Dataverse.
 
 "Constants" may be a bit strong, but the only constant is the
 presence of change.
 
+<a id="dryad2dataverse.constants.MAX_UPLOAD"></a>
+
+##### MAX\_UPLOAD
+
+Max 3GB upload
+
 <a id="dryad2dataverse.handlers"></a>
 
 ## dryad2dataverse.handlers
 
 Custom log handlers for sending log information to recipients.
 
 <a id="dryad2dataverse.handlers.SSLSMTPHandler"></a>
@@ -621,45 +625,52 @@
   ----------------------------------------
 
 <a id="dryad2dataverse.transfer.Transfer.download_file"></a>
 
 ##### download\_file
 
 ```python
-def download_file(url, filename, tmp=None, size=None, chk=None, timeout=45)
+def download_file(url=None,
+                  filename=None,
+                  tmp=None,
+                  size=None,
+                  chk=None,
+                  timeout=45,
+                  **kwargs)
 ```
 
 Downloads a file via requests streaming and saves to constants.TMP.
-returns md5sum on success and an exception on failure.
+returns checksum on success and an exception on failure.
 
 ----------------------------------------
+Required keyword arguments:
 
-**Arguments**:
+url : str
+    — URL of download.
 
-  
-  url : str
-  — URL of download.
-  
-  filename : str
-  — Output file name.
-  
-  timeout : int
-  — Requests timeout.
-  
-  tmp : str
-  — Temporary directory for downloads.
-  Defaults to dryad2dataverse.constants.TMP.
-  
-  size : int
-  — Reported file size in bytes.
-  Defaults to dryad2dataverse.constants.MAX_UPLOAD.
-  
-  chk : str
-  - md5 sum of file (if available and known).
-  ----------------------------------------
+filename : str
+    — Output file name.
+
+timeout : int
+    — Requests timeout.
+
+tmp : str
+    — Temporary directory for downloads.
+      Defaults to dryad2dataverse.constants.TMP.
+
+size : int
+    — Reported file size in bytes.
+      Defaults to dryad2dataverse.constants.MAX_UPLOAD.
+
+digest_type: str
+    — checksum type (ie, md5, sha-256, etc)
+
+chk : str
+    —  checksum of file (if available and known).
+----------------------------------------
 
 <a id="dryad2dataverse.transfer.Transfer.download_files"></a>
 
 ##### download\_files
 
 ```python
 def download_files(files=None)
@@ -931,14 +942,243 @@
   dvurl : str
   — Base URL of Dataverse. Defaults to dryad2dataverse.constants.DVURL.
   
   key : str
   — API key for Dataverse. Defaults to dryad2dataverse.constants.APIKEY.
   ----------------------------------------
 
+<a id="dryad2dataverse.scripts.dryadd"></a>
+
+## dryad2dataverse.scripts.dryadd
+
+Dryad daemon for monitoring and automatically uploading studies associated with a particular ROR
+
+Requires Python 3.6+ and requests library
+
+<a id="dryad2dataverse.scripts.dryadd.new_content"></a>
+
+##### new\_content
+
+```python
+def new_content(serial)
+```
+
+Creates content for new study upload message (potentially redundant
+with Dataverse emailer).
+serial : dryad2dataverse.serializer.Serializer instance
+
+<a id="dryad2dataverse.scripts.dryadd.changed_content"></a>
+
+##### changed\_content
+
+```python
+def changed_content(serial, monitor)
+```
+
+Creates content for file update message.
+serial : dryad2dataverse.serializer.Serializer instance
+monitor : dryad2dataverse.monitor.Monitor instance
+
+<a id="dryad2dataverse.scripts.dryadd.notify"></a>
+
+##### notify
+
+```python
+def notify(msgtxt, width=100, **kwargs)
+```
+
+Basic email change notifier. Will sent email outlining metadata changes
+to recipient. Uses SSL.
+
+Has only really been tested with Gmail (although it should work with anything,
+and Gmail requires 'Allow less secure apps' or whatever they call it.
+If you are having troubles with GMail:
+
+1. Enable less secure access
+
+2. Disable the CAPTCHA:
+https://accounts.google.com/DisplayUnlockCaptcha
+
+Note: Google will automatically revert settings after some arbitrary period
+of time. You have been warned.
+
+If your application worked before but suddenly it crashes with authenication
+errors, this is why.
+
+msgtext : tuple
+Tuple containing strings of ('subject', 'message content')
+width : int
+Maximum line length. Max 1000
+
+From the argument parser these keys and values are required:
+email : str
+From address for account
+user : str
+User name for email account
+pwd : str
+Password for email account
+mailserv : str
+SMTP server for sending mail
+port : int
+Mailserver port. Default 465
+recipients : list
+List of email addresses of recipients
+
+<a id="dryad2dataverse.scripts.dryadd.get_records"></a>
+
+##### get\_records
+
+```python
+def get_records(ror: 'str', mod_date=None, verbosity=True, timeout=100)
+```
+
+returns a tuple of ((doi, metadata), ...). Dryad searches return complete
+study metadata from the search, surprisingly.
+
+ror : str
+    ROR string including http. To find your ROR, see
+    https://ror.org/
+
+mod_date : str
+    UTC datetime string in the format suitable for the Dryad API.
+    eg. 2021-01-21T21:42:40Z
+    or .strftime('%Y-%m-%dT%H:%M:%SZ')
+    if no mod_date is passed, all studies will be retrieved
+
+verbosity : bool
+   Output some data to stdout
+
+timeout : int
+    request timeout in seconds
+
+<a id="dryad2dataverse.scripts.dryadd.argp"></a>
+
+##### argp
+
+```python
+def argp()
+```
+
+Argument parser
+
+<a id="dryad2dataverse.scripts.dryadd.set_constants"></a>
+
+##### set\_constants
+
+```python
+def set_constants(args)
+```
+
+Set the appropriate dryad2dataverse constants
+
+<a id="dryad2dataverse.scripts.dryadd.email_log"></a>
+
+##### email\_log
+
+```python
+def email_log(mailhost,
+              fromaddr,
+              toaddrs,
+              credentials,
+              port=465,
+              secure=(),
+              level=logging.WARNING,
+              timeout=100)
+```
+
+Emails log error messages to recipient
+
+mailhost : str
+    Address of mail server. Eg. smtp.gmail.com
+fromaddr : str
+    "From" address for email
+toaddrs :
+    Recipient of email
+credentials : tuple
+    (Username, password) tuple
+port : Mailserver port. Default 465
+secure : tuple
+    The tuple should be either an empty tuple, or a single-value tuple with
+    the name of a keyfile, or a 2-value tuple with the names of the keyfile
+    and certificate file.
+    See https://docs.python.org/3/library/logging.handlers.html
+level : int
+    logging level. Default logging.WARNING
+
+<a id="dryad2dataverse.scripts.dryadd.rotating_log"></a>
+
+##### rotating\_log
+
+```python
+def rotating_log(path, level)
+```
+
+Create log of transactions
+
+path : str
+    Complete path to log
+level : logging.LOGLEVEL
+    logging level (eg, logging.DEBUG)
+
+<a id="dryad2dataverse.scripts.dryadd.checkwarn"></a>
+
+##### checkwarn
+
+```python
+def checkwarn(val: int, **kwargs) -> None
+```
+
+Halt program execution before processing if threshold value of modified
+Dryad studies exceeded. Useful for checking if the Dryad API has changed
+and caused havoc.
+
+val: int
+    Number of modified or new studies
+kwargs: dict
+    Email notification information.
+    {'user': user email,
+     'recipients':[list of recipients],
+     'pwd' ; email server password],
+     'mailserv' : smtp mail server,
+     'warn': Threshold for number of warnings (int)}
+    see dryadd.notify for full details of parameters.
+
+    Include log info:
+    {loggers: [logging.logger, logging.logger,...]}
+    Skip check
+    {'warn_too_many': bool}
+
+<a id="dryad2dataverse.scripts.dryadd.verbo"></a>
+
+##### verbo
+
+```python
+def verbo(verbosity: bool, **kwargs) -> None
+```
+
+verbosity: bool
+    if True, print dict
+kwargs : dict
+    Dictionary to print out
+
+<a id="dryad2dataverse.scripts.dryadd.main"></a>
+
+##### main
+
+```python
+def main(log='/var/log/dryadd.log', level=logging.WARNING)
+```
+
+Main Dryad transfer daemon
+
+log : str
+    path to logfile
+level : int
+    log level, usually one of logging.LOGLEVEL (ie, logging.warning)
+
 <a id="dryad2dataverse.serializer"></a>
 
 ## dryad2dataverse.serializer
 
 Serializes Dryad study JSON to Dataverse JSON, as well as
 producing associated file information.
```

### Comparing `dryad2dataverse-0.6.2/docs/changelog.md` & `dryad2dataverse-0.7.1/docs/changelog.md`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/compiling.md` & `dryad2dataverse-0.7.1/docs/compiling.md`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/credits.md` & `dryad2dataverse-0.7.1/docs/credits.md`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/anomalies.html` & `dryad2dataverse-0.7.1/docs/dbase_structure/anomalies.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.css` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.css.map` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.min.css` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.min.css.map` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.css` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.css.map` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.min.css` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.min.css.map` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.eot` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.svg` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.ttf` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.woff` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.woff2` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/js/bootstrap.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/bootstrap/js/bootstrap.min.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/plugins/fastclick/fastclick.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/plugins/fastclick/fastclick.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/plugins/fastclick/fastclick.min.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/plugins/fastclick/fastclick.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/plugins/jQuery/jquery-2.2.3.min.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/plugins/jQuery/jquery-2.2.3.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/plugins/jQueryUI/jquery-ui.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/plugins/jQueryUI/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/plugins/jQueryUI/jquery-ui.min.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/plugins/jQueryUI/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/plugins/slimScroll/jquery.slimscroll.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/plugins/slimScroll/jquery.slimscroll.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/admin-lte/plugins/slimScroll/jquery.slimscroll.min.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/admin-lte/plugins/slimScroll/jquery.slimscroll.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/anchor-js/anchor.min.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/anchor-js/anchor.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/codemirror/codemirror.css` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/codemirror/codemirror.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/codemirror/codemirror.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/codemirror/codemirror.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/codemirror/sql.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/codemirror/sql.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net/jquery.dataTables.min.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-bs/css/dataTables.bootstrap.css` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-bs/css/dataTables.bootstrap.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-bs/css/dataTables.bootstrap.min.css` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-bs/css/dataTables.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-bs/js/dataTables.bootstrap.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-bs/js/dataTables.bootstrap.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-bs/js/dataTables.bootstrap.min.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-bs/js/dataTables.bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons/buttons.colVis.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.colVis.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons/buttons.colVis.min.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.colVis.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons/buttons.flash.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.flash.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons/buttons.flash.min.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.flash.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons/buttons.html5.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.html5.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons/buttons.html5.min.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.html5.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons/buttons.print.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.print.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons/buttons.print.min.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons/buttons.print.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons/dataTables.buttons.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons/dataTables.buttons.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons/dataTables.buttons.min.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons/dataTables.buttons.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons-bs/css/buttons.bootstrap.css` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons-bs/css/buttons.bootstrap.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons-bs/css/buttons.bootstrap.min.css` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons-bs/css/buttons.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons-bs/js/buttons.bootstrap.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons-bs/js/buttons.bootstrap.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/datatables.net-buttons-bs/js/buttons.bootstrap.min.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/datatables.net-buttons-bs/js/buttons.bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/font-awesome/css/font-awesome.css` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/font-awesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/font-awesome/css/font-awesome.css.map` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/font-awesome/css/font-awesome.css.map`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/font-awesome/css/font-awesome.min.css` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/font-awesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/font-awesome/fonts/FontAwesome.otf` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/font-awesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.eot` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.svg` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.ttf` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.woff` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.woff2` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/font-awesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/html5shiv/html5shiv.min.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/html5shiv/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/ionicons/css/ionicons.css` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/ionicons/css/ionicons.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/ionicons/css/ionicons.min.css` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/ionicons/css/ionicons.min.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/ionicons/fonts/ionicons.eot` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/ionicons/fonts/ionicons.eot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/ionicons/fonts/ionicons.svg` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/ionicons/fonts/ionicons.svg`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/ionicons/fonts/ionicons.ttf` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/ionicons/fonts/ionicons.ttf`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/ionicons/fonts/ionicons.woff` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/ionicons/fonts/ionicons.woff`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/jquery/jquery.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/js-xlsx/xlsx.full.min.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/js-xlsx/xlsx.full.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/pdfmake/pdfmake.min.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/pdfmake/pdfmake.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/pdfmake/vfs_fonts.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/pdfmake/vfs_fonts.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/respond/respond.min.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/respond/respond.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/salvattore/salvattore.css` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/salvattore/salvattore.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/bower/salvattore/salvattore.min.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/bower/salvattore/salvattore.min.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/column.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/column.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/columns.html` & `dryad2dataverse-0.7.1/docs/dbase_structure/columns.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/constraints.html` & `dryad2dataverse-0.7.1/docs/dbase_structure/constraints.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/orphans/orphans.dot` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/orphans/orphans.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/orphans/orphans.png` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/orphans/orphans.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/summary/relationships.real.compact.dot` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/summary/relationships.real.compact.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/summary/relationships.real.compact.png` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/summary/relationships.real.compact.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/summary/relationships.real.large.dot` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/summary/relationships.real.large.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/summary/relationships.real.large.png` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/summary/relationships.real.large.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dryadFiles.1degree.dot` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dryadFiles.1degree.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dryadFiles.1degree.png` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dryadFiles.1degree.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dryadFiles.2degrees.dot` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dryadFiles.2degrees.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dryadFiles.2degrees.png` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dryadFiles.2degrees.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dryadStudy.1degree.dot` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dryadStudy.1degree.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dryadStudy.1degree.png` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dryadStudy.1degree.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dvFiles.1degree.dot` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dvFiles.1degree.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dvFiles.1degree.png` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dvFiles.1degree.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dvFiles.2degrees.dot` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dvFiles.2degrees.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dvFiles.2degrees.png` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dvFiles.2degrees.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dvStudy.1degree.dot` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dvStudy.1degree.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dvStudy.1degree.png` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dvStudy.1degree.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dvStudy.2degrees.dot` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dvStudy.2degrees.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/dvStudy.2degrees.png` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/dvStudy.2degrees.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/failed_uploads.1degree.dot` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/failed_uploads.1degree.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/failed_uploads.1degree.png` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/failed_uploads.1degree.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/failed_uploads.2degrees.dot` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/failed_uploads.2degrees.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/failed_uploads.2degrees.png` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/failed_uploads.2degrees.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/lastcheck.1degree.dot` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/lastcheck.1degree.dot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/diagrams/tables/lastcheck.1degree.png` & `dryad2dataverse-0.7.1/docs/dbase_structure/diagrams/tables/lastcheck.1degree.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/dryad_dataverse_monitor.sqlite3.%.xml` & `dryad2dataverse-0.7.1/docs/dbase_structure/dryad_dataverse_monitor.sqlite3.%.xml`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/favicon.png` & `dryad2dataverse-0.7.1/docs/dbase_structure/favicon.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.eot` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.svg` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.ttf` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.woff` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.woff2` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/indieflower/indie-flower-v8-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/indieflower/indie-flower.css` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/indieflower/indie-flower.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.eot` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.eot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.svg` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.svg`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.ttf` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.ttf`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.woff` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.woff`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.woff2` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300.woff2`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.eot` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.eot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.svg` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.svg`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.ttf` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.ttf`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.woff` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.woff`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.woff2` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-300italic.woff2`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.eot` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.eot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.svg` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.svg`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.ttf` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.ttf`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.woff` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.woff`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.woff2` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600.woff2`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.eot` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.eot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.svg` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.svg`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.ttf` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.ttf`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.woff` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.woff`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.woff2` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-600italic.woff2`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.eot` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.eot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.svg` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.svg`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.ttf` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.ttf`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.woff` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.woff`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.woff2` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.eot` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.svg` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.ttf` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.woff` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.woff2` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro-v10-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro.css` & `dryad2dataverse-0.7.1/docs/dbase_structure/fonts/source-sans-pro/source-sans-pro.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/images/foreignKey.png` & `dryad2dataverse-0.7.1/docs/dbase_structure/images/foreignKey.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/images/foreignKeys.png` & `dryad2dataverse-0.7.1/docs/dbase_structure/images/foreignKeys.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/images/primaryKey.png` & `dryad2dataverse-0.7.1/docs/dbase_structure/images/primaryKey.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/images/primaryKeys.png` & `dryad2dataverse-0.7.1/docs/dbase_structure/images/primaryKeys.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/index.html` & `dryad2dataverse-0.7.1/docs/dbase_structure/index.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/main.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/main.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/orphans.html` & `dryad2dataverse-0.7.1/docs/dbase_structure/orphans.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/relationships.html` & `dryad2dataverse-0.7.1/docs/dbase_structure/relationships.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/routines/routine.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/routines/routine.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/routines.html` & `dryad2dataverse-0.7.1/docs/dbase_structure/routines.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/routines.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/routines.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/schemaSpy.css` & `dryad2dataverse-0.7.1/docs/dbase_structure/schemaSpy.css`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/schemaSpy.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/schemaSpy.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/tables/dryadFiles.html` & `dryad2dataverse-0.7.1/docs/dbase_structure/tables/dryadFiles.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/tables/dryadStudy.html` & `dryad2dataverse-0.7.1/docs/dbase_structure/tables/dryadStudy.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/tables/dvFiles.html` & `dryad2dataverse-0.7.1/docs/dbase_structure/tables/dvFiles.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/tables/dvStudy.html` & `dryad2dataverse-0.7.1/docs/dbase_structure/tables/dvStudy.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/tables/failed_uploads.html` & `dryad2dataverse-0.7.1/docs/dbase_structure/tables/failed_uploads.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/tables/lastcheck.html` & `dryad2dataverse-0.7.1/docs/dbase_structure/tables/lastcheck.html`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/dbase_structure/tables/table.js` & `dryad2dataverse-0.7.1/docs/dbase_structure/tables/table.js`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/faq.md` & `dryad2dataverse-0.7.1/docs/faq.md`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/images/dryad2dataverseLogo.png` & `dryad2dataverse-0.7.1/docs/images/dryad2dataverseLogo.png`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/images/dryad2dataverseLogo.svg` & `dryad2dataverse-0.7.1/docs/images/dryad2dataverseLogo.svg`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/index.md` & `dryad2dataverse-0.7.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/installation.md` & `dryad2dataverse-0.7.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/pydoc-markdown.yml` & `dryad2dataverse-0.7.1/docs/pydoc-markdown.yml`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/reference.md` & `dryad2dataverse-0.7.1/docs/reference.md`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/docs/script.md` & `dryad2dataverse-0.7.1/docs/script.md`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/license.md` & `dryad2dataverse-0.7.1/license.md`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/mkdocs.yml` & `dryad2dataverse-0.7.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/pyproject.toml` & `dryad2dataverse-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/src/dryad2dataverse/__init__.py` & `dryad2dataverse-0.7.1/src/dryad2dataverse/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,10 +19,10 @@
     dryad2dataverse.monitor : Monitoring and database tools
     for maintaining a pipeline to Dataverse without unnecessary
     downloading and file duplication.
 
     dryad2dataverse.exceptions : Custom exceptions.
 '''
 
-VERSION = (0, 6, 2)
+VERSION = (0, 7, 1)
 
 __version__ = '.'.join([str(x) for x in VERSION])
```

### Comparing `dryad2dataverse-0.6.2/src/dryad2dataverse/constants.py` & `dryad2dataverse-0.7.1/src/dryad2dataverse/constants.py`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/src/dryad2dataverse/exceptions.py` & `dryad2dataverse-0.7.1/src/dryad2dataverse/exceptions.py`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/src/dryad2dataverse/handlers.py` & `dryad2dataverse-0.7.1/src/dryad2dataverse/handlers.py`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/src/dryad2dataverse/monitor.py` & `dryad2dataverse-0.7.1/src/dryad2dataverse/monitor.py`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/src/dryad2dataverse/scripts/dryadd.py` & `dryad2dataverse-0.7.1/src/dryad2dataverse/scripts/dryadd.py`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/src/dryad2dataverse/serializer.py` & `dryad2dataverse-0.7.1/src/dryad2dataverse/serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,19 @@
         'sha-384','sha-512'
         '''
         out = []
         for page in self.fileJson:
             files = page['_embedded'].get('stash:files')
             if files:
                 for f in files:
-                    downLink = f['_links']['stash:file-download']['href']
+                    #This broke with this commit:
+                    # https://github.com/datadryad/dryad-app/commit/b8a333ba34b14e55cbc1d7ed5aa4451e0f41db66
+
+                    #downLink = f['_links']['stash:file-download']['href']
+                    downLink = f['_links']['stash:download']['href']
                     downLink = f'{constants.DRYURL}{downLink}'
                     name = f['path']
                     mimeType = f['mimeType']
                     size = f['size']
                     #HOW ABOUT PUTTING THIS IN THE DRYAD API PAGE?
                     descr = f.get('description', '')
                     digestType = f.get('digestType', '')
```

### Comparing `dryad2dataverse-0.6.2/src/dryad2dataverse/transfer.py` & `dryad2dataverse-0.7.1/src/dryad2dataverse/transfer.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,25 +5,36 @@
 import hashlib
 import io
 import json
 import logging
 import os
 import time
 import traceback
+import zlib #crc32, adler32
 
+import Crypto.Hash.MD2 #md2
 import requests
 from requests.adapters import HTTPAdapter
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 
 from dryad2dataverse import constants
 from dryad2dataverse import exceptions
 
 LOGGER = logging.getLogger(__name__)
 URL_LOGGER = logging.getLogger('urllib3')
 
+HASHTABLE = {'adler-32' : zlib.adler32, #zlib?
+             'crc-32' : zlib.crc32, #zlib
+             'md2' : Crypto.Hash.MD2, #insecure
+             'md5' : hashlib.md5,
+             'sha-1' : hashlib.sha1,
+             'sha-256' : hashlib.sha256,
+             'sha-384' : hashlib.sha384,
+             'sha-512': hashlib.sha512}
+
 class Transfer():
     '''
     Transfers metadata and data files from a
     Dryad installation to Dataverse installation.
     '''
     def __init__(self, dryad):
         '''
@@ -338,42 +349,68 @@
         if targetDv:
             self.dryad.dvpid = updata['data'].get('persistentId')
         if dvpid:
             self.dryad.dvpid = updata['data'].get('datasetPersistentId')
         return self.dvpid
 
     @staticmethod
-    def _check_md5(infile):
+    def _check_md5(infile, dig_type):
         '''
         Returns the md5 checksum of a file.
 
         ----------------------------------------
         Parameters:
 
         infile : str
             — Complete path to target file.
+
+        dig_type : str or None
+            — Digest type
         ----------------------------------------
         '''
+        #From Ryan Scherle
+        #When Dryad calculates a digest, it only uses MD5.
+        #But if you have precomputed some other type of digest, we should accept it.
+        #The list of allowed values is:
+        #('adler-32','crc-32','md2','md5','sha-1','sha-256','sha-384','sha-512')
+        #hashlib doesn't support adler-32, crc-32, md2
+
         blocksize = 2**16
+        #Well, this is inelegant
         with open(infile, 'rb') as m:
-            fmd5 = hashlib.md5()
-            fblock = m.read(blocksize)
-            while fblock:
-                fmd5.update(fblock)
+            #fmd5 = hashlib.md5()
+            ## var name kept for posterity. Maybe refactor
+            if dig_type in ['sha-1', 'sha-256', 'sha-384', 'sha-512', 'md5', 'md2']:
+                if dig_type == 'md2':
+                    fmd5 = Crypto.Hash.MD2.new()
+                else:
+                    fmd5 = HASHTABLE[dig_type]()
+                fblock = m.read(blocksize)
+                while fblock:
+                    fmd5.update(fblock)
+                    fblock = m.read(blocksize)
+                return fmd5.hexdigest()
+            if dig_type in ['adler-32', 'crc-32']:
                 fblock = m.read(blocksize)
-        return fmd5.hexdigest()
+                curvalue = HASHTABLE[dig_type](fblock)
+                while fblock:
+                    fblock = m.read(blocksize)
+                    curvalue = HASHTABLE[dig_type](fblock, curvalue)
+                return curvalue
+        raise exceptions.HashError(f'Unable to determine hash type for{infile}: {dig_type}')
 
-    def download_file(self, url, filename, tmp=None,
-                      size=None, chk=None, timeout=45):
+
+    def download_file(self, url=None, filename=None, tmp=None,
+                      size=None, chk=None, timeout=45, **kwargs):
         '''
         Downloads a file via requests streaming and saves to constants.TMP.
-        returns md5sum on success and an exception on failure.
+        returns checksum on success and an exception on failure.
 
         ----------------------------------------
-        Parameters:
+        Required keyword arguments:
 
         url : str
             — URL of download.
 
         filename : str
             — Output file name.
 
@@ -384,16 +421,19 @@
             — Temporary directory for downloads.
               Defaults to dryad2dataverse.constants.TMP.
 
         size : int
             — Reported file size in bytes.
               Defaults to dryad2dataverse.constants.MAX_UPLOAD.
 
+        digest_type: str
+            — checksum type (ie, md5, sha-256, etc)
+
         chk : str
-            - md5 sum of file (if available and known).
+            —  checksum of file (if available and known).
         ----------------------------------------
         '''
         LOGGER.debug('Start download sequence')
         LOGGER.debug('MAX SIZE = %s', constants.MAX_UPLOAD)
         LOGGER.debug('Filename: %s, size=%s', filename, size)
         if not tmp:
             tmp = constants.TMP
@@ -426,19 +466,21 @@
                     try:
                         raise exceptions.DownloadSizeError('Download size does not match '
                                                            'reported size')
                     except exceptions.DownloadSizeError as e:
                         LOGGER.exception(e)
                         raise
             #now check the md5
-            md5 = Transfer._check_md5(f'{tmp}{os.sep}{filename}')
-            if chk:
+            md5 = None
+            if chk and kwargs.get('digest_type') in HASHTABLE:
+                md5 = Transfer._check_md5(f'{tmp}{os.sep}{filename}',
+                                      kwargs['digest_type'])
                 if md5 != chk:
                     try:
-                        raise exceptions.HashError('Hex digest mismatch: {md5} : {chk}')
+                        raise exceptions.HashError(f'Hex digest mismatch: {md5} : {chk}')
                         #is this really what I want to do on a bad checksum?
                     except exceptions.HashError as e:
                         LOGGER.exception(e)
                         raise
             for i in self._files:
                 if url == i[0]:
                     i[-1] = md5
@@ -470,15 +512,21 @@
               files with a Dryad study.
         ----------------------------------------
         '''
         if not files:
             files = self.files
         try:
             for f in files:
-                self.download_file(f[0], f[1], size=f[3], chk=f[-1])
+                self.download_file(url=f[0],
+                                   filename=f[1],
+                                   mimetype=f[2],
+                                   size=f[3],
+                                   descr=f[4],
+                                   digest_type=f[5],
+                                   chk=f[-1])
         except exceptions.DataverseDownloadError as e:
             LOGGER.exception('Unable to download file with info %s\n%s', f, e)
             raise
 
     def file_lock_check(self, study, dv_url, apikey=None, count=0):
         '''
         Checks for a study lock
```

### Comparing `dryad2dataverse-0.6.2/src/dryad2dataverse.egg-info/PKG-INFO` & `dryad2dataverse-0.7.1/src/dryad2dataverse.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dryad2dataverse
-Version: 0.6.2
+Version: 0.7.1
 Summary: Utility for copying and syncing data from a Dryad data repository to a Dataverse repository
 Author-email: Paul Lesack <paul.lesack@ubc.ca>
 Project-URL: Homepage, https://ubc-library-rc.github.io/dryad2dataverse
 Project-URL: Documentation, https://ubc-library-rc.github.io/dryad2dataverse
 Project-URL: Repository, https://github.com/ubc-library-rc/dryad2dataverse.git
 Project-URL: Tracker, https://github.com/ubc-library-rc/dryad2dataverse/issues
 Keywords: Harvard Dataverse,Dataverse,research data management,data repository,Dryad,datadryad.org,dataverse.org
@@ -13,14 +13,22 @@
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Education
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: certifi>=2022.12.7
+Requires-Dist: charset-normalizer>=2.0.4
+Requires-Dist: chardet>=3.0.4
+Requires-Dist: idna>=2.10
+Requires-Dist: pycryptodome>=3.20.0
+Requires-Dist: requests>=2.26.0
+Requires-Dist: requests-toolbelt>=0.9.1
+Requires-Dist: urllib3>=1.26.6
 
 # dryad2dataverse
 
 **dryad2dataverse** is a [Python](https://python.org) package and an associated console line application which allows easier transfer of metadata and data from a Dryad data repository (ie, <https://datadryad.org>) to a [Dataverse](https://dataverse.org/ "Dataverse software main site") repository. Dryad2dataverse is pure Python and should run on any platform which supports Python 3.6 or greater.
 
 Data transfers between repositories require local storage, so not all platforms will be equally suitable.
```

### Comparing `dryad2dataverse-0.6.2/src/dryad2dataverse.egg-info/SOURCES.txt` & `dryad2dataverse-0.7.1/src/dryad2dataverse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/tests/badURL.json` & `dryad2dataverse-0.7.1/tests/badURL.json`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/tests/tests_monitor.py` & `dryad2dataverse-0.7.1/tests/tests_monitor.py`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/tests/tests_serializer.py` & `dryad2dataverse-0.7.1/tests/tests_serializer.py`

 * *Files identical despite different names*

### Comparing `dryad2dataverse-0.6.2/tests/tests_transfer.py` & `dryad2dataverse-0.7.1/tests/tests_transfer.py`

 * *Files identical despite different names*


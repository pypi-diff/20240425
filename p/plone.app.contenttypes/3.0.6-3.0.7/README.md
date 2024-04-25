# Comparing `tmp/plone.app.contenttypes-3.0.6.tar.gz` & `tmp/plone_app_contenttypes-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.contenttypes-3.0.6.tar", last modified: Fri Mar 15 10:30:31 2024, max compression
+gzip compressed data, was "plone_app_contenttypes-3.0.7.tar", last modified: Thu Apr 25 19:34:07 2024, max compression
```

## Comparing `plone.app.contenttypes-3.0.6.tar` & `plone_app_contenttypes-3.0.7.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:30:31.613779 plone.app.contenttypes-3.0.6/
--rw-r--r--   0 maurits    (501) staff       (20)    46773 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      122 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    56296 2024-03-15 10:30:31.613296 plone.app.contenttypes-3.0.6/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     7005 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:30:31.568152 plone.app.contenttypes-3.0.6/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     1334 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/docs/INSTALL.txt
--rw-r--r--   0 maurits    (501) staff       (20)    17987 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      737 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     7005 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/docs/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:30:31.568951 plone.app.contenttypes-3.0.6/docs/source/
--rw-r--r--   0 maurits    (501) staff       (20)     8036 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/docs/source/conf.py
--rw-r--r--   0 maurits    (501) staff       (20)      471 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/docs/source/index.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:30:31.569275 plone.app.contenttypes-3.0.6/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:30:31.572044 plone.app.contenttypes-3.0.6/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:30:31.578215 plone.app.contenttypes-3.0.6/plone/app/contenttypes/
--rw-r--r--   0 maurits    (501) staff       (20)      127 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:30:31.582004 plone.app.contenttypes-3.0.6/plone/app/contenttypes/behaviors/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/behaviors/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     6169 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/behaviors/collection.py
--rw-r--r--   0 maurits    (501) staff       (20)     2809 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/behaviors/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      548 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/behaviors/leadimage.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1320 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/behaviors/leadimage.py
--rw-r--r--   0 maurits    (501) staff       (20)     1312 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/behaviors/richtext.py
--rw-r--r--   0 maurits    (501) staff       (20)       63 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/behaviors/richtext_gettext.pt
--rw-r--r--   0 maurits    (501) staff       (20)      728 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/behaviors/tableofcontents.py
--rw-r--r--   0 maurits    (501) staff       (20)     2787 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/behaviors/thumb_icon.py
--rw-r--r--   0 maurits    (501) staff       (20)      340 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/behaviors/viewlets.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:30:31.585464 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2931 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/collection.py
--rw-r--r--   0 maurits    (501) staff       (20)     6736 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1091 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/file.py
--rw-r--r--   0 maurits    (501) staff       (20)     8782 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/folder.py
--rw-r--r--   0 maurits    (501) staff       (20)      991 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/full_view.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:30:31.586220 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/images/
--rw-r--r--   0 maurits    (501) staff       (20)      414 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/images/icon_export_ical.png
--rw-r--r--   0 maurits    (501) staff       (20)      427 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/images/icon_export_vcal.png
--rw-r--r--   0 maurits    (501) staff       (20)     4980 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/link_redirect_view.py
--rw-r--r--   0 maurits    (501) staff       (20)     4092 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/migration.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:30:31.590589 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/
--rw-r--r--   0 maurits    (501) staff       (20)     1045 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/document.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3434 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/file.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1264 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/full_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2497 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/full_view_item.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3921 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/image.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2069 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/image_view_fullscreen.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2552 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/link.pt
--rw-r--r--   0 maurits    (501) staff       (20)     8895 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/listing.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4474 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/listing_album.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2926 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/listing_summary.pt
--rw-r--r--   0 maurits    (501) staff       (20)     7518 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/listing_tabular.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1091 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/newsitem.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1964 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1842 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     6481 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/content.py
--rw-r--r--   0 maurits    (501) staff       (20)     5847 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/indexers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1251 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/indexers.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1018 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      912 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/permissions.py
--rw-r--r--   0 maurits    (501) staff       (20)     1227 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/permissions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:30:31.563688 plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:30:31.591263 plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/content/
--rw-r--r--   0 maurits    (501) staff       (20)      191 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/content/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      591 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/content/portlets.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:30:31.592921 plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      184 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1031 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/diff_tool.xml
--rw-r--r--   0 maurits    (501) staff       (20)      461 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2113 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/rolemap.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:30:31.595939 plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/types/
--rw-r--r--   0 maurits    (501) staff       (20)     3097 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/types/Collection.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2943 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/types/Document.xml
--rw-r--r--   0 maurits    (501) staff       (20)     3175 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/types/Event.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2810 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/types/File.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2974 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/types/Folder.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2844 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/types/Image.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2692 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/types/Link.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2947 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/types/News_Item.xml
--rw-r--r--   0 maurits    (501) staff       (20)      648 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/types/Plone_Site.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1957 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)      963 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:30:31.598922 plone.app.contenttypes-3.0.6/plone/app/contenttypes/schema/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/schema/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      131 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/schema/collection.xml
--rw-r--r--   0 maurits    (501) staff       (20)      131 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/schema/document.xml
--rw-r--r--   0 maurits    (501) staff       (20)      131 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/schema/event.xml
--rw-r--r--   0 maurits    (501) staff       (20)      865 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/schema/file.xml
--rw-r--r--   0 maurits    (501) staff       (20)      131 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/schema/folder.xml
--rw-r--r--   0 maurits    (501) staff       (20)      869 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/schema/image.xml
--rw-r--r--   0 maurits    (501) staff       (20)      880 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/schema/link.xml
--rw-r--r--   0 maurits    (501) staff       (20)      131 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/schema/news_item.xml
--rw-r--r--   0 maurits    (501) staff       (20)    12750 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)      585 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/subscribers.py
--rw-r--r--   0 maurits    (501) staff       (20)      401 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/subscribers.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2477 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:30:31.608060 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     9216 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/file.doc
--rw-r--r--   0 maurits    (501) staff       (20)     9338 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/file.odt
--rw-r--r--   0 maurits    (501) staff       (20)     8561 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/file.pdf
--rw-r--r--   0 maurits    (501) staff       (20)     5131 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/image.jpg
--rw-r--r--   0 maurits    (501) staff       (20)     1185 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/image.png
--rw-r--r--   0 maurits    (501) staff       (20)     9344 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/image.svg
--rw-r--r--   0 maurits    (501) staff       (20)     4063 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/oldtypes.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:30:31.611059 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/robot/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/robot/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     5132 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/robot/keywords.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2117 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/robot/test_collection_creator_criterion.robot
--rw-r--r--   0 maurits    (501) staff       (20)     4067 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/robot/test_collection_location_criterion.robot
--rw-r--r--   0 maurits    (501) staff       (20)     2088 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/robot/test_collection_review_state_criterion.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1869 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/robot/test_collection_short_name_criterion.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1818 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/robot/test_collection_type_criterion.robot
--rw-r--r--   0 maurits    (501) staff       (20)    11981 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/robot/test_folderlisting.robot
--rw-r--r--   0 maurits    (501) staff       (20)      339 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/robot/variables.py
--rw-r--r--   0 maurits    (501) staff       (20)     3888 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_behaviors_collection.py
--rw-r--r--   0 maurits    (501) staff       (20)     3277 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_behaviors_leadimage.py
--rw-r--r--   0 maurits    (501) staff       (20)     2205 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_behaviors_richtext.py
--rw-r--r--   0 maurits    (501) staff       (20)     2278 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_behaviors_table_of_contents.py
--rw-r--r--   0 maurits    (501) staff       (20)     1524 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_browser_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)    14842 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_collection.py
--rw-r--r--   0 maurits    (501) staff       (20)     2521 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_collection_rss.py
--rw-r--r--   0 maurits    (501) staff       (20)     5127 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_content_profile.py
--rw-r--r--   0 maurits    (501) staff       (20)     4321 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_document.py
--rw-r--r--   0 maurits    (501) staff       (20)     4358 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_event.py
--rw-r--r--   0 maurits    (501) staff       (20)     8996 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_file.py
--rw-r--r--   0 maurits    (501) staff       (20)     9734 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_folder.py
--rw-r--r--   0 maurits    (501) staff       (20)     7360 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_image.py
--rw-r--r--   0 maurits    (501) staff       (20)    11959 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_indexes.py
--rw-r--r--   0 maurits    (501) staff       (20)    18488 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_link.py
--rw-r--r--   0 maurits    (501) staff       (20)     5564 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_news_item.py
--rw-r--r--   0 maurits    (501) staff       (20)      965 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_robot.py
--rw-r--r--   0 maurits    (501) staff       (20)     8278 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_security.py
--rw-r--r--   0 maurits    (501) staff       (20)     1542 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)     2318 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_webdav.py
--rw-r--r--   0 maurits    (501) staff       (20)     4530 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)      392 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/upgrades.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4071 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/plone/app/contenttypes/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-15 10:30:31.611460 plone.app.contenttypes-3.0.6/plone.app.contenttypes.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    56296 2024-03-15 10:30:31.000000 plone.app.contenttypes-3.0.6/plone.app.contenttypes.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     5920 2024-03-15 10:30:31.000000 plone.app.contenttypes-3.0.6/plone.app.contenttypes.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-03-15 10:30:31.000000 plone.app.contenttypes-3.0.6/plone.app.contenttypes.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2024-03-15 10:30:31.000000 plone.app.contenttypes-3.0.6/plone.app.contenttypes.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-03-15 10:30:31.000000 plone.app.contenttypes-3.0.6/plone.app.contenttypes.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      803 2024-03-15 10:30:31.000000 plone.app.contenttypes-3.0.6/plone.app.contenttypes.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-03-15 10:30:31.000000 plone.app.contenttypes-3.0.6/plone.app.contenttypes.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4315 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2024-03-15 10:30:31.613863 plone.app.contenttypes-3.0.6/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     3091 2024-03-15 10:30:30.000000 plone.app.contenttypes-3.0.6/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:07.331145 plone_app_contenttypes-3.0.7/
+-rw-r--r--   0 maurits    (501) staff       (20)    46952 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      122 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    56399 2024-04-25 19:34:07.330477 plone_app_contenttypes-3.0.7/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     6929 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:07.286040 plone_app_contenttypes-3.0.7/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     1334 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/docs/INSTALL.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    17987 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      737 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     6929 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/docs/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:07.286702 plone_app_contenttypes-3.0.7/docs/source/
+-rw-r--r--   0 maurits    (501) staff       (20)     8036 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/docs/source/conf.py
+-rw-r--r--   0 maurits    (501) staff       (20)      471 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/docs/source/index.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:07.287008 plone_app_contenttypes-3.0.7/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:07.289713 plone_app_contenttypes-3.0.7/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:07.295144 plone_app_contenttypes-3.0.7/plone/app/contenttypes/
+-rw-r--r--   0 maurits    (501) staff       (20)      127 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:07.298493 plone_app_contenttypes-3.0.7/plone/app/contenttypes/behaviors/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/behaviors/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6169 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/behaviors/collection.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2809 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/behaviors/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      548 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/behaviors/leadimage.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1320 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/behaviors/leadimage.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1312 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/behaviors/richtext.py
+-rw-r--r--   0 maurits    (501) staff       (20)       63 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/behaviors/richtext_gettext.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      728 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/behaviors/tableofcontents.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2787 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/behaviors/thumb_icon.py
+-rw-r--r--   0 maurits    (501) staff       (20)      348 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/behaviors/viewlets.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:07.301706 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2931 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/collection.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6736 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1091 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/file.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8782 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/folder.py
+-rw-r--r--   0 maurits    (501) staff       (20)      991 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/full_view.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:07.302403 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/images/
+-rw-r--r--   0 maurits    (501) staff       (20)      414 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/images/icon_export_ical.png
+-rw-r--r--   0 maurits    (501) staff       (20)      427 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/images/icon_export_vcal.png
+-rw-r--r--   0 maurits    (501) staff       (20)     4980 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/link_redirect_view.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4092 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/migration.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:07.306176 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)     1045 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/document.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3434 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/file.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1264 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/full_view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2497 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/full_view_item.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3921 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/image.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2069 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/image_view_fullscreen.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2552 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/link.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     8895 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/listing.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4474 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/listing_album.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2926 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/listing_summary.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     7518 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/listing_tabular.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1091 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/newsitem.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1964 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1842 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     6481 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/content.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5863 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/indexers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1251 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/indexers.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1018 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      912 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/permissions.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1227 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/permissions.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:07.280394 plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:07.306828 plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/content/
+-rw-r--r--   0 maurits    (501) staff       (20)      191 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/content/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      591 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/content/portlets.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:07.308390 plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      184 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1031 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/diff_tool.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      461 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2113 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/rolemap.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:07.311195 plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     3097 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/types/Collection.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2943 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/types/Document.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     3175 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/types/Event.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2810 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/types/File.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2974 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/types/Folder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2844 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/types/Image.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2692 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/types/Link.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2947 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/types/News_Item.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      648 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/types/Plone_Site.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1957 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/types.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      963 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:07.313905 plone_app_contenttypes-3.0.7/plone/app/contenttypes/schema/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/schema/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      131 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/schema/collection.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      131 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/schema/document.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      131 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/schema/event.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      865 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/schema/file.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      131 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/schema/folder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      869 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/schema/image.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      880 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/schema/link.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      131 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/schema/news_item.xml
+-rw-r--r--   0 maurits    (501) staff       (20)    12750 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)      585 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/subscribers.py
+-rw-r--r--   0 maurits    (501) staff       (20)      401 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/subscribers.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2477 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:07.325620 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9216 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/file.doc
+-rw-r--r--   0 maurits    (501) staff       (20)     9338 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/file.odt
+-rw-r--r--   0 maurits    (501) staff       (20)     8561 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/file.pdf
+-rw-r--r--   0 maurits    (501) staff       (20)     5131 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/image.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)     1185 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/image.png
+-rw-r--r--   0 maurits    (501) staff       (20)     9344 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/image.svg
+-rw-r--r--   0 maurits    (501) staff       (20)     4063 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/oldtypes.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:07.328727 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/robot/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/robot/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5132 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/robot/keywords.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2117 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/robot/test_collection_creator_criterion.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     4067 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/robot/test_collection_location_criterion.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     2088 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/robot/test_collection_review_state_criterion.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1869 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/robot/test_collection_short_name_criterion.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1818 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/robot/test_collection_type_criterion.robot
+-rw-r--r--   0 maurits    (501) staff       (20)    11981 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/robot/test_folderlisting.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      339 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/robot/variables.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3888 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_behaviors_collection.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3277 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_behaviors_leadimage.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2205 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_behaviors_richtext.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2278 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_behaviors_table_of_contents.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1524 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_browser_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14842 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_collection.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2521 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_collection_rss.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5127 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_content_profile.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4321 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_document.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4358 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_event.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8996 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_file.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9734 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_folder.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7360 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_image.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11959 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_indexes.py
+-rw-r--r--   0 maurits    (501) staff       (20)    18488 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_link.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5564 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_news_item.py
+-rw-r--r--   0 maurits    (501) staff       (20)      965 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_robot.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8278 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_security.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1542 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2318 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_webdav.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4530 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)      392 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/upgrades.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4071 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/plone/app/contenttypes/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:07.329092 plone_app_contenttypes-3.0.7/plone.app.contenttypes.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    56399 2024-04-25 19:34:07.000000 plone_app_contenttypes-3.0.7/plone.app.contenttypes.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     5920 2024-04-25 19:34:07.000000 plone_app_contenttypes-3.0.7/plone.app.contenttypes.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-25 19:34:07.000000 plone_app_contenttypes-3.0.7/plone.app.contenttypes.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2024-04-25 19:34:07.000000 plone_app_contenttypes-3.0.7/plone.app.contenttypes.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-25 19:34:07.000000 plone_app_contenttypes-3.0.7/plone.app.contenttypes.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      803 2024-04-25 19:34:07.000000 plone_app_contenttypes-3.0.7/plone.app.contenttypes.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-25 19:34:07.000000 plone_app_contenttypes-3.0.7/plone.app.contenttypes.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4315 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-04-25 19:34:07.331236 plone_app_contenttypes-3.0.7/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     3091 2024-04-25 19:34:06.000000 plone_app_contenttypes-3.0.7/setup.py
```

### Comparing `plone.app.contenttypes-3.0.6/CHANGES.rst` & `plone_app_contenttypes-3.0.7/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.7 (2024-04-25)
+------------------
+
+Bug fixes:
+
+
+- Fix ILeadImageBehavior and IRichTextBehavior interfaces were the name change was forgotten.
+  [thet] (#681)
+
+
 3.0.6 (2024-03-15)
 ------------------
 
 Bug fixes:
 
 
 - Fix folder listing template when `plone.eventlocation` behavior is disabled for Events.
@@ -469,15 +479,15 @@
 
 2.1.0 (2019-06-19)
 ------------------
 
 New features:
 
 
-- Support ILeadImage behavior when display collection album view.
+- Support ILeadImageBehavior when display collection album view.
   [rodfersou] (#524)
 - Add more log-messages during migration from AT to DX.
   [pbauer] (#526)
 
 
 Bug fixes:
 
@@ -548,15 +558,15 @@
 
 
 2.0.0 (2018-10-30)
 ------------------
 
 Breaking changes:
 
-- ILeadImage and IRichText behaviors now have proper "Marker"-Interfaces.
+- ILeadImageBehavior and IRichTextBehavior behaviors now have proper "Marker"-Interfaces.
   As this was only possible by renaming the schema adapter to *Behavior* to
   not break with implementations inside the collective, the FTI-behavior-definition
   has changed:
 
   - ``plone.app.contenttypes.behaviors.leadimage.ILeadImage``
     becomes
     ``plone.app.contenttypes.behaviors.leadimage.ILeadImageBehavior``
```

### Comparing `plone.app.contenttypes-3.0.6/PKG-INFO` & `plone_app_contenttypes-3.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.contenttypes
-Version: 3.0.6
+Version: 3.0.7
 Summary: Default content types for Plone based on Dexterity
 Home-page: https://github.com/plone/plone.app.contenttypes
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: plone content types dexterity
 Classifier: Development Status :: 5 - Production/Stable
@@ -142,27 +142,27 @@
    Here is an example that enables the image-behavior for Folders in ``[yourpackage]/profiles/default/types/Folder.xml``:
 
    .. code:: xml
 
     <?xml version="1.0"?>
     <object name="Folder" meta_type="Dexterity FTI">
      <property name="behaviors" purge="False">
-      <element value="plone.app.contenttypes.behaviors.leadimage.ILeadImage"/>
+      <element value="plone.leadimage"/>
      </property>
     </object>
 
    By adding a schema-definition to the profile you can add fields.
 
    .. code:: xml
 
     <?xml version="1.0"?>
     <object name="Folder" meta_type="Dexterity FTI">
      <property name="model_file">your.package.content:folder.xml</property>
      <property name="behaviors" purge="False">
-      <element value="plone.app.contenttypes.behaviors.leadimage.ILeadImage"/>
+      <element value="plone.leadimage"/>
      </property>
     </object>
 
    Put the schema-xml in ``your/package/content/folder.xml`` (the folder ``content`` needs a ``__init__.py``)
 
    .. code:: xml
 
@@ -260,14 +260,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.7 (2024-04-25)
+------------------
+
+Bug fixes:
+
+
+- Fix ILeadImageBehavior and IRichTextBehavior interfaces were the name change was forgotten.
+  [thet] (#681)
+
+
 3.0.6 (2024-03-15)
 ------------------
 
 Bug fixes:
 
 
 - Fix folder listing template when `plone.eventlocation` behavior is disabled for Events.
@@ -725,15 +735,15 @@
 
 2.1.0 (2019-06-19)
 ------------------
 
 New features:
 
 
-- Support ILeadImage behavior when display collection album view.
+- Support ILeadImageBehavior when display collection album view.
   [rodfersou] (#524)
 - Add more log-messages during migration from AT to DX.
   [pbauer] (#526)
 
 
 Bug fixes:
 
@@ -804,15 +814,15 @@
 
 
 2.0.0 (2018-10-30)
 ------------------
 
 Breaking changes:
 
-- ILeadImage and IRichText behaviors now have proper "Marker"-Interfaces.
+- ILeadImageBehavior and IRichTextBehavior behaviors now have proper "Marker"-Interfaces.
   As this was only possible by renaming the schema adapter to *Behavior* to
   not break with implementations inside the collective, the FTI-behavior-definition
   has changed:
 
   - ``plone.app.contenttypes.behaviors.leadimage.ILeadImage``
     becomes
     ``plone.app.contenttypes.behaviors.leadimage.ILeadImageBehavior``
```

### Comparing `plone.app.contenttypes-3.0.6/README.rst` & `plone_app_contenttypes-3.0.7/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -75,27 +75,27 @@
    Here is an example that enables the image-behavior for Folders in ``[yourpackage]/profiles/default/types/Folder.xml``:
 
    .. code:: xml
 
     <?xml version="1.0"?>
     <object name="Folder" meta_type="Dexterity FTI">
      <property name="behaviors" purge="False">
-      <element value="plone.app.contenttypes.behaviors.leadimage.ILeadImage"/>
+      <element value="plone.leadimage"/>
      </property>
     </object>
 
    By adding a schema-definition to the profile you can add fields.
 
    .. code:: xml
 
     <?xml version="1.0"?>
     <object name="Folder" meta_type="Dexterity FTI">
      <property name="model_file">your.package.content:folder.xml</property>
      <property name="behaviors" purge="False">
-      <element value="plone.app.contenttypes.behaviors.leadimage.ILeadImage"/>
+      <element value="plone.leadimage"/>
      </property>
     </object>
 
    Put the schema-xml in ``your/package/content/folder.xml`` (the folder ``content`` needs a ``__init__.py``)
 
    .. code:: xml
```

### Comparing `plone.app.contenttypes-3.0.6/docs/INSTALL.txt` & `plone_app_contenttypes-3.0.7/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/docs/LICENSE.GPL` & `plone_app_contenttypes-3.0.7/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/docs/LICENSE.txt` & `plone_app_contenttypes-3.0.7/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/docs/README.rst` & `plone_app_contenttypes-3.0.7/docs/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -75,27 +75,27 @@
    Here is an example that enables the image-behavior for Folders in ``[yourpackage]/profiles/default/types/Folder.xml``:
 
    .. code:: xml
 
     <?xml version="1.0"?>
     <object name="Folder" meta_type="Dexterity FTI">
      <property name="behaviors" purge="False">
-      <element value="plone.app.contenttypes.behaviors.leadimage.ILeadImage"/>
+      <element value="plone.leadimage"/>
      </property>
     </object>
 
    By adding a schema-definition to the profile you can add fields.
 
    .. code:: xml
 
     <?xml version="1.0"?>
     <object name="Folder" meta_type="Dexterity FTI">
      <property name="model_file">your.package.content:folder.xml</property>
      <property name="behaviors" purge="False">
-      <element value="plone.app.contenttypes.behaviors.leadimage.ILeadImage"/>
+      <element value="plone.leadimage"/>
      </property>
     </object>
 
    Put the schema-xml in ``your/package/content/folder.xml`` (the folder ``content`` needs a ``__init__.py``)
 
    .. code:: xml
```

### Comparing `plone.app.contenttypes-3.0.6/docs/source/conf.py` & `plone_app_contenttypes-3.0.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/behaviors/collection.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/behaviors/collection.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/behaviors/configure.zcml` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/behaviors/leadimage.pt` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/behaviors/leadimage.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/behaviors/leadimage.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/behaviors/leadimage.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/behaviors/richtext.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/behaviors/richtext.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/behaviors/tableofcontents.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/behaviors/tableofcontents.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/behaviors/thumb_icon.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/behaviors/thumb_icon.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/collection.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/collection.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/configure.zcml` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/file.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/file.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/folder.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/folder.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/full_view.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/full_view.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/link_redirect_view.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/link_redirect_view.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/migration.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/migration.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/document.pt` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/document.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/file.pt` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/file.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/full_view.pt` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/full_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/full_view_item.pt` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/full_view_item.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/image.pt` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/image.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/image_view_fullscreen.pt` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/image_view_fullscreen.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/link.pt` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/link.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/listing.pt` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/listing.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/listing_album.pt` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/listing_album.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/listing_summary.pt` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/listing_summary.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/listing_tabular.pt` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/listing_tabular.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/templates/newsitem.pt` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/templates/newsitem.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/browser/utils.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/browser/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/configure.zcml` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/content.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/content.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/indexers.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/indexers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from Acquisition import aq_base
 from logging import getLogger
-from plone.app.contenttypes.behaviors.richtext import IRichText
+from plone.app.contenttypes.behaviors.richtext import IRichTextBehavior
 from plone.app.contenttypes.interfaces import ICollection
 from plone.app.contenttypes.interfaces import IDocument
 from plone.app.contenttypes.interfaces import IFile
 from plone.app.contenttypes.interfaces import IFolder
 from plone.app.contenttypes.interfaces import IImage
 from plone.app.contenttypes.interfaces import ILink
 from plone.app.contenttypes.interfaces import INewsItem
@@ -36,15 +36,15 @@
             value = safe_text(value)
         result = " ".join((result, value))
     return result
 
 
 def SearchableText(obj):
     text = ""
-    richtext = IRichText(obj, None)
+    richtext = IRichTextBehavior(obj, None)
     if richtext:
         textvalue = richtext.text
         if IRichTextValue.providedBy(textvalue):
             transforms = getToolByName(obj, "portal_transforms")
             # Before you think about switching raw/output
             # or mimeType/outputMimeType, first read
             # https://github.com/plone/Products.CMFPlone/issues/2066
```

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/indexers.zcml` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/indexers.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/interfaces.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/permissions.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/permissions.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/permissions.zcml` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/permissions.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/content/portlets.xml` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/content/portlets.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/diff_tool.xml` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/diff_tool.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/rolemap.xml` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/types/Collection.xml` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/types/Collection.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/types/Document.xml` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/types/Document.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/types/Event.xml` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/types/Event.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/types/File.xml` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/types/File.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/types/Folder.xml` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/types/Folder.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/types/Image.xml` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/types/Image.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/types/Link.xml` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/types/Link.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/types/News_Item.xml` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/types/News_Item.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/types/Plone_Site.xml` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/types/Plone_Site.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles/default/types.xml` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles/default/types.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/profiles.zcml` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/profiles.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/schema/file.xml` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/schema/file.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/schema/image.xml` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/schema/image.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/schema/link.xml` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/schema/link.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/setuphandlers.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/subscribers.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/subscribers.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/testing.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/file.doc` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/file.doc`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/file.odt` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/file.odt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/file.pdf` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/file.pdf`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/image.jpg` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/image.jpg`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/image.png` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/image.png`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/image.svg` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/image.svg`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/oldtypes.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/oldtypes.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/robot/keywords.txt` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/robot/keywords.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/robot/test_collection_creator_criterion.robot` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/robot/test_collection_creator_criterion.robot`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/robot/test_collection_location_criterion.robot` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/robot/test_collection_location_criterion.robot`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/robot/test_collection_review_state_criterion.robot` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/robot/test_collection_review_state_criterion.robot`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/robot/test_collection_short_name_criterion.robot` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/robot/test_collection_short_name_criterion.robot`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/robot/test_collection_type_criterion.robot` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/robot/test_collection_type_criterion.robot`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/robot/test_folderlisting.robot` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/robot/test_folderlisting.robot`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_behaviors_collection.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_behaviors_collection.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_behaviors_leadimage.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_behaviors_leadimage.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_behaviors_richtext.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_behaviors_richtext.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_behaviors_table_of_contents.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_behaviors_table_of_contents.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_browser_utils.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_browser_utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_collection.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_collection_rss.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_collection_rss.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_content_profile.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_content_profile.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_document.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_event.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_file.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_folder.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_folder.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_image.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_indexes.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_link.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_news_item.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_news_item.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_robot.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_security.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_setup.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/tests/test_webdav.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/tests/test_webdav.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/upgrades.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone/app/contenttypes/utils.py` & `plone_app_contenttypes-3.0.7/plone/app/contenttypes/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone.app.contenttypes.egg-info/PKG-INFO` & `plone_app_contenttypes-3.0.7/plone.app.contenttypes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.contenttypes
-Version: 3.0.6
+Version: 3.0.7
 Summary: Default content types for Plone based on Dexterity
 Home-page: https://github.com/plone/plone.app.contenttypes
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: plone content types dexterity
 Classifier: Development Status :: 5 - Production/Stable
@@ -142,27 +142,27 @@
    Here is an example that enables the image-behavior for Folders in ``[yourpackage]/profiles/default/types/Folder.xml``:
 
    .. code:: xml
 
     <?xml version="1.0"?>
     <object name="Folder" meta_type="Dexterity FTI">
      <property name="behaviors" purge="False">
-      <element value="plone.app.contenttypes.behaviors.leadimage.ILeadImage"/>
+      <element value="plone.leadimage"/>
      </property>
     </object>
 
    By adding a schema-definition to the profile you can add fields.
 
    .. code:: xml
 
     <?xml version="1.0"?>
     <object name="Folder" meta_type="Dexterity FTI">
      <property name="model_file">your.package.content:folder.xml</property>
      <property name="behaviors" purge="False">
-      <element value="plone.app.contenttypes.behaviors.leadimage.ILeadImage"/>
+      <element value="plone.leadimage"/>
      </property>
     </object>
 
    Put the schema-xml in ``your/package/content/folder.xml`` (the folder ``content`` needs a ``__init__.py``)
 
    .. code:: xml
 
@@ -260,14 +260,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.7 (2024-04-25)
+------------------
+
+Bug fixes:
+
+
+- Fix ILeadImageBehavior and IRichTextBehavior interfaces were the name change was forgotten.
+  [thet] (#681)
+
+
 3.0.6 (2024-03-15)
 ------------------
 
 Bug fixes:
 
 
 - Fix folder listing template when `plone.eventlocation` behavior is disabled for Events.
@@ -725,15 +735,15 @@
 
 2.1.0 (2019-06-19)
 ------------------
 
 New features:
 
 
-- Support ILeadImage behavior when display collection album view.
+- Support ILeadImageBehavior when display collection album view.
   [rodfersou] (#524)
 - Add more log-messages during migration from AT to DX.
   [pbauer] (#526)
 
 
 Bug fixes:
 
@@ -804,15 +814,15 @@
 
 
 2.0.0 (2018-10-30)
 ------------------
 
 Breaking changes:
 
-- ILeadImage and IRichText behaviors now have proper "Marker"-Interfaces.
+- ILeadImageBehavior and IRichTextBehavior behaviors now have proper "Marker"-Interfaces.
   As this was only possible by renaming the schema adapter to *Behavior* to
   not break with implementations inside the collective, the FTI-behavior-definition
   has changed:
 
   - ``plone.app.contenttypes.behaviors.leadimage.ILeadImage``
     becomes
     ``plone.app.contenttypes.behaviors.leadimage.ILeadImageBehavior``
```

### Comparing `plone.app.contenttypes-3.0.6/plone.app.contenttypes.egg-info/SOURCES.txt` & `plone_app_contenttypes-3.0.7/plone.app.contenttypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/plone.app.contenttypes.egg-info/requires.txt` & `plone_app_contenttypes-3.0.7/plone.app.contenttypes.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/pyproject.toml` & `plone_app_contenttypes-3.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.6/setup.py` & `plone_app_contenttypes-3.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages
 from setuptools import setup
 
 import os
 
 
-version = "3.0.6"
+version = "3.0.7"
 
 
 def read(*rnames):
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 
 long_description = read("README.rst") + "\n\n" + read("CHANGES.rst")
```


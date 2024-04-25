# Comparing `tmp/plone.dexterity-3.0.5.tar.gz` & `tmp/plone_dexterity-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.dexterity-3.0.5.tar", last modified: Tue Feb 27 14:48:01 2024, max compression
+gzip compressed data, was "plone_dexterity-3.0.6.tar", last modified: Thu Apr 25 19:34:52 2024, max compression
```

## Comparing `plone.dexterity-3.0.5.tar` & `plone_dexterity-3.0.6.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 14:48:01.106526 plone.dexterity-3.0.5/
--rw-r--r--   0 maurits    (501) staff       (20)    25804 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      207 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    41152 2024-02-27 14:48:01.105645 plone.dexterity-3.0.5/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)    13724 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 14:48:01.080787 plone.dexterity-3.0.5/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     1230 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/docs/INSTALL.txt
--rw-r--r--   0 maurits    (501) staff       (20)    12289 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      693 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)    12444 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/docs/WebDAV.txt
--rw-r--r--   0 maurits    (501) staff       (20)       88 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/extract.ini
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 14:48:01.081359 plone.dexterity-3.0.5/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 14:48:01.091899 plone.dexterity-3.0.5/plone/dexterity/
--rw-r--r--   0 maurits    (501) staff       (20)       59 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      789 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/behavior.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 14:48:01.096447 plone.dexterity-3.0.5/plone/dexterity/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     7264 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/browser/add.py
--rw-r--r--   0 maurits    (501) staff       (20)      896 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/browser/base.py
--rw-r--r--   0 maurits    (501) staff       (20)     2406 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      870 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/browser/containercontentcore.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2812 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/browser/edit.py
--rw-r--r--   0 maurits    (501) staff       (20)     1930 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/browser/fti.pt
--rw-r--r--   0 maurits    (501) staff       (20)      317 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/browser/fti.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 14:48:01.097487 plone.dexterity-3.0.5/plone/dexterity/browser/icons/
--rw-r--r--   0 maurits    (501) staff       (20)      940 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/browser/icons/container_icon.gif
--rw-r--r--   0 maurits    (501) staff       (20)      915 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/browser/icons/item_icon.gif
--rw-r--r--   0 maurits    (501) staff       (20)     4530 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/browser/icons/typeinfo.gif
--rw-r--r--   0 maurits    (501) staff       (20)     1490 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/browser/item.pt
--rw-r--r--   0 maurits    (501) staff       (20)      870 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/browser/itemcontentcore.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3243 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/browser/traversal.py
--rw-r--r--   0 maurits    (501) staff       (20)      599 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/browser/view.py
--rw-r--r--   0 maurits    (501) staff       (20)     3990 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    30030 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/content.py
--rw-r--r--   0 maurits    (501) staff       (20)      997 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/events.py
--rw-r--r--   0 maurits    (501) staff       (20)     4955 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/exportimport.py
--rw-r--r--   0 maurits    (501) staff       (20)     1987 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/factory.py
--rw-r--r--   0 maurits    (501) staff       (20)    26980 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/filerepresentation.py
--rw-r--r--   0 maurits    (501) staff       (20)    17449 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/fti.py
--rw-r--r--   0 maurits    (501) staff       (20)       88 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/i18n.py
--rw-r--r--   0 maurits    (501) staff       (20)     5176 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      228 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/meta.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      903 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/primary.py
--rw-r--r--   0 maurits    (501) staff       (20)    14496 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/schema.py
--rw-r--r--   0 maurits    (501) staff       (20)      423 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/synchronize.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 14:48:01.103798 plone.dexterity-3.0.5/plone/dexterity/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3712 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/tests/case.py
--rw-r--r--   0 maurits    (501) staff       (20)      612 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/tests/schemata.py
--rw-r--r--   0 maurits    (501) staff       (20)      480 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/tests/test.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1957 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/tests/test_behavior.py
--rw-r--r--   0 maurits    (501) staff       (20)    40528 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/tests/test_content.py
--rw-r--r--   0 maurits    (501) staff       (20)      943 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/tests/test_content_integration.py
--rw-r--r--   0 maurits    (501) staff       (20)     1483 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/tests/test_exportimport.py
--rw-r--r--   0 maurits    (501) staff       (20)     5070 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/tests/test_factory.py
--rw-r--r--   0 maurits    (501) staff       (20)      653 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/tests/test_filerepresentation.py
--rw-r--r--   0 maurits    (501) staff       (20)    36350 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/tests/test_fti.py
--rw-r--r--   0 maurits    (501) staff       (20)     1091 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/tests/test_primary.py
--rw-r--r--   0 maurits    (501) staff       (20)     7553 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/tests/test_schema.py
--rw-r--r--   0 maurits    (501) staff       (20)     7420 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/tests/test_schema_cache.py
--rw-r--r--   0 maurits    (501) staff       (20)    12652 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/tests/test_security.py
--rw-r--r--   0 maurits    (501) staff       (20)     1397 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/tests/test_synchronize.py
--rw-r--r--   0 maurits    (501) staff       (20)     4027 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)    22036 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/tests/test_views.py
--rw-r--r--   0 maurits    (501) staff       (20)    42920 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/tests/test_webdav.py
--rw-r--r--   0 maurits    (501) staff       (20)     7983 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone/dexterity/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-27 14:48:01.104217 plone.dexterity-3.0.5/plone.dexterity.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    41152 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone.dexterity.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2189 2024-02-27 14:48:01.000000 plone.dexterity-3.0.5/plone.dexterity.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone.dexterity.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone.dexterity.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone.dexterity.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      271 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone.dexterity.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/plone.dexterity.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4238 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2024-02-27 14:48:01.106636 plone.dexterity-3.0.5/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2130 2024-02-27 14:48:00.000000 plone.dexterity-3.0.5/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:52.616786 plone_dexterity-3.0.6/
+-rw-r--r--   0 maurits    (501) staff       (20)    25978 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      207 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    41326 2024-04-25 19:34:52.616368 plone_dexterity-3.0.6/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)    13724 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:52.594748 plone_dexterity-3.0.6/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     1230 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/docs/INSTALL.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    12289 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      693 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    12444 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/docs/WebDAV.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       88 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/extract.ini
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:52.595332 plone_dexterity-3.0.6/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:52.604023 plone_dexterity-3.0.6/plone/dexterity/
+-rw-r--r--   0 maurits    (501) staff       (20)       59 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      789 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/behavior.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:52.608098 plone_dexterity-3.0.6/plone/dexterity/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7264 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/browser/add.py
+-rw-r--r--   0 maurits    (501) staff       (20)      896 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/browser/base.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2406 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      870 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/browser/containercontentcore.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2812 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/browser/edit.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1930 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/browser/fti.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      317 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/browser/fti.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:52.609009 plone_dexterity-3.0.6/plone/dexterity/browser/icons/
+-rw-r--r--   0 maurits    (501) staff       (20)      940 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/browser/icons/container_icon.gif
+-rw-r--r--   0 maurits    (501) staff       (20)      915 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/browser/icons/item_icon.gif
+-rw-r--r--   0 maurits    (501) staff       (20)     4530 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/browser/icons/typeinfo.gif
+-rw-r--r--   0 maurits    (501) staff       (20)     1490 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/browser/item.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      870 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/browser/itemcontentcore.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3243 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/browser/traversal.py
+-rw-r--r--   0 maurits    (501) staff       (20)      599 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/browser/view.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3990 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    30030 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/content.py
+-rw-r--r--   0 maurits    (501) staff       (20)      997 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/events.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4955 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/exportimport.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1987 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/factory.py
+-rw-r--r--   0 maurits    (501) staff       (20)    26980 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/filerepresentation.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17449 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/fti.py
+-rw-r--r--   0 maurits    (501) staff       (20)       88 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/i18n.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5176 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      228 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/meta.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      903 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/primary.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14496 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/schema.py
+-rw-r--r--   0 maurits    (501) staff       (20)      423 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/synchronize.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:52.614995 plone_dexterity-3.0.6/plone/dexterity/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3712 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/tests/case.py
+-rw-r--r--   0 maurits    (501) staff       (20)      612 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/tests/schemata.py
+-rw-r--r--   0 maurits    (501) staff       (20)      480 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/tests/test.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1957 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/tests/test_behavior.py
+-rw-r--r--   0 maurits    (501) staff       (20)    40528 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/tests/test_content.py
+-rw-r--r--   0 maurits    (501) staff       (20)      943 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/tests/test_content_integration.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1483 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/tests/test_exportimport.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5070 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/tests/test_factory.py
+-rw-r--r--   0 maurits    (501) staff       (20)      653 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/tests/test_filerepresentation.py
+-rw-r--r--   0 maurits    (501) staff       (20)    36350 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/tests/test_fti.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1091 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/tests/test_primary.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7553 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/tests/test_schema.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7420 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/tests/test_schema_cache.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12652 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/tests/test_security.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1397 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/tests/test_synchronize.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4027 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)    22036 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/tests/test_views.py
+-rw-r--r--   0 maurits    (501) staff       (20)    42975 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/tests/test_webdav.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7983 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/plone/dexterity/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:34:52.615405 plone_dexterity-3.0.6/plone.dexterity.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    41326 2024-04-25 19:34:52.000000 plone_dexterity-3.0.6/plone.dexterity.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2189 2024-04-25 19:34:52.000000 plone_dexterity-3.0.6/plone.dexterity.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-25 19:34:52.000000 plone_dexterity-3.0.6/plone.dexterity.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-25 19:34:52.000000 plone_dexterity-3.0.6/plone.dexterity.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-25 19:34:52.000000 plone_dexterity-3.0.6/plone.dexterity.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      271 2024-04-25 19:34:52.000000 plone_dexterity-3.0.6/plone.dexterity.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-25 19:34:52.000000 plone_dexterity-3.0.6/plone.dexterity.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4229 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-04-25 19:34:52.616868 plone_dexterity-3.0.6/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2130 2024-04-25 19:34:51.000000 plone_dexterity-3.0.6/setup.py
```

### Comparing `plone.dexterity-3.0.5/CHANGES.rst` & `plone_dexterity-3.0.6/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.6 (2024-04-25)
+------------------
+
+Bug fixes:
+
+
+- Fix tests to work with Zope master which expects requests to have an `ensure_publishable` method.
+  [maurits] (#1202)
+
+
 3.0.5 (2024-02-27)
 ------------------
 
 Bug fixes:
 
 
 - Fix a traversal error that happens when traversing a WebDAV resource and the virtual host monster is used.
```

### Comparing `plone.dexterity-3.0.5/PKG-INFO` & `plone_dexterity-3.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.dexterity
-Version: 3.0.5
+Version: 3.0.6
 Summary: Framework for content types as filesystem code and TTW (Zope/CMF/Plone)
 Home-page: https://github.com/plone/plone.dexterity
 Author: Martin Aspeli
 Author-email: optilude@gmail.com
 Maintainer: The Plone Release Team and Community
 Maintainer-email: releaseteam@plone.org
 License: GPL version 2
@@ -281,14 +281,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.6 (2024-04-25)
+------------------
+
+Bug fixes:
+
+
+- Fix tests to work with Zope master which expects requests to have an `ensure_publishable` method.
+  [maurits] (#1202)
+
+
 3.0.5 (2024-02-27)
 ------------------
 
 Bug fixes:
 
 
 - Fix a traversal error that happens when traversing a WebDAV resource and the virtual host monster is used.
```

### Comparing `plone.dexterity-3.0.5/README.rst` & `plone_dexterity-3.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/docs/INSTALL.txt` & `plone_dexterity-3.0.6/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/docs/LICENSE.GPL` & `plone_dexterity-3.0.6/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/docs/LICENSE.txt` & `plone_dexterity-3.0.6/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/docs/WebDAV.txt` & `plone_dexterity-3.0.6/docs/WebDAV.txt`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/behavior.py` & `plone_dexterity-3.0.6/plone/dexterity/behavior.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/browser/add.py` & `plone_dexterity-3.0.6/plone/dexterity/browser/add.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/browser/base.py` & `plone_dexterity-3.0.6/plone/dexterity/browser/base.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/browser/configure.zcml` & `plone_dexterity-3.0.6/plone/dexterity/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/browser/containercontentcore.pt` & `plone_dexterity-3.0.6/plone/dexterity/browser/containercontentcore.pt`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/browser/edit.py` & `plone_dexterity-3.0.6/plone/dexterity/browser/edit.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/browser/fti.pt` & `plone_dexterity-3.0.6/plone/dexterity/browser/fti.pt`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/browser/icons/container_icon.gif` & `plone_dexterity-3.0.6/plone/dexterity/browser/icons/container_icon.gif`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/browser/icons/item_icon.gif` & `plone_dexterity-3.0.6/plone/dexterity/browser/icons/item_icon.gif`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/browser/icons/typeinfo.gif` & `plone_dexterity-3.0.6/plone/dexterity/browser/icons/typeinfo.gif`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/browser/item.pt` & `plone_dexterity-3.0.6/plone/dexterity/browser/item.pt`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/browser/itemcontentcore.pt` & `plone_dexterity-3.0.6/plone/dexterity/browser/itemcontentcore.pt`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/browser/traversal.py` & `plone_dexterity-3.0.6/plone/dexterity/browser/traversal.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/browser/view.py` & `plone_dexterity-3.0.6/plone/dexterity/browser/view.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/configure.zcml` & `plone_dexterity-3.0.6/plone/dexterity/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/content.py` & `plone_dexterity-3.0.6/plone/dexterity/content.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/events.py` & `plone_dexterity-3.0.6/plone/dexterity/events.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/exportimport.py` & `plone_dexterity-3.0.6/plone/dexterity/exportimport.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/factory.py` & `plone_dexterity-3.0.6/plone/dexterity/factory.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/filerepresentation.py` & `plone_dexterity-3.0.6/plone/dexterity/filerepresentation.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/fti.py` & `plone_dexterity-3.0.6/plone/dexterity/fti.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/interfaces.py` & `plone_dexterity-3.0.6/plone/dexterity/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/primary.py` & `plone_dexterity-3.0.6/plone/dexterity/primary.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/schema.py` & `plone_dexterity-3.0.6/plone/dexterity/schema.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/tests/case.py` & `plone_dexterity-3.0.6/plone/dexterity/tests/case.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/tests/schemata.py` & `plone_dexterity-3.0.6/plone/dexterity/tests/schemata.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/tests/test_behavior.py` & `plone_dexterity-3.0.6/plone/dexterity/tests/test_behavior.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/tests/test_content.py` & `plone_dexterity-3.0.6/plone/dexterity/tests/test_content.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/tests/test_content_integration.py` & `plone_dexterity-3.0.6/plone/dexterity/tests/test_content_integration.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/tests/test_exportimport.py` & `plone_dexterity-3.0.6/plone/dexterity/tests/test_exportimport.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/tests/test_factory.py` & `plone_dexterity-3.0.6/plone/dexterity/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/tests/test_filerepresentation.py` & `plone_dexterity-3.0.6/plone/dexterity/tests/test_filerepresentation.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/tests/test_fti.py` & `plone_dexterity-3.0.6/plone/dexterity/tests/test_fti.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/tests/test_primary.py` & `plone_dexterity-3.0.6/plone/dexterity/tests/test_primary.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/tests/test_schema.py` & `plone_dexterity-3.0.6/plone/dexterity/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/tests/test_schema_cache.py` & `plone_dexterity-3.0.6/plone/dexterity/tests/test_schema_cache.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/tests/test_security.py` & `plone_dexterity-3.0.6/plone/dexterity/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/tests/test_synchronize.py` & `plone_dexterity-3.0.6/plone/dexterity/tests/test_synchronize.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/tests/test_utils.py` & `plone_dexterity-3.0.6/plone/dexterity/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/tests/test_views.py` & `plone_dexterity-3.0.6/plone/dexterity/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone/dexterity/tests/test_webdav.py` & `plone_dexterity-3.0.6/plone/dexterity/tests/test_webdav.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,18 @@
 
 class DAVTestRequest(TestRequest):
     get_header = TestRequest.getHeader
 
     def _createResponse(self):
         return HTTPResponse()
 
+    def ensure_publishable(self, obj, for_call=False):
+        # Needed for Zope > 5.9.
+        return
+
 
 class TestWebZope2DAVAPI(MockTestCase):
     def test_get_size_no_adapter(self):
         item = Item("test")
 
         self.assertEqual(0, item.get_size())
 
@@ -597,17 +601,14 @@
 </d:responsedescription>
 </d:response>
 </d:multistatus>
 """
         )
         body = body.strip()
         result = response.getBody().strip()
-        # TODO: remove next line when Zope 5.8.1 is released and used in coredev.
-        # Then also remove codespell settings from .meta.toml and pyproject.toml.
-        result = result.replace(b"succeded", b"succeeded")
         self.assertEqual(body, result)
 
     def test_LOCK(self):
         # Too much WebDAV magic - just test that it delegates correctly
         class TestContainer(Container):
             def LOCK(self, request, response):
                 self._locked = (
@@ -1291,46 +1292,52 @@
     def lock_request(self):
         lock_request = self.get_request.clone()
         lock_request["REQUEST_METHOD"] = "LOCK"
         lock_request.maybe_webdav_client = True
         return lock_request
 
     def test_get_subfolder(self):
-        traversal = DexterityPublishTraverse(self.folder, None)
-        traversed = traversal.publishTraverse(self.get_request, "subfolder")
+        request = self.get_request
+        traversal = DexterityPublishTraverse(self.folder, request)
+        traversed = traversal.publishTraverse(request, "subfolder")
         self.assertEqual(traversed, self.subfolder)
 
     def test_lock_subfolder(self):
-        traversal = DexterityPublishTraverse(self.folder, None)
-        traversed = traversal.publishTraverse(self.lock_request, "subfolder")
+        request = self.lock_request
+        traversal = DexterityPublishTraverse(self.folder, request)
+        traversed = traversal.publishTraverse(request, "subfolder")
         self.assertEqual(traversed, self.subfolder)
 
     def test_get_acquired(self):
-        traversal = DexterityPublishTraverse(self.subfolder, None)
-        traversed = traversal.publishTraverse(self.get_request, "folder")
+        request = self.get_request
+        traversal = DexterityPublishTraverse(self.subfolder, request)
+        traversed = traversal.publishTraverse(request, "folder")
         self.assertEqual(traversed, self.folder)
 
     def test_lock_acquired(self):
         """Ensure we are protected against acquisition:
         traversing to an acquired object should return a NullResource
         """
         from webdav.NullResource import NullResource
 
-        traversal = DexterityPublishTraverse(self.subfolder, None)
-        traversed = traversal.publishTraverse(self.lock_request, "folder")
+        request = self.lock_request
+        traversal = DexterityPublishTraverse(self.subfolder, request)
+        traversed = traversal.publishTraverse(request, "folder")
         self.assertIsInstance(traversed, NullResource)
 
     def test_get_vhm(self):
         """Ensure we can handle virtual hosting with regular requests"""
         from Products.SiteAccess.VirtualHostMonster import VirtualHostMonster
 
-        traversal = DexterityPublishTraverse(self.folder, None)
-        traversed = traversal.publishTraverse(self.get_request, "virtual_hosting")
+        request = self.get_request
+        traversal = DexterityPublishTraverse(self.folder, request)
+        traversed = traversal.publishTraverse(request, "virtual_hosting")
         self.assertIsInstance(traversed, VirtualHostMonster)
 
     def test_lock_vhm(self):
         """Ensure we can handle virtual hosting with dav requests"""
         from Products.SiteAccess.VirtualHostMonster import VirtualHostMonster
 
-        traversal = DexterityPublishTraverse(self.folder, None)
-        traversed = traversal.publishTraverse(self.lock_request, "virtual_hosting")
+        request = self.lock_request
+        traversal = DexterityPublishTraverse(self.folder, request)
+        traversed = traversal.publishTraverse(request, "virtual_hosting")
         self.assertIsInstance(traversed, VirtualHostMonster)
```

### Comparing `plone.dexterity-3.0.5/plone/dexterity/utils.py` & `plone_dexterity-3.0.6/plone/dexterity/utils.py`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/plone.dexterity.egg-info/PKG-INFO` & `plone_dexterity-3.0.6/plone.dexterity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.dexterity
-Version: 3.0.5
+Version: 3.0.6
 Summary: Framework for content types as filesystem code and TTW (Zope/CMF/Plone)
 Home-page: https://github.com/plone/plone.dexterity
 Author: Martin Aspeli
 Author-email: optilude@gmail.com
 Maintainer: The Plone Release Team and Community
 Maintainer-email: releaseteam@plone.org
 License: GPL version 2
@@ -281,14 +281,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.6 (2024-04-25)
+------------------
+
+Bug fixes:
+
+
+- Fix tests to work with Zope master which expects requests to have an `ensure_publishable` method.
+  [maurits] (#1202)
+
+
 3.0.5 (2024-02-27)
 ------------------
 
 Bug fixes:
 
 
 - Fix a traversal error that happens when traversing a WebDAV resource and the virtual host monster is used.
```

### Comparing `plone.dexterity-3.0.5/plone.dexterity.egg-info/SOURCES.txt` & `plone_dexterity-3.0.6/plone.dexterity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.dexterity-3.0.5/pyproject.toml` & `plone_dexterity-3.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 #  [pyproject]
 #  black_extra_lines = """
 #  extra_configuration
 #  """
 ##
 
 [tool.codespell]
-ignore-words-list = "discreet,succeded"
+ignore-words-list = "discreet"
 skip = "*.po,"
 ##
 # Add extra configuration options in .meta.toml:
 #  [pyproject]
 #  codespell_ignores = "foo,bar"
 #  codespell_skip = "*.po,*.map,package-lock.json"
 ##
```

### Comparing `plone.dexterity-3.0.5/setup.py` & `plone_dexterity-3.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.0.5"
+version = "3.0.6"
 
 
 long_description = (
     f"{Path('README.rst').read_text()}\n{Path('CHANGES.rst').read_text()}"
 )
```


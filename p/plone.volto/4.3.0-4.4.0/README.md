# Comparing `tmp/plone.volto-4.3.0.tar.gz` & `tmp/plone_volto-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.volto-4.3.0.tar", last modified: Tue Jan 30 18:02:23 2024, max compression
+gzip compressed data, was "plone_volto-4.4.0.tar", last modified: Thu Apr 25 19:38:13 2024, max compression
```

## Comparing `plone.volto-4.3.0.tar` & `plone_volto-4.4.0.tar`

### file list

```diff
@@ -1,161 +1,168 @@
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.516196 plone.volto-4.3.0/
--rw-r--r--   0 davisagli   (501) staff       (20)    15342 2024-01-30 18:02:23.000000 plone.volto-4.3.0/CHANGES.rst
--rw-r--r--   0 davisagli   (501) staff       (20)      369 2024-01-30 18:02:23.000000 plone.volto-4.3.0/CONTRIBUTORS.rst
--rw-r--r--   0 davisagli   (501) staff       (20)    28103 2024-01-30 18:02:23.516056 plone.volto-4.3.0/PKG-INFO
--rw-r--r--   0 davisagli   (501) staff       (20)    11466 2024-01-30 18:02:23.000000 plone.volto-4.3.0/README.rst
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.501638 plone.volto-4.3.0/docs/
--rw-r--r--   0 davisagli   (501) staff       (20)    18092 2024-01-30 18:02:23.000000 plone.volto-4.3.0/docs/LICENSE.GPL
--rw-r--r--   0 davisagli   (501) staff       (20)      657 2024-01-30 18:02:23.000000 plone.volto-4.3.0/docs/LICENSE.rst
--rw-r--r--   0 davisagli   (501) staff       (20)       74 2024-01-30 18:02:23.000000 plone.volto-4.3.0/docs/index.rst
--rw-r--r--   0 davisagli   (501) staff       (20)      881 2024-01-30 18:02:23.000000 plone.volto-4.3.0/pyproject.toml
--rw-r--r--   0 davisagli   (501) staff       (20)      402 2024-01-30 18:02:23.000000 plone.volto-4.3.0/requirements.txt
--rw-r--r--   0 davisagli   (501) staff       (20)       38 2024-01-30 18:02:23.516234 plone.volto-4.3.0/setup.cfg
--rw-r--r--   0 davisagli   (501) staff       (20)     2227 2024-01-30 18:02:23.000000 plone.volto-4.3.0/setup.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.497670 plone.volto-4.3.0/src/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.501789 plone.volto-4.3.0/src/plone/
--rw-r--r--   0 davisagli   (501) staff       (20)       80 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/__init__.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.505472 plone.volto-4.3.0/src/plone/volto/
--rw-r--r--   0 davisagli   (501) staff       (20)      222 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/__init__.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.506227 plone.volto-4.3.0/src/plone/volto/behaviors/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/behaviors/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1168 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/behaviors/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)      534 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/behaviors/headtitle.py
--rw-r--r--   0 davisagli   (501) staff       (20)      345 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/behaviors/navtitle.py
--rw-r--r--   0 davisagli   (501) staff       (20)      727 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/behaviors/preview.py
--rw-r--r--   0 davisagli   (501) staff       (20)     2475 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/behaviors/preview_link.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1614 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/blocksuuidfixer.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.507247 plone.volto-4.3.0/src/plone/volto/browser/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/browser/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     2046 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/browser/breadcrumbs.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1780 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/browser/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)     3673 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/browser/migrate_richtext.pt
--rw-r--r--   0 davisagli   (501) staff       (20)     5573 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/browser/migrate_richtext.py
--rw-r--r--   0 davisagli   (501) staff       (20)     6949 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/browser/migrate_to_volto.pt
--rw-r--r--   0 davisagli   (501) staff       (20)    14011 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/browser/migrate_to_volto.py
--rw-r--r--   0 davisagli   (501) staff       (20)     4499 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/browser/navigation.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.507373 plone.volto-4.3.0/src/plone/volto/browser/static/
--rw-r--r--   0 davisagli   (501) staff       (20)      754 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/browser/static/volto.svg
--rw-r--r--   0 davisagli   (501) staff       (20)     1368 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/browser/voltobackendwarning.pt
--rw-r--r--   0 davisagli   (501) staff       (20)     2713 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)      697 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/content.py
--rw-r--r--   0 davisagli   (501) staff       (20)      974 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/controlpanel.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.507838 plone.volto-4.3.0/src/plone/volto/coresandbox/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/coresandbox/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)      540 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/coresandbox/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)    28820 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/coresandbox/example.py
--rw-r--r--   0 davisagli   (501) staff       (20)      745 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/coresandbox/vocabularies.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.508043 plone.volto-4.3.0/src/plone/volto/cors/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/cors/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)      462 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/cors/configure.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.508524 plone.volto-4.3.0/src/plone/volto/default_homepage/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/default_homepage/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)    34756 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/default_homepage/default.py
--rw-r--r--   0 davisagli   (501) staff       (20)    28345 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/default_homepage/demo.py
--rw-r--r--   0 davisagli   (501) staff       (20)     3019 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/default_homepage/lrf.py
--rw-r--r--   0 davisagli   (501) staff       (20)      516 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/dependencies.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)     1447 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/indexers.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1006 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/interfaces.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1576 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/linkintegrity.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.508745 plone.volto-4.3.0/src/plone/volto/locales/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.498309 plone.volto-4.3.0/src/plone/volto/locales/de/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.508857 plone.volto-4.3.0/src/plone/volto/locales/de/LC_MESSAGES/
--rw-r--r--   0 davisagli   (501) staff       (20)     4905 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/locales/de/LC_MESSAGES/plone.volto.po
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.498422 plone.volto-4.3.0/src/plone/volto/locales/en/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.508975 plone.volto-4.3.0/src/plone/volto/locales/en/LC_MESSAGES/
--rw-r--r--   0 davisagli   (501) staff       (20)     4201 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/locales/en/LC_MESSAGES/plone.volto.po
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.498543 plone.volto-4.3.0/src/plone/volto/locales/es/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.509093 plone.volto-4.3.0/src/plone/volto/locales/es/LC_MESSAGES/
--rw-r--r--   0 davisagli   (501) staff       (20)     5074 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/locales/es/LC_MESSAGES/plone.volto.po
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.498655 plone.volto-4.3.0/src/plone/volto/locales/eu/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.509203 plone.volto-4.3.0/src/plone/volto/locales/eu/LC_MESSAGES/
--rw-r--r--   0 davisagli   (501) staff       (20)     4982 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/locales/eu/LC_MESSAGES/plone.volto.po
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.498767 plone.volto-4.3.0/src/plone/volto/locales/it/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.509315 plone.volto-4.3.0/src/plone/volto/locales/it/LC_MESSAGES/
--rw-r--r--   0 davisagli   (501) staff       (20)     4457 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/locales/it/LC_MESSAGES/plone.volto.po
--rw-r--r--   0 davisagli   (501) staff       (20)     4148 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/locales/plone.volto.pot
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.498887 plone.volto-4.3.0/src/plone/volto/locales/pt_BR/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.509431 plone.volto-4.3.0/src/plone/volto/locales/pt_BR/LC_MESSAGES/
--rw-r--r--   0 davisagli   (501) staff       (20)     5477 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/locales/pt_BR/LC_MESSAGES/plone.volto.po
--rwxr-xr-x   0 davisagli   (501) staff       (20)      502 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/locales/update.sh
--rw-r--r--   0 davisagli   (501) staff       (20)      256 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/overrides.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)     2599 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/patches.py
--rw-r--r--   0 davisagli   (501) staff       (20)      858 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/patches.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.499801 plone.volto-4.3.0/src/plone/volto/profiles/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.510154 plone.volto-4.3.0/src/plone/volto/profiles/coresandbox/
--rw-r--r--   0 davisagli   (501) staff       (20)      206 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/coresandbox/diff_tool.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      141 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/coresandbox/metadata.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      210 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/coresandbox/repositorytool.xml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.510285 plone.volto-4.3.0/src/plone/volto/profiles/coresandbox/types/
--rw-r--r--   0 davisagli   (501) staff       (20)     2515 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/coresandbox/types/example.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      165 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/coresandbox/types.xml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.511003 plone.volto-4.3.0/src/plone/volto/profiles/default/
--rw-r--r--   0 davisagli   (501) staff       (20)      639 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/default/actions.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      156 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/default/browserlayer.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      314 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/default/catalog.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      612 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/default/controlpanel.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      181 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/default/metadata.xml
--rw-r--r--   0 davisagli   (501) staff       (20)     1791 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/default/registry.xml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.511836 plone.volto-4.3.0/src/plone/volto/profiles/default/types/
--rw-r--r--   0 davisagli   (501) staff       (20)      286 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/default/types/Collection.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      814 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/default/types/Document.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      501 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/default/types/Event.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      278 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/default/types/Folder.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      604 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/default/types/LRF.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      464 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/default/types/News_Item.xml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.512127 plone.volto-4.3.0/src/plone/volto/profiles/demo/
--rw-r--r--   0 davisagli   (501) staff       (20)      141 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/demo/metadata.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      291 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/demo/rolemap.xml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.512259 plone.volto-4.3.0/src/plone/volto/profiles/homepage/
--rw-r--r--   0 davisagli   (501) staff       (20)      141 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/homepage/metadata.xml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.512565 plone.volto-4.3.0/src/plone/volto/profiles/multilingual/
--rw-r--r--   0 davisagli   (501) staff       (20)      209 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/multilingual/metadata.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      546 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/multilingual/registry.xml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.512837 plone.volto-4.3.0/src/plone/volto/profiles/richtext/
--rw-r--r--   0 davisagli   (501) staff       (20)      141 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/richtext/metadata.xml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.512976 plone.volto-4.3.0/src/plone/volto/profiles/richtext/types/
--rw-r--r--   0 davisagli   (501) staff       (20)      320 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/richtext/types/Document.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      166 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/richtext/types.xml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.513122 plone.volto-4.3.0/src/plone/volto/profiles/uninstall/
--rw-r--r--   0 davisagli   (501) staff       (20)      114 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 davisagli   (501) staff       (20)     3696 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/profiles.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)     3436 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/scaling.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.514050 plone.volto-4.3.0/src/plone/volto/scripts/
--rw-r--r--   0 davisagli   (501) staff       (20)      736 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/scripts/add_image_field_metadata.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1206 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/scripts/auditblocks.py
--rw-r--r--   0 davisagli   (501) staff       (20)      202 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/scripts/clear-rebuild-catalog.py
--rw-r--r--   0 davisagli   (501) staff       (20)      773 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/scripts/listingaddsummary.py
--rw-r--r--   0 davisagli   (501) staff       (20)      724 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/scripts/migrate_richtext.py
--rwxr-xr-x   0 davisagli   (501) staff       (20)      123 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/scripts/packdb.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1594 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/scripts/searchscalesinimageblocks.py
--rw-r--r--   0 davisagli   (501) staff       (20)      932 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/scripts/utils.py
--rw-r--r--   0 davisagli   (501) staff       (20)    10185 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/setuphandlers.py
--rw-r--r--   0 davisagli   (501) staff       (20)      312 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/summary.py
--rw-r--r--   0 davisagli   (501) staff       (20)     4513 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/testing.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.515406 plone.volto-4.3.0/src/plone/volto/tests/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/tests/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1172 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/tests/test_coresandbox.py
--rw-r--r--   0 davisagli   (501) staff       (20)     3609 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/tests/test_indexers.py
--rw-r--r--   0 davisagli   (501) staff       (20)     2442 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/tests/test_linkintegrity.py
--rw-r--r--   0 davisagli   (501) staff       (20)    11771 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/tests/test_migrate_to_volto.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1823 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/tests/test_preview_link_behavior.py
--rw-r--r--   0 davisagli   (501) staff       (20)     2126 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/tests/test_scripts.py
--rw-r--r--   0 davisagli   (501) staff       (20)     3102 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/tests/test_setup.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1709 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/tests/test_summary_serialization.py
--rw-r--r--   0 davisagli   (501) staff       (20)    11245 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/tests/test_transforms.py
--rw-r--r--   0 davisagli   (501) staff       (20)     6498 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/tests/test_upgrades.py
--rw-r--r--   0 davisagli   (501) staff       (20)     4777 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/transforms.py
--rw-r--r--   0 davisagli   (501) staff       (20)     6086 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/upgrades.py
--rw-r--r--   0 davisagli   (501) staff       (20)     2222 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/upgrades.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.515826 plone.volto-4.3.0/src/plone/volto/vocabularies/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/vocabularies/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)      105 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/vocabularies/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)     4305 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone/volto/vocabularies/subject.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-01-30 18:02:23.502824 plone.volto-4.3.0/src/plone.volto.egg-info/
--rw-r--r--   0 davisagli   (501) staff       (20)    28103 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone.volto.egg-info/PKG-INFO
--rw-r--r--   0 davisagli   (501) staff       (20)     4741 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone.volto.egg-info/SOURCES.txt
--rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone.volto.egg-info/dependency_links.txt
--rw-r--r--   0 davisagli   (501) staff       (20)       40 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone.volto.egg-info/entry_points.txt
--rw-r--r--   0 davisagli   (501) staff       (20)        6 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone.volto.egg-info/namespace_packages.txt
--rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone.volto.egg-info/not-zip-safe
--rw-r--r--   0 davisagli   (501) staff       (20)      249 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone.volto.egg-info/requires.txt
--rw-r--r--   0 davisagli   (501) staff       (20)        6 2024-01-30 18:02:23.000000 plone.volto-4.3.0/src/plone.volto.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.343583 plone_volto-4.4.0/
+-rw-r--r--   0 maurits    (501) staff       (20)    15669 2024-04-25 19:38:12.000000 plone_volto-4.4.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      369 2024-04-25 19:38:12.000000 plone_volto-4.4.0/CONTRIBUTORS.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    28953 2024-04-25 19:38:13.343169 plone_volto-4.4.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)    11466 2024-04-25 19:38:12.000000 plone_volto-4.4.0/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.299133 plone_volto-4.4.0/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    18092 2024-04-25 19:38:12.000000 plone_volto-4.4.0/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      657 2024-04-25 19:38:12.000000 plone_volto-4.4.0/docs/LICENSE.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       74 2024-04-25 19:38:12.000000 plone_volto-4.4.0/docs/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      881 2024-04-25 19:38:12.000000 plone_volto-4.4.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      402 2024-04-25 19:38:12.000000 plone_volto-4.4.0/requirements.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-04-25 19:38:13.343657 plone_volto-4.4.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2227 2024-04-25 19:38:12.000000 plone_volto-4.4.0/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.290663 plone_volto-4.4.0/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.299517 plone_volto-4.4.0/src/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       80 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.309208 plone_volto-4.4.0/src/plone/volto/
+-rw-r--r--   0 maurits    (501) staff       (20)      222 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      281 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/bbb.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.311723 plone_volto-4.4.0/src/plone/volto/behaviors/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/behaviors/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1168 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/behaviors/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      534 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/behaviors/headtitle.py
+-rw-r--r--   0 maurits    (501) staff       (20)      345 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/behaviors/navtitle.py
+-rw-r--r--   0 maurits    (501) staff       (20)      727 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/behaviors/preview.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2475 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/behaviors/preview_link.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1614 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/blocksuuidfixer.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.315734 plone_volto-4.4.0/src/plone/volto/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2207 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/browser/breadcrumbs.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1780 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3673 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/browser/migrate_richtext.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5573 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/browser/migrate_richtext.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6949 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/browser/migrate_to_volto.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    14003 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/browser/migrate_to_volto.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4586 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/browser/navigation.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.316024 plone_volto-4.4.0/src/plone/volto/browser/static/
+-rw-r--r--   0 maurits    (501) staff       (20)      754 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/browser/static/volto.svg
+-rw-r--r--   0 maurits    (501) staff       (20)     1368 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/browser/voltobackendwarning.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2665 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      697 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/content.py
+-rw-r--r--   0 maurits    (501) staff       (20)      974 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/controlpanel.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.317491 plone_volto-4.4.0/src/plone/volto/coresandbox/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/coresandbox/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      540 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/coresandbox/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    28820 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/coresandbox/example.py
+-rw-r--r--   0 maurits    (501) staff       (20)      745 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/coresandbox/vocabularies.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.318338 plone_volto-4.4.0/src/plone/volto/cors/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/cors/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      462 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/cors/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.319742 plone_volto-4.4.0/src/plone/volto/default_homepage/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/default_homepage/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    34756 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/default_homepage/default.py
+-rw-r--r--   0 maurits    (501) staff       (20)    28345 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/default_homepage/demo.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3019 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/default_homepage/lrf.py
+-rw-r--r--   0 maurits    (501) staff       (20)      516 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/dependencies.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1447 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/indexers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1006 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1576 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/linkintegrity.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.320598 plone_volto-4.4.0/src/plone/volto/locales/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.292111 plone_volto-4.4.0/src/plone/volto/locales/de/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.321373 plone_volto-4.4.0/src/plone/volto/locales/de/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)     2223 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/locales/de/LC_MESSAGES/plone.volto.mo
+-rw-r--r--   0 maurits    (501) staff       (20)     4905 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/locales/de/LC_MESSAGES/plone.volto.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.292372 plone_volto-4.4.0/src/plone/volto/locales/en/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.321948 plone_volto-4.4.0/src/plone/volto/locales/en/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)      622 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/locales/en/LC_MESSAGES/plone.volto.mo
+-rw-r--r--   0 maurits    (501) staff       (20)     4201 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/locales/en/LC_MESSAGES/plone.volto.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.292714 plone_volto-4.4.0/src/plone/volto/locales/es/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.322600 plone_volto-4.4.0/src/plone/volto/locales/es/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)     2528 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/locales/es/LC_MESSAGES/plone.volto.mo
+-rw-r--r--   0 maurits    (501) staff       (20)     5074 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/locales/es/LC_MESSAGES/plone.volto.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.292971 plone_volto-4.4.0/src/plone/volto/locales/eu/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.323396 plone_volto-4.4.0/src/plone/volto/locales/eu/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)     2437 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/locales/eu/LC_MESSAGES/plone.volto.mo
+-rw-r--r--   0 maurits    (501) staff       (20)     4982 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/locales/eu/LC_MESSAGES/plone.volto.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.293229 plone_volto-4.4.0/src/plone/volto/locales/it/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.324028 plone_volto-4.4.0/src/plone/volto/locales/it/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)     1145 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/locales/it/LC_MESSAGES/plone.volto.mo
+-rw-r--r--   0 maurits    (501) staff       (20)     4457 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/locales/it/LC_MESSAGES/plone.volto.po
+-rw-r--r--   0 maurits    (501) staff       (20)     4148 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/locales/plone.volto.pot
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.293486 plone_volto-4.4.0/src/plone/volto/locales/pt_BR/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.324868 plone_volto-4.4.0/src/plone/volto/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)     3322 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/locales/pt_BR/LC_MESSAGES/plone.volto.mo
+-rw-r--r--   0 maurits    (501) staff       (20)     5477 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/locales/pt_BR/LC_MESSAGES/plone.volto.po
+-rwxr-xr-x   0 maurits    (501) staff       (20)      502 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/locales/update.sh
+-rw-r--r--   0 maurits    (501) staff       (20)      256 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/overrides.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2599 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/patches.py
+-rw-r--r--   0 maurits    (501) staff       (20)      858 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/patches.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.295463 plone_volto-4.4.0/src/plone/volto/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.326249 plone_volto-4.4.0/src/plone/volto/profiles/coresandbox/
+-rw-r--r--   0 maurits    (501) staff       (20)      206 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/coresandbox/diff_tool.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      141 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/coresandbox/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      210 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/coresandbox/repositorytool.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.326626 plone_volto-4.4.0/src/plone/volto/profiles/coresandbox/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     2515 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/coresandbox/types/example.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      165 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/coresandbox/types.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.329038 plone_volto-4.4.0/src/plone/volto/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      639 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/default/actions.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      156 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      314 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/default/catalog.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      612 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/default/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      181 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1791 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/default/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.331442 plone_volto-4.4.0/src/plone/volto/profiles/default/types/
+-rw-r--r--   0 maurits    (501) staff       (20)      286 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/default/types/Collection.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      814 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/default/types/Document.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      501 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/default/types/Event.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      278 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/default/types/Folder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      604 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/default/types/LRF.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      464 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/default/types/News_Item.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.332282 plone_volto-4.4.0/src/plone/volto/profiles/demo/
+-rw-r--r--   0 maurits    (501) staff       (20)      141 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/demo/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      291 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/demo/rolemap.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.332597 plone_volto-4.4.0/src/plone/volto/profiles/homepage/
+-rw-r--r--   0 maurits    (501) staff       (20)      141 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/homepage/metadata.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.333458 plone_volto-4.4.0/src/plone/volto/profiles/multilingual/
+-rw-r--r--   0 maurits    (501) staff       (20)      209 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/multilingual/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      501 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/multilingual/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.334165 plone_volto-4.4.0/src/plone/volto/profiles/richtext/
+-rw-r--r--   0 maurits    (501) staff       (20)      141 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/richtext/metadata.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.334468 plone_volto-4.4.0/src/plone/volto/profiles/richtext/types/
+-rw-r--r--   0 maurits    (501) staff       (20)      320 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/richtext/types/Document.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      166 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/richtext/types.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.334920 plone_volto-4.4.0/src/plone/volto/profiles/uninstall/
+-rw-r--r--   0 maurits    (501) staff       (20)      114 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     3696 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/profiles.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3436 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/scaling.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.337581 plone_volto-4.4.0/src/plone/volto/scripts/
+-rw-r--r--   0 maurits    (501) staff       (20)      736 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/scripts/add_image_field_metadata.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1206 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/scripts/auditblocks.py
+-rw-r--r--   0 maurits    (501) staff       (20)      202 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/scripts/clear-rebuild-catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)      773 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/scripts/listingaddsummary.py
+-rw-r--r--   0 maurits    (501) staff       (20)      724 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/scripts/migrate_richtext.py
+-rwxr-xr-x   0 maurits    (501) staff       (20)      123 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/scripts/packdb.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1594 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/scripts/searchscalesinimageblocks.py
+-rw-r--r--   0 maurits    (501) staff       (20)      932 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/scripts/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10177 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)      312 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/summary.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4513 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.340873 plone_volto-4.4.0/src/plone/volto/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1172 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/tests/test_coresandbox.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3609 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/tests/test_indexers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2442 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/tests/test_linkintegrity.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11763 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/tests/test_migrate_to_volto.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1823 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/tests/test_preview_link_behavior.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2126 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/tests/test_scripts.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2444 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/tests/test_setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1709 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/tests/test_summary_serialization.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11245 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/tests/test_transforms.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6498 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/tests/test_upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4764 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/transforms.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6086 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2222 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/upgrades.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.341752 plone_volto-4.4.0/src/plone/volto/vocabularies/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/vocabularies/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      105 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/vocabularies/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4305 2024-04-25 19:38:12.000000 plone_volto-4.4.0/src/plone/volto/vocabularies/subject.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:38:13.342145 plone_volto-4.4.0/src/plone.volto.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    28953 2024-04-25 19:38:13.000000 plone_volto-4.4.0/src/plone.volto.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     5091 2024-04-25 19:38:13.000000 plone_volto-4.4.0/src/plone.volto.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-25 19:38:13.000000 plone_volto-4.4.0/src/plone.volto.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2024-04-25 19:38:13.000000 plone_volto-4.4.0/src/plone.volto.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-25 19:38:13.000000 plone_volto-4.4.0/src/plone.volto.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-25 19:38:13.000000 plone_volto-4.4.0/src/plone.volto.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      249 2024-04-25 19:38:13.000000 plone_volto-4.4.0/src/plone.volto.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-25 19:38:13.000000 plone_volto-4.4.0/src/plone.volto.egg-info/top_level.txt
```

### Comparing `plone.volto-4.3.0/CHANGES.rst` & `plone_volto-4.4.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,30 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.4.0 (2024-04-25)
+------------------
+
+New features:
+
+
+- Import ILanguageSchema from plone.i18n.interfaces instead of Products.CMFPlone.interfaces.controlpanel. @ksuess
+  profile "plone.volto:multilingual": Add language german. @ksuess (#144)
+
+
+Bug fixes:
+
+
+- Avoid a deprecated import warnings in Plone 6. @davisagli (#147)
+
+
 4.3.0 (2024-01-30)
 ------------------
 
 New features:
 
 
 - Add `VOLTO_FRONTEND_DOMAIN` as env var for `volto.frontend_domain` registry setting
```

### Comparing `plone.volto-4.3.0/PKG-INFO` & `plone_volto-4.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.volto
-Version: 4.3.0
+Version: 4.4.0
 Summary: Volto integration add-on for Plone
 Home-page: https://github.com/plone/plone.volto
 Author: Plone Foundation
 Author-email: tisto@plone.org
 License: GPL version 2
 Keywords: Python Plone CMS
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,27 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.7
+Requires-Dist: plone.api
+Requires-Dist: Products.GenericSetup
+Requires-Dist: setuptools
+Requires-Dist: plone.restapi>=8.41.0
+Requires-Dist: plone.app.vocabularies>=4.3.0
+Requires-Dist: collective.monkeypatcher
 Provides-Extra: test
+Requires-Dist: plone.app.testing; extra == "test"
+Requires-Dist: plone.testing; extra == "test"
+Requires-Dist: plone.app.contenttypes; extra == "test"
+Requires-Dist: plone.app.robotframework[debug]; extra == "test"
+Requires-Dist: collective.MockMailHost; extra == "test"
+Requires-Dist: responses; extra == "test"
 
 .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
    If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
    This text does not appear on pypi or github. It is a comment.
 
 .. image:: https://img.shields.io/pypi/v/plone.volto.svg
   :target: https://pypi.python.org/pypi/plone.volto
@@ -339,14 +351,30 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.4.0 (2024-04-25)
+------------------
+
+New features:
+
+
+- Import ILanguageSchema from plone.i18n.interfaces instead of Products.CMFPlone.interfaces.controlpanel. @ksuess
+  profile "plone.volto:multilingual": Add language german. @ksuess (#144)
+
+
+Bug fixes:
+
+
+- Avoid a deprecated import warnings in Plone 6. @davisagli (#147)
+
+
 4.3.0 (2024-01-30)
 ------------------
 
 New features:
 
 
 - Add `VOLTO_FRONTEND_DOMAIN` as env var for `volto.frontend_domain` registry setting
```

### Comparing `plone.volto-4.3.0/README.rst` & `plone_volto-4.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/docs/LICENSE.GPL` & `plone_volto-4.4.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/docs/LICENSE.rst` & `plone_volto-4.4.0/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/pyproject.toml` & `plone_volto-4.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/setup.py` & `plone_volto-4.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         readfile("CONTRIBUTORS.rst"),
         readfile("CHANGES.rst"),
     ]
 )
 
 setup(
     name="plone.volto",
-    version="4.3.0",
+    version="4.4.0",
     description="Volto integration add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `plone.volto-4.3.0/src/plone/volto/behaviors/configure.zcml` & `plone_volto-4.4.0/src/plone/volto/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/behaviors/headtitle.py` & `plone_volto-4.4.0/src/plone/volto/behaviors/headtitle.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/behaviors/preview.py` & `plone_volto-4.4.0/src/plone/volto/behaviors/preview.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/behaviors/preview_link.py` & `plone_volto-4.4.0/src/plone/volto/behaviors/preview_link.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/blocksuuidfixer.py` & `plone_volto-4.4.0/src/plone/volto/blocksuuidfixer.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/browser/breadcrumbs.py` & `plone_volto-4.4.0/src/plone/volto/browser/breadcrumbs.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,27 @@
 from Acquisition import aq_base
 from Acquisition import aq_inner
 from plone.app.layout.navigation.interfaces import INavigationRoot
 from plone.app.layout.navigation.root import getNavigationRoot
 from Products.CMFPlone import utils
 from Products.CMFPlone.browser.interfaces import INavigationBreadcrumbs
 from Products.CMFPlone.browser.navigation import get_view_url
-from Products.CMFPlone.defaultpage import check_default_page_via_view
-from Products.CMFPlone.interfaces import IHideFromBreadcrumbs
 from Products.Five import BrowserView
 from zope.component import getMultiAdapter
 from zope.interface import implementer
 
 
+try:
+    from plone.base.defaultpage import check_default_page_via_view
+    from plone.base.interfaces import IHideFromBreadcrumbs
+except ImportError:
+    from Products.CMFPlone.defaultpage import check_default_page_via_view
+    from Products.CMFPlone.interfaces import IHideFromBreadcrumbs
+
+
 @implementer(INavigationBreadcrumbs)
 class PhysicalNavigationBreadcrumbs(BrowserView):
     def breadcrumbs(self):
         context = aq_inner(self.context)
         request = self.request
         container = utils.parent(context)
```

### Comparing `plone.volto-4.3.0/src/plone/volto/browser/configure.zcml` & `plone_volto-4.4.0/src/plone/volto/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/browser/migrate_richtext.pt` & `plone_volto-4.4.0/src/plone/volto/browser/migrate_richtext.pt`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/browser/migrate_richtext.py` & `plone_volto-4.4.0/src/plone/volto/browser/migrate_richtext.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/browser/migrate_to_volto.pt` & `plone_volto-4.4.0/src/plone/volto/browser/migrate_to_volto.pt`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/browser/migrate_to_volto.py` & `plone_volto-4.4.0/src/plone/volto/browser/migrate_to_volto.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from plone.app.contenttypes.behaviors.collection import ICollection
 from plone.app.contenttypes.utils import get_old_class_name_string
 from plone.app.contenttypes.utils import get_portal_type_name_string
 from plone.app.linkintegrity.utils import referencedRelationship
 from plone.app.redirector.interfaces import IRedirectionStorage
 from plone.app.textfield.value import RichTextValue
 from plone.dexterity.interfaces import IDexterityFTI
+from plone.volto.bbb import get_installer
 from plone.volto.browser.migrate_richtext import get_blocks_from_richtext
 from plone.volto.browser.migrate_richtext import migrate_richtext_to_blocks
 from Products.BTreeFolder2.BTreeFolder2 import BTreeFolder2Base
 from Products.CMFCore.utils import getToolByName
 from Products.CMFPlone.relationhelper import restore_relations
-from Products.CMFPlone.utils import get_installer
 from Products.Five import BrowserView
 from uuid import uuid4
 from zope.component import getUtility
 from zope.lifecycleevent import modified
 
 
 try:
```

### Comparing `plone.volto-4.3.0/src/plone/volto/browser/navigation.py` & `plone_volto-4.4.0/src/plone/volto/browser/navigation.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,26 @@
 from plone.app.layout.navigation.root import getNavigationRoot
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.utils import getToolByName
 from Products.CMFPlone import utils
 from Products.CMFPlone.browser.interfaces import INavigationTabs
 from Products.CMFPlone.browser.navigation import get_id
 from Products.CMFPlone.browser.navigation import get_view_url
-from Products.CMFPlone.interfaces import INavigationSchema
 from Products.Five import BrowserView
 from zope.component import getMultiAdapter
 from zope.component import getUtility
 from zope.interface import implementer
 
 
+try:
+    from plone.base.interfaces import INavigationSchema
+except ImportError:
+    from Products.CMFPlone.interfaces import INavigationSchema
+
+
 @implementer(INavigationTabs)
 class CatalogNavigationTabs(BrowserView):
     def _getNavQuery(self):
         # check whether we only want actions
         registry = getUtility(IRegistry)
         navigation_settings = registry.forInterface(
             INavigationSchema, prefix="plone", check=False
```

### Comparing `plone.volto-4.3.0/src/plone/volto/browser/static/volto.svg` & `plone_volto-4.4.0/src/plone/volto/browser/static/volto.svg`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/browser/voltobackendwarning.pt` & `plone_volto-4.4.0/src/plone/volto/browser/voltobackendwarning.pt`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/configure.zcml` & `plone_volto-4.4.0/src/plone/volto/configure.zcml`

 * *Files 5% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 
   <include file="profiles.zcml" />
   <include file="patches.zcml" />
   <include file="upgrades.zcml" />
 
   <browser:page
       name="blocksuuidfixer"
-      for="Products.CMFPlone.interfaces.IPloneSiteRoot"
+      for=".bbb.IPloneSiteRoot"
       class=".blocksuuidfixer.DuplicatedBlocksUUIDFixer"
       permission="cmf.ManagePortal"
       />
 
   <browser:page
       name="volto_settings"
-      for="Products.CMFPlone.interfaces.IPloneSiteRoot"
+      for=".bbb.IPloneSiteRoot"
       class=".controlpanel.VoltoSettingsControlPanel"
       permission="cmf.ManagePortal"
       />
 
   <adapter
       factory=".controlpanel.VoltoControlpanel"
       name="volto-settings"
```

### Comparing `plone.volto-4.3.0/src/plone/volto/content.py` & `plone_volto-4.4.0/src/plone/volto/content.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/controlpanel.py` & `plone_volto-4.4.0/src/plone/volto/controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/coresandbox/configure.zcml` & `plone_volto-4.4.0/src/plone/volto/coresandbox/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/coresandbox/example.py` & `plone_volto-4.4.0/src/plone/volto/coresandbox/example.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/coresandbox/vocabularies.py` & `plone_volto-4.4.0/src/plone/volto/coresandbox/vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/default_homepage/default.py` & `plone_volto-4.4.0/src/plone/volto/default_homepage/default.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/default_homepage/demo.py` & `plone_volto-4.4.0/src/plone/volto/default_homepage/demo.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/default_homepage/lrf.py` & `plone_volto-4.4.0/src/plone/volto/default_homepage/lrf.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/dependencies.zcml` & `plone_volto-4.4.0/src/plone/volto/dependencies.zcml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/indexers.py` & `plone_volto-4.4.0/src/plone/volto/indexers.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/interfaces.py` & `plone_volto-4.4.0/src/plone/volto/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/linkintegrity.py` & `plone_volto-4.4.0/src/plone/volto/linkintegrity.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/locales/de/LC_MESSAGES/plone.volto.po` & `plone_volto-4.4.0/src/plone/volto/locales/de/LC_MESSAGES/plone.volto.po`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/locales/en/LC_MESSAGES/plone.volto.po` & `plone_volto-4.4.0/src/plone/volto/locales/en/LC_MESSAGES/plone.volto.po`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/locales/es/LC_MESSAGES/plone.volto.po` & `plone_volto-4.4.0/src/plone/volto/locales/es/LC_MESSAGES/plone.volto.po`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/locales/eu/LC_MESSAGES/plone.volto.po` & `plone_volto-4.4.0/src/plone/volto/locales/eu/LC_MESSAGES/plone.volto.po`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/locales/it/LC_MESSAGES/plone.volto.po` & `plone_volto-4.4.0/src/plone/volto/locales/it/LC_MESSAGES/plone.volto.po`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/locales/plone.volto.pot` & `plone_volto-4.4.0/src/plone/volto/locales/plone.volto.pot`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/locales/pt_BR/LC_MESSAGES/plone.volto.po` & `plone_volto-4.4.0/src/plone/volto/locales/pt_BR/LC_MESSAGES/plone.volto.po`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/patches.py` & `plone_volto-4.4.0/src/plone/volto/patches.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/patches.zcml` & `plone_volto-4.4.0/src/plone/volto/patches.zcml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/profiles/coresandbox/types/example.xml` & `plone_volto-4.4.0/src/plone/volto/profiles/coresandbox/types/example.xml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/profiles/default/actions.xml` & `plone_volto-4.4.0/src/plone/volto/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/profiles/default/controlpanel.xml` & `plone_volto-4.4.0/src/plone/volto/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/profiles/default/registry.xml` & `plone_volto-4.4.0/src/plone/volto/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/profiles/default/types/Document.xml` & `plone_volto-4.4.0/src/plone/volto/profiles/default/types/Document.xml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/profiles/default/types/LRF.xml` & `plone_volto-4.4.0/src/plone/volto/profiles/default/types/LRF.xml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/profiles.zcml` & `plone_volto-4.4.0/src/plone/volto/profiles.zcml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/scaling.py` & `plone_volto-4.4.0/src/plone/volto/scaling.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/scripts/add_image_field_metadata.py` & `plone_volto-4.4.0/src/plone/volto/scripts/add_image_field_metadata.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/scripts/auditblocks.py` & `plone_volto-4.4.0/src/plone/volto/scripts/auditblocks.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/scripts/listingaddsummary.py` & `plone_volto-4.4.0/src/plone/volto/scripts/listingaddsummary.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/scripts/migrate_richtext.py` & `plone_volto-4.4.0/src/plone/volto/scripts/migrate_richtext.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/scripts/searchscalesinimageblocks.py` & `plone_volto-4.4.0/src/plone/volto/scripts/searchscalesinimageblocks.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/scripts/utils.py` & `plone_volto-4.4.0/src/plone/volto/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/setuphandlers.py` & `plone_volto-4.4.0/src/plone/volto/setuphandlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 from importlib import import_module
 from plone import api
 from plone.dexterity.interfaces import IDexterityFTI
+from plone.volto.bbb import get_installer
 from plone.volto.default_homepage.default import default_home
 from plone.volto.default_homepage.demo import demo_home_page
 from plone.volto.default_homepage.lrf import default_lrf_home
 from Products.CMFCore.utils import getToolByName
 from Products.CMFPlone.interfaces import INonInstallable
-from Products.CMFPlone.utils import get_installer
 from zope.component import queryUtility
 from zope.interface import implementer
 
 import json
 import logging
 import pkg_resources
 import transaction
```

### Comparing `plone.volto-4.3.0/src/plone/volto/testing.py` & `plone_volto-4.4.0/src/plone/volto/testing.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/tests/test_coresandbox.py` & `plone_volto-4.4.0/src/plone/volto/tests/test_coresandbox.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/tests/test_indexers.py` & `plone_volto-4.4.0/src/plone/volto/tests/test_indexers.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/tests/test_linkintegrity.py` & `plone_volto-4.4.0/src/plone/volto/tests/test_linkintegrity.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/tests/test_migrate_to_volto.py` & `plone_volto-4.4.0/src/plone/volto/tests/test_migrate_to_volto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from Acquisition import aq_base
 from plone import api
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.app.textfield.value import RichTextValue
+from plone.volto.bbb import get_installer
 from plone.volto.content import FolderishDocument
 from plone.volto.content import FolderishEvent
 from plone.volto.content import FolderishNewsItem
 from plone.volto.testing import PLONE_6
 from plone.volto.testing import PLONE_VOLTO_MIGRATION_FUNCTIONAL_TESTING
-from Products.CMFPlone.utils import get_installer
 
 import json
 import responses
 import unittest
 
 
 @unittest.skipIf(
```

### Comparing `plone.volto-4.3.0/src/plone/volto/tests/test_preview_link_behavior.py` & `plone_volto-4.4.0/src/plone/volto/tests/test_preview_link_behavior.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/tests/test_scripts.py` & `plone_volto-4.4.0/src/plone/volto/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/tests/test_setup.py` & `plone_volto-4.4.0/src/plone/volto/tests/test_setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,33 @@
 # -*- coding: utf-8 -*-
 """Setup tests for this package."""
 from importlib import import_module
 from plone import api
+from plone.volto.bbb import get_installer
 from plone.volto.testing import PLONE_VOLTO_CORE_INTEGRATION_TESTING  # noqa
 
-
-try:
-    from Products.CMFPlone.utils import get_installer
-except ImportError:  # Plone < 5.1
-    HAS_INSTALLER = False
-else:
-    HAS_INSTALLER = True
-
 import unittest
 
 
 PLONE_6 = getattr(import_module("Products.CMFPlone.factory"), "PLONE60MARKER", False)
 
 
 class TestSetup(unittest.TestCase):
     """Test that plone.volto is properly installed."""
 
     layer = PLONE_VOLTO_CORE_INTEGRATION_TESTING
 
     def setUp(self):
         """Custom shared utility setup for tests."""
         self.portal = self.layer["portal"]
-        if HAS_INSTALLER:
-            self.installer = get_installer(self.portal)
-        else:
-            self.installer = api.portal.get_tool("portal_quickinstaller")
+        self.installer = get_installer(self.portal)
 
     def test_product_installed(self):
         """Test if plone.volto is installed."""
-        if HAS_INSTALLER:
-            self.assertTrue(self.installer.is_product_installed("plone.volto"))
-        else:
-            self.assertTrue(self.installer.isProductInstalled("plone.volto"))
+        self.assertTrue(self.installer.is_product_installed("plone.volto"))
 
     def test_browserlayer(self):
         """Test that IPloneVoltoCoreLayer is registered."""
         from plone.browserlayer import utils
         from plone.volto.interfaces import IPloneVoltoCoreLayer
 
         self.assertIn(IPloneVoltoCoreLayer, utils.registered_layers())
@@ -66,27 +53,20 @@
 
 class TestUninstall(unittest.TestCase):
 
     layer = PLONE_VOLTO_CORE_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
-        if HAS_INSTALLER:
-            self.installer = get_installer(self.portal)
-            self.installer.uninstall_product("plone.volto")
-        else:
-            self.installer = api.portal.get_tool("portal_quickinstaller")
-            self.installer.uninstallProducts(["plone.volto"])
+        self.installer = get_installer(self.portal)
+        self.installer.uninstall_product("plone.volto")
 
     def test_product_uninstalled(self):
         """Test if plone.volto is cleanly uninstalled."""
-        if HAS_INSTALLER:
-            self.assertFalse(self.installer.is_product_installed("plone.volto"))
-        else:
-            self.assertFalse(self.installer.isProductInstalled("plone.volto"))
+        self.assertFalse(self.installer.is_product_installed("plone.volto"))
 
     def test_browserlayer_removed(self):
         """Test that IPloneVoltoCoreLayer is removed."""
         from plone.browserlayer import utils
         from plone.volto.interfaces import IPloneVoltoCoreLayer
 
         self.assertNotIn(IPloneVoltoCoreLayer, utils.registered_layers())
```

### Comparing `plone.volto-4.3.0/src/plone/volto/tests/test_summary_serialization.py` & `plone_volto-4.4.0/src/plone/volto/tests/test_summary_serialization.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/tests/test_transforms.py` & `plone_volto-4.4.0/src/plone/volto/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/tests/test_upgrades.py` & `plone_volto-4.4.0/src/plone/volto/tests/test_upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/transforms.py` & `plone_volto-4.4.0/src/plone/volto/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from plone.restapi.behaviors import IBlocks
 from plone.restapi.deserializer.blocks import ResolveUIDDeserializerBase
 from plone.restapi.interfaces import IBlockFieldDeserializationTransformer
 from plone.restapi.interfaces import IBlockFieldSerializationTransformer
 from plone.restapi.interfaces import IBlockVisitor
 from plone.restapi.serializer.blocks import ResolveUIDSerializerBase
-from Products.CMFPlone.interfaces import IPloneSiteRoot
+from plone.volto.bbb import IPloneSiteRoot
 from zope.component import adapter
 from zope.component import subscribers
 from zope.interface import implementer
 from zope.interface import Interface
 from zope.publisher.interfaces.browser import IBrowserRequest
```

### Comparing `plone.volto-4.3.0/src/plone/volto/upgrades.py` & `plone_volto-4.4.0/src/plone/volto/upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/upgrades.zcml` & `plone_volto-4.4.0/src/plone/volto/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone/volto/vocabularies/subject.py` & `plone_volto-4.4.0/src/plone/volto/vocabularies/subject.py`

 * *Files identical despite different names*

### Comparing `plone.volto-4.3.0/src/plone.volto.egg-info/PKG-INFO` & `plone_volto-4.4.0/src/plone.volto.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.volto
-Version: 4.3.0
+Version: 4.4.0
 Summary: Volto integration add-on for Plone
 Home-page: https://github.com/plone/plone.volto
 Author: Plone Foundation
 Author-email: tisto@plone.org
 License: GPL version 2
 Keywords: Python Plone CMS
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,27 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.7
+Requires-Dist: plone.api
+Requires-Dist: Products.GenericSetup
+Requires-Dist: setuptools
+Requires-Dist: plone.restapi>=8.41.0
+Requires-Dist: plone.app.vocabularies>=4.3.0
+Requires-Dist: collective.monkeypatcher
 Provides-Extra: test
+Requires-Dist: plone.app.testing; extra == "test"
+Requires-Dist: plone.testing; extra == "test"
+Requires-Dist: plone.app.contenttypes; extra == "test"
+Requires-Dist: plone.app.robotframework[debug]; extra == "test"
+Requires-Dist: collective.MockMailHost; extra == "test"
+Requires-Dist: responses; extra == "test"
 
 .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
    If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
    This text does not appear on pypi or github. It is a comment.
 
 .. image:: https://img.shields.io/pypi/v/plone.volto.svg
   :target: https://pypi.python.org/pypi/plone.volto
@@ -339,14 +351,30 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.4.0 (2024-04-25)
+------------------
+
+New features:
+
+
+- Import ILanguageSchema from plone.i18n.interfaces instead of Products.CMFPlone.interfaces.controlpanel. @ksuess
+  profile "plone.volto:multilingual": Add language german. @ksuess (#144)
+
+
+Bug fixes:
+
+
+- Avoid a deprecated import warnings in Plone 6. @davisagli (#147)
+
+
 4.3.0 (2024-01-30)
 ------------------
 
 New features:
 
 
 - Add `VOLTO_FRONTEND_DOMAIN` as env var for `volto.frontend_domain` registry setting
```

### Comparing `plone.volto-4.3.0/src/plone.volto.egg-info/SOURCES.txt` & `plone_volto-4.4.0/src/plone.volto.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 src/plone.volto.egg-info/dependency_links.txt
 src/plone.volto.egg-info/entry_points.txt
 src/plone.volto.egg-info/namespace_packages.txt
 src/plone.volto.egg-info/not-zip-safe
 src/plone.volto.egg-info/requires.txt
 src/plone.volto.egg-info/top_level.txt
 src/plone/volto/__init__.py
+src/plone/volto/bbb.py
 src/plone/volto/blocksuuidfixer.py
 src/plone/volto/configure.zcml
 src/plone/volto/content.py
 src/plone/volto/controlpanel.py
 src/plone/volto/dependencies.zcml
 src/plone/volto/indexers.py
 src/plone/volto/interfaces.py
@@ -60,19 +61,25 @@
 src/plone/volto/cors/configure.zcml
 src/plone/volto/default_homepage/__init__.py
 src/plone/volto/default_homepage/default.py
 src/plone/volto/default_homepage/demo.py
 src/plone/volto/default_homepage/lrf.py
 src/plone/volto/locales/plone.volto.pot
 src/plone/volto/locales/update.sh
+src/plone/volto/locales/de/LC_MESSAGES/plone.volto.mo
 src/plone/volto/locales/de/LC_MESSAGES/plone.volto.po
+src/plone/volto/locales/en/LC_MESSAGES/plone.volto.mo
 src/plone/volto/locales/en/LC_MESSAGES/plone.volto.po
+src/plone/volto/locales/es/LC_MESSAGES/plone.volto.mo
 src/plone/volto/locales/es/LC_MESSAGES/plone.volto.po
+src/plone/volto/locales/eu/LC_MESSAGES/plone.volto.mo
 src/plone/volto/locales/eu/LC_MESSAGES/plone.volto.po
+src/plone/volto/locales/it/LC_MESSAGES/plone.volto.mo
 src/plone/volto/locales/it/LC_MESSAGES/plone.volto.po
+src/plone/volto/locales/pt_BR/LC_MESSAGES/plone.volto.mo
 src/plone/volto/locales/pt_BR/LC_MESSAGES/plone.volto.po
 src/plone/volto/profiles/coresandbox/diff_tool.xml
 src/plone/volto/profiles/coresandbox/metadata.xml
 src/plone/volto/profiles/coresandbox/repositorytool.xml
 src/plone/volto/profiles/coresandbox/types.xml
 src/plone/volto/profiles/coresandbox/types/example.xml
 src/plone/volto/profiles/default/actions.xml
```


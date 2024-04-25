# Comparing `tmp/plone.app.upgrade-3.1.3.tar.gz` & `tmp/plone_app_upgrade-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.upgrade-3.1.3.tar", last modified: Thu Feb 22 22:16:31 2024, max compression
+gzip compressed data, was "plone_app_upgrade-3.1.4.tar", last modified: Thu Apr 25 19:47:43 2024, max compression
```

## Comparing `plone.app.upgrade-3.1.3.tar` & `plone_app_upgrade-3.1.4.tar`

### file list

```diff
@@ -1,122 +1,125 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.917987 plone.app.upgrade-3.1.3/
--rw-r--r--   0 maurits    (501) staff       (20)    11702 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      148 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    13632 2024-02-22 22:16:31.917610 plone.app.upgrade-3.1.3/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      351 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.880561 plone.app.upgrade-3.1.3/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      679 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.881014 plone.app.upgrade-3.1.3/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.885190 plone.app.upgrade-3.1.3/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.886511 plone.app.upgrade-3.1.3/plone/app/upgrade/
--rw-r--r--   0 maurits    (501) staff       (20)      767 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.887913 plone.app.upgrade-3.1.3/plone/app/upgrade/bbb_qi/
--rw-r--r--   0 maurits    (501) staff       (20)      266 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/bbb_qi/InstalledProduct.py
--rw-r--r--   0 maurits    (501) staff       (20)      784 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/bbb_qi/QuickInstallerTool.py
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/bbb_qi/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.889175 plone.app.upgrade-3.1.3/plone/app/upgrade/bbb_qi/interfaces/
--rw-r--r--   0 maurits    (501) staff       (20)      158 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/bbb_qi/interfaces/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      215 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/bbb_qi/interfaces/installable.py
--rw-r--r--   0 maurits    (501) staff       (20)      133 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/bbb_qi/interfaces/portal_quickinstaller.py
--rw-r--r--   0 maurits    (501) staff       (20)      510 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.891348 plone.app.upgrade-3.1.3/plone/app/upgrade/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     5732 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/tests/base.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.891808 plone.app.upgrade-3.1.3/plone/app/upgrade/tests/skin_test/
--rw-r--r--   0 maurits    (501) staff       (20)       15 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/tests/skin_test/README.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.892278 plone.app.upgrade-3.1.3/plone/app/upgrade/tests/skin_test/sub1/
--rw-r--r--   0 maurits    (501) staff       (20)       21 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/tests/skin_test/sub1/README.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.892728 plone.app.upgrade-3.1.3/plone/app/upgrade/tests/skin_test/sub1/subsub1/
--rw-r--r--   0 maurits    (501) staff       (20)       25 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/tests/skin_test/sub1/subsub1/README.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.893185 plone.app.upgrade-3.1.3/plone/app/upgrade/tests/skin_test/sub2/
--rw-r--r--   0 maurits    (501) staff       (20)       21 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/tests/skin_test/sub2/README.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2184 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/tests/test_fix_registry_settings.py
--rw-r--r--   0 maurits    (501) staff       (20)     2845 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/tests/test_upgrade.py
--rw-r--r--   0 maurits    (501) staff       (20)     3624 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)    15675 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.896392 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3740 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/alphas.py
--rw-r--r--   0 maurits    (501) staff       (20)     5567 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/betas.py
--rw-r--r--   0 maurits    (501) staff       (20)     6810 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    11549 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/final.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.873387 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.896947 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_521/
--rw-r--r--   0 maurits    (501) staff       (20)      268 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_521/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.872234 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_522/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.897882 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_522/registry/
--rw-r--r--   0 maurits    (501) staff       (20)      348 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_522/registry/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      397 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_522/registry/image_captioning.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.899262 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_alpha1/
--rw-r--r--   0 maurits    (501) staff       (20)     1639 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_alpha1/componentregistry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1337 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_alpha1/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)      554 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_alpha1/skins.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.902107 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_beta1/
--rw-r--r--   0 maurits    (501) staff       (20)     1000 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_beta1/actions.xml
--rw-r--r--   0 maurits    (501) staff       (20)      533 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_beta1/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2404 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_beta1/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1054 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_beta1/repositorytool.xml
--rw-r--r--   0 maurits    (501) staff       (20)      428 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_beta1/rolemap.xml
--rw-r--r--   0 maurits    (501) staff       (20)      187 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_beta1/toolset.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.873137 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_rc1/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.902605 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_rc1/registry/
--rw-r--r--   0 maurits    (501) staff       (20)      329 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_rc1/registry/resources.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.873575 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_rc4/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.903579 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_rc4/registry/
--rw-r--r--   0 maurits    (501) staff       (20)      145 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_rc4/registry/security.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1113 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_rc4/registry/staticresources.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1878 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    11140 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v52/tests.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.907003 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    17085 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/alphas.py
--rw-r--r--   0 maurits    (501) staff       (20)     4269 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/betas.py
--rw-r--r--   0 maurits    (501) staff       (20)     8866 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     9306 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/final.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.875937 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.908839 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6000/
--rw-r--r--   0 maurits    (501) staff       (20)      387 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6000/actions.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2067 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6000/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      611 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6000/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)      146 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6000/toolset.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.909741 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6003/
--rw-r--r--   0 maurits    (501) staff       (20)      507 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6003/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      140 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6003/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.911559 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6004/
--rw-r--r--   0 maurits    (501) staff       (20)      435 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6004/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2553 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6004/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)      291 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6004/skins.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.912021 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6004/types/
--rw-r--r--   0 maurits    (501) staff       (20)      267 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6004/types/Event.xml
--rw-r--r--   0 maurits    (501) staff       (20)      162 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6004/viewlets.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.912936 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6005/
--rw-r--r--   0 maurits    (501) staff       (20)      575 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6005/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)      195 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6005/skins.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.913412 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6007/
--rw-r--r--   0 maurits    (501) staff       (20)     4558 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6007/actions.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.913914 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6012/
--rw-r--r--   0 maurits    (501) staff       (20)      234 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6012/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.914406 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to_dx_site_root/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.914889 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to_dx_site_root/types/
--rw-r--r--   0 maurits    (501) staff       (20)     2782 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to_dx_site_root/types/Plone_Site.xml
--rw-r--r--   0 maurits    (501) staff       (20)      146 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to_dx_site_root/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2248 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     6695 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v60/tests.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.915701 plone.app.upgrade-3.1.3/plone/app/upgrade/v61/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v61/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      686 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/plone/app/upgrade/v61/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-02-22 22:16:31.916282 plone.app.upgrade-3.1.3/plone.app.upgrade.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    13632 2024-02-22 22:16:31.000000 plone.app.upgrade-3.1.3/plone.app.upgrade.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     3574 2024-02-22 22:16:31.000000 plone.app.upgrade-3.1.3/plone.app.upgrade.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-02-22 22:16:31.000000 plone.app.upgrade-3.1.3/plone.app.upgrade.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2024-02-22 22:16:31.000000 plone.app.upgrade-3.1.3/plone.app.upgrade.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2024-02-22 22:16:31.000000 plone.app.upgrade-3.1.3/plone.app.upgrade.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-02-22 22:16:31.000000 plone.app.upgrade-3.1.3/plone.app.upgrade.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      318 2024-02-22 22:16:31.000000 plone.app.upgrade-3.1.3/plone.app.upgrade.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-02-22 22:16:31.000000 plone.app.upgrade-3.1.3/plone.app.upgrade.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      658 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      116 2024-02-22 22:16:31.918638 plone.app.upgrade-3.1.3/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1967 2024-02-22 22:16:30.000000 plone.app.upgrade-3.1.3/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.044010 plone_app_upgrade-3.1.4/
+-rw-r--r--   0 maurits    (501) staff       (20)    12143 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      148 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    14073 2024-04-25 19:47:43.043825 plone_app_upgrade-3.1.4/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      351 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.016543 plone_app_upgrade-3.1.4/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      679 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.016988 plone_app_upgrade-3.1.4/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.019813 plone_app_upgrade-3.1.4/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.021018 plone_app_upgrade-3.1.4/plone/app/upgrade/
+-rw-r--r--   0 maurits    (501) staff       (20)      767 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.022185 plone_app_upgrade-3.1.4/plone/app/upgrade/bbb_qi/
+-rw-r--r--   0 maurits    (501) staff       (20)      266 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/bbb_qi/InstalledProduct.py
+-rw-r--r--   0 maurits    (501) staff       (20)      784 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/bbb_qi/QuickInstallerTool.py
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/bbb_qi/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.023247 plone_app_upgrade-3.1.4/plone/app/upgrade/bbb_qi/interfaces/
+-rw-r--r--   0 maurits    (501) staff       (20)      158 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/bbb_qi/interfaces/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      215 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/bbb_qi/interfaces/installable.py
+-rw-r--r--   0 maurits    (501) staff       (20)      133 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/bbb_qi/interfaces/portal_quickinstaller.py
+-rw-r--r--   0 maurits    (501) staff       (20)      510 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.024716 plone_app_upgrade-3.1.4/plone/app/upgrade/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5732 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/tests/base.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.024986 plone_app_upgrade-3.1.4/plone/app/upgrade/tests/skin_test/
+-rw-r--r--   0 maurits    (501) staff       (20)       15 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/tests/skin_test/README.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.025365 plone_app_upgrade-3.1.4/plone/app/upgrade/tests/skin_test/sub1/
+-rw-r--r--   0 maurits    (501) staff       (20)       21 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/tests/skin_test/sub1/README.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.025643 plone_app_upgrade-3.1.4/plone/app/upgrade/tests/skin_test/sub1/subsub1/
+-rw-r--r--   0 maurits    (501) staff       (20)       25 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/tests/skin_test/sub1/subsub1/README.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.026026 plone_app_upgrade-3.1.4/plone/app/upgrade/tests/skin_test/sub2/
+-rw-r--r--   0 maurits    (501) staff       (20)       21 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/tests/skin_test/sub2/README.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2184 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/tests/test_fix_registry_settings.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2845 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/tests/test_upgrade.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3624 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)    15675 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.028072 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3740 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/alphas.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5567 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/betas.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6810 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    11549 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/final.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.011516 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.028368 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_521/
+-rw-r--r--   0 maurits    (501) staff       (20)      268 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_521/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.010695 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_522/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.029009 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_522/registry/
+-rw-r--r--   0 maurits    (501) staff       (20)      348 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_522/registry/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      397 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_522/registry/image_captioning.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.030087 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_alpha1/
+-rw-r--r--   0 maurits    (501) staff       (20)     1639 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_alpha1/componentregistry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1337 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_alpha1/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      554 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_alpha1/skins.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.032436 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_beta1/
+-rw-r--r--   0 maurits    (501) staff       (20)     1000 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_beta1/actions.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      533 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_beta1/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2404 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_beta1/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1054 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_beta1/repositorytool.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      428 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_beta1/rolemap.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      187 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_beta1/toolset.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.011356 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_rc1/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.032769 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_rc1/registry/
+-rw-r--r--   0 maurits    (501) staff       (20)      329 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_rc1/registry/resources.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.011629 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_rc4/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.033364 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_rc4/registry/
+-rw-r--r--   0 maurits    (501) staff       (20)      145 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_rc4/registry/security.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1113 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_rc4/registry/staticresources.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1878 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    11140 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v52/tests.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.035749 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17085 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/alphas.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4269 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/betas.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9445 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     9306 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/final.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.013549 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.037076 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6000/
+-rw-r--r--   0 maurits    (501) staff       (20)      387 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6000/actions.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2067 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6000/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      611 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6000/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      146 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6000/toolset.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.037631 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6003/
+-rw-r--r--   0 maurits    (501) staff       (20)      507 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6003/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      140 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6003/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.038828 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6004/
+-rw-r--r--   0 maurits    (501) staff       (20)      435 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6004/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2553 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6004/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      291 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6004/skins.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.039113 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6004/types/
+-rw-r--r--   0 maurits    (501) staff       (20)      267 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6004/types/Event.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      162 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6004/viewlets.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.040076 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6005/
+-rw-r--r--   0 maurits    (501) staff       (20)      575 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6005/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      195 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6005/skins.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.040349 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6007/
+-rw-r--r--   0 maurits    (501) staff       (20)     4558 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6007/actions.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.040654 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6012/
+-rw-r--r--   0 maurits    (501) staff       (20)      234 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6012/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.040982 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to_dx_site_root/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.041409 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to_dx_site_root/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     2782 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to_dx_site_root/types/Plone_Site.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      146 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to_dx_site_root/types.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.041692 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to_isiteschema/
+-rw-r--r--   0 maurits    (501) staff       (20)      140 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to_isiteschema/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2625 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     6695 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v60/tests.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.042771 plone_app_upgrade-3.1.4/plone/app/upgrade/v61/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v61/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1892 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v61/alpha.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1236 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone/app/upgrade/v61/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-25 19:47:43.043130 plone_app_upgrade-3.1.4/plone.app.upgrade.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    14073 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone.app.upgrade.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     3664 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone.app.upgrade.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone.app.upgrade.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone.app.upgrade.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone.app.upgrade.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone.app.upgrade.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      318 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone.app.upgrade.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/plone.app.upgrade.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      658 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      116 2024-04-25 19:47:43.044417 plone_app_upgrade-3.1.4/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1967 2024-04-25 19:47:42.000000 plone_app_upgrade-3.1.4/setup.py
```

### Comparing `plone.app.upgrade-3.1.3/CHANGES.rst` & `plone_app_upgrade-3.1.4/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,37 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.1.4 (2024-04-25)
+------------------
+
+Bug fixes:
+
+
+- Add upgrade step for enable TinyMCE Plugin accordion to v60
+  [1letter] (324-1)
+- Add upgrade step for enable TinyMCE Plugin accordion
+  [1letter] (#324)
+- Add upgrade to add registry record ``webstats_head_js`` to ``ISiteSchema``.
+  [maurits] (#3931)
+
+
+Internal:
+
+
+- Added upgrade to 6022, Plone 6.0.11.
+  [maurits] (#6022)
+- Added upgrade to 6102, Plone 6.1.0a3.
+  [maurits] (#6102)
+
+
 3.1.3 (2024-02-22)
 ------------------
 
 Bug fixes:
 
 
 - Update TinyMCE format icon names.
```

### Comparing `plone.app.upgrade-3.1.3/PKG-INFO` & `plone_app_upgrade-3.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.upgrade
-Version: 3.1.3
+Version: 3.1.4
 Summary: Upgrade machinery for Plone.
 Home-page: https://pypi.org/project/plone.app.upgrade/
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: Plone upgrade migration
 Classifier: Development Status :: 6 - Mature
@@ -61,14 +61,37 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.1.4 (2024-04-25)
+------------------
+
+Bug fixes:
+
+
+- Add upgrade step for enable TinyMCE Plugin accordion to v60
+  [1letter] (324-1)
+- Add upgrade step for enable TinyMCE Plugin accordion
+  [1letter] (#324)
+- Add upgrade to add registry record ``webstats_head_js`` to ``ISiteSchema``.
+  [maurits] (#3931)
+
+
+Internal:
+
+
+- Added upgrade to 6022, Plone 6.0.11.
+  [maurits] (#6022)
+- Added upgrade to 6102, Plone 6.1.0a3.
+  [maurits] (#6102)
+
+
 3.1.3 (2024-02-22)
 ------------------
 
 Bug fixes:
 
 
 - Update TinyMCE format icon names.
```

### Comparing `plone.app.upgrade-3.1.3/docs/LICENSE.GPL` & `plone_app_upgrade-3.1.4/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/docs/LICENSE.txt` & `plone_app_upgrade-3.1.4/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/__init__.py` & `plone_app_upgrade-3.1.4/plone/app/upgrade/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/bbb_qi/QuickInstallerTool.py` & `plone_app_upgrade-3.1.4/plone/app/upgrade/bbb_qi/QuickInstallerTool.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/tests/base.py` & `plone_app_upgrade-3.1.4/plone/app/upgrade/tests/base.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/tests/test_fix_registry_settings.py` & `plone_app_upgrade-3.1.4/plone/app/upgrade/tests/test_fix_registry_settings.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/tests/test_upgrade.py` & `plone_app_upgrade-3.1.4/plone/app/upgrade/tests/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/tests/test_utils.py` & `plone_app_upgrade-3.1.4/plone/app/upgrade/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/utils.py` & `plone_app_upgrade-3.1.4/plone/app/upgrade/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from Acquisition import aq_base
 from Missing import MV
+from plone.base.utils import base_hasattr
 from plone.base.utils import get_installer
 from plone.indexer.interfaces import IIndexableObject
 from Products.CMFCore.DirectoryView import _dirreg
 from Products.CMFCore.utils import getToolByName
-from plone.base.utils import base_hasattr
 from Products.GenericSetup.interfaces import ISetupTool
 from Products.GenericSetup.registry import _export_step_registry
 from Products.GenericSetup.registry import _import_step_registry
 from Products.PluginIndexes.util import safe_callable
 from Products.ZCatalog.ProgressHandler import ZLogHandler
 from types import ModuleType
 from ZODB.POSException import ConflictError
```

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v52/alphas.py` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v52/alphas.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v52/betas.py` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v52/betas.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v52/configure.zcml` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v52/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v52/final.py` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v52/final.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from AccessControl.Permissions import view
 from plone.app.upgrade.utils import loadMigrationProfile
+from plone.base.utils import base_hasattr
 from plone.base.utils import get_installer
 from plone.registry import field
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.utils import getToolByName
 from Products.CMFPlone.interfaces import IMarkupSchema
 from Products.CMFPlone.interfaces import ISiteSchema
-from plone.base.utils import base_hasattr
 from Products.CMFPlone.utils import safe_unicode
 from zope.component import getUtility
 
 import logging
 
 
 logger = logging.getLogger("plone.app.upgrade")
```

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_alpha1/componentregistry.xml` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_alpha1/componentregistry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_alpha1/registry.xml` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_alpha1/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_alpha1/skins.xml` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_alpha1/skins.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_beta1/actions.xml` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_beta1/actions.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_beta1/controlpanel.xml` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_beta1/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_beta1/registry.xml` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_beta1/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_beta1/repositorytool.xml` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_beta1/repositorytool.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles/to_rc4/registry/staticresources.xml` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles/to_rc4/registry/staticresources.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v52/profiles.zcml` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v52/profiles.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v52/tests.py` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v52/tests.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v60/alphas.py` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v60/alphas.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v60/betas.py` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v60/betas.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v60/configure.zcml` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v60/configure.zcml`

 * *Files 2% similar despite different names*

```diff
@@ -360,8 +360,29 @@
         <gs:upgradeStep
             title="Fix TinyMCE format icon names"
             handler=".final.fix_tinymce_format_iconnames"
             />
 
     </gs:upgradeSteps>
 
+    <gs:upgradeSteps
+        profile="Products.CMFPlone:plone"
+        source="6021"
+        destination="6022"
+        >
+        <!-- Plone 6.0.11 -->
+
+        <gs:upgradeDepends
+          title="Run to_isiteschema upgrade profile."
+          import_profile="plone.app.upgrade.v60:to_isiteschema"
+          />
+
+        
+        <gs:upgradeStep
+          title="Add Feature to TinyMCE Editor"
+          description="add accordion plugin to tinymce editor"
+          handler="plone.app.upgrade.v61.alpha.add_feature_tinymce_accordion_plugin"
+          />
+
+    </gs:upgradeSteps>
+
 </configure>
```

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v60/final.py` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v60/final.py`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6000/controlpanel.xml` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6000/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6000/registry.xml` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6000/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6004/registry.xml` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6004/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6005/registry.xml` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6005/registry.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to6007/actions.xml` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to6007/actions.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles/to_dx_site_root/types/Plone_Site.xml` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles/to_dx_site_root/types/Plone_Site.xml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v60/profiles.zcml` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v60/profiles.zcml`

 * *Files 7% similar despite different names*

```diff
@@ -58,8 +58,17 @@
       name="to_dx_site_root"
       title="Upgrade profile to change the FTI for the Plone Site object a dexterity one"
       directory="profiles/to_dx_site_root"
       for="plone.base.interfaces.IMigratingPloneSiteRoot"
       provides="Products.GenericSetup.interfaces.EXTENSION"
       />
 
+  <!-- to_isiteschema needs to be applied in Plone 6.0.11 and 6.1.0a3. -->
+  <genericsetup:registerProfile
+      name="to_isiteschema"
+      title="Reregister ISiteSchema to get new webstats_head_js record"
+      directory="profiles/to_isiteschema"
+      for="plone.base.interfaces.IMigratingPloneSiteRoot"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      />
+
 </configure>
```

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v60/tests.py` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v60/tests.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from plone.app.testing import PLONE_INTEGRATION_TESTING
+from plone.dexterity.interfaces import IDexterityFTI
 from plone.registry.interfaces import IRegistry
 from Products.CMFCore.utils import getToolByName
 from zope.component import getUtility
-from plone.dexterity.interfaces import IDexterityFTI
 
 import unittest
 
 
 class Various60Test(unittest.TestCase):
     layer = PLONE_INTEGRATION_TESTING
```

### Comparing `plone.app.upgrade-3.1.3/plone/app/upgrade/v61/configure.zcml` & `plone_app_upgrade-3.1.4/plone/app/upgrade/v61/configure.zcml`

 * *Files 19% similar despite different names*

```diff
@@ -17,15 +17,33 @@
   </gs:upgradeSteps>
 
   <gs:upgradeSteps
       profile="Products.CMFPlone:plone"
       source="6100"
       destination="6101"
       >
-    <!-- Plone 6.1.0a1 -->
+    <!-- Plone 6.1.0a2 -->
     <gs:upgradeStep
         title="Miscellaneous"
         handler="..utils.null_upgrade_step"
         />
   </gs:upgradeSteps>
 
+  <gs:upgradeSteps
+      profile="Products.CMFPlone:plone"
+      source="6101"
+      destination="6102"
+      >
+    <!-- Plone 6.1.0a3 -->
+    <gs:upgradeStep
+        title="Add Feature to TinyMCE Editor"
+        description="add accordion plugin to tinymce editor"
+        handler=".alpha.add_feature_tinymce_accordion_plugin"
+        />
+    <!-- We reuse an upgrade step from v60 -->
+    <gs:upgradeDepends
+      title="Run to_isiteschema upgrade profile."
+      import_profile="plone.app.upgrade.v60:to_isiteschema"
+      />
+  </gs:upgradeSteps>
+
 </configure>
```

### Comparing `plone.app.upgrade-3.1.3/plone.app.upgrade.egg-info/PKG-INFO` & `plone_app_upgrade-3.1.4/plone.app.upgrade.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.upgrade
-Version: 3.1.3
+Version: 3.1.4
 Summary: Upgrade machinery for Plone.
 Home-page: https://pypi.org/project/plone.app.upgrade/
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: Plone upgrade migration
 Classifier: Development Status :: 6 - Mature
@@ -61,14 +61,37 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.1.4 (2024-04-25)
+------------------
+
+Bug fixes:
+
+
+- Add upgrade step for enable TinyMCE Plugin accordion to v60
+  [1letter] (324-1)
+- Add upgrade step for enable TinyMCE Plugin accordion
+  [1letter] (#324)
+- Add upgrade to add registry record ``webstats_head_js`` to ``ISiteSchema``.
+  [maurits] (#3931)
+
+
+Internal:
+
+
+- Added upgrade to 6022, Plone 6.0.11.
+  [maurits] (#6022)
+- Added upgrade to 6102, Plone 6.1.0a3.
+  [maurits] (#6102)
+
+
 3.1.3 (2024-02-22)
 ------------------
 
 Bug fixes:
 
 
 - Update TinyMCE format icon names.
```

### Comparing `plone.app.upgrade-3.1.3/plone.app.upgrade.egg-info/SOURCES.txt` & `plone_app_upgrade-3.1.4/plone.app.upgrade.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -77,9 +77,11 @@
 plone/app/upgrade/v60/profiles/to6004/types/Event.xml
 plone/app/upgrade/v60/profiles/to6005/registry.xml
 plone/app/upgrade/v60/profiles/to6005/skins.xml
 plone/app/upgrade/v60/profiles/to6007/actions.xml
 plone/app/upgrade/v60/profiles/to6012/registry.xml
 plone/app/upgrade/v60/profiles/to_dx_site_root/types.xml
 plone/app/upgrade/v60/profiles/to_dx_site_root/types/Plone_Site.xml
+plone/app/upgrade/v60/profiles/to_isiteschema/registry.xml
 plone/app/upgrade/v61/__init__.py
+plone/app/upgrade/v61/alpha.py
 plone/app/upgrade/v61/configure.zcml
```

### Comparing `plone.app.upgrade-3.1.3/pyproject.toml` & `plone_app_upgrade-3.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.upgrade-3.1.3/setup.py` & `plone_app_upgrade-3.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.1.3"
+version = "3.1.4"
 
 setup(
     name="plone.app.upgrade",
     version=version,
     description="Upgrade machinery for Plone.",
     long_description=(open("README.rst").read() + "\n" + open("CHANGES.rst").read()),
     classifiers=[
```


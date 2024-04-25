# Comparing `tmp/imio.schedule-2.2.1.tar.gz` & `tmp/imio.schedule-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imio.schedule-2.2.1.tar", last modified: Wed Apr 10 10:54:25 2024, max compression
+gzip compressed data, was "dist/imio.schedule-2.2.2.tar", last modified: Thu Apr 25 16:23:22 2024, max compression
```

## Comparing `imio.schedule-2.2.1.tar` & `imio.schedule-2.2.2.tar`

### file list

```diff
@@ -1,168 +1,170 @@
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/
--rw-r--r--   0 mpeeters   (501) staff       (20)     2019 2024-04-10 10:54:23.000000 imio.schedule-2.2.1/CHANGES.rst
--rw-r--r--   0 mpeeters   (501) staff       (20)       41 2024-04-10 10:54:23.000000 imio.schedule-2.2.1/CONTRIBUTORS.rst
--rw-r--r--   0 mpeeters   (501) staff       (20)       91 2024-04-10 10:54:23.000000 imio.schedule-2.2.1/MANIFEST.in
--rw-r--r--   0 mpeeters   (501) staff       (20)      703 2024-04-10 10:54:23.000000 imio.schedule-2.2.1/Makefile
--rw-r--r--   0 mpeeters   (501) staff       (20)     4274 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/PKG-INFO
--rw-r--r--   0 mpeeters   (501) staff       (20)     1543 2024-04-10 10:54:23.000000 imio.schedule-2.2.1/README.rst
--rw-r--r--   0 mpeeters   (501) staff       (20)     7458 2024-04-10 10:54:23.000000 imio.schedule-2.2.1/bootstrap.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/docs/
--rw-r--r--   0 mpeeters   (501) staff       (20)    18092 2024-04-10 10:54:23.000000 imio.schedule-2.2.1/docs/LICENSE.GPL
--rw-r--r--   0 mpeeters   (501) staff       (20)      658 2024-04-10 10:54:23.000000 imio.schedule-2.2.1/docs/LICENSE.rst
--rw-r--r--   0 mpeeters   (501) staff       (20)       76 2024-04-10 10:54:23.000000 imio.schedule-2.2.1/docs/index.rst
--rw-r--r--   0 mpeeters   (501) staff       (20)      140 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/setup.cfg
--rw-r--r--   0 mpeeters   (501) staff       (20)     1858 2024-04-10 10:54:23.000000 imio.schedule-2.2.1/setup.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio/
--rw-r--r--   0 mpeeters   (501) staff       (20)       80 2024-04-10 10:54:23.000000 imio.schedule-2.2.1/src/imio/__init__.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio/schedule/
--rw-r--r--   0 mpeeters   (501) staff       (20)      130 2024-04-10 10:54:23.000000 imio.schedule-2.2.1/src/imio/schedule/__init__.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio/schedule/browser/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:23.000000 imio.schedule-2.2.1/src/imio/schedule/browser/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1071 2024-04-10 10:54:23.000000 imio.schedule-2.2.1/src/imio/schedule/browser/close_task.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1806 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/browser/configure.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio/schedule/browser/overrides/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/browser/overrides/.gitkeep
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio/schedule/browser/static/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/browser/static/.gitkeep
--rw-r--r--   0 mpeeters   (501) staff       (20)      175 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/browser/static/overlay.js
--rw-r--r--   0 mpeeters   (501) staff       (20)     1276 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/browser/static/schedule.css
--rw-r--r--   0 mpeeters   (501) staff       (20)     3696 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/browser/task_completion.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1324 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/browser/task_owner.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio/schedule/browser/templates/
--rw-r--r--   0 mpeeters   (501) staff       (20)      566 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/browser/templates/close_task.pt
--rw-r--r--   0 mpeeters   (501) staff       (20)      577 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/browser/templates/task_change_owner.pt
--rw-r--r--   0 mpeeters   (501) staff       (20)     3167 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/browser/templates/task_completion.pt
--rw-r--r--   0 mpeeters   (501) staff       (20)     5112 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/browser/templates/taskmacros.pt
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio/schedule/collectionwidget/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/collectionwidget/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      638 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/collectionwidget/configure.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio/schedule/collectionwidget/templates/
--rw-r--r--   0 mpeeters   (501) staff       (20)     1569 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/collectionwidget/templates/term.pt
--rw-r--r--   0 mpeeters   (501) staff       (20)      439 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/collectionwidget/views.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1266 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/collectionwidget/vocabulary.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      661 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/config.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2155 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/configure.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio/schedule/content/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/content/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     5091 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/content/condition.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2177 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/content/conditions.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      362 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/content/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     2273 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/content/delay.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      592 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/content/delay.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     4054 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/content/logic.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1276 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/content/logic.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     6337 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/content/object_factories.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     3432 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/content/object_factories.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     2764 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/content/schedule_config.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1641 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/content/subform_context_choice.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     8001 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/content/task.py
--rw-r--r--   0 mpeeters   (501) staff       (20)    46099 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/content/task_config.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      460 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/content/view.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      304 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/content/view.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)    16202 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/content/vocabulary.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     5614 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/content/vocabulary.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      616 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/content/widget.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     2811 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/converter.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio/schedule/dashboard/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/dashboard/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     8625 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/dashboard/columns.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2640 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/dashboard/columns.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      178 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/dashboard/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      624 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/dashboard/interfaces.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1386 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/dashboard/vocabulary.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      534 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/dashboard/vocabulary.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     1988 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/deserializer.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio/schedule/events/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/events/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     5177 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/events/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     1810 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/events/create_task.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2883 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/events/dashboard_collection.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2174 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/events/task_config.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     7941 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/events/update_tasks.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     8333 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/events/zope_registration.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      611 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/indexes.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      378 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/indexes.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     5668 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/interfaces.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio/schedule/locales/
--rw-r--r--   0 mpeeters   (501) staff       (20)      767 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/locales/collective.eeafaceted.z3ctable.pot
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio/schedule/locales/fr/
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio/schedule/locales/fr/LC_MESSAGES/
--rw-r--r--   0 mpeeters   (501) staff       (20)      666 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.mo
--rw-r--r--   0 mpeeters   (501) staff       (20)      701 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.po
--rw-r--r--   0 mpeeters   (501) staff       (20)     8878 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/locales/fr/LC_MESSAGES/imio.schedule.mo
--rw-r--r--   0 mpeeters   (501) staff       (20)    13000 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/locales/fr/LC_MESSAGES/imio.schedule.po
--rw-r--r--   0 mpeeters   (501) staff       (20)     9745 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/locales/imio.schedule.pot
--rw-r--r--   0 mpeeters   (501) staff       (20)     1575 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/locales/manual_translations.pot
--rwxr-xr-x   0 mpeeters   (501) staff       (20)      686 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/locales/update.sh
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio/schedule/migration/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/migration/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      244 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/migration/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      561 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/migration/migrate_to_18.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1985 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/migration/upgrades.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      951 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/migration/upgrades.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio/schedule/profiles/
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio/schedule/profiles/default/
--rw-r--r--   0 mpeeters   (501) staff       (20)      148 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/profiles/default/browserlayer.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      554 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/profiles/default/catalog.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      490 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/profiles/default/cssregistry.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/profiles/default/imioschedule_default.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)      655 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/profiles/default/jsregistry.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      367 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/profiles/default/metadata.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      231 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/profiles/default/propertiestool.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     1824 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/profiles/default/registry.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio/schedule/profiles/default/types/
--rw-r--r--   0 mpeeters   (501) staff       (20)     2134 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/profiles/default/types/AutomatedMacroTask.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     1955 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/profiles/default/types/AutomatedTask.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     2193 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/profiles/default/types/MacroTaskConfig.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     2193 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/profiles/default/types/ScheduleConfig.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     2087 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/profiles/default/types/TaskConfig.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      488 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/profiles/default/types.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      369 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/profiles/default/workflows.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio/schedule/profiles/testing/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/profiles/testing/imioschedule_testing.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)      164 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/profiles/testing/metadata.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      222 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/setuphandlers.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     7829 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/testing.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      782 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/testing.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio/schedule/tests/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/tests/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1774 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/tests/condition.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     3056 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/tests/conditions.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      396 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/tests/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      279 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/tests/due_date.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      391 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/tests/due_date.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      318 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/tests/holidays.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      426 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/tests/logic.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      455 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/tests/logic.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio/schedule/tests/robot/
--rw-r--r--   0 mpeeters   (501) staff       (20)     1542 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/tests/robot/test_example.robot
--rw-r--r--   0 mpeeters   (501) staff       (20)     9742 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/tests/setup.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1003 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/tests/test_dashboardcollection.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2292 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/tests/test_delay.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1197 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/tests/test_indexes.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2792 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/tests/test_logic.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     6586 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/tests/test_registration_events.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     4809 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/tests/test_scheduleconfig.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     3294 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/tests/test_setup.py
--rw-r--r--   0 mpeeters   (501) staff       (20)    10523 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/tests/test_task.py
--rw-r--r--   0 mpeeters   (501) staff       (20)    17095 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/tests/test_task_events.py
--rw-r--r--   0 mpeeters   (501) staff       (20)    57639 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/tests/test_taskconfig.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     3361 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/tests/test_utils.py
--rw-r--r--   0 mpeeters   (501) staff       (20)    13257 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/tests/test_vocabulary.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     7651 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/utils.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      847 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/vocabularies.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      461 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/vocabularies.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio/schedule/workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/workflow/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      404 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/workflow/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     1286 2024-04-10 10:54:24.000000 imio.schedule-2.2.1/src/imio/schedule/workflow/freeze_task.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio.schedule.egg-info/
--rw-r--r--   0 mpeeters   (501) staff       (20)     4274 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio.schedule.egg-info/PKG-INFO
--rw-r--r--   0 mpeeters   (501) staff       (20)     5744 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio.schedule.egg-info/SOURCES.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)        1 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio.schedule.egg-info/dependency_links.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)       40 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio.schedule.egg-info/entry_points.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)        5 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio.schedule.egg-info/namespace_packages.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)        1 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio.schedule.egg-info/not-zip-safe
--rw-r--r--   0 mpeeters   (501) staff       (20)      240 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio.schedule.egg-info/requires.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)        5 2024-04-10 10:54:25.000000 imio.schedule-2.2.1/src/imio.schedule.egg-info/top_level.txt
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2507 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/CHANGES.rst
+-rw-r--r--   0 mpeeters   (501) staff       (20)       41 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/CONTRIBUTORS.rst
+-rw-r--r--   0 mpeeters   (501) staff       (20)      135 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/MANIFEST.in
+-rw-r--r--   0 mpeeters   (501) staff       (20)      703 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/Makefile
+-rw-r--r--   0 mpeeters   (501) staff       (20)     4762 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/PKG-INFO
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1543 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/README.rst
+-rw-r--r--   0 mpeeters   (501) staff       (20)     7202 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/bootstrap.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/docs/
+-rw-r--r--   0 mpeeters   (501) staff       (20)    18092 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/docs/LICENSE.GPL
+-rw-r--r--   0 mpeeters   (501) staff       (20)      658 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/docs/LICENSE.rst
+-rw-r--r--   0 mpeeters   (501) staff       (20)       76 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/docs/index.rst
+-rw-r--r--   0 mpeeters   (501) staff       (20)      579 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/pyproject.toml
+-rw-r--r--   0 mpeeters   (501) staff       (20)       45 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/requirements.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)      140 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/setup.cfg
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1884 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/setup.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio/
+-rw-r--r--   0 mpeeters   (501) staff       (20)       80 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/__init__.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio/schedule/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      130 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/__init__.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio/schedule/browser/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/browser/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1071 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/browser/close_task.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1806 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/browser/configure.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio/schedule/browser/overrides/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/browser/overrides/.gitkeep
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio/schedule/browser/static/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/browser/static/.gitkeep
+-rw-r--r--   0 mpeeters   (501) staff       (20)      175 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/browser/static/overlay.js
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1276 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/browser/static/schedule.css
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3656 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/browser/task_completion.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1324 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/browser/task_owner.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio/schedule/browser/templates/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      566 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/browser/templates/close_task.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)      577 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/browser/templates/task_change_owner.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3167 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/browser/templates/task_completion.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5112 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/browser/templates/taskmacros.pt
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio/schedule/collectionwidget/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/collectionwidget/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      638 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/collectionwidget/configure.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio/schedule/collectionwidget/templates/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1569 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/collectionwidget/templates/term.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)      435 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/collectionwidget/views.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1290 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/collectionwidget/vocabulary.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      583 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/config.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2155 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/configure.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio/schedule/content/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/content/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5057 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/content/condition.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2177 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/content/conditions.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      362 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/content/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2289 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/content/delay.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      592 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/content/delay.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     4056 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/content/logic.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1276 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/content/logic.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     6337 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/content/object_factories.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3432 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/content/object_factories.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2764 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/content/schedule_config.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1640 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/content/subform_context_choice.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     7930 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/content/task.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)    47831 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/content/task_config.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      460 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/content/view.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      304 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/content/view.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)    16557 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/content/vocabulary.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5614 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/content/vocabulary.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      616 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/content/widget.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2811 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/converter.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio/schedule/dashboard/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/dashboard/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     8699 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/dashboard/columns.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2640 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/dashboard/columns.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      178 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/dashboard/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      607 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/dashboard/interfaces.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1309 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/dashboard/vocabulary.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      534 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/dashboard/vocabulary.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1988 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/deserializer.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio/schedule/events/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/events/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5177 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/events/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1848 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/events/create_task.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2903 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/events/dashboard_collection.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2253 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/events/task_config.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     7931 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/events/update_tasks.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     8329 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/events/zope_registration.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      611 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/indexes.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      378 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/indexes.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5791 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/interfaces.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio/schedule/locales/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      767 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/locales/collective.eeafaceted.z3ctable.pot
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio/schedule/locales/fr/
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio/schedule/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      666 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.mo
+-rw-r--r--   0 mpeeters   (501) staff       (20)      701 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.po
+-rw-r--r--   0 mpeeters   (501) staff       (20)     9352 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/locales/fr/LC_MESSAGES/imio.schedule.mo
+-rw-r--r--   0 mpeeters   (501) staff       (20)    13756 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/locales/fr/LC_MESSAGES/imio.schedule.po
+-rw-r--r--   0 mpeeters   (501) staff       (20)    10281 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/locales/imio.schedule.pot
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1575 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/locales/manual_translations.pot
+-rwxr-xr-x   0 mpeeters   (501) staff       (20)      686 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/locales/update.sh
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio/schedule/migration/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/migration/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      244 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/migration/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      561 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/migration/migrate_to_18.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2016 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/migration/upgrades.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      951 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/migration/upgrades.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio/schedule/profiles/
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio/schedule/profiles/default/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      148 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/profiles/default/browserlayer.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      554 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/profiles/default/catalog.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      490 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/profiles/default/cssregistry.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/profiles/default/imioschedule_default.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)      655 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/profiles/default/jsregistry.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      367 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/profiles/default/metadata.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      231 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/profiles/default/propertiestool.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1824 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/profiles/default/registry.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio/schedule/profiles/default/types/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2134 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/profiles/default/types/AutomatedMacroTask.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1955 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/profiles/default/types/AutomatedTask.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2193 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/profiles/default/types/MacroTaskConfig.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2193 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/profiles/default/types/ScheduleConfig.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2087 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/profiles/default/types/TaskConfig.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      488 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/profiles/default/types.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      369 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/profiles/default/workflows.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio/schedule/profiles/testing/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/profiles/testing/imioschedule_testing.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)      164 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/profiles/testing/metadata.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      222 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/setuphandlers.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     8204 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/testing.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      782 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/testing.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio/schedule/tests/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/tests/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1774 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/tests/condition.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3056 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/tests/conditions.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      396 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/tests/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      279 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/tests/due_date.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      391 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/tests/due_date.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      317 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/tests/holidays.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      426 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/tests/logic.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      455 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/tests/logic.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio/schedule/tests/robot/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1542 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/tests/robot/test_example.robot
+-rw-r--r--   0 mpeeters   (501) staff       (20)     9639 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/tests/setup.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      999 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/tests/test_dashboardcollection.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2312 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/tests/test_delay.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1197 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/tests/test_indexes.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2696 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/tests/test_logic.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     6618 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/tests/test_registration_events.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     4810 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/tests/test_scheduleconfig.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3326 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/tests/test_setup.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)    10613 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/tests/test_task.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)    17199 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/tests/test_task_events.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)    61395 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/tests/test_taskconfig.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3403 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/tests/test_utils.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)    13559 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/tests/test_vocabulary.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     7668 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/utils.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      933 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/vocabularies.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      461 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/vocabularies.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio/schedule/workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/workflow/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      404 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/workflow/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1286 2024-04-25 16:23:20.000000 imio.schedule-2.2.2/src/imio/schedule/workflow/freeze_task.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio.schedule.egg-info/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     4762 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio.schedule.egg-info/PKG-INFO
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5776 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio.schedule.egg-info/SOURCES.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)        1 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio.schedule.egg-info/dependency_links.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)       40 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio.schedule.egg-info/entry_points.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)        5 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio.schedule.egg-info/namespace_packages.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)        1 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio.schedule.egg-info/not-zip-safe
+-rw-r--r--   0 mpeeters   (501) staff       (20)      254 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio.schedule.egg-info/requires.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)        5 2024-04-25 16:23:22.000000 imio.schedule-2.2.2/src/imio.schedule.egg-info/top_level.txt
```

### Comparing `imio.schedule-2.2.1/CHANGES.rst` & `imio.schedule-2.2.2/CHANGES.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,35 @@
 Changelog
 =========
 
+.. You should *NOT* be adding new change log entries to this file.
+   You should create a file in the news directory instead.
+   For helpful instructions, please see:
+   https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
+
+.. towncrier release notes start
+
+2.2.2 (2024-04-25)
+------------------
+
+New features:
+
+
+- Allow additional delay to be a TAL expression
+  [mpeeters] (URB-3005)
+
+
+Internal:
+
+
+- Black
+  [mpeeters] (SUP-27104)
+- Fix tests
+  [mpeeters] (URB-3005)
+
 
 2.2.1 (2024-04-10)
 ------------------
 
 - Fix object deserializer
   [jchandelle]
```

### Comparing `imio.schedule-2.2.1/Makefile` & `imio.schedule-2.2.2/Makefile`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/PKG-INFO` & `imio.schedule-2.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.schedule
-Version: 2.2.1
+Version: 2.2.2
 Summary: Schedule for imio products
 Home-page: https://pypi.python.org/pypi/imio.schedule
 Author: Simon Delcourt
 Author-email: simon.delcourt@imio.be
 License: GPL version 2
 Keywords: Python Plone
 Classifier: Environment :: Web Environment
@@ -94,14 +94,39 @@
 ============
 
 - Simon Delcourt, simon.delcourt@imio.be
 
 Changelog
 =========
 
+.. You should *NOT* be adding new change log entries to this file.
+   You should create a file in the news directory instead.
+   For helpful instructions, please see:
+   https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
+
+.. towncrier release notes start
+
+2.2.2 (2024-04-25)
+------------------
+
+New features:
+
+
+- Allow additional delay to be a TAL expression
+  [mpeeters] (URB-3005)
+
+
+Internal:
+
+
+- Black
+  [mpeeters] (SUP-27104)
+- Fix tests
+  [mpeeters] (URB-3005)
+
 
 2.2.1 (2024-04-10)
 ------------------
 
 - Fix object deserializer
   [jchandelle]
```

### Comparing `imio.schedule-2.2.1/README.rst` & `imio.schedule-2.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/bootstrap.py` & `imio.schedule-2.2.2/bootstrap.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,59 +21,73 @@
 import os
 import shutil
 import sys
 import tempfile
 
 from optparse import OptionParser
 
-__version__ = '2015-07-01'
+__version__ = "2015-07-01"
 # See zc.buildout's changelog if this version is up to date.
 
-tmpeggs = tempfile.mkdtemp(prefix='bootstrap-')
+tmpeggs = tempfile.mkdtemp(prefix="bootstrap-")
 
-usage = '''\
+usage = """\
 [DESIRED PYTHON FOR BUILDOUT] bootstrap.py [options]
 
 Bootstraps a buildout-based project.
 
 Simply run this script in a directory containing a buildout.cfg, using the
 Python that you want bin/buildout to use.
 
 Note that by using --find-links to point to local resources, you can keep
 this script from going over the network.
-'''
+"""
 
 parser = OptionParser(usage=usage)
-parser.add_option("--version",
-                  action="store_true", default=False,
-                  help=("Return bootstrap.py version."))
-parser.add_option("-t", "--accept-buildout-test-releases",
-                  dest='accept_buildout_test_releases',
-                  action="store_true", default=False,
-                  help=("Normally, if you do not specify a --version, the "
-                        "bootstrap script and buildout gets the newest "
-                        "*final* versions of zc.buildout and its recipes and "
-                        "extensions for you.  If you use this flag, "
-                        "bootstrap and buildout will get the newest releases "
-                        "even if they are alphas or betas."))
-parser.add_option("-c", "--config-file",
-                  help=("Specify the path to the buildout configuration "
-                        "file to be used."))
-parser.add_option("-f", "--find-links",
-                  help=("Specify a URL to search for buildout releases"))
-parser.add_option("--allow-site-packages",
-                  action="store_true", default=False,
-                  help=("Let bootstrap.py use existing site packages"))
-parser.add_option("--buildout-version",
-                  help="Use a specific zc.buildout version")
-parser.add_option("--setuptools-version",
-                  help="Use a specific setuptools version")
-parser.add_option("--setuptools-to-dir",
-                  help=("Allow for re-use of existing directory of "
-                        "setuptools versions"))
+parser.add_option(
+    "--version",
+    action="store_true",
+    default=False,
+    help=("Return bootstrap.py version."),
+)
+parser.add_option(
+    "-t",
+    "--accept-buildout-test-releases",
+    dest="accept_buildout_test_releases",
+    action="store_true",
+    default=False,
+    help=(
+        "Normally, if you do not specify a --version, the "
+        "bootstrap script and buildout gets the newest "
+        "*final* versions of zc.buildout and its recipes and "
+        "extensions for you.  If you use this flag, "
+        "bootstrap and buildout will get the newest releases "
+        "even if they are alphas or betas."
+    ),
+)
+parser.add_option(
+    "-c",
+    "--config-file",
+    help=("Specify the path to the buildout configuration " "file to be used."),
+)
+parser.add_option(
+    "-f", "--find-links", help=("Specify a URL to search for buildout releases")
+)
+parser.add_option(
+    "--allow-site-packages",
+    action="store_true",
+    default=False,
+    help=("Let bootstrap.py use existing site packages"),
+)
+parser.add_option("--buildout-version", help="Use a specific zc.buildout version")
+parser.add_option("--setuptools-version", help="Use a specific setuptools version")
+parser.add_option(
+    "--setuptools-to-dir",
+    help=("Allow for re-use of existing directory of " "setuptools versions"),
+)
 
 options, args = parser.parse_args()
 if options.version:
     print("bootstrap.py version %s" % __version__)
     sys.exit(0)
 
 
@@ -82,94 +96,100 @@
 
 try:
     from urllib.request import urlopen
 except ImportError:
     from urllib2 import urlopen
 
 ez = {}
-if os.path.exists('ez_setup.py'):
-    exec(open('ez_setup.py').read(), ez)
+if os.path.exists("ez_setup.py"):
+    exec(open("ez_setup.py").read(), ez)
 else:
-    exec(urlopen('https://bootstrap.pypa.io/ez_setup.py').read(), ez)
+    exec(urlopen("https://bootstrap.pypa.io/ez_setup.py").read(), ez)
 
 if not options.allow_site_packages:
     # ez_setup imports site, which adds site packages
     # this will remove them from the path to ensure that incompatible versions
     # of setuptools are not in the path
     import site
+
     # inside a virtualenv, there is no 'getsitepackages'.
     # We can't remove these reliably
-    if hasattr(site, 'getsitepackages'):
+    if hasattr(site, "getsitepackages"):
         for sitepackage_path in site.getsitepackages():
             # Strip all site-packages directories from sys.path that
             # are not sys.prefix; this is because on Windows
             # sys.prefix is a site-package directory.
             if sitepackage_path != sys.prefix:
-                sys.path[:] = [x for x in sys.path
-                               if sitepackage_path not in x]
+                sys.path[:] = [x for x in sys.path if sitepackage_path not in x]
 
 setup_args = dict(to_dir=tmpeggs, download_delay=0)
 
 if options.setuptools_version is not None:
-    setup_args['version'] = options.setuptools_version
+    setup_args["version"] = options.setuptools_version
 if options.setuptools_to_dir is not None:
-    setup_args['to_dir'] = options.setuptools_to_dir
+    setup_args["to_dir"] = options.setuptools_to_dir
 
-ez['use_setuptools'](**setup_args)
+ez["use_setuptools"](**setup_args)
 import setuptools
 import pkg_resources
 
 # This does not (always?) update the default working set.  We will
 # do it.
 for path in sys.path:
     if path not in pkg_resources.working_set.entries:
         pkg_resources.working_set.add_entry(path)
 
 ######################################################################
 # Install buildout
 
 ws = pkg_resources.working_set
 
-setuptools_path = ws.find(
-    pkg_resources.Requirement.parse('setuptools')).location
+setuptools_path = ws.find(pkg_resources.Requirement.parse("setuptools")).location
 
 # Fix sys.path here as easy_install.pth added before PYTHONPATH
-cmd = [sys.executable, '-c',
-       'import sys; sys.path[0:0] = [%r]; ' % setuptools_path +
-       'from setuptools.command.easy_install import main; main()',
-       '-mZqNxd', tmpeggs]
+cmd = [
+    sys.executable,
+    "-c",
+    "import sys; sys.path[0:0] = [%r]; " % setuptools_path
+    + "from setuptools.command.easy_install import main; main()",
+    "-mZqNxd",
+    tmpeggs,
+]
 
 find_links = os.environ.get(
-    'bootstrap-testing-find-links',
-    options.find_links or
-    ('http://downloads.buildout.org/'
-     if options.accept_buildout_test_releases else None)
-    )
+    "bootstrap-testing-find-links",
+    options.find_links
+    or (
+        "http://downloads.buildout.org/"
+        if options.accept_buildout_test_releases
+        else None
+    ),
+)
 if find_links:
-    cmd.extend(['-f', find_links])
+    cmd.extend(["-f", find_links])
 
-requirement = 'zc.buildout'
+requirement = "zc.buildout"
 version = options.buildout_version
 if version is None and not options.accept_buildout_test_releases:
     # Figure out the most recent final version of zc.buildout.
     import setuptools.package_index
-    _final_parts = '*final-', '*final'
+
+    _final_parts = "*final-", "*final"
 
     def _final_version(parsed_version):
         try:
             return not parsed_version.is_prerelease
         except AttributeError:
             # Older setuptools
             for part in parsed_version:
-                if (part[:1] == '*') and (part not in _final_parts):
+                if (part[:1] == "*") and (part not in _final_parts):
                     return False
             return True
 
-    index = setuptools.package_index.PackageIndex(
-        search_path=[setuptools_path])
+    index = setuptools.package_index.PackageIndex(search_path=[setuptools_path])
     if find_links:
         index.add_find_links((find_links,))
     req = pkg_resources.Requirement.parse(requirement)
     if index.obtain(req) is not None:
         best = []
         bestv = None
         for dist in index[req.project_name]:
@@ -180,31 +200,31 @@
                     bestv = distv
                 elif distv == bestv:
                     best.append(dist)
         if best:
             best.sort()
             version = best[-1].version
 if version:
-    requirement = '=='.join((requirement, version))
+    requirement = "==".join((requirement, version))
 cmd.append(requirement)
 
 import subprocess
+
 if subprocess.call(cmd) != 0:
-    raise Exception(
-        "Failed to execute command:\n%s" % repr(cmd)[1:-1])
+    raise Exception("Failed to execute command:\n%s" % repr(cmd)[1:-1])
 
 ######################################################################
 # Import and run buildout
 
 ws.add_entry(tmpeggs)
 ws.require(requirement)
 import zc.buildout.buildout
 
-if not [a for a in args if '=' not in a]:
-    args.append('bootstrap')
+if not [a for a in args if "=" not in a]:
+    args.append("bootstrap")
 
 # if -c was provided, we push it back into args for buildout' main function
 if options.config_file is not None:
-    args[0:0] = ['-c', options.config_file]
+    args[0:0] = ["-c", options.config_file]
 
 zc.buildout.buildout.main(args)
 shutil.rmtree(tmpeggs)
```

### Comparing `imio.schedule-2.2.1/docs/LICENSE.GPL` & `imio.schedule-2.2.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/docs/LICENSE.rst` & `imio.schedule-2.2.2/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/setup.py` & `imio.schedule-2.2.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,67 +2,69 @@
 """Installer for the imio.schedule package."""
 
 from setuptools import find_packages
 from setuptools import setup
 
 
 long_description = (
-    open('README.rst').read() +
-    '\n' +
-    'Contributors\n' +
-    '============\n' +
-    '\n' +
-    open('CONTRIBUTORS.rst').read() +
-    '\n' +
-    open('CHANGES.rst').read() +
-    '\n')
+    open("README.rst").read()
+    + "\n"
+    + "Contributors\n"
+    + "============\n"
+    + "\n"
+    + open("CONTRIBUTORS.rst").read()
+    + "\n"
+    + open("CHANGES.rst").read()
+    + "\n"
+)
 
 
 setup(
-    name='imio.schedule',
-    version='2.2.1',
+    name="imio.schedule",
+    version="2.2.2",
     description="Schedule for imio products",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 4.3",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
-    keywords='Python Plone',
-    author='Simon Delcourt',
-    author_email='simon.delcourt@imio.be',
-    url='https://pypi.python.org/pypi/imio.schedule',
-    license='GPL version 2',
-    packages=find_packages('src', exclude=['ez_setup']),
-    namespace_packages=['imio'],
-    package_dir={'': 'src'},
+    keywords="Python Plone",
+    author="Simon Delcourt",
+    author_email="simon.delcourt@imio.be",
+    url="https://pypi.python.org/pypi/imio.schedule",
+    license="GPL version 2",
+    packages=find_packages("src", exclude=["ez_setup"]),
+    namespace_packages=["imio"],
+    package_dir={"": "src"},
     include_package_data=True,
     zip_safe=False,
     install_requires=[
-        'collective.eeafaceted.collectionwidget',
-        'collective.faceted.task',
-        'collective.wfadaptations',
-        'collective.z3cform.datagridfield',
-        'imio.dashboard',
-        'plone.api',
-        'plone.app.dexterity',
-        'Products.cron4plone',
-        'setuptools',
-        'workalendar',
+        "collective.eeafaceted.collectionwidget",
+        "collective.faceted.task",
+        "collective.wfadaptations",
+        "collective.z3cform.datagridfield",
+        "imio.dashboard",
+        "plone.api",
+        "plone.app.dexterity",
+        "plone.restapi",
+        "Products.cron4plone",
+        "setuptools",
+        "workalendar",
     ],
     extras_require={
-        'test': [
-            'Mock',
-            'plone.app.testing',
+        "test": [
+            "Mock",
+            "plone.app.testing",
         ],
     },
     entry_points="""
     [z3c.autoinclude.plugin]
     target = plone
     """,
 )
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/browser/close_task.py` & `imio.schedule-2.2.2/src/imio/schedule/browser/close_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     """ """
 
 
 class CloseTaskForm(Form):
     fields = field.Fields(ICloseTask)
     ignoreContext = True
 
-    @button.buttonAndHandler(_(u'Confirm'))
+    @button.buttonAndHandler(_(u"Confirm"))
     def handleApply(self, action):
         messages = IStatusMessage(self.request)
         data, errors = self.extractData()
         if errors:
             self.status = self.formErrorsMessage
             messages.addStatusMessage(self.status, type="error")
             return
         self.context._end()
-        self.context.reindex_parent_tasks(idxs=['is_solvable_task'])
-        self.status = _(u'Task Closed')
+        self.context.reindex_parent_tasks(idxs=["is_solvable_task"])
+        self.status = _(u"Task Closed")
 
 
 class CloseTaskView(FormWrapper):
     form = CloseTaskForm
-    index = ViewPageTemplateFile('templates/close_task.pt')
+    index = ViewPageTemplateFile("templates/close_task.pt")
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/browser/configure.zcml` & `imio.schedule-2.2.2/src/imio/schedule/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/browser/static/schedule.css` & `imio.schedule-2.2.2/src/imio/schedule/browser/static/schedule.css`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/browser/task_completion.py` & `imio.schedule-2.2.2/src/imio/schedule/browser/task_completion.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,38 +12,36 @@
 class TaskCompletionView(BrowserView):
     """
     View of the popup showing the completion details of a task.
     Display the status of each start/end condition of the task.
     Display if the starting/ending state is matched or not.
     """
 
-    subtask_title_label = 'Title'
-    subtask_todo_title_label = 'Title'
-    subtask_status_label = 'Status'
-    due_date_label = 'Due date'
-    end_date_label = 'End date'
-    assigned_user_label = 'Assigned to'
+    subtask_title_label = "Title"
+    subtask_todo_title_label = "Title"
+    subtask_status_label = "Status"
+    due_date_label = "Due date"
+    end_date_label = "End date"
+    assigned_user_label = "Assigned to"
 
     def __init__(self, context, request):
         self.context = context
         self.request = request
         self.task = context
 
     def get_conditions_status(self):
         """
         List all the tasks conditions status (except for workflow state).
         """
 
     def get_state_status(self):
-        """
-        """
+        """ """
 
     def get_subtasks_status(self):
-        """
-        """
+        """ """
         created = []
         started = []
         done = []
         for subtask in self.task.get_last_subtasks():
             status = status_by_state[self.get_state(subtask)]
             if status is DONE:
                 done.append(subtask)
@@ -61,26 +59,25 @@
         return api.content.get_state(context)
 
     def display_user_name(self, user_id):
         """
         Return the full name of the given user id.
         """
         user = api.user.get(user_id)
-        user_name = user and user.getProperty('fullname') or user_id
+        user_name = user and user.getProperty("fullname") or user_id
         return user_name
 
     def display_date(self, date):
-        """
-        """
+        """ """
         if not date:
-            return '-'
+            return "-"
         if date.year == 9999:
-            return u'\u221E'.encode('utf-8')
+            return u"\u221E".encode("utf-8")
 
-        return date.strftime('%d/%m/%Y')
+        return date.strftime("%d/%m/%Y")
 
 
 class TaskStartStatusView(TaskCompletionView):
     """
     View of the popup showing the start completion details of a created task.
     Display the status of each start condition of the task.
     Display the status of each subtask.
@@ -90,16 +87,15 @@
     def get_conditions_status(self):
         """
         List all the tasks conditions status (except for workflow state).
         """
         return self.task.start_conditions_status()
 
     def get_state_status(self):
-        """
-        """
+        """ """
         return self.task.starting_states_status()
 
 
 class TaskStartSimpleStatusView(TaskStartStatusView):
     """
     Same as the above but without subtasks status.
     """
@@ -121,16 +117,15 @@
     def get_conditions_status(self):
         """
         List all the tasks conditions status (except for workflow state).
         """
         return self.task.end_conditions_status()
 
     def get_state_status(self):
-        """
-        """
+        """ """
         return self.task.ending_states_status()
 
 
 class TaskEndSimpleStatusView(TaskEndStatusView):
     """
     Same as the above but without subtasks status.
     """
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/browser/task_owner.py` & `imio.schedule-2.2.2/src/imio/schedule/browser/task_owner.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,34 +11,34 @@
 
 from imio.schedule import _
 
 
 class ITaskChangeOwner(Interface):
 
     new_owner = schema.Choice(
-        title=_(u'New owner'),
-        vocabulary='schedule.task_owner',
+        title=_(u"New owner"),
+        vocabulary="schedule.task_owner",
         required=True,
     )
 
 
 class TaskChangeOwnerForm(Form):
     fields = field.Fields(ITaskChangeOwner)
     ignoreContext = True
 
-    @button.buttonAndHandler(_(u'Confirm'))
+    @button.buttonAndHandler(_(u"Confirm"))
     def handleApply(self, action):
         messages = IStatusMessage(self.request)
         data, errors = self.extractData()
         if errors:
             self.status = self.formErrorsMessage
             messages.addStatusMessage(self.status, type="error")
             return
-        self.context.assigned_user = data.get('new_owner')
+        self.context.assigned_user = data.get("new_owner")
         self.context.reindexObject()
-        self.context.reindex_parent_tasks(idxs=['is_solvable_task'])
-        self.status = _(u'Owner changed')
+        self.context.reindex_parent_tasks(idxs=["is_solvable_task"])
+        self.status = _(u"Owner changed")
 
 
 class TaskChangeOwnerView(FormWrapper):
     form = TaskChangeOwnerForm
-    index = ViewPageTemplateFile('templates/task_change_owner.pt')
+    index = ViewPageTemplateFile("templates/task_change_owner.pt")
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/browser/templates/close_task.pt` & `imio.schedule-2.2.2/src/imio/schedule/browser/templates/close_task.pt`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/browser/templates/task_change_owner.pt` & `imio.schedule-2.2.2/src/imio/schedule/browser/templates/task_change_owner.pt`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/browser/templates/task_completion.pt` & `imio.schedule-2.2.2/src/imio/schedule/browser/templates/task_completion.pt`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/browser/templates/taskmacros.pt` & `imio.schedule-2.2.2/src/imio/schedule/browser/templates/taskmacros.pt`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/collectionwidget/configure.zcml` & `imio.schedule-2.2.2/src/imio/schedule/collectionwidget/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/collectionwidget/templates/term.pt` & `imio.schedule-2.2.2/src/imio/schedule/collectionwidget/templates/term.pt`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/collectionwidget/vocabulary.py` & `imio.schedule-2.2.2/src/imio/schedule/collectionwidget/vocabulary.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,25 +12,28 @@
     Return vocabulary of base searchs for schedule faceted view.
     """
 
     def _brains(self, context):
         """
         Return all the DashboardCollections in the 'schedule' folder.
         """
-        configs_UID = IAnnotations(context).get('imio.schedule.schedule_configs', [])
-        catalog = api.portal.get_tool('portal_catalog')
+        configs_UID = IAnnotations(context).get("imio.schedule.schedule_configs", [])
+        catalog = api.portal.get_tool("portal_catalog")
         config_brains = catalog(UID=configs_UID)
         collections_brains = []
         for brain in config_brains:
             config = brain.getObject()
             brains = catalog(
                 path={
-                    'query': '/'.join(config.getPhysicalPath()),
+                    "query": "/".join(config.getPhysicalPath()),
                 },
-                object_provides='plone.app.contenttypes.interfaces.ICollection',
-                sort_on='getObjPositionInParent'
+                object_provides="plone.app.contenttypes.interfaces.ICollection",
+                sort_on="getObjPositionInParent",
             )
             collections_brains.extend(brains)
-        collections_brains = [b for b in collections_brains if b.getObject().aq_parent.enabled]
+        collections_brains = [
+            b for b in collections_brains if b.getObject().aq_parent.enabled
+        ]
         return collections_brains
 
+
 ScheduleCollectionVocabularyFactory = ScheduleCollectionVocabulary()
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/configure.zcml` & `imio.schedule-2.2.2/src/imio/schedule/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/content/condition.py` & `imio.schedule-2.2.2/src/imio/schedule/content/condition.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,57 +169,51 @@
 
 class CreateIfSubtaskCanBeCreated(MacroTaskCreationCondition):
     """
     Return True if at least one substask can be created.
     """
 
     def evaluate(self):
-        """
-        """
+        """ """
 
 
 class CreateIfAllSubtasksCanBeCreated(MacroTaskCreationCondition):
     """
     Return True if all substasks can be created.
     """
 
     def evaluate(self):
-        """
-        """
+        """ """
 
 
 class StartIfAnySubtaskStarted(MacroTaskStartCondition):
     """
     Return True if at least one substask started.
     """
 
     def evaluate(self):
-        """
-        """
+        """ """
 
 
 class StartIfAllSubtasksStarted(MacroTaskStartCondition):
     """
     Return True if all substasks started.
     """
 
     def evaluate(self):
-        """
-        """
+        """ """
 
 
 class RecurrencyCondition(Condition):
-
     def __init__(self, task_container, task_config):
         self.task_container = task_container
         self.task_config = task_config
 
 
 class NoRecurencyCondition(RecurrencyCondition):
-
     def evaluate(self):
         return False
 
 
 class TaskDueDateReachedCondition(EndCondition):
     """
     Return True if the task delay is overdue.
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/content/conditions.zcml` & `imio.schedule-2.2.2/src/imio/schedule/content/conditions.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/content/delay.py` & `imio.schedule-2.2.2/src/imio/schedule/content/delay.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,30 +45,30 @@
 
     def compute_due_date(self, date):
         """Return the addition of the given date and the extra delay"""
         return date + relativedelta(days=+self.delta)
 
 
 class CalculationDefaultDelay(BaseCalculationDelay):
-    """
-    """
+    """ """
 
     def calculate_delay(self):
         return 0
 
 
 class DefaultFreezeDuration(object):
-    """
-    """
+    """ """
 
     def __init__(self, task_container, task):
         self.container = task_container
         self.task = task
 
     @property
     def freeze_duration(self):
         annotations = IAnnotations(self.task)
-        freeze_infos = annotations['imio.schedule.freeze_task']
-        freeze_date = datetime.strptime(freeze_infos['freeze_date'], '%Y-%m-%d')
+        freeze_infos = annotations["imio.schedule.freeze_task"]
+        freeze_date = datetime.strptime(freeze_infos["freeze_date"], "%Y-%m-%d")
         freeze_delta = datetime.now().date() - freeze_date.date()
-        new_freeze_duration = freeze_infos['previous_freeze_duration'] + freeze_delta.days
+        new_freeze_duration = (
+            freeze_infos["previous_freeze_duration"] + freeze_delta.days
+        )
         return new_freeze_duration
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/content/delay.zcml` & `imio.schedule-2.2.2/src/imio/schedule/content/delay.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/content/logic.py` & `imio.schedule-2.2.2/src/imio/schedule/content/logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,16 +80,16 @@
 
     def start_date(self):
         """
         Return the date when the task started.
         """
         history = self.task.workflow_history.values()[0]
         for state_history in history:
-            if status_by_state[state_history.get('review_state')] is STARTED:
-                return state_history['time']
+            if status_by_state[state_history.get("review_state")] is STARTED:
+                return state_history["time"]
 
 
 class SubtaskHighestDueDate(MacroTaskStartDate):
     """
     Return the highest due date of the subtasks.
     """
 
@@ -107,14 +107,15 @@
 class AssignTaskUser(TaskLogic):
     """
     Base class for adapters adapting a TaskContainer to return a user to
     assign to its tasks.
     Register adapters inheriting this class in the products using
     imio.schedule and override 'user_id' method.
     """
+
     implements(IDefaultTaskUser)
 
     def user_id(self):
         """
         To override.
         """
 
@@ -152,13 +153,14 @@
 class AssignTaskGroup(TaskLogic):
     """
     Base class for adapters adapting a TaskContainer to return a group to
     assign to its tasks.
     Register adapters inheriting this class in the products using
     imio.schedule and override 'group_id' method.
     """
+
     implements(IDefaultTaskGroup)
 
     def group_id(self):
         """
         To override.
         """
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/content/logic.zcml` & `imio.schedule-2.2.2/src/imio/schedule/content/logic.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/content/object_factories.py` & `imio.schedule-2.2.2/src/imio/schedule/content/object_factories.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,163 +19,163 @@
 
 
 class BaseConditionObject(object):
     """
     Base class for condition objects.
     """
 
-    __name__ = ''
+    __name__ = ""
     __parent__ = None
 
     def __init__(self, condition=None, operator=None, display_status=True):
         if condition is not None:
-            self.__dict__['condition'] = condition
+            self.__dict__["condition"] = condition
         if operator is not None:
-            self.__dict__['operator'] = operator
-        self.__dict__['display_status'] = display_status
+            self.__dict__["operator"] = operator
+        self.__dict__["display_status"] = display_status
 
     def getId(self):
-        return self.__name__ or ''
+        return self.__name__ or ""
 
 
 class CreationConditionObject(BaseConditionObject):
     implements(ICreationConditionSchema)
 
-    condition = FieldProperty(ICreationConditionSchema['condition'])
-    operator = FieldProperty(ICreationConditionSchema['operator'])
-    display_status = FieldProperty(ICreationConditionSchema['display_status'])
+    condition = FieldProperty(ICreationConditionSchema["condition"])
+    operator = FieldProperty(ICreationConditionSchema["operator"])
+    display_status = FieldProperty(ICreationConditionSchema["display_status"])
 
 
 class CreationConditionAdapter(FactoryAdapter):
     factory = CreationConditionObject
 
 
 class StartConditionObject(BaseConditionObject):
     implements(IStartConditionSchema)
 
-    condition = FieldProperty(IStartConditionSchema['condition'])
-    operator = FieldProperty(IStartConditionSchema['operator'])
-    display_status = FieldProperty(IStartConditionSchema['display_status'])
+    condition = FieldProperty(IStartConditionSchema["condition"])
+    operator = FieldProperty(IStartConditionSchema["operator"])
+    display_status = FieldProperty(IStartConditionSchema["display_status"])
 
 
 class StartConditionAdapter(FactoryAdapter):
     factory = StartConditionObject
 
 
 class EndConditionObject(BaseConditionObject):
     implements(IEndConditionSchema)
 
-    condition = FieldProperty(IEndConditionSchema['condition'])
-    operator = FieldProperty(IEndConditionSchema['operator'])
-    display_status = FieldProperty(IEndConditionSchema['display_status'])
+    condition = FieldProperty(IEndConditionSchema["condition"])
+    operator = FieldProperty(IEndConditionSchema["operator"])
+    display_status = FieldProperty(IEndConditionSchema["display_status"])
 
 
 class EndConditionAdapter(FactoryAdapter):
     factory = EndConditionObject
 
 
 class FreezeConditionObject(BaseConditionObject):
     implements(IFreezeConditionSchema)
 
-    condition = FieldProperty(IFreezeConditionSchema['condition'])
-    operator = FieldProperty(IFreezeConditionSchema['operator'])
-    display_status = FieldProperty(IFreezeConditionSchema['display_status'])
+    condition = FieldProperty(IFreezeConditionSchema["condition"])
+    operator = FieldProperty(IFreezeConditionSchema["operator"])
+    display_status = FieldProperty(IFreezeConditionSchema["display_status"])
 
 
 class FreezeConditionAdapter(FactoryAdapter):
     factory = FreezeConditionObject
 
 
 class ThawConditionObject(BaseConditionObject):
     implements(IThawConditionSchema)
 
-    condition = FieldProperty(IThawConditionSchema['condition'])
-    operator = FieldProperty(IThawConditionSchema['operator'])
-    display_status = FieldProperty(IThawConditionSchema['display_status'])
+    condition = FieldProperty(IThawConditionSchema["condition"])
+    operator = FieldProperty(IThawConditionSchema["operator"])
+    display_status = FieldProperty(IThawConditionSchema["display_status"])
 
 
 class ThawConditionAdapter(FactoryAdapter):
     factory = ThawConditionObject
 
 
 class MacroCreationConditionObject(BaseConditionObject):
     implements(IMacroCreationConditionSchema)
 
-    condition = FieldProperty(IMacroCreationConditionSchema['condition'])
-    operator = FieldProperty(IMacroCreationConditionSchema['operator'])
-    display_status = FieldProperty(IMacroCreationConditionSchema['display_status'])
+    condition = FieldProperty(IMacroCreationConditionSchema["condition"])
+    operator = FieldProperty(IMacroCreationConditionSchema["operator"])
+    display_status = FieldProperty(IMacroCreationConditionSchema["display_status"])
 
 
 class MacroCreationConditionAdapter(FactoryAdapter):
     factory = MacroCreationConditionObject
 
 
 class MacroStartConditionObject(BaseConditionObject):
     implements(IMacroStartConditionSchema)
 
-    condition = FieldProperty(IMacroStartConditionSchema['condition'])
-    operator = FieldProperty(IMacroStartConditionSchema['operator'])
-    display_status = FieldProperty(IMacroStartConditionSchema['display_status'])
+    condition = FieldProperty(IMacroStartConditionSchema["condition"])
+    operator = FieldProperty(IMacroStartConditionSchema["operator"])
+    display_status = FieldProperty(IMacroStartConditionSchema["display_status"])
 
 
 class MacroStartConditionAdapter(FactoryAdapter):
     factory = MacroStartConditionObject
 
 
 class MacroEndConditionObject(BaseConditionObject):
     implements(IMacroEndConditionSchema)
 
-    condition = FieldProperty(IMacroEndConditionSchema['condition'])
-    operator = FieldProperty(IMacroEndConditionSchema['operator'])
-    display_status = FieldProperty(IMacroEndConditionSchema['display_status'])
+    condition = FieldProperty(IMacroEndConditionSchema["condition"])
+    operator = FieldProperty(IMacroEndConditionSchema["operator"])
+    display_status = FieldProperty(IMacroEndConditionSchema["display_status"])
 
 
 class MacroEndConditionAdapter(FactoryAdapter):
     factory = MacroEndConditionObject
 
 
 class MacroFreezeConditionObject(BaseConditionObject):
     implements(IMacroFreezeConditionSchema)
 
-    condition = FieldProperty(IMacroFreezeConditionSchema['condition'])
-    operator = FieldProperty(IMacroFreezeConditionSchema['operator'])
-    display_status = FieldProperty(IMacroFreezeConditionSchema['display_status'])
+    condition = FieldProperty(IMacroFreezeConditionSchema["condition"])
+    operator = FieldProperty(IMacroFreezeConditionSchema["operator"])
+    display_status = FieldProperty(IMacroFreezeConditionSchema["display_status"])
 
 
 class MacroFreezeConditionAdapter(FactoryAdapter):
     factory = MacroFreezeConditionObject
 
 
 class MacroThawConditionObject(BaseConditionObject):
     implements(IMacroThawConditionSchema)
 
-    condition = FieldProperty(IMacroThawConditionSchema['condition'])
-    operator = FieldProperty(IMacroThawConditionSchema['operator'])
-    display_status = FieldProperty(IMacroThawConditionSchema['display_status'])
+    condition = FieldProperty(IMacroThawConditionSchema["condition"])
+    operator = FieldProperty(IMacroThawConditionSchema["operator"])
+    display_status = FieldProperty(IMacroThawConditionSchema["display_status"])
 
 
 class MacroThawConditionAdapter(FactoryAdapter):
     factory = MacroThawConditionObject
 
 
 class RecurrenceConditionObject(BaseConditionObject):
     implements(IRecurrenceConditionSchema)
 
-    condition = FieldProperty(IRecurrenceConditionSchema['condition'])
-    operator = FieldProperty(IRecurrenceConditionSchema['operator'])
-    display_status = FieldProperty(IRecurrenceConditionSchema['display_status'])
+    condition = FieldProperty(IRecurrenceConditionSchema["condition"])
+    operator = FieldProperty(IRecurrenceConditionSchema["operator"])
+    display_status = FieldProperty(IRecurrenceConditionSchema["display_status"])
 
 
 class RecurrenceConditionAdapter(FactoryAdapter):
     factory = RecurrenceConditionObject
 
 
 class MacroRecurrenceConditionObject(BaseConditionObject):
     implements(IMacroRecurrenceConditionSchema)
 
-    condition = FieldProperty(IMacroRecurrenceConditionSchema['condition'])
-    operator = FieldProperty(IMacroRecurrenceConditionSchema['operator'])
-    display_status = FieldProperty(IMacroRecurrenceConditionSchema['display_status'])
+    condition = FieldProperty(IMacroRecurrenceConditionSchema["condition"])
+    operator = FieldProperty(IMacroRecurrenceConditionSchema["operator"])
+    display_status = FieldProperty(IMacroRecurrenceConditionSchema["display_status"])
 
 
 class MacroRecurrenceConditionAdapter(FactoryAdapter):
     factory = MacroRecurrenceConditionObject
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/content/object_factories.zcml` & `imio.schedule-2.2.2/src/imio/schedule/content/object_factories.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/content/schedule_config.py` & `imio.schedule-2.2.2/src/imio/schedule/content/schedule_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 
 class IScheduleConfig(model.Schema):
     """
     ScheduleConfig dexterity schema.
     """
 
     enabled = schema.Bool(
-        title=_(u'Enabled'),
+        title=_(u"Enabled"),
         default=True,
         required=False,
     )
 
     scheduled_contenttype = schema.Choice(
-        title=_(u'Scheduled content type'),
-        description=_(u'Select the content type to apply schedule.'),
-        vocabulary='schedule.scheduled_contenttype',
+        title=_(u"Scheduled content type"),
+        description=_(u"Select the content type to apply schedule."),
+        vocabulary="schedule.scheduled_contenttype",
         required=True,
     )
 
 
 class ScheduleConfig(Container):
     """
     ScheduleConfig dexterity class.
@@ -46,45 +46,45 @@
         """
         return 0
 
     def query_task_configs(self, query={}):
         """
         Query the TaskConfig of this ScheduleConfig.
         """
-        catalog = api.portal.get_tool('portal_catalog')
-        config_path = '/'.join(self.getPhysicalPath())
+        catalog = api.portal.get_tool("portal_catalog")
+        config_path = "/".join(self.getPhysicalPath())
 
         base_query = {
-            'object_provides': ITaskConfig.__identifier__,
-            'path': {'query': config_path},
-            'sort_on': 'getObjPositionInParent',
+            "object_provides": ITaskConfig.__identifier__,
+            "path": {"query": config_path},
+            "sort_on": "getObjPositionInParent",
         }
 
         base_query.update(query)
 
         config_brains = catalog(**base_query)
 
         return config_brains
 
-    @cache(get_key=lambda m, schedule_cfg: schedule_cfg.id, get_request='self.REQUEST')
+    @cache(get_key=lambda m, schedule_cfg: schedule_cfg.id, get_request="self.REQUEST")
     def get_all_task_configs(self):
         """
         Return all the TaskConfig of this ScheduleConfig.
         """
         config_brains = self.query_task_configs()
-        with api.env.adopt_roles(['Manager']):
+        with api.env.adopt_roles(["Manager"]):
             task_configs = [brain.getObject() for brain in config_brains]
 
         return task_configs
 
     def get_scheduled_portal_type(self):
         """
         Return the portal_type of the selected scheduled_contenttype.
         """
-        return self.scheduled_contenttype and self.scheduled_contenttype[0] or ''
+        return self.scheduled_contenttype and self.scheduled_contenttype[0] or ""
 
     def get_scheduled_interfaces(self):
         """
         Return the registration interface of the selected scheduled_contenttype.
         """
         portal_type, interface_tuples = self.scheduled_contenttype
         if type(interface_tuples[0]) not in [list, tuple]:
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/content/subform_context_choice.py` & `imio.schedule-2.2.2/src/imio/schedule/content/subform_context_choice.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,35 +18,34 @@
     pass
 
 
 class SubFormContextChoice(schema.Choice):
     implements(ISubFormContextChoice)
 
     def __init__(self, *args, **kwargs):
-        kwargs['values'] = []
-        vocabulary_name = kwargs.pop('vocabulary')
+        kwargs["values"] = []
+        vocabulary_name = kwargs.pop("vocabulary")
         super(SubFormContextChoice, self).__init__(*args, **kwargs)
         self.vocabulary_name = vocabulary_name
 
 
 class SubFormContextSelectWidget(SelectWidget):
-
     def update(self):
         super(SubFormContextSelectWidget, self).update()
         self.field.vocabulary = self.terms.terms
 
 
 @adapter(ISubFormContextChoice, IFormLayer)
 @implementer(IFieldWidget)
 def subform_context_select_field_widget(field, request):
     return FieldWidget(field, SubFormContextSelectWidget(request))
 
 
 def subform_context_choice_terms(context, request, form, field, widget):
-    if hasattr(form, 'parentForm'):
+    if hasattr(form, "parentForm"):
         context = form.parentForm.context
     field = field.bind(context)
     voc = getUtility(IVocabularyFactory, name=field.vocabulary_name)
     return term.ChoiceTermsVocabulary(
         context,
         request,
         form,
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/content/task.py` & `imio.schedule-2.2.2/src/imio/schedule/content/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,39 +24,40 @@
 
 
 class IAutomatedTask(ITask):
     """
     AutomatedTask dexterity schema.
     """
 
-    directives.order_before(assigned_group='assigned_user')
-    directives.order_before(assigned_group='ITask.assigned_user')
+    directives.order_before(assigned_group="assigned_user")
+    directives.order_before(assigned_group="ITask.assigned_user")
     assigned_group = LocalRoleMasterSelectField(
         title=CTMF(u"Assigned group"),
         required=True,
         vocabulary="collective.task.AssignedGroups",
         slave_fields=(
-            {'name': 'ITask.assigned_user',
-             'slaveID': '#form-widgets-ITask-assigned_user',
-             'action': 'vocabulary',
-             'vocab_method': get_users_vocabulary,
-             'control_param': 'group',
-             },
+            {
+                "name": "ITask.assigned_user",
+                "slaveID": "#form-widgets-ITask-assigned_user",
+                "action": "vocabulary",
+                "vocab_method": get_users_vocabulary,
+                "control_param": "group",
+            },
         ),
-        defaultFactory=get_parent_assigned_group
+        defaultFactory=get_parent_assigned_group,
     )
 
 
 class BaseAutomatedTask(object):
     """
     Base class for AutomatedTask content types.
     """
 
-    task_config_UID = ''
-    schedule_config_UID = ''
+    task_config_UID = ""
+    schedule_config_UID = ""
 
     def get_container(self):
         """
         Return the task container.
         """
         container = self
         while IAutomatedTask.providedBy(container):
@@ -76,80 +77,74 @@
 
         return level
 
     def get_schedule_config(self):
         """
         Return associated schedule config.
         """
-        catalog = api.portal.get_tool('portal_catalog')
+        catalog = api.portal.get_tool("portal_catalog")
         brains = catalog(UID=self.schedule_config_UID)
         if brains:
             return brains[0].getObject()
         else:
-            raise ScheduleConfigNotFound(
-                'UID {}'.format(self.schedule_config_UID)
-            )
+            raise ScheduleConfigNotFound("UID {}".format(self.schedule_config_UID))
 
-    @cache(get_key=lambda m, task: task.id, get_request='self.REQUEST')
+    @cache(get_key=lambda m, task: task.id, get_request="self.REQUEST")
     def get_task_config(self):
         """
         Return associated task config.
         """
-        catalog = api.portal.get_tool('portal_catalog')
-        with api.env.adopt_roles(['Manager']):
+        catalog = api.portal.get_tool("portal_catalog")
+        with api.env.adopt_roles(["Manager"]):
             brains = catalog.unrestrictedSearchResults(UID=self.task_config_UID)
             if brains:
                 return brains[0].getObject()
             else:
-                raise TaskConfigNotFound(
-                    'UID {}'.format(self.task_config_UID)
-                )
+                raise TaskConfigNotFound("UID {}".format(self.task_config_UID))
 
     def get_status(self):
         """
         Return the status of the task
         """
         return status_by_state[self.get_state()]
 
-    @cache(get_key=lambda m, task: task.id, get_request='self.REQUEST')
+    @cache(get_key=lambda m, task: task.id, get_request="self.REQUEST")
     def start_conditions_status(self):
         """
         See start_conditions_status of TaskConfig.
         """
         task_config = self.get_task_config()
         container = self.get_container()
         status = task_config.start_conditions_status(container, self)
         return status
 
-    @cache(get_key=lambda m, task: task.id, get_request='self.REQUEST')
+    @cache(get_key=lambda m, task: task.id, get_request="self.REQUEST")
     def starting_states_status(self):
-        """
-        """
+        """ """
         config = self.get_task_config()
         starting_states = config.starting_states
         if not starting_states:
             return
 
         container = self.get_container()
         container_state = api.content.get_state(container)
         return (container_state, starting_states)
 
-    @cache(get_key=lambda m, task: task.id, get_request='self.REQUEST')
+    @cache(get_key=lambda m, task: task.id, get_request="self.REQUEST")
     def end_conditions_status(self):
         """
         See end_conditions_status of TaskConfig.
         """
         task_config = self.get_task_config()
         container = self.get_container()
         status = task_config.end_conditions_status(container, self)
         return status
 
     def ending_states_status(self):
-        """
-        """
+        """ """
         config = self.get_task_config()
         ending_states = config.ending_states
         if not ending_states:
             return
 
         container = self.get_container()
         container_state = api.content.get_state(container)
@@ -162,21 +157,20 @@
         """
         A normal task has no sub tasks.
         """
         return []
 
     @property
     def end_date(self):
-        """
-        """
+        """ """
         if self.get_status() == DONE:
-            wf_history = self.workflow_history['task_workflow'][::-1]
+            wf_history = self.workflow_history["task_workflow"][::-1]
             for action in wf_history:
-                if status_by_state[action['review_state']] is DONE:
-                    end_date = action['time']
+                if status_by_state[action["review_state"]] is DONE:
+                    end_date = action["time"]
                     return end_date.asdatetime()
         return None
 
     def reindex_parent_tasks(self, idxs=[]):
         """
         Reindex 'idxs' indexes of all the parent tasks of this task.
         """
@@ -209,15 +203,15 @@
         task_config.start_task(self)
 
     def _end(self):
         """
         Delegate end operation to the task_config
         """
         task_config = self.get_task_config()
-        with api.env.adopt_roles(['Manager']):
+        with api.env.adopt_roles(["Manager"]):
             task_config.end_task(self)
 
     def _freeze(self):
         """
         Delegate freeze operation to the task_config
         """
         task_config = self.get_task_config()
@@ -228,29 +222,27 @@
         Delegate thaw operation to the task_config
         """
         task_config = self.get_task_config()
         task_config.thaw_task(self)
 
 
 class AutomatedTask(Item, BaseAutomatedTask):
-    """
-    """
+    """ """
 
     implements(IAutomatedTask)
 
 
 class IAutomatedMacroTask(IAutomatedTask):
     """
     AutomatedTask dexterity schema.
     """
 
 
 class AutomatedMacroTask(Container, BaseAutomatedTask):
-    """
-    """
+    """ """
 
     implements(IAutomatedMacroTask)
 
     def get_subtasks(self):
         """
         Return all sub tasks of this macro task.
         """
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/content/task_config.py` & `imio.schedule-2.2.2/src/imio/schedule/content/task_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,415 +1,452 @@
 # -*- coding: utf-8 -*-
 
+from Products.CMFCore.Expression import Expression
+from Products.PageTemplates.Expressions import getEngine
 from datetime import date
 from datetime import datetime
 from dateutil.relativedelta import relativedelta
-
 from imio.schedule import _
 from imio.schedule.config import CREATION
 from imio.schedule.config import DONE
 from imio.schedule.config import FROZEN
 from imio.schedule.config import STARTED
 from imio.schedule.config import states_by_status
-from imio.schedule.content.task import IAutomatedTask
 from imio.schedule.content.subform_context_choice import SubFormContextChoice
+from imio.schedule.content.task import IAutomatedTask
+from imio.schedule.interfaces import ICalculationDelay
 from imio.schedule.interfaces import ICreationCondition
 from imio.schedule.interfaces import IDefaultEndingStates
 from imio.schedule.interfaces import IDefaultFreezeStates
 from imio.schedule.interfaces import IDefaultTaskGroup
 from imio.schedule.interfaces import IDefaultTaskUser
 from imio.schedule.interfaces import IDefaultThawStates
 from imio.schedule.interfaces import IEndCondition
 from imio.schedule.interfaces import IFreezeCondition
 from imio.schedule.interfaces import IFreezeDuration
 from imio.schedule.interfaces import IStartCondition
 from imio.schedule.interfaces import IThawCondition
 from imio.schedule.interfaces import TaskAlreadyExists
-from imio.schedule.interfaces import ICalculationDelay
-from imio.schedule.utils import round_to_weekday
 from imio.schedule.utils import WorkingDaysCalendar
-
+from imio.schedule.utils import round_to_weekday
 from plone import api
 from plone.dexterity.content import Container
 from plone.supermodel import model
-
 from zope import schema
 from zope.annotation import IAnnotations
 from zope.component import getMultiAdapter
 from zope.component import queryAdapter
 from zope.component import queryMultiAdapter
 from zope.component.interface import getInterface
-from zope.interface import alsoProvides
 from zope.interface import Interface
+from zope.interface import Invalid
+from zope.interface import alsoProvides
 from zope.interface import implements
+from zope.interface import invariant
+
+import logging
+
+
+logger = logging.getLogger("imio.schedule")
 
 
 class ICreationConditionSchema(Interface):
 
     condition = SubFormContextChoice(
-        title=_(u'Condition'),
-        vocabulary='schedule.creation_conditions',
+        title=_(u"Condition"),
+        vocabulary="schedule.creation_conditions",
         required=True,
     )
 
     operator = schema.Choice(
-        title=_(u'Operator'),
-        vocabulary='schedule.logical_operator',
-        default='AND',
+        title=_(u"Operator"),
+        vocabulary="schedule.logical_operator",
+        default="AND",
     )
 
     display_status = schema.Bool(
-        title=_(u'display_status'),
+        title=_(u"display_status"),
         default=True,
     )
 
 
 class IStartConditionSchema(Interface):
 
     condition = SubFormContextChoice(
-        title=_(u'Condition'),
-        vocabulary='schedule.start_conditions',
+        title=_(u"Condition"),
+        vocabulary="schedule.start_conditions",
         required=True,
     )
 
     operator = schema.Choice(
-        title=_(u'Operator'),
-        vocabulary='schedule.logical_operator',
-        default='AND',
+        title=_(u"Operator"),
+        vocabulary="schedule.logical_operator",
+        default="AND",
     )
 
     display_status = schema.Bool(
-        title=_(u'display_status'),
+        title=_(u"display_status"),
         default=True,
     )
 
 
 class IEndConditionSchema(Interface):
 
     condition = SubFormContextChoice(
-        title=_(u'Condition'),
-        vocabulary='schedule.end_conditions',
+        title=_(u"Condition"),
+        vocabulary="schedule.end_conditions",
         required=True,
     )
 
     operator = schema.Choice(
-        title=_(u'Operator'),
-        vocabulary='schedule.logical_operator',
-        default='AND',
+        title=_(u"Operator"),
+        vocabulary="schedule.logical_operator",
+        default="AND",
     )
 
     display_status = schema.Bool(
-        title=_(u'display_status'),
+        title=_(u"display_status"),
         default=True,
     )
 
 
 class IRecurrenceConditionSchema(Interface):
 
     condition = SubFormContextChoice(
-        title=_(u'Condition'),
-        vocabulary='schedule.creation_conditions',
+        title=_(u"Condition"),
+        vocabulary="schedule.creation_conditions",
         required=True,
     )
 
     operator = schema.Choice(
-        title=_(u'Operator'),
-        vocabulary='schedule.logical_operator',
-        default='AND',
+        title=_(u"Operator"),
+        vocabulary="schedule.logical_operator",
+        default="AND",
     )
 
     display_status = schema.Bool(
-        title=_(u'display_status'),
+        title=_(u"display_status"),
         default=True,
     )
 
 
 class IFreezeConditionSchema(Interface):
 
     condition = SubFormContextChoice(
-        title=_(u'Condition'),
-        vocabulary='schedule.freeze_conditions',
+        title=_(u"Condition"),
+        vocabulary="schedule.freeze_conditions",
         required=True,
     )
 
     operator = schema.Choice(
-        title=_(u'Operator'),
-        vocabulary='schedule.logical_operator',
-        default='AND',
+        title=_(u"Operator"),
+        vocabulary="schedule.logical_operator",
+        default="AND",
     )
 
     display_status = schema.Bool(
-        title=_(u'display_status'),
+        title=_(u"display_status"),
         default=True,
     )
 
 
 class IThawConditionSchema(Interface):
 
     condition = SubFormContextChoice(
-        title=_(u'Condition'),
-        vocabulary='schedule.thaw_conditions',
+        title=_(u"Condition"),
+        vocabulary="schedule.thaw_conditions",
         required=True,
     )
 
     operator = schema.Choice(
-        title=_(u'Operator'),
-        vocabulary='schedule.logical_operator',
-        default='AND',
+        title=_(u"Operator"),
+        vocabulary="schedule.logical_operator",
+        default="AND",
     )
 
     display_status = schema.Bool(
-        title=_(u'display_status'),
+        title=_(u"display_status"),
         default=True,
     )
 
 
 class ITaskConfig(model.Schema):
     """
     TaskConfig dexterity schema.
     """
 
     model.fieldset(
-        'general',
+        "general",
         label=_(u"General informations"),
         fields=[
-            'enabled', 'default_assigned_group',
-            'default_assigned_user', 'marker_interfaces'
-        ]
+            "enabled",
+            "default_assigned_group",
+            "default_assigned_user",
+            "marker_interfaces",
+        ],
     )
 
     enabled = schema.Bool(
-        title=_(u'Enabled'),
+        title=_(u"Enabled"),
         default=True,
         required=False,
     )
 
     default_assigned_group = schema.Choice(
-        title=_(u'Assigned group'),
-        description=_(u'Select default group assigned to this task.'),
-        vocabulary='schedule.assigned_group',
+        title=_(u"Assigned group"),
+        description=_(u"Select default group assigned to this task."),
+        vocabulary="schedule.assigned_group",
         required=False,
     )
 
     default_assigned_user = schema.Choice(
-        title=_(u'Assigned user'),
-        description=_(u'Select default user assigned to this task.'),
-        vocabulary='schedule.assigned_user',
+        title=_(u"Assigned user"),
+        description=_(u"Select default user assigned to this task."),
+        vocabulary="schedule.assigned_user",
         required=True,
     )
 
     marker_interfaces = schema.Set(
-        title=_(u'Marker interfaces'),
-        description=_(u'Custom marker interfaces for this task.'),
-        value_type=schema.Choice(source='schedule.task_marker_interfaces'),
+        title=_(u"Marker interfaces"),
+        description=_(u"Custom marker interfaces for this task."),
+        value_type=schema.Choice(source="schedule.task_marker_interfaces"),
         required=False,
     )
 
     model.fieldset(
-        'creation',
+        "creation",
         label=_(u"Creation"),
-        fields=['creation_state', 'creation_conditions']
+        fields=["creation_state", "creation_conditions"],
     )
 
     creation_state = schema.Set(
-        title=_(u'Task container creation state'),
-        description=_(u'Select the state of the container where the task is automatically created.'),
-        value_type=schema.Choice(source='schedule.container_state'),
+        title=_(u"Task container creation state"),
+        description=_(
+            u"Select the state of the container where the task is automatically created."
+        ),
+        value_type=schema.Choice(source="schedule.container_state"),
         required=False,
     )
 
     creation_conditions = schema.List(
-        title=_(u'Creation conditions'),
-        description=_(u'Select creation conditions of the task'),
+        title=_(u"Creation conditions"),
+        description=_(u"Select creation conditions of the task"),
         value_type=schema.Object(
-            title=_(u'Conditions'),
+            title=_(u"Conditions"),
             schema=ICreationConditionSchema,
         ),
         required=False,
     )
 
     model.fieldset(
-        'start',
-        label=_(u"Start"),
-        fields=['starting_states', 'start_conditions']
+        "start", label=_(u"Start"), fields=["starting_states", "start_conditions"]
     )
 
     starting_states = schema.Set(
-        title=_(u'Task container start states'),
-        description=_(u'Select the state of the container where the task is automatically started.'),
-        value_type=schema.Choice(source='schedule.container_state'),
+        title=_(u"Task container start states"),
+        description=_(
+            u"Select the state of the container where the task is automatically started."
+        ),
+        value_type=schema.Choice(source="schedule.container_state"),
         required=False,
     )
 
     start_conditions = schema.List(
-        title=_(u'Start conditions'),
-        description=_(u'Select start conditions of the task'),
+        title=_(u"Start conditions"),
+        description=_(u"Select start conditions of the task"),
         value_type=schema.Object(
-            title=_(u'Conditions'),
+            title=_(u"Conditions"),
             schema=IStartConditionSchema,
         ),
         required=False,
     )
 
     model.fieldset(
-        'ending',
-        label=_(u"Ending"),
-        fields=['ending_states', 'end_conditions']
+        "ending", label=_(u"Ending"), fields=["ending_states", "end_conditions"]
     )
 
     ending_states = schema.Set(
-        title=_(u'Task container end states'),
-        description=_(u'Select the states of the container where the task is automatically closed.'),
-        value_type=schema.Choice(source='schedule.container_state'),
+        title=_(u"Task container end states"),
+        description=_(
+            u"Select the states of the container where the task is automatically closed."
+        ),
+        value_type=schema.Choice(source="schedule.container_state"),
         required=False,
     )
 
     end_conditions = schema.List(
-        title=_(u'End conditions'),
-        description=_(u'Select end conditions of the task.'),
+        title=_(u"End conditions"),
+        description=_(u"Select end conditions of the task."),
         value_type=schema.Object(
-            title=_(u'Conditions'),
+            title=_(u"Conditions"),
             schema=IEndConditionSchema,
         ),
         required=False,
     )
 
     model.fieldset(
-        'delay',
-        label=_(u'Calculation delay'),
+        "delay",
+        label=_(u"Calculation delay"),
         fields=[
-            'start_date', 'warning_delay',
-            'calculation_delay', 'additional_delay', 'additional_delay_type',
-            'round_to_day'
+            "start_date",
+            "warning_delay",
+            "calculation_delay",
+            "additional_delay",
+            "additional_delay_tal",
+            "additional_delay_type",
+            "round_to_day",
         ],
     )
 
     start_date = schema.Choice(
-        title=_(u'Start date'),
-        description=_(u'Select the start date used to compute the due date.'),
-        vocabulary='schedule.start_date',
+        title=_(u"Start date"),
+        description=_(u"Select the start date used to compute the due date."),
+        vocabulary="schedule.start_date",
         required=True,
     )
 
     warning_delay = schema.Int(
-        title=_(u'Warning delay'),
+        title=_(u"Warning delay"),
         required=False,
     )
 
     calculation_delay = schema.List(
-        title=_(u'Calculation delay method'),
+        title=_(u"Calculation delay method"),
         value_type=schema.Choice(
-            title=_(u'Calculation delay'),
-            vocabulary='schedule.calculation_delay',
-            default='schedule.calculation_default_delay',
+            title=_(u"Calculation delay"),
+            vocabulary="schedule.calculation_delay",
+            default="schedule.calculation_default_delay",
         ),
         required=True,
     )
 
-    additional_delay = schema.Int(
-        title=_(u'Additional delay'),
-        description=_(u'This delay is added to the due date of the task.'),
+    additional_delay = schema.TextLine(
+        title=_(u"Additional delay"),
+        description=_(u"This delay is added to the due date of the task."),
         required=False,
-        default=0,
+        default=u"0",
     )
 
+    additional_delay_tal = schema.Bool(
+        title=_(u"Additional delay is a tal expression?"),
+        description=_(
+            u"Define if the additional delay should be interpreted as a tal expression"
+        ),
+        required=False,
+        default=False,
+    )
+
+    @invariant
+    def validate_additional_delay(task_config):
+        if task_config.additional_delay_tal is False:
+            try:
+                int(task_config.additional_delay)
+            except ValueError:
+                raise Invalid(_("The additional delay is not a valid integer"))
+
     additional_delay_type = schema.Choice(
-        title=_(u'Additional delay type'),
-        description=_(u'Define the calculation method for the additional delay'),
-        vocabulary='imio.schedule.additional_delay_type',
+        title=_(u"Additional delay type"),
+        description=_(u"Define the calculation method for the additional delay"),
+        vocabulary="imio.schedule.additional_delay_type",
         required=True,
     )
 
     round_to_day = schema.Choice(
-        title=_(u'Round to week day'),
-        vocabulary='schedule.vocabulary.week_days_rounding',
-        default='0',
+        title=_(u"Round to week day"),
+        vocabulary="schedule.vocabulary.week_days_rounding",
+        default="0",
         required=True,
     )
 
     model.fieldset(
-        'freeze',
-        label=_(u'Freeze'),
+        "freeze",
+        label=_(u"Freeze"),
         fields=[
-            'freeze_states',
-            'freeze_conditions',
+            "freeze_states",
+            "freeze_conditions",
         ],
     )
 
     freeze_states = schema.Set(
-        title=_(u'Task container freeze states'),
-        description=_(u'Select the states of the container where the task is automatically closed.'),
-        value_type=schema.Choice(source='schedule.container_state'),
+        title=_(u"Task container freeze states"),
+        description=_(
+            u"Select the states of the container where the task is automatically closed."
+        ),
+        value_type=schema.Choice(source="schedule.container_state"),
         required=False,
     )
 
     freeze_conditions = schema.List(
-        title=_(u'Freeze conditions'),
-        description=_(u'Select freeze conditions of the task.'),
+        title=_(u"Freeze conditions"),
+        description=_(u"Select freeze conditions of the task."),
         value_type=schema.Object(
-            title=_(u'Conditions'),
+            title=_(u"Conditions"),
             schema=IFreezeConditionSchema,
         ),
         required=False,
     )
 
     model.fieldset(
-        'thaw',
-        label=_(u'Thaw'),
+        "thaw",
+        label=_(u"Thaw"),
         fields=[
-            'thaw_states',
-            'thaw_conditions',
+            "thaw_states",
+            "thaw_conditions",
         ],
     )
 
     thaw_states = schema.Set(
-        title=_(u'Task container thaw states'),
-        description=_(u'Select the states of the container where the task is automatically closed.'),
-        value_type=schema.Choice(source='schedule.container_state'),
+        title=_(u"Task container thaw states"),
+        description=_(
+            u"Select the states of the container where the task is automatically closed."
+        ),
+        value_type=schema.Choice(source="schedule.container_state"),
         required=False,
     )
 
     thaw_conditions = schema.List(
-        title=_(u'Thaw conditions'),
-        description=_(u'Select thaw conditions of the task.'),
+        title=_(u"Thaw conditions"),
+        description=_(u"Select thaw conditions of the task."),
         value_type=schema.Object(
-            title=_(u'Conditions'),
+            title=_(u"Conditions"),
             schema=IThawConditionSchema,
         ),
         required=False,
     )
 
     model.fieldset(
-        'recurrence',
-        label=_(u'Recurrence'),
+        "recurrence",
+        label=_(u"Recurrence"),
         fields=[
-            'activate_recurrency',
-            'recurrence_states',
-            'recurrence_conditions',
+            "activate_recurrency",
+            "recurrence_states",
+            "recurrence_conditions",
         ],
     )
 
     activate_recurrency = schema.Bool(
-        title=_(u'Activate recurrency'),
+        title=_(u"Activate recurrency"),
         required=False,
         default=False,
     )
 
     recurrence_states = schema.Set(
-        title=_(u'Task container recurrence states'),
-        description=_(u'Select the state of the container where the task should be recurred'),
-        value_type=schema.Choice(source='schedule.container_state'),
+        title=_(u"Task container recurrence states"),
+        description=_(
+            u"Select the state of the container where the task should be recurred"
+        ),
+        value_type=schema.Choice(source="schedule.container_state"),
         required=False,
     )
 
     recurrence_conditions = schema.List(
-        title=_(u'Recurrence condition'),
-        description=_(u'Select recurrence conditions of the task.'),
+        title=_(u"Recurrence condition"),
+        description=_(u"Select recurrence conditions of the task."),
         value_type=schema.Object(
-            title=_('Conditions'),
+            title=_("Conditions"),
             schema=IRecurrenceConditionSchema,
         ),
         required=False,
     )
 
 
 class BaseTaskConfig(object):
@@ -439,15 +476,15 @@
     def get_schedule_config(self):
         """
         Return the parent ScheduleConfig.
         """
         from imio.schedule.content.schedule_config import IScheduleConfig
 
         context = self
-        while(not IScheduleConfig.providedBy(context)):
+        while not IScheduleConfig.providedBy(context):
             context = context.getParentNode()
 
         return context
 
     def get_scheduled_portal_type(self):
         """
         Return the portal_type of the selected scheduled_contenttype.
@@ -468,17 +505,15 @@
         """
         # the value could be either the name of an adapter to call or the id
         # of an existing group
         group_id = self.default_assigned_group
         # try to get the adapter named 'group_id'
         default_group = None
         assign_group = queryMultiAdapter(
-            (task_container, task),
-            IDefaultTaskGroup,
-            name=group_id
+            (task_container, task), IDefaultTaskGroup, name=group_id
         )
         if assign_group:
             default_group = assign_group.group_id()
 
         # if no group was found use group_id
         group_id = default_group or group_id
         return group_id
@@ -489,17 +524,15 @@
         """
         # the value could be either the name of an adapter to call or the id
         # of an existing user
         user_id = self.default_assigned_user
         # try to get the adapter named 'user_id'
         default_user = None
         assign_user = queryMultiAdapter(
-            (task_container, task),
-            IDefaultTaskUser,
-            name=user_id
+            (task_container, task), IDefaultTaskUser, name=user_id
         )
         if assign_user:
             default_user = assign_user.user_id()
 
         # if no user was found use user_id
         user_id = default_user or user_id
         return user_id
@@ -509,20 +542,23 @@
         Catalog query to return every AutomatedTask created
         from this TaskConfig contained in 'root_container'.
         """
         tasks = []
         to_explore = [root_container]
         while to_explore:
             current = to_explore.pop()
-            if IAutomatedTask.providedBy(current) and current.task_config_UID == self.UID():
+            if (
+                IAutomatedTask.providedBy(current)
+                and current.task_config_UID == self.UID()
+            ):
                 if not states:
                     tasks.append(current)
                 elif api.content.get_state(current) in states:
                     tasks.append(current)
-            if hasattr(current, 'objectValues'):
+            if hasattr(current, "objectValues"):
                 to_explore.extend(current.objectValues())
         tasks = sorted(tasks, key=lambda x: x.created())
         return tasks
 
     def get_task(self, task_container):
         """
         Return the unique AutomatedTask object created from this
@@ -534,54 +570,46 @@
 
     def get_created_task(self, task_container):
         """
         Return the unique AutomatedTask object created from this
         TaskConfig in 'task_container' if it exists and is not started yet..
         """
         tasks = self.get_task_instances(
-            task_container,
-            states=states_by_status[CREATION]
+            task_container, states=states_by_status[CREATION]
         )
         task_instance = tasks and tasks[0] or None
         return task_instance
 
     def get_started_task(self, task_container):
         """
         Return the unique AutomatedTask object created from this
         TaskConfig in 'task_container' if it exists and is started.
         """
         tasks = self.get_task_instances(
-            task_container,
-            states=states_by_status[STARTED]
+            task_container, states=states_by_status[STARTED]
         )
         task_instance = tasks and tasks[0] or None
         return task_instance
 
     def get_open_task(self, task_container):
         """
         Return the unique AutomatedTask object created from this
         TaskConfig in 'task_container' if it exists and is not closed yet.
         """
         states = states_by_status[CREATION] + states_by_status[STARTED]
-        tasks = self.get_task_instances(
-            task_container,
-            states=states
-        )
+        tasks = self.get_task_instances(task_container, states=states)
         task_instance = tasks and tasks[0] or None
         return task_instance
 
     def get_closed_tasks(self, task_container):
         """
         Return all the closed automatedTask objects created from this
         TaskConfig in 'task_container' .
         """
-        tasks = self.get_task_instances(
-            task_container,
-            states=states_by_status[DONE]
-        )
+        tasks = self.get_task_instances(task_container, states=states_by_status[DONE])
         return tasks
 
     def get_closed_task(self, task_container):
         """
         Return the unique AutomatedTask object created from this
         TaskConfig in 'task_container' if it exists and is closed.
         """
@@ -590,76 +618,67 @@
         return task_instance
 
     def get_frozen_task(self, task_container):
         """
         Return the unique AutomatedTask object created from this
         TaskConfig in 'task_container' if it exists and is frozen.
         """
-        tasks = self.get_task_instances(
-            task_container,
-            states=states_by_status[FROZEN]
-        )
+        tasks = self.get_task_instances(task_container, states=states_by_status[FROZEN])
         task_instance = tasks and tasks[0] or None
         return task_instance
 
     def task_already_exists(self, task_container):
         """
         Check if the task_container already has a task from this config.
         """
         return self.get_task_instances(task_container)
 
     def evaluate_conditions(self, conditions, to_adapt, interface):
-        """
-        """
+        """ """
         value = True
         for condition_object in conditions or []:
             value = self.evaluate_one_condition(
                 to_adapt=to_adapt,
                 interface=interface,
                 name=condition_object.condition,
             )
             operator = condition_object.operator
 
             # in these cases, its useless to evaluate further because:
             # TRUE or (... ) <=> TRUE
-            if operator == 'OR' and value is True:
+            if operator == "OR" and value is True:
                 return True
             # FALSE and (... ) <=> FALSE
-            elif operator == 'AND' and value is False:
+            elif operator == "AND" and value is False:
                 return False
             # else, just continue to loop to evaluate the rest of the expression because:
             # FALSE or (... ) <=> (... )
             # TRUE and (... ) <=> (... )
             # so only the remaining '(... )' expression is relevant
 
         # return the last value
         return value
 
     def evaluate_one_condition(self, to_adapt, interface, name):
-        """
-        """
-        condition = getMultiAdapter(
-            to_adapt,
-            interface=interface,
-            name=name
-        )
+        """ """
+        condition = getMultiAdapter(to_adapt, interface=interface, name=name)
         value = condition.evaluate() and True or False
         return value
 
     def get_conditions_status(self, conditions, to_adapt, interface):
         """
         Return two lists of all conditions status for a given task
         and task container.
         The first list is all the matched conditions, the second is
         all the unmatched conditions.
         """
         matched = []
         not_matched = []
         for condition_object in conditions or []:
-            if not getattr(condition_object, 'display_status', True):
+            if not getattr(condition_object, "display_status", True):
                 continue
             value = self.evaluate_one_condition(
                 to_adapt=to_adapt,
                 interface=interface,
                 name=condition_object.condition,
             )
             if value:
@@ -697,25 +716,23 @@
         # each conditions is matched?
         if not self.match_creation_conditions(task_container):
             return False
 
         return True
 
     def match_creation_state(self, task_container):
-        """
-        """
+        """ """
         if not self.creation_state:
             return True
 
         container_state = api.content.get_state(task_container)
         return container_state in (self.creation_state or [])
 
     def match_creation_conditions(self, task_container):
-        """
-        """
+        """ """
         return self.evaluate_conditions(
             conditions=self.creation_conditions,
             to_adapt=(task_container, self),
             interface=ICreationCondition,
         )
 
     def should_start_task(self, task_container, task):
@@ -737,25 +754,23 @@
 
         if not task.assigned_user:
             return False
 
         return True
 
     def match_starting_states(self, task_container):
-        """
-        """
+        """ """
         if not self.starting_states:
             return True
 
         container_state = api.content.get_state(task_container)
         return container_state in (self.starting_states or [])
 
     def match_start_conditions(self, task_container, task):
-        """
-        """
+        """ """
         return self.evaluate_conditions(
             conditions=self.start_conditions,
             to_adapt=(task_container, task),
             interface=IStartCondition,
         )
 
     def start_conditions_status(self, task_container, task):
@@ -787,30 +802,32 @@
 
         if not self.match_end_conditions(task_container, task):
             return False
 
         return True
 
     def match_ending_states(self, task_container):
-        """
-        """
+        """ """
         default_ending_states = queryAdapter(task_container, IDefaultEndingStates)
         default_ending_states = default_ending_states and default_ending_states() or []
 
-        ending_states = self.ending_states and list(default_ending_states) + list(self.ending_states) or []
+        ending_states = (
+            self.ending_states
+            and list(default_ending_states) + list(self.ending_states)
+            or []
+        )
 
         if not ending_states:
             return True
 
         container_state = api.content.get_state(task_container)
         return container_state in ending_states
 
     def match_end_conditions(self, task_container, task):
-        """
-        """
+        """ """
         return self.evaluate_conditions(
             conditions=self.end_conditions,
             to_adapt=(task_container, task),
             interface=IEndCondition,
         )
 
     def end_conditions_status(self, task_container, task):
@@ -846,26 +863,26 @@
 
         if not self.match_freeze_conditions(task_container, task):
             return False
 
         return True
 
     def match_freeze_states(self, task_container):
-        """
-        """
+        """ """
         default_freeze_states = queryAdapter(task_container, IDefaultFreezeStates)
         default_freeze_states = default_freeze_states and default_freeze_states() or []
-        freeze_states = list(default_freeze_states) + list(self.freeze_states or []) or []
+        freeze_states = (
+            list(default_freeze_states) + list(self.freeze_states or []) or []
+        )
 
         container_state = api.content.get_state(task_container)
         return container_state in freeze_states
 
     def match_freeze_conditions(self, task_container, task):
-        """
-        """
+        """ """
         return self.evaluate_conditions(
             conditions=self.freeze_conditions,
             to_adapt=(task_container, task),
             interface=IFreezeCondition,
         )
 
     def freeze_conditions_status(self, task_container, task):
@@ -899,26 +916,24 @@
 
         if not self.match_thaw_conditions(task_container, task):
             return False
 
         return True
 
     def match_thaw_states(self, task_container):
-        """
-        """
+        """ """
         default_thaw_states = queryAdapter(task_container, IDefaultThawStates)
         default_thaw_states = default_thaw_states and default_thaw_states() or []
         thaw_states = list(default_thaw_states) + list(self.thaw_states or []) or []
 
         container_state = api.content.get_state(task_container)
         return container_state in thaw_states
 
     def match_thaw_conditions(self, task_container, task):
-        """
-        """
+        """ """
         return self.evaluate_conditions(
             conditions=self.thaw_conditions,
             to_adapt=(task_container, task),
             interface=IThawCondition,
         )
 
     def thaw_conditions_status(self, task_container, task):
@@ -937,32 +952,31 @@
         depending on the recurrence condition
         """
         # schedule config should be enabled
         schedule_config = self.get_schedule_config()
         if not schedule_config.enabled:
             return False
 
-        if getattr(self, 'activate_recurrency', False) is False:
+        if getattr(self, "activate_recurrency", False) is False:
             return False
 
         if self.match_recurrence_states(task_container) is False:
             return False
 
-        if not getattr(self, 'recurrence_conditions', None):
+        if not getattr(self, "recurrence_conditions", None):
             return True
 
         return self.evaluate_conditions(
             conditions=self.recurrence_conditions,
             to_adapt=(task_container, self),
             interface=ICreationCondition,
         )
 
     def match_recurrence_states(self, task_container):
-        """
-        """
+        """ """
         if not self.recurrence_states:
             return True
 
         container_state = api.content.get_state(task_container)
         return container_state in (self.recurrence_states or [])
 
     def create_task(self, task_container):
@@ -970,119 +984,140 @@
         To implements in subclasses.
         """
 
     def start_task(self, task):
         """
         Default implementation is to put the task on the state 'to_do'.
         """
-        with api.env.adopt_roles(['Manager']):
-            if api.content.get_state(task) == 'created':
-                api.content.transition(obj=task, transition='do_to_assign')
-            if api.content.get_state(task) == 'to_assign' and task.assigned_user:
-                api.content.transition(obj=task, transition='do_to_do')
-        task.reindex_parent_tasks(idxs=['is_solvable_task'])
+        with api.env.adopt_roles(["Manager"]):
+            if api.content.get_state(task) == "created":
+                api.content.transition(obj=task, transition="do_to_assign")
+            if api.content.get_state(task) == "to_assign" and task.assigned_user:
+                api.content.transition(obj=task, transition="do_to_do")
+        task.reindex_parent_tasks(idxs=["is_solvable_task"])
 
     def end_task(self, task):
         """
         Default implementation is to put the task on the state 'closed'.
         """
-        if api.content.get_state(task) == 'created':
-            api.content.transition(obj=task, transition='do_to_assign')
-        if api.content.get_state(task) == 'to_assign':
-            api.content.transition(obj=task, transition='do_to_do')
-        if api.content.get_state(task) == 'to_do':
-            api.content.transition(obj=task, transition='do_realized')
-        if api.content.get_state(task) == 'realized':
-            with api.env.adopt_roles(['Reviewer']):
-                api.content.transition(obj=task, transition='do_closed')
-        task.reindex_parent_tasks(idxs=['is_solvable_task'])
+        if api.content.get_state(task) == "created":
+            api.content.transition(obj=task, transition="do_to_assign")
+        if api.content.get_state(task) == "to_assign":
+            api.content.transition(obj=task, transition="do_to_do")
+        if api.content.get_state(task) == "to_do":
+            api.content.transition(obj=task, transition="do_realized")
+        if api.content.get_state(task) == "realized":
+            with api.env.adopt_roles(["Reviewer"]):
+                api.content.transition(obj=task, transition="do_closed")
+        task.reindex_parent_tasks(idxs=["is_solvable_task"])
 
     def freeze_task(self, task):
         """
         Default implementation is to put the task on the state 'frozen'.
         """
         annotations = IAnnotations(task)
         freeze_infos = annotations.get(
-            'imio.schedule.freeze_task',
+            "imio.schedule.freeze_task",
             {
-                'freeze_date': None,
-                'previous_state': task.get_state(),
-                'previous_freeze_duration': 0
-            }
-        )
-        freeze_infos['freeze_date'] = str(datetime.now().date())
-        freeze_infos['freeze_state'] = task.get_state()
-        annotations['imio.schedule.freeze_task'] = freeze_infos
+                "freeze_date": None,
+                "previous_state": task.get_state(),
+                "previous_freeze_duration": 0,
+            },
+        )
+        freeze_infos["freeze_date"] = str(datetime.now().date())
+        freeze_infos["freeze_state"] = task.get_state()
+        annotations["imio.schedule.freeze_task"] = freeze_infos
 
-        portal_workflow = api.portal.get_tool('portal_workflow')
+        portal_workflow = api.portal.get_tool("portal_workflow")
         workflow_def = portal_workflow.getWorkflowsFor(task)[0]
         workflow_id = workflow_def.getId()
         workflow_state = portal_workflow.getStatusOf(workflow_id, task)
-        workflow_state['review_state'] = 'frozen'
+        workflow_state["review_state"] = "frozen"
         portal_workflow.setStatusOf(workflow_id, task, workflow_state.copy())
 
-        task.reindex_parent_tasks(idxs=['is_solvable_task'])
+        task.reindex_parent_tasks(idxs=["is_solvable_task"])
 
     def thaw_task(self, task):
         """
         Default implementation is to put the task on the state 'frozen'.
         """
 
         annotations = IAnnotations(task)
-        freeze_infos = annotations['imio.schedule.freeze_task']
+        freeze_infos = annotations["imio.schedule.freeze_task"]
         calculator = getMultiAdapter(
             (task.get_container(), task),
             interface=IFreezeDuration,
-            name='schedule.freeze_duration',
+            name="schedule.freeze_duration",
         )
         new_freeze_duration = calculator.freeze_duration
         new_freeze_infos = freeze_infos.copy()
-        new_freeze_infos['previous_freeze_duration'] = new_freeze_duration
-        annotations['imio.schedule.freeze_task'] = new_freeze_infos
+        new_freeze_infos["previous_freeze_duration"] = new_freeze_duration
+        annotations["imio.schedule.freeze_task"] = new_freeze_infos
 
-        portal_workflow = api.portal.get_tool('portal_workflow')
+        portal_workflow = api.portal.get_tool("portal_workflow")
         workflow_def = portal_workflow.getWorkflowsFor(task)[0]
         workflow_id = workflow_def.getId()
         workflow_state = portal_workflow.getStatusOf(workflow_id, task)
-        workflow_state['review_state'] = freeze_infos['previous_state']
+        workflow_state["review_state"] = freeze_infos["previous_state"]
         portal_workflow.setStatusOf(workflow_id, task, workflow_state.copy())
 
-        task.reindex_parent_tasks(idxs=['is_solvable_task'])
+        task.reindex_parent_tasks(idxs=["is_solvable_task"])
 
     def compute_due_date(self, task_container, task):
         """
         Evaluate 'task_container' and 'task' to compute the due date of a task.
         This should be checked in a zope event to automatically compute and set the
         due date of 'task'.
         """
-        adapters = getattr(self, 'calculation_delay', [])
+        adapters = getattr(self, "calculation_delay", [])
         # Backward compatibility
         if not adapters:
-            adapters = ['schedule.calculation_default_delay']
+            adapters = ["schedule.calculation_default_delay"]
         due_date = None
         for adapter in adapters:
             calculator = getMultiAdapter(
                 (task_container, task),
                 interface=ICalculationDelay,
                 name=adapter,
             )
             due_date = calculator.due_date
 
-        additional_delay = self.additional_delay or 0
-        delay_type = getattr(self, 'additional_delay_type', 'absolute')
-        if additional_delay and delay_type == 'working_days':
+        additional_delay = self.additional_delay or "0"
+        additional_delay_tal = getattr(self, "additional_delay_tal", False)
+        if additional_delay_tal is True:
+            data = {
+                "nothing": None,
+                "licence": task_container,
+                "task": task,
+                "request": getattr(task_container, "REQUEST", None),
+            }
+            ctx = getEngine().getContext(data)
+            try:
+                additional_delay = Expression(additional_delay)(ctx)
+            except Exception as e:
+                logger.warn(
+                    "The condition '%s' defined for element at '%s' is wrong!  Message is : %s"
+                    % (additional_delay, task.absolute_url(), e)
+                )
+                additional_delay = 0
+        else:
+            additional_delay = int(additional_delay)
+        delay_type = getattr(self, "additional_delay_type", "absolute")
+        if additional_delay and delay_type == "working_days":
             calendar = WorkingDaysCalendar()
             due_date = calendar.add_working_days(due_date, additional_delay)
         elif additional_delay:
             due_date = due_date + relativedelta(days=+additional_delay)
 
         annotations = IAnnotations(task)
-        freeze_infos = annotations.get('imio.schedule.freeze_task', None)
+        freeze_infos = annotations.get("imio.schedule.freeze_task", None)
         if freeze_infos:
-            due_date = due_date + relativedelta(days=+freeze_infos['previous_freeze_duration'])
+            due_date = due_date + relativedelta(
+                days=+freeze_infos["previous_freeze_duration"]
+            )
 
         round_day = int(self.round_to_day)
         if round_day:
             due_date = round_to_weekday(due_date, round_day)
 
         # frozen tasks have infinite due date
         if task.get_status() in FROZEN:
@@ -1094,49 +1129,52 @@
         """
         Helper method to use to implement 'create_task'.
         """
         if task_id in creation_place.objectIds():
             raise TaskAlreadyExists(task_id)
 
         task_portal_type = self.get_task_type()
-        portal_types = api.portal.get_tool('portal_types')
+        portal_types = api.portal.get_tool("portal_types")
         type_info = portal_types.getTypeInfo(task_portal_type)
 
         task = type_info._constructInstance(
             container=creation_place,
             id=task_id,
             title=self.Title(),
             schedule_config_UID=self.get_schedule_config().UID(),
             task_config_UID=self.UID(),
         )
 
-        marker_interfaces = [getInterface('', i) for i in self.marker_interfaces or []]
+        marker_interfaces = [getInterface("", i) for i in self.marker_interfaces or []]
         alsoProvides(task, *marker_interfaces)
 
         return task
 
     @property
     def default_task_id(self):
-        return 'TASK_{0}'.format(self.id)
+        return "TASK_{0}".format(self.id)
 
     def create_recurring_task(self, task_container, creation_place=None):
         """
         Create a recurring task
         """
         creation_place = creation_place or task_container
         object_ids = creation_place.objectIds()
-        related_ids = [i for i in object_ids
-                       if i.startswith(self.default_task_id)
-                       and creation_place[i].get_task_config() == self]
+        related_ids = [
+            i
+            for i in object_ids
+            if i.startswith(self.default_task_id)
+            and creation_place[i].get_task_config() == self
+        ]
         if len(related_ids) > 0:
             object_id = related_ids[-1]
-            if api.content.get_state(creation_place[object_id]) != 'closed':
+            if api.content.get_state(creation_place[object_id]) != "closed":
                 return
         if self.default_task_id in object_ids:
-            task_id = '{0}-{1}'.format(
+            task_id = "{0}-{1}".format(
                 self.default_task_id,
                 len(related_ids),
             )
         else:
             task_id = self.default_task_id
         return self.create_task(
             task_container,
@@ -1152,220 +1190,220 @@
 
     implements(ITaskConfig)
 
     def get_task_type(self):
         """
         Return the content type of task to create.
         """
-        return 'AutomatedTask'
+        return "AutomatedTask"
 
     def create_task(self, task_container, creation_place=None, task_id=None):
         """
         Just create the task and return it.
         """
         creation_place = creation_place or task_container
         task_id = task_id or self.default_task_id
         task = self._create_task_instance(creation_place, task_id)
 
         task.assigned_group = self.group_to_assign(task_container, task)
         task.assigned_user = self.user_to_assign(task_container, task)
         task.due_date = self.compute_due_date(task_container, task)
         task.reindexObject()
-        task.reindex_parent_tasks(idxs=['is_solvable_task'])
+        task.reindex_parent_tasks(idxs=["is_solvable_task"])
 
         return task
 
 
 class IMacroCreationConditionSchema(Interface):
 
     condition = SubFormContextChoice(
-        title=_(u'Condition'),
-        vocabulary='schedule.macrotask_creation_conditions',
+        title=_(u"Condition"),
+        vocabulary="schedule.macrotask_creation_conditions",
         required=True,
     )
 
     operator = schema.Choice(
-        title=_(u'Operator'),
-        vocabulary='schedule.logical_operator',
-        default='AND',
+        title=_(u"Operator"),
+        vocabulary="schedule.logical_operator",
+        default="AND",
     )
 
     display_status = schema.Bool(
-        title=_(u'display_status'),
+        title=_(u"display_status"),
         default=True,
     )
 
 
 class IMacroStartConditionSchema(Interface):
 
     condition = SubFormContextChoice(
-        title=_(u'Condition'),
-        vocabulary='schedule.macrotask_start_conditions',
+        title=_(u"Condition"),
+        vocabulary="schedule.macrotask_start_conditions",
         required=True,
     )
 
     operator = schema.Choice(
-        title=_(u'Operator'),
-        vocabulary='schedule.logical_operator',
-        default='AND',
+        title=_(u"Operator"),
+        vocabulary="schedule.logical_operator",
+        default="AND",
     )
 
     display_status = schema.Bool(
-        title=_(u'display_status'),
+        title=_(u"display_status"),
         default=True,
     )
 
 
 class IMacroEndConditionSchema(Interface):
 
     condition = SubFormContextChoice(
-        title=_(u'Condition'),
-        vocabulary='schedule.macrotask_end_conditions',
+        title=_(u"Condition"),
+        vocabulary="schedule.macrotask_end_conditions",
         required=True,
     )
 
     operator = schema.Choice(
-        title=_(u'Operator'),
-        vocabulary='schedule.logical_operator',
-        default='AND',
+        title=_(u"Operator"),
+        vocabulary="schedule.logical_operator",
+        default="AND",
     )
 
     display_status = schema.Bool(
-        title=_(u'display_status'),
+        title=_(u"display_status"),
         default=True,
     )
 
 
 class IMacroFreezeConditionSchema(Interface):
 
     condition = SubFormContextChoice(
-        title=_(u'Condition'),
-        vocabulary='schedule.macrotask_freeze_conditions',
+        title=_(u"Condition"),
+        vocabulary="schedule.macrotask_freeze_conditions",
         required=True,
     )
 
     operator = schema.Choice(
-        title=_(u'Operator'),
-        vocabulary='schedule.logical_operator',
-        default='AND',
+        title=_(u"Operator"),
+        vocabulary="schedule.logical_operator",
+        default="AND",
     )
 
     display_status = schema.Bool(
-        title=_(u'display_status'),
+        title=_(u"display_status"),
         default=True,
     )
 
 
 class IMacroThawConditionSchema(Interface):
 
     condition = SubFormContextChoice(
-        title=_(u'Condition'),
-        vocabulary='schedule.macrotask_thaw_conditions',
+        title=_(u"Condition"),
+        vocabulary="schedule.macrotask_thaw_conditions",
         required=True,
     )
 
     operator = schema.Choice(
-        title=_(u'Operator'),
-        vocabulary='schedule.logical_operator',
-        default='AND',
+        title=_(u"Operator"),
+        vocabulary="schedule.logical_operator",
+        default="AND",
     )
 
     display_status = schema.Bool(
-        title=_(u'display_status'),
+        title=_(u"display_status"),
         default=True,
     )
 
 
 class IMacroRecurrenceConditionSchema(Interface):
 
     condition = SubFormContextChoice(
-        title=_(u'Condition'),
-        vocabulary='schedule.macrotask_creation_conditions',
+        title=_(u"Condition"),
+        vocabulary="schedule.macrotask_creation_conditions",
         required=True,
     )
 
     operator = schema.Choice(
-        title=_(u'Operator'),
-        vocabulary='schedule.logical_operator',
-        default='AND',
+        title=_(u"Operator"),
+        vocabulary="schedule.logical_operator",
+        default="AND",
     )
 
     display_status = schema.Bool(
-        title=_(u'display_status'),
+        title=_(u"display_status"),
         default=True,
     )
 
 
 class IMacroTaskConfig(ITaskConfig):
     """
     TaskConfig dexterity schema.
     """
 
     start_date = schema.Choice(
-        title=_(u'Start date'),
-        description=_(u'Select the start date used to compute the due date.'),
-        vocabulary='schedule.macrotask_start_date',
+        title=_(u"Start date"),
+        description=_(u"Select the start date used to compute the due date."),
+        vocabulary="schedule.macrotask_start_date",
         required=True,
     )
 
     creation_conditions = schema.List(
-        title=_(u'Creation conditions'),
-        description=_(u'Select creation conditions of the task'),
+        title=_(u"Creation conditions"),
+        description=_(u"Select creation conditions of the task"),
         value_type=schema.Object(
-            title=_(u'Conditions'),
+            title=_(u"Conditions"),
             schema=IMacroCreationConditionSchema,
         ),
         required=False,
     )
 
     start_conditions = schema.List(
-        title=_(u'Start conditions'),
-        description=_(u'Select start conditions of the task'),
+        title=_(u"Start conditions"),
+        description=_(u"Select start conditions of the task"),
         value_type=schema.Object(
-            title=_(u'Conditions'),
+            title=_(u"Conditions"),
             schema=IMacroStartConditionSchema,
         ),
         required=False,
     )
 
     end_conditions = schema.List(
-        title=_(u'End conditions'),
-        description=_(u'Select end conditions of the task.'),
+        title=_(u"End conditions"),
+        description=_(u"Select end conditions of the task."),
         value_type=schema.Object(
-            title=_(u'Conditions'),
+            title=_(u"Conditions"),
             schema=IMacroEndConditionSchema,
         ),
         required=False,
     )
 
     freeze_conditions = schema.List(
-        title=_(u'Freeze conditions'),
-        description=_(u'Select freeze conditions of the task.'),
+        title=_(u"Freeze conditions"),
+        description=_(u"Select freeze conditions of the task."),
         value_type=schema.Object(
-            title=_(u'Conditions'),
+            title=_(u"Conditions"),
             schema=IMacroFreezeConditionSchema,
         ),
         required=False,
     )
 
     thaw_conditions = schema.List(
-        title=_(u'Thaw conditions'),
-        description=_(u'Select thaw conditions of the task.'),
+        title=_(u"Thaw conditions"),
+        description=_(u"Select thaw conditions of the task."),
         value_type=schema.Object(
-            title=_(u'Conditions'),
+            title=_(u"Conditions"),
             schema=IMacroThawConditionSchema,
         ),
         required=False,
     )
 
     recurrence_conditions = schema.List(
-        title=_(u'Recurrence condition'),
-        description=_(u'Select recurrence conditions of the task.'),
+        title=_(u"Recurrence condition"),
+        description=_(u"Select recurrence conditions of the task."),
         value_type=schema.Object(
-            title=_('Conditions'),
+            title=_("Conditions"),
             schema=IMacroRecurrenceConditionSchema,
         ),
         required=False,
     )
 
 
 class MacroTaskConfig(Container, BaseTaskConfig):
@@ -1375,27 +1413,27 @@
 
     implements(IMacroTaskConfig)
 
     def get_task_type(self):
         """
         Return the content type of task to create.
         """
-        return 'AutomatedMacroTask'
+        return "AutomatedMacroTask"
 
     def get_subtask_configs(self):
         """
         Return all the subtasks configs of this macro task.
         """
-        catalog = api.portal.get_tool('portal_catalog')
-        config_path = '/'.join(self.getPhysicalPath())
+        catalog = api.portal.get_tool("portal_catalog")
+        config_path = "/".join(self.getPhysicalPath())
 
         query = {
-            'object_provides': ITaskConfig.__identifier__,
-            'path': {'query': config_path, 'depth': 1},
-            'sort_on': 'getObjPositionInParent',
+            "object_provides": ITaskConfig.__identifier__,
+            "path": {"query": config_path, "depth": 1},
+            "sort_on": "getObjPositionInParent",
         }
 
         config_brains = catalog(**query)
         subtask_configs = [brain.getObject() for brain in config_brains]
 
         return subtask_configs
 
@@ -1430,36 +1468,42 @@
          - If all the subtasks are ended.
         This should be checked in a zope event to automatically close a task.
         """
         task_done = super(MacroTaskConfig, self).should_end_task(task_container, task)
         if not task_done:
             return False
 
-        subtasks_done = all([subtask.get_status() == DONE for subtask in task.get_subtasks()])
+        subtasks_done = all(
+            [subtask.get_status() == DONE for subtask in task.get_subtasks()]
+        )
         if not subtasks_done:
             return False
 
         return True
 
     def freeze_task(self, task):
         """
         Default implementation is to put the task  and all its subtasks on the
         state 'frozen'.
         """
-        subtasks_to_freeze = [tsk for tsk in task.get_subtasks() if tsk.get_status() not in [FROZEN, DONE]]
+        subtasks_to_freeze = [
+            tsk for tsk in task.get_subtasks() if tsk.get_status() not in [FROZEN, DONE]
+        ]
         for subtask in subtasks_to_freeze:
             subtask_config = subtask.get_task_config()
             subtask_config.freeze_task(subtask)
 
         super(MacroTaskConfig, self).freeze_task(task)
 
     def thaw_task(self, task):
         """
         Default implementation is to resume the task and all its subtasks on their
         previous state.
         """
-        subtasks_to_thaw = [tsk for tsk in task.get_subtasks() if tsk.get_status() == FROZEN]
+        subtasks_to_thaw = [
+            tsk for tsk in task.get_subtasks() if tsk.get_status() == FROZEN
+        ]
         for subtask in subtasks_to_thaw:
             subtask_config = subtask.get_task_config()
             subtask_config.thaw_task(subtask)
 
         super(MacroTaskConfig, self).thaw_task(task)
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/content/vocabulary.py` & `imio.schedule-2.2.2/src/imio/schedule/content/vocabulary.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,16 +57,16 @@
 
     def get_portal_type(self, context):
         """
         Return the portal_type of the (future?) context.
         """
         request = context.REQUEST
         try:
-            add_view = request.get('PUBLISHED', request['PARENTS'][-1])
-            if hasattr(add_view, 'form_instance'):
+            add_view = request.get("PUBLISHED", request["PARENTS"][-1])
+            if hasattr(add_view, "form_instance"):
                 form = add_view.form_instance
                 portal_type = form.portal_type
             else:
                 form = add_view.context.form_instance
                 portal_type = form.portal_type
         except:
             portal_type = context.portal_type
@@ -74,15 +74,15 @@
         return portal_type
 
     def get_fti(self, context):
         """
         Return the fti of the (future?) context.
         """
         portal_type = self.get_portal_type(context)
-        portal_types = api.portal.get_tool('portal_types')
+        portal_types = api.portal.get_tool("portal_types")
         fti = portal_types.getTypeInfo(portal_type)
         return fti
 
 
 class ScheduledContentTypeVocabularyFactory(BaseVocabularyFactory):
     """
     Vocabulary factory for 'scheduled_contenttype' field.
@@ -124,17 +124,15 @@
 
         voc_terms = []
         content_types = self.content_types()
         message_factory = self.get_message_factory()
 
         for portal_type, interface in content_types.iteritems():
             key = self.to_vocabulary_key(portal_type, interface)
-            voc_terms.append(
-                SimpleTerm(key, key, message_factory(portal_type))
-            )
+            voc_terms.append(SimpleTerm(key, key, message_factory(portal_type)))
 
         vocabulary = SimpleVocabulary(voc_terms)
 
         return vocabulary
 
     def content_types(self):
         """
@@ -177,16 +175,17 @@
         gsm = getGlobalSiteManager()
         scheduled_interfaces = context.get_scheduled_interfaces()
 
         voc_terms = []
         for scheduled_interface in scheduled_interfaces:
             for adapter in gsm.registeredAdapters():
                 implements_IGroup = adapter.provided is IDefaultTaskGroup
-                specific_enough = adapter.required[0].implementedBy(scheduled_interface) or \
-                    issubclass(scheduled_interface, adapter.required[0])
+                specific_enough = adapter.required[0].implementedBy(
+                    scheduled_interface
+                ) or issubclass(scheduled_interface, adapter.required[0])
                 if implements_IGroup and specific_enough:
                     voc_terms.append(
                         SimpleTerm(adapter.name, adapter.name, _(adapter.name))
                     )
 
         # enrich the vocabulary with available groups
         for group in api.group.get_groups():
@@ -211,28 +210,36 @@
         gsm = getGlobalSiteManager()
         scheduled_interfaces = context.get_scheduled_interfaces()
 
         voc_terms = []
         for scheduled_interface in scheduled_interfaces:
             for adapter in gsm.registeredAdapters():
                 implements_IUser = adapter.provided is IDefaultTaskUser
-                specific_enough = adapter.required[0].implementedBy(scheduled_interface) or \
-                    issubclass(scheduled_interface, adapter.required[0])
+                specific_enough = adapter.required[0].implementedBy(
+                    scheduled_interface
+                ) or issubclass(scheduled_interface, adapter.required[0])
                 if implements_IUser and specific_enough:
                     voc_terms.append(
                         SimpleTerm(adapter.name, adapter.name, _(adapter.name))
                     )
 
         # enrich the vocabulary with available users
         for user in api.user.get_users():
             voc_terms.append(
-                SimpleTerm(user.id, user.id, user.getProperty('fullname') or user.getUserName())
+                SimpleTerm(
+                    user.id, user.id, user.getProperty("fullname") or user.getUserName()
+                )
             )
 
-        vocabulary = SimpleVocabulary(sorted(unify_vocabularies(voc_terms), key=lambda term: term.title.decode('utf-8')))
+        vocabulary = SimpleVocabulary(
+            sorted(
+                unify_vocabularies(voc_terms),
+                key=lambda term: term.title.decode("utf-8"),
+            )
+        )
         return vocabulary
 
 
 class ContainerStateVocabularyFactory(object):
     """
     Vocabulary factory for 'container_state' field.
     """
@@ -242,20 +249,22 @@
         Call the adapter vocabulary for the 'container_state' field
         and returns it.
         """
         portal_type = context.get_scheduled_portal_type()
         if not portal_type:
             return SimpleVocabulary([])
 
-        wf_tool = api.portal.get_tool('portal_workflow')
+        wf_tool = api.portal.get_tool("portal_workflow")
         request = api.portal.get().REQUEST
 
         workfow = wf_tool.get(wf_tool.getChainForPortalType(portal_type)[0])
         voc_terms = [
-            SimpleTerm(state_id, state_id, translate(state.title, 'plone', context=request))
+            SimpleTerm(
+                state_id, state_id, translate(state.title, "plone", context=request)
+            )
             for state_id, state in workfow.states.items()
         ]
 
         vocabulary = SimpleVocabulary(voc_terms)
 
         return vocabulary
 
@@ -273,18 +282,18 @@
         for interface_name, marker_interface in interfaces:
             items.append(
                 SimpleTerm(
                     interface_name,
                     marker_interface.__doc__,
                     utranslate(
                         msgid=marker_interface.__doc__,
-                        domain='imio.schedule',
+                        domain="imio.schedule",
                         context=context,
-                        default=marker_interface.__doc__
-                    )
+                        default=marker_interface.__doc__,
+                    ),
                 )
             )
 
         # sort elements by title
         items.sort(lambda a, b: cmp(a.title, b.title))
 
         return SimpleVocabulary(items)
@@ -294,16 +303,24 @@
     """
     Return True/False vocabulary.
     """
 
     def __call__(self, context):
         request = api.portal.get().REQUEST
         items = [
-            SimpleTerm('True', 'True', translate('Doable alone', 'imio.schedule', context=request)),
-            SimpleTerm('False', 'False', translate('Subtasks dependencies', 'imio.schedule', context=request)),
+            SimpleTerm(
+                "True",
+                "True",
+                translate("Doable alone", "imio.schedule", context=request),
+            ),
+            SimpleTerm(
+                "False",
+                "False",
+                translate("Subtasks dependencies", "imio.schedule", context=request),
+            ),
         ]
 
         return SimpleVocabulary(items)
 
 
 class TaskLogicVocabularyFactory(object):
     """
@@ -322,18 +339,20 @@
         """
         gsm = getGlobalSiteManager()
         scheduled_interfaces = context.get_scheduled_interfaces()
 
         terms = []
         for scheduled_interface in scheduled_interfaces:
             for adapter in gsm.registeredAdapters():
-                implements_interface = issubclass(adapter.provided, ITaskLogic) and \
-                    issubclass(self.provides_interface, adapter.provided)
-                specific_enough = adapter.required[0].implementedBy(scheduled_interface) or \
-                    issubclass(scheduled_interface, adapter.required[0])
+                implements_interface = issubclass(
+                    adapter.provided, ITaskLogic
+                ) and issubclass(self.provides_interface, adapter.provided)
+                specific_enough = adapter.required[0].implementedBy(
+                    scheduled_interface
+                ) or issubclass(scheduled_interface, adapter.required[0])
                 if implements_interface and specific_enough:
                     terms.append(
                         SimpleTerm(adapter.name, adapter.name, _(adapter.name))
                     )
 
         vocabulary = SimpleVocabulary(unify_vocabularies(terms))
         return vocabulary
@@ -394,22 +413,24 @@
 
 
 class RecurrenceConditionVocabularyFactory(TaskLogicVocabularyFactory):
     """
     Vocabulary factory for 'recurrence_conditions' field.
     Return recurrence conditions for a task config.
     """
+
     provides_interface = IRecurrenceCondition
 
 
 class CalculationDelayVocabularyFactory(TaskLogicVocabularyFactory):
     """
     Vocabulary factory for 'calculation_delay' field.
     Return calculation delay methods for a task config.
     """
+
     provides_interface = ICalculationDelay
 
 
 class MacroTaskCreationConditionVocabularyFactory(TaskLogicVocabularyFactory):
     """
     Vocabulary factory for 'creation_conditions' field.
     Return available creation conditions of a macro task config.
@@ -442,65 +463,66 @@
     Return start date of a macro task config.
     """
 
     provides_interface = IMacroTaskStartDate
 
 
 class LogicalOperatorVocabularyFactory(BaseVocabularyFactory):
-
     def __call__(self, context):
-        return dict_list_2_vocabulary([
-            {'AND': _(u'and')},
-            {'OR': _(u'or')},
-        ])
+        return dict_list_2_vocabulary(
+            [
+                {"AND": _(u"and")},
+                {"OR": _(u"or")},
+            ]
+        )
 
 
 class WeekDaysRoundingVocabulary(object):
-    """
-    """
+    """ """
 
     def __call__(self, context):
         raw_terms = [
-            ('0', '0', _('None')),
-            ('1', '1', _('Next Monday')),
-            ('2', '2', _('Next Tuesday')),
-            ('3', '3', _('Next Wednesday')),
-            ('4', '4', _('Next Thursday')),
-            ('5', '5', _('Next Friday')),
-            ('6', '6', _('Next Saturday')),
-            ('7', '7', _('Next Sunday')),
-            ('-1', '-1', _('Previous Monday')),
-            ('-2', '-2', _('Previous Tuesday')),
-            ('-3', '-3', _('Previous Wednesday')),
-            ('-4', '-4', _('Previous Thursday')),
-            ('-5', '-5', _('Previous Friday')),
-            ('-6', '-6', _('Previous Saturday')),
-            ('-7', '-7', _('Previous Sunday')),
+            ("0", "0", _("None")),
+            ("1", "1", _("Next Monday")),
+            ("2", "2", _("Next Tuesday")),
+            ("3", "3", _("Next Wednesday")),
+            ("4", "4", _("Next Thursday")),
+            ("5", "5", _("Next Friday")),
+            ("6", "6", _("Next Saturday")),
+            ("7", "7", _("Next Sunday")),
+            ("-1", "-1", _("Previous Monday")),
+            ("-2", "-2", _("Previous Tuesday")),
+            ("-3", "-3", _("Previous Wednesday")),
+            ("-4", "-4", _("Previous Thursday")),
+            ("-5", "-5", _("Previous Friday")),
+            ("-6", "-6", _("Previous Saturday")),
+            ("-7", "-7", _("Previous Sunday")),
         ]
         voc_terms = [SimpleTerm(*term) for term in raw_terms]
         vocabulary = SimpleVocabulary(voc_terms)
 
         return vocabulary
 
 
 class TaskOwnerSource(PrincipalSource):
-
     def __init__(self, context):
         super(TaskOwnerSource, self).__init__(context)
 
     def _search(self, id=None, exact_match=True):
         users = api.user.get_users(self.context.assigned_group)
         if id is not None:
-            return sorted([{'id': u.id} for u in users if u.id == id], key=lambda u_id: u_id['id'])
-        return sorted([{'id': u.id} for u in users], key=lambda u_id: u_id['id'])
+            return sorted(
+                [{"id": u.id} for u in users if u.id == id], key=lambda u_id: u_id["id"]
+            )
+        return sorted([{"id": u.id} for u in users], key=lambda u_id: u_id["id"])
 
 
 class TaskOwnerSourceBinder(object):
-    """Bind the principal source with either users or groups
-    """
+    """Bind the principal source with either users or groups"""
+
     implements(IContextSourceBinder)
 
     def __call__(self, context):
         return TaskOwnerSource(context)
 
 
 TaskOwnerVocabulary = TaskOwnerSourceBinder()
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/content/vocabulary.zcml` & `imio.schedule-2.2.2/src/imio/schedule/content/vocabulary.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/content/widget.zcml` & `imio.schedule-2.2.2/src/imio/schedule/content/widget.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/converter.py` & `imio.schedule-2.2.2/src/imio/schedule/converter.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/dashboard/columns.py` & `imio.schedule-2.2.2/src/imio/schedule/dashboard/columns.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,119 +20,122 @@
 from zope.interface import implements
 from zope.i18n import translate
 
 
 def due_date_extra_classes(due_date, review_state):
     extra_classes = ""
 
-    if review_state != 'closed' and due_date and due_date.year != 9999:
+    if review_state != "closed" and due_date and due_date.year != 9999:
         orange_limit = api.portal.get_registry_record(
-            'imio.schedule.interfaces.IDueDateSettings.color_orange_x_days_before_due_date',
-            default=None
+            "imio.schedule.interfaces.IDueDateSettings.color_orange_x_days_before_due_date",
+            default=None,
         )
         red_limit = api.portal.get_registry_record(
-            'imio.schedule.interfaces.IDueDateSettings.color_red_x_days_before_due_date',
-            default=None
+            "imio.schedule.interfaces.IDueDateSettings.color_red_x_days_before_due_date",
+            default=None,
         )
         if red_limit is not None and close_or_past_date(due_date, by_days=red_limit):
             extra_classes += " red_close_due_date"
-        elif orange_limit is not None and close_or_past_date(due_date, by_days=orange_limit):
+        elif orange_limit is not None and close_or_past_date(
+            due_date, by_days=orange_limit
+        ):
             extra_classes += " orange_close_due_date"
 
     return extra_classes
 
 
 class DueDateColumn(BaseColumn):
-    """ Due date column for schedule listings."""
+    """Due date column for schedule listings."""
 
     def renderCell(self, item):
         due_date = item.due_date
         if not due_date or due_date.year == 9999:
-            return u'\u221E'
+            return u"\u221E"
 
-        return due_date.strftime('%d/%m/%Y')
+        return due_date.strftime("%d/%m/%Y")
 
     def getCSSClasses(self, item):
         """Returns a CSS class specific to current content."""
         cssClasses = super(DueDateColumn, self).getCSSClasses(item)
 
         cssClasses["td"] += due_date_extra_classes(item.due_date, item.review_state)
 
         return cssClasses
 
 
 class AssignedUserColumn(BaseColumn):
-    """ display licence address in SearchResultTable """
+    """display licence address in SearchResultTable"""
 
     def renderCell(self, item):
         username = item.assigned_user
         groupname = item.assigned_group
 
         user = username and api.user.get(username)
-        username = user and user.getProperty('fullname').decode('utf-8') or username
+        username = user and user.getProperty("fullname").decode("utf-8") or username
         assigned = username
         if groupname:
             to_icon = queryAdapter(item, IToIcon)
             group = api.group.get(groupname)
             if to_icon:
                 icon_url = to_icon.get_icon_url()
                 groupname = '<img src="{}">'.format(icon_url)
             else:
-                groupname = group and group.getProperty('title').decode('utf-8') or groupname
-                groupname = '({})'.format(groupname)
+                groupname = (
+                    group and group.getProperty("title").decode("utf-8") or groupname
+                )
+                groupname = "({})".format(groupname)
 
-            assigned = u'{user} {group}'.format(
-                user=username,
-                group=groupname
-            )
+            assigned = u"{user} {group}".format(user=username, group=groupname)
 
         return assigned
 
 
 class StatusColum(BaseColumn):
     """
     Column displaying the status of the tasks and its subtasks if it has any.
     """
+
     implements(IStatusColumn)
 
     sort_index = -1
     display_status_interface = IDisplayTaskStatus
     escape = False
 
     def renderHeadCell(self):
         """Override rendering of head of the cell to include jQuery
-           call to initialize annexes menu and to show the 'more/less details' if we are listing items."""
+        call to initialize annexes menu and to show the 'more/less details' if we are listing items."""
         # activate necessary javascripts
         if not self.header_js:
             # avoid problems while concataining None and unicode
-            self.header_js = u''
-        self.header_js += u'<script type="text/javascript">' + \
-            u'$("#task_status a").prepOverlay({subtype: "ajax"});' + \
-            '</script>'
+            self.header_js = u""
+        self.header_js += (
+            u'<script type="text/javascript">'
+            + u'$("#task_status a").prepOverlay({subtype: "ajax"});'
+            + "</script>"
+        )
         return super(StatusColum, self).renderHeadCell()
 
     def renderCell(self, item):
-        """
-        """
-        status = ''
+        """ """
+        status = ""
         task = item.getObject()
 
         adapter = queryMultiAdapter(
-            (self, task, api.portal.getRequest()),
-            self.display_status_interface
+            (self, task, api.portal.getRequest()), self.display_status_interface
         )
         if adapter:
             status = adapter.render()
         return status
 
 
 class SimpleStatusColumn(StatusColum):
     """
     Used for task listing on a single task container.
     """
+
     display_status_interface = ISimpleDisplayTaskStatus
 
 
 class SimpleTaskStatusDisplay(object):
     """
     Adpater, adapting a task and returning some html
     table cell displaying its status.
@@ -143,17 +146,18 @@
     def __init__(self, column, task, request):
         self.task = task
         self.request = request
 
     def render(self):
         task = self.task
         status = u'<span class="simple_task">&nbsp&nbsp&nbsp</span>'
-        link = '<a class="link-overlay" href="{task_url}/@@item_view">{status}</a>'.format(
-            task_url=task.absolute_url(),
-            status=status
+        link = (
+            '<a class="link-overlay" href="{task_url}/@@item_view">{status}</a>'.format(
+                task_url=task.absolute_url(), status=status
+            )
         )
         status_display = '<span id="task_status">{}</span>'.format(link)
         return status_display
 
 
 class TaskStatusDisplay(object):
     """
@@ -165,81 +169,84 @@
 
     def __init__(self, column, task, request):
         self.task = task
         self.request = request
 
     def render(self):
         task = self.task
-        return self.display_task_status(task, with_subtasks=IAutomatedMacroTask.providedBy(task))
+        return self.display_task_status(
+            task, with_subtasks=IAutomatedMacroTask.providedBy(task)
+        )
 
     def display_task_status(self, task, with_subtasks=False):
         """
         By default just put a code colour of the state of the task.
         """
-        css_class = 'schedule_{}'.format(api.content.get_state(task))
-        css_level = 'term-level-{}'.format(self.task.level())
+        css_class = "schedule_{}".format(api.content.get_state(task))
+        css_level = "term-level-{}".format(self.task.level())
         status = u'<span class="{css_level}"><span class="{css_class}">&nbsp&nbsp&nbsp</span></span>'.format(
             css_level=css_level,
             css_class=css_class,
         )
         if task.get_status() in [CREATION, STARTED]:
-            viewname = '{}{}_status'.format(
-                (not with_subtasks) and 'simple_' or '',
-                task.get_status() is CREATION and 'start' or 'end',
+            viewname = "{}{}_status".format(
+                (not with_subtasks) and "simple_" or "",
+                task.get_status() is CREATION and "start" or "end",
             )
             status = '<a class="link-overlay" href="{task_url}/@@{view}">{status}</a>'.format(
-                task_url=task.absolute_url(),
-                view=viewname,
-                status=status
+                task_url=task.absolute_url(), view=viewname, status=status
             )
         status = '<span id="task_status">{}</span>'.format(status)
         return status
 
 
 class MacroTaskStatusDisplay(TaskStatusDisplay):
     """
     Adapts a macro task and return some html table cell
     displaying the status of all subtasks that need to be done.
     """
 
     def render(self):
-        """
-        """
+        """ """
         all_subtasks = self.task.get_last_subtasks()
         subtasks_to_do = [task for task in all_subtasks if task.get_status() != DONE]
         if not subtasks_to_do:
             return self.display_task_status(self.task)
 
         rows = [
             u'<tr><th class="subtask_status_icon">{icon}</th>\
             <th i18n:translate="">{subtask}</th>\
             <th i18n:translate="">{due_date}</th></tr>'.format(
-                icon=self.display_task_status(self.task, with_subtasks=bool(subtasks_to_do)),
-                subtask=translate(_('Subtask'), context=self.request),
-                due_date=translate(_('Due date'), context=self.request),
+                icon=self.display_task_status(
+                    self.task, with_subtasks=bool(subtasks_to_do)
+                ),
+                subtask=translate(_("Subtask"), context=self.request),
+                due_date=translate(_("Due date"), context=self.request),
             ),
         ]
         for task in subtasks_to_do:
             title = task.Title()
             display_subtasks = IAutomatedMacroTask.providedBy(task)
             status_icon = u'<td class="subtask_status_icon">{status}</td>'.format(
                 status=self.display_task_status(task, with_subtasks=display_subtasks),
             )
             status_title = u'<td class="subtask_status_title">{title}</td>'.format(
-                title=title.decode('utf-8'),
+                title=title.decode("utf-8"),
             )
             date = task.due_date
-            due_date = date.year == 9999 and u'\u221E' or date.strftime('%d/%m/%Y')
+            due_date = date.year == 9999 and u"\u221E" or date.strftime("%d/%m/%Y")
             extra_css_classes = due_date_extra_classes(
                 task.due_date,
                 api.content.get_state(task),
             )
-            due_date = u'<td class="subtask_status_date{}">{}</td>'.format(extra_css_classes, due_date)
-            row = u'<tr>{icon}{title}{due_date}</tr>'.format(
-                icon=status_icon,
-                title=status_title,
-                due_date=due_date
+            due_date = u'<td class="subtask_status_date{}">{}</td>'.format(
+                extra_css_classes, due_date
+            )
+            row = u"<tr>{icon}{title}{due_date}</tr>".format(
+                icon=status_icon, title=status_title, due_date=due_date
             )
             rows.append(row)
 
-        status_display = u'<table class=subtask_status_table>{}</table>'.format(''.join(rows))
+        status_display = u"<table class=subtask_status_table>{}</table>".format(
+            "".join(rows)
+        )
         return status_display
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/dashboard/columns.zcml` & `imio.schedule-2.2.2/src/imio/schedule/dashboard/columns.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/dashboard/interfaces.py` & `imio.schedule-2.2.2/src/imio/schedule/dashboard/interfaces.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,24 +9,22 @@
 class IDisplayTaskStatus(Interface):
     """
     Adapts a task instance into a z3c table cell
     displaying the task status.
     """
 
     def render(self):
-        """
-        """
+        """ """
 
 
 class ISimpleDisplayTaskStatus(Interface):
     """
     Adapts a task instance into a z3c table cell
     displaying the task status.
     """
 
     def render(self):
-        """
-        """
+        """ """
 
 
 class IStatusColumn(IColumn):
-    """ Marker interface for Task Status columns."""
+    """Marker interface for Task Status columns."""
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/dashboard/vocabulary.py` & `imio.schedule-2.2.2/src/imio/schedule/dashboard/vocabulary.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,45 +12,41 @@
 class TaskWorkflowStates(object):
     """
     List all states of urban licence workflow.
     """
 
     def __call__(self, context):
 
-        states = ['created', 'to_do', 'closed']
+        states = ["created", "to_do", "closed"]
 
         vocabulary_terms = []
         for state in states:
             vocabulary_terms.append(
-                SimpleTerm(
-                    state,
-                    state,
-                    _(state, 'collective.task', context.REQUEST)
-                )
+                SimpleTerm(state, state, _(state, "collective.task", context.REQUEST))
             )
 
         vocabulary = SimpleVocabulary(vocabulary_terms)
         return vocabulary
 
 
 class TaskPortalTypes(object):
     """
     List all states of urban licence workflow.
     """
 
     def __call__(self, context):
 
-        portal_types = api.portal.get_tool('portal_types')
+        portal_types = api.portal.get_tool("portal_types")
         vocabulary_terms = []
 
         for task_type in task_types:
             p_type = portal_types[task_type]
             vocabulary_terms.append(
                 SimpleTerm(
                     task_type,
                     task_type,
-                    _(p_type.Title(), 'imio.schedule', context.REQUEST)
+                    _(p_type.Title(), "imio.schedule", context.REQUEST),
                 )
             )
 
         vocabulary = SimpleVocabulary(vocabulary_terms)
         return vocabulary
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/dashboard/vocabulary.zcml` & `imio.schedule-2.2.2/src/imio/schedule/dashboard/vocabulary.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/deserializer.py` & `imio.schedule-2.2.2/src/imio/schedule/deserializer.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/events/configure.zcml` & `imio.schedule-2.2.2/src/imio/schedule/events/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/events/create_task.py` & `imio.schedule-2.2.2/src/imio/schedule/events/create_task.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,34 +14,36 @@
     check the task config creations conditions and create the task if
     we can.
     """
 
     # This handler can be triggered for archetypes containers by the
     # workflow modification event but we want to create tasks only if
     # the container really exists (more than just created in portal_factory...)
-    if hasattr(aq_base(task_container), 'checkCreationFlag'):
+    if hasattr(aq_base(task_container), "checkCreationFlag"):
         if task_container.checkCreationFlag():
             return
 
     # descending=True <= it's important to create to macro tasks first
     task_configs = get_task_configs(task_container, descending=True)
 
     if not task_configs:
         return
 
-    with api.env.adopt_roles(['Manager']):
+    with api.env.adopt_roles(["Manager"]):
         for config in task_configs:
             if config.is_main_taskconfig():
                 if config.should_create_task(task_container):
                     try:
                         config.create_task(task_container)
                     except TaskAlreadyExists:
                         continue
             # case of a sub-task creation, the parent should have been created first
             else:
                 macro_config = config.getParentNode()
                 parent_task = macro_config.get_open_task(task_container)
-                if parent_task and config.should_create_task(task_container, parent_container=parent_task):
+                if parent_task and config.should_create_task(
+                    task_container, parent_container=parent_task
+                ):
                     try:
                         config.create_task(task_container, creation_place=parent_task)
                     except TaskAlreadyExists:
                         continue
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/events/dashboard_collection.py` & `imio.schedule-2.2.2/src/imio/schedule/events/dashboard_collection.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,78 +6,81 @@
 
 from plone import api
 
 from zope.interface import alsoProvides
 
 
 def create(schedule_container, event):
-    """
-    """
-    #do not automatically re-create the collection during upgrade steps
-    if 'portal_setup/manage_importSteps' in schedule_container.REQUEST.URL:
+    """ """
+    # do not automatically re-create the collection during upgrade steps
+    if "portal_setup/manage_importSteps" in schedule_container.REQUEST.URL:
         return
 
-    collection_id = 'dashboard_collection'
-    title = IScheduleConfig.providedBy(schedule_container) and _('All') or schedule_container.Title()
+    collection_id = "dashboard_collection"
+    title = (
+        IScheduleConfig.providedBy(schedule_container)
+        and _("All")
+        or schedule_container.Title()
+    )
 
     if collection_id not in schedule_container.objectIds():
         factory_args = {
-            'id': 'dashboard_collection',
-            'title': title,
-            'query': [
+            "id": "dashboard_collection",
+            "title": title,
+            "query": [
                 {
-                    'i': 'CompoundCriterion',
-                    'o': 'plone.app.querystring.operation.compound.is',
-                    'v': schedule_container.UID()
+                    "i": "CompoundCriterion",
+                    "o": "plone.app.querystring.operation.compound.is",
+                    "v": schedule_container.UID(),
                 },
                 {
-                    'i': 'review_state',
-                    'o': 'plone.app.querystring.operation.selection.is',
-                    'v': ['to_do']
-                }
+                    "i": "review_state",
+                    "o": "plone.app.querystring.operation.selection.is",
+                    "v": ["to_do"],
+                },
             ],
-            'customViewFields': (
-                u'assigned_user',
-                u'status',
-                u'due_date'
-            ),
-            'sort_on': u'due_date',
-            'sort_reversed': True,
-            'b_size': 30
+            "customViewFields": (u"assigned_user", u"status", u"due_date"),
+            "sort_on": u"due_date",
+            "sort_reversed": True,
+            "b_size": 30,
         }
 
         if IScheduleConfig.providedBy(schedule_container):
-            factory_args['customViewFields'] = (
-                u'pretty_link',
-                u'sortable_title',
-                u'assigned_user',
-                u'status',
-                u'due_date'
+            factory_args["customViewFields"] = (
+                u"pretty_link",
+                u"sortable_title",
+                u"assigned_user",
+                u"status",
+                u"due_date",
             )
 
         kwargs = {}
-        additional_queries = kwargs.pop('query', [])
+        additional_queries = kwargs.pop("query", [])
         for query in additional_queries:
-            factory_args['query'].append(query)
+            factory_args["query"].append(query)
         factory_args.update(kwargs)
 
-        portal_types = api.portal.get_tool('portal_types')
-        type_info = portal_types.getTypeInfo('DashboardCollection')
+        portal_types = api.portal.get_tool("portal_types")
+        type_info = portal_types.getTypeInfo("DashboardCollection")
         collection = type_info._constructInstance(schedule_container, **factory_args)
         # mark the collection with an interface to to customize the render
         # term view of collection widget
         alsoProvides(collection, IScheduleCollection)
 
 
 def update_title(schedule_container, event):
     """
     Dashboard Collection title should always be the title of the parent task.
     """
     # do not automatically re-create the collection during upgrade steps
-    if 'portal_setup' in schedule_container.REQUEST.URL:
+    if "portal_setup" in schedule_container.REQUEST.URL:
         return
 
-    collection = getattr(schedule_container, 'dashboard_collection', None)
+    collection = getattr(schedule_container, "dashboard_collection", None)
     if collection:
-        title = IScheduleConfig.providedBy(schedule_container) and _('All') or schedule_container.Title()
+        title = (
+            IScheduleConfig.providedBy(schedule_container)
+            and _("All")
+            or schedule_container.Title()
+        )
         collection.title = title
-        collection.reindexObject(idxs=('Title', 'sortable_title'))
+        collection.reindexObject(idxs=("Title", "sortable_title"))
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/events/task_config.py` & `imio.schedule-2.2.2/src/imio/schedule/events/task_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,43 +13,49 @@
 
 
 def update_marker_interfaces(task_config, event):
     """
     When the 'marker_interfaces' field is updated, update the interface
     provided on all the tasks of this task config as well.
     """
-    catalog = api.portal.get_tool('portal_catalog')
+    catalog = api.portal.get_tool("portal_catalog")
 
-    vocname = ITaskConfig.get('marker_interfaces').value_type.vocabularyName
+    vocname = ITaskConfig.get("marker_interfaces").value_type.vocabularyName
     interfaces_voc = getUtility(IVocabularyFactory, vocname)(task_config)
-    marker_interfaces = dict([(i, getInterface('', i)) for i in interfaces_voc.by_value])
+    marker_interfaces = dict(
+        [(i, getInterface("", i)) for i in interfaces_voc.by_value]
+    )
 
     task_brains = catalog(
-        object_provides=IAutomatedTask.__identifier__,
-        task_config_UID=task_config.UID()
+        object_provides=IAutomatedTask.__identifier__, task_config_UID=task_config.UID()
     )
     sample_task = task_brains and task_brains[0].getObject() or None
 
     # verify if the update is needed
     do_update = False
     for interface_name, marker_interface in marker_interfaces.iteritems():
         is_provided = marker_interface.providedBy(sample_task)
         # new interface on the config but not present yet on the tasks => update
         if interface_name in (task_config.marker_interfaces or []) and not is_provided:
             do_update = True
             break
         # old interface on the tasks no longer present on the config => update
-        elif interface_name not in (task_config.marker_interfaces or []) and is_provided:
+        elif (
+            interface_name not in (task_config.marker_interfaces or []) and is_provided
+        ):
             do_update = True
             break
 
     if do_update:
         for task_brain in task_brains:
             task = task_brain.getObject()
 
-            for marker_interface_name, marker_interface in marker_interfaces.iteritems():
+            for (
+                marker_interface_name,
+                marker_interface,
+            ) in marker_interfaces.iteritems():
                 if marker_interface_name in task_config.marker_interfaces:
                     alsoProvides(task, marker_interface)
                 else:
                     noLongerProvides(task, marker_interface)
 
-            task.reindexObject(idxs=['object_provides'])
+            task.reindexObject(idxs=["object_provides"])
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/events/update_tasks.py` & `imio.schedule-2.2.2/src/imio/schedule/events/update_tasks.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,98 +6,96 @@
 
 from imio.schedule.interfaces import TaskAlreadyExists
 from imio.schedule.utils import get_task_configs
 from imio.schedule.utils import get_container_open_tasks
 
 
 class TaskEventHandler(object):
-
     def __init__(self, task_container, event):
         self.container = task_container
         self.event = event
 
         if self.is_created is False:
             return
 
         self.task_configs = get_task_configs(self.container)
         if not self.task_configs:
             return
 
-        with api.env.adopt_roles(['Manager']):
+        with api.env.adopt_roles(["Manager"]):
             self.handle()
 
     @property
     def is_created(self):
         """
         This event can be triggered for archetype containers after a workflow
         modification so we need to ensured that the container really exists
         (more than just created in portal_factory).
         """
-        if hasattr(aq_base(self.container), 'checkCreationFlag'):
+        if hasattr(aq_base(self.container), "checkCreationFlag"):
             if self.container.checkCreationFlag():
                 return False
         return True
 
     def handle(self):
-        """
-        """
+        """ """
         raise NotImplementedError
 
 
 def start_tasks(task_container, event):
     """
     Automatically start tasks matching start conditions of a given
     task container.
     """
 
     # This handler can be triggered for archetypes containers by the
     # workflow modification event but we want to create tasks only if
     # the container really exists (more than just created in portal_factory...)
-    if hasattr(aq_base(task_container), 'checkCreationFlag'):
+    if hasattr(aq_base(task_container), "checkCreationFlag"):
         if task_container.checkCreationFlag():
             return
 
     task_configs = get_task_configs(task_container)
 
     if not task_configs:
         return
 
-    with api.env.adopt_roles(['Manager']):
+    with api.env.adopt_roles(["Manager"]):
         for config in task_configs:
             task = config.get_created_task(task_container)
             if task and config.should_start_task(task_container, task):
                 # delegate the starting action to the config so different behaviors
                 # can be easily configured
                 config.start_task(task)
 
                 # update due date after the task has started, because some date
                 # computation can rely on the task starting date
                 task.due_date = config.compute_due_date(task_container, task)
-                task.reindexObject(idxs=('due_date',))
+                task.reindexObject(idxs=("due_date",))
 
 
 def end_tasks(task_container, event):
     """
     Automatically end tasks matching end conditions of a given
     task container.
     """
 
     # This handler can be triggered for archetypes containers by the
     # workflow modification event but we want to create tasks only if
     # the container really exists (more than just created in portal_factory...)
-    if hasattr(aq_base(task_container), 'checkCreationFlag'):
+    if hasattr(aq_base(task_container), "checkCreationFlag"):
         if task_container.checkCreationFlag():
             return
 
     task_configs = get_task_configs(task_container)
 
     if not task_configs:
         return
 
-    with api.env.adopt_roles(['Manager']):
+    with api.env.adopt_roles(["Manager"]):
         for config in task_configs:
             task = config.get_open_task(task_container)
             if task and config.should_end_task(task_container, task):
                 # delegate the closure action to the config so different behaviors
                 # can be easily configured
                 config.end_task(task)
 
@@ -107,96 +105,95 @@
     Automatically freeze tasks matching freeze conditions of a given
     task container.
     """
 
     # This handler can be triggered for archetypes containers by the
     # workflow modification event but we want to create tasks only if
     # the container really exists (more than just created in portal_factory...)
-    if hasattr(aq_base(task_container), 'checkCreationFlag'):
+    if hasattr(aq_base(task_container), "checkCreationFlag"):
         if task_container.checkCreationFlag():
             return
 
     task_configs = get_task_configs(task_container)
 
     if not task_configs:
         return
 
-    with api.env.adopt_roles(['Manager']):
+    with api.env.adopt_roles(["Manager"]):
         for config in task_configs:
             task = config.get_open_task(task_container)
             if task and config.should_freeze_task(task_container, task):
                 # delegate the freeze action to the config so different behaviors
                 # can be easily configured
                 config.freeze_task(task)
 
                 # update due date after the task has frozen
                 task.due_date = config.compute_due_date(task_container, task)
-                task.reindexObject(idxs=('due_date',))
+                task.reindexObject(idxs=("due_date",))
 
 
 def thaw_tasks(task_container, event):
     """
     Automatically thaw tasks matching thaw conditions of a given
     task container.
     """
 
     # This handler can be triggered for archetypes containers by the
     # workflow modification event but we want to create tasks only if
     # the container really exists (more than just created in portal_factory...)
-    if hasattr(aq_base(task_container), 'checkCreationFlag'):
+    if hasattr(aq_base(task_container), "checkCreationFlag"):
         if task_container.checkCreationFlag():
             return
 
     task_configs = get_task_configs(task_container)
 
     if not task_configs:
         return
 
-    with api.env.adopt_roles(['Manager']):
+    with api.env.adopt_roles(["Manager"]):
         for config in task_configs:
             task = config.get_frozen_task(task_container)
             if task and config.should_thaw_task(task_container, task):
                 # delegate the thaw action to the config so different behaviors
                 # can be easily configured
                 config.thaw_task(task)
 
                 # update due date after the task has thawed, because some date
                 # computation can rely on the task thawing date
                 task.due_date = config.compute_due_date(task_container, task)
-                task.reindexObject(idxs=('due_date',))
+                task.reindexObject(idxs=("due_date",))
 
 
 def update_due_date(task_container, event):
     """
     If the task_container has been modified, compute
     the due date again and update it on the task.
     """
 
     # This handler can be triggered for archetypes containers by the
     # workflow modification event but we want to create tasks only if
     # the container really exists (more than just created in portal_factory...)
-    if hasattr(aq_base(task_container), 'checkCreationFlag'):
+    if hasattr(aq_base(task_container), "checkCreationFlag"):
         if task_container.checkCreationFlag():
             return
 
     task_configs = get_task_configs(task_container)
 
     if not task_configs:
         return
 
-    with api.env.adopt_roles(['Manager']):
+    with api.env.adopt_roles(["Manager"]):
         for config in task_configs:
             task = config.get_open_task(task_container)
             if task:
                 task.due_date = config.compute_due_date(task_container, task)
-                task.reindexObject(idxs=('due_date',))
+                task.reindexObject(idxs=("due_date",))
 
 
 class UpdateRecurrenceHandler(TaskEventHandler):
-
     def handle(self):
         open_tasks = get_container_open_tasks(self.container)
         open_tasks_by_cfg_UIDs = dict([(t.task_config_UID, t) for t in open_tasks])
         for config in self.task_configs:
             if config.is_main_taskconfig():
                 has_open_task = config.UID() in open_tasks_by_cfg_UIDs.keys()
                 if not has_open_task and config.should_recurred(self.container):
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/events/zope_registration.py` & `imio.schedule-2.2.2/src/imio/schedule/events/zope_registration.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,144 +14,140 @@
 from zope.component import getGlobalSiteManager
 from zope.interface import Interface
 from zope.interface import implements
 
 
 import logging
 
-logger = logging.getLogger('schedule')
+logger = logging.getLogger("schedule")
 
 
 def subscribe_task_configs_for_content_type(task_config, event):
     """
     Register adapter returning 'task_config' to the interface
     of the content_type selected in the field 'task_container'.
     """
 
     gsm = getGlobalSiteManager()
     task_config_UID = task_config.UID()
 
     class TaskConfigSubscriber(object):
         """ """
+
         implements(IToTaskConfig)
 
         def __init__(self, context):
             """ """
             self.context = context
             self.task_config_UID = task_config_UID
 
         @property
         def task_config(self):
-            catalog = api.portal.get_tool('portal_catalog')
+            catalog = api.portal.get_tool("portal_catalog")
             brains = catalog.unrestrictedSearchResults(UID=self.task_config_UID)
             if brains:
                 task_config = brains[0].getObject()
                 return task_config
             else:
-                raise TaskConfigNotFound(
-                    'UID {}'.format(self.task_config_UID)
-                )
+                raise TaskConfigNotFound("UID {}".format(self.task_config_UID))
 
     registration_interfaces = task_config.get_scheduled_interfaces()
 
     for registration_interface in registration_interfaces:
         gsm.registerAdapter(
             factory=TaskConfigSubscriber,
             required=(registration_interface,),
             provided=IToTaskConfig,
-            name=task_config.UID()
+            name=task_config.UID(),
         )
         msg = "Registered IToTaskConfig adapter '{}' for {}".format(
-            task_config.Title(),
-            registration_interface
+            task_config.Title(), registration_interface
         )
         logger.info(msg)
 
 
 def unsubscribe_task_configs_for_content_type(task_config, event):
     """
     Unregister adapter returning 'task_config' to the interface
     of the content_type selected in the field 'task_container'.
     """
 
     gsm = getGlobalSiteManager()
     schedule_config = task_config.get_schedule_config()
 
-    previous_interfaces = getattr(schedule_config, '_scheduled_interface_', None)
+    previous_interfaces = getattr(schedule_config, "_scheduled_interface_", None)
     if previous_interfaces and type(previous_interfaces[0]) not in [list, tuple]:
         previous_interfaces = (previous_interfaces,)
     previous_interfaces = [tuple_to_interface(i) for i in previous_interfaces]
 
     for previous_interface in previous_interfaces:
         removed = gsm.unregisterAdapter(
             required=(previous_interface,),
             provided=IToTaskConfig,
-            name=task_config.UID()
+            name=task_config.UID(),
         )
         if removed:
             msg = "Unregistered IToTaskConfig adapter '{}' for {}".format(
-                task_config.Title(),
-                previous_interface
+                task_config.Title(), previous_interface
             )
             logger.info(msg)
 
 
 def update_task_configs_subscriptions(schedule_config, event):
     """
     When the scheduled_contenttype value of a ScheduleConfig is changed,
     we have to unregister all the adapters providing IToTaskConfig
     and register them again for the new selected content type.
     """
 
-    previous_interfaces = getattr(schedule_config, '_scheduled_interface_', None)
+    previous_interfaces = getattr(schedule_config, "_scheduled_interface_", None)
     new_interfaces = schedule_config.get_scheduled_interfaces()
     new_interfaces = tuple([interface_to_tuple(i) for i in new_interfaces])
 
     # if there were no previous values, just save it and return
     if not previous_interfaces:
-        setattr(schedule_config, '_scheduled_interface_', new_interfaces)
+        setattr(schedule_config, "_scheduled_interface_", new_interfaces)
         return
 
     # if the value did not change, do nothing
     if previous_interfaces == new_interfaces:
         return
 
     for task_config in schedule_config.get_all_task_configs():
         # unregister the IToTaskConfig adapter for the previous interface
         unsubscribe_task_configs_for_content_type(task_config, event)
         # register the new IToTaskConfig adapter for the new interface
         subscribe_task_configs_for_content_type(task_config, event)
 
     # replace the _schedule_interface_ attribute with the new value
-    setattr(schedule_config, '_scheduled_interface_', new_interfaces)
+    setattr(schedule_config, "_scheduled_interface_", new_interfaces)
 
 
 def register_schedule_collection_criterion(schedule_config, event):
     """
     Register adapter turning a schedule config into a collection
     criterion filtering all tasks from this schedule config.
     """
 
     gsm = getGlobalSiteManager()
     schedule_config_UID = schedule_config.UID()
 
     class FilterTasksCriterion(object):
-
         def __init__(self, context):
             self.context = context
 
         @property
         def query(self):
-            return {'schedule_config_UID': {'query': schedule_config_UID}}
+            return {"schedule_config_UID": {"query": schedule_config_UID}}
 
     gsm.registerAdapter(
         factory=FilterTasksCriterion,
         required=(Interface,),
         provided=ICompoundCriterionFilter,
-        name=schedule_config.UID()
+        name=schedule_config.UID(),
     )
     msg = "Registered schedule CollectionCriterion adapter '{}'".format(
         schedule_config.Title()
     )
     logger.info(msg)
 
 
@@ -162,15 +158,15 @@
     """
 
     gsm = getGlobalSiteManager()
 
     removed = gsm.unregisterAdapter(
         required=(Interface,),
         provided=ICompoundCriterionFilter,
-        name=schedule_config.UID()
+        name=schedule_config.UID(),
     )
     if removed:
         msg = "Unregistered schedule CollectionCriterion adapter '{}'".format(
             schedule_config.Title()
         )
         logger.info(msg)
 
@@ -181,46 +177,41 @@
     criterion filtering all tasks from this task config.
     """
 
     gsm = getGlobalSiteManager()
     task_config_UID = task_config.UID()
 
     class FilterTasksCriterion(object):
-
         def __init__(self, context):
             self.context = context
 
         @property
         def query(self):
-            return {'task_config_UID': {'query': task_config_UID}}
+            return {"task_config_UID": {"query": task_config_UID}}
 
     gsm.registerAdapter(
         factory=FilterTasksCriterion,
         required=(Interface,),
         provided=ICompoundCriterionFilter,
-        name=task_config.UID()
-    )
-    msg = "Registered task CollectionCriterion adapter '{}'".format(
-        task_config.Title()
+        name=task_config.UID(),
     )
+    msg = "Registered task CollectionCriterion adapter '{}'".format(task_config.Title())
     logger.info(msg)
 
 
 def unregister_task_collection_criterion(task_config, event):
     """
     Unregister adapter turning a task config into a collection
     criterion.
     """
 
     gsm = getGlobalSiteManager()
 
     removed = gsm.unregisterAdapter(
-        required=(Interface,),
-        provided=ICompoundCriterionFilter,
-        name=task_config.UID()
+        required=(Interface,), provided=ICompoundCriterionFilter, name=task_config.UID()
     )
     if removed:
         msg = "Unregistered task CollectionCriterion adapter '{}'".format(
             task_config.Title()
         )
         logger.info(msg)
 
@@ -235,23 +226,31 @@
         - collections criterions
         - tasks vocabulary of each ScheduleConfig
     when zope instance is started.
     """
     if site.id not in _registered_sites:
 
         # register task configs subscribers and task configs criterion
-        catalog = api.portal.get_tool('portal_catalog')
-        task_brains = catalog.unrestrictedSearchResults(object_provides=ITaskConfig.__identifier__)
-        all_task_configs = [site.unrestrictedTraverse(brain.getPath()) for brain in task_brains]
+        catalog = api.portal.get_tool("portal_catalog")
+        task_brains = catalog.unrestrictedSearchResults(
+            object_provides=ITaskConfig.__identifier__
+        )
+        all_task_configs = [
+            site.unrestrictedTraverse(brain.getPath()) for brain in task_brains
+        ]
 
         for task_config in all_task_configs:
             subscribe_task_configs_for_content_type(task_config, event)
             register_task_collection_criterion(task_config, event)
 
         # register schedule configs criterion and tasks vocabulary
-        schedule_brains = catalog.unrestrictedSearchResults(object_provides=IScheduleConfig.__identifier__)
-        all_schedule_configs = [site.unrestrictedTraverse(brain.getPath()) for brain in schedule_brains]
+        schedule_brains = catalog.unrestrictedSearchResults(
+            object_provides=IScheduleConfig.__identifier__
+        )
+        all_schedule_configs = [
+            site.unrestrictedTraverse(brain.getPath()) for brain in schedule_brains
+        ]
 
         for schedule_config in all_schedule_configs:
             register_schedule_collection_criterion(schedule_config, event)
 
         _registered_sites.add(site.id)
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/indexes.py` & `imio.schedule-2.2.2/src/imio/schedule/indexes.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/interfaces.py` & `imio.schedule-2.2.2/src/imio/schedule/interfaces.py`

 * *Files 3% similar despite different names*

```diff
@@ -217,18 +217,18 @@
         Return the icon url.
         """
 
 
 class ISettings(model.Schema):
 
     working_days = schema.List(
-        title=_(u'List of working days'),
+        title=_(u"List of working days"),
         value_type=schema.Choice(
-            title=_(u'Day'),
-            vocabulary='imio.schedule.working_days',
+            title=_(u"Day"),
+            vocabulary="imio.schedule.working_days",
         ),
         required=True,
     )
 
 
 class IDueDateSettings(Interface):
     """ """
@@ -247,19 +247,28 @@
         required=False,
         default=5,
         min=0,
     )
 
     @invariant
     def orange_is_before_red_invariant(data):
-        if data.color_orange_x_days_before_due_date is None or data.color_red_x_days_before_due_date is None:
+        if (
+            data.color_orange_x_days_before_due_date is None
+            or data.color_red_x_days_before_due_date is None
+        ):
             return
-        if data.color_orange_x_days_before_due_date < data.color_red_x_days_before_due_date:
+        if (
+            data.color_orange_x_days_before_due_date
+            < data.color_red_x_days_before_due_date
+        ):
             raise Invalid(
-                _(u"The orange value should be higher than the red one, as it is used as a first warning."))
+                _(
+                    u"The orange value should be higher than the red one, as it is used as a first warning."
+                )
+            )
 
 
 class ICalendarExtraHolidays(Interface):
     """Interface for extra holidays utility"""
 
     def get_holidays(self, year):
         """
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/locales/collective.eeafaceted.z3ctable.pot` & `imio.schedule-2.2.2/src/imio/schedule/locales/collective.eeafaceted.z3ctable.pot`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.mo` & `imio.schedule-2.2.2/src/imio/schedule/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.mo`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.po` & `imio.schedule-2.2.2/src/imio/schedule/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.po`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/locales/fr/LC_MESSAGES/imio.schedule.mo` & `imio.schedule-2.2.2/src/imio/schedule/locales/fr/LC_MESSAGES/imio.schedule.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2019-10-08 11:36+0000\n"
+"POT-Creation-Date: 2024-04-08 09:18+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
@@ -25,16 +25,19 @@
 
 msgid "Activate recurrency"
 msgstr "Tache récurente"
 
 msgid "Additional delay"
 msgstr "Délai supplémentaire"
 
+msgid "Additional delay is a tal expression?"
+msgstr "Le délai supplémentaire est une expression TAL?"
+
 msgid "Additional delay type"
-msgstr "Délai aditionnel"
+msgstr "Délai additionnel"
 
 msgid "All"
 msgstr "Tous"
 
 msgid "Assigned group"
 msgstr "Groupe responsable de la tâche"
 
@@ -55,14 +58,17 @@
 
 msgid "Calculation delay method"
 msgstr "Calcul du délai"
 
 msgid "Change the task owner"
 msgstr "Réassigner"
 
+msgid "Close task"
+msgstr "Fermer la tâche"
+
 msgid "Color due date in orange if it comes close to X days"
 msgstr "Souligner l'échéance en ORANGE quand elle a atteint X jours restants"
 
 msgid "Color due date in red if it comes close to X days"
 msgstr "Souligner l'échéance en ROUGE quand elle a atteint X jours restants"
 
 msgid "Condition"
@@ -82,14 +88,20 @@
 
 msgid "Custom marker interfaces for this task."
 msgstr "Interfaces marqueurs"
 
 msgid "Day"
 msgstr "Jour"
 
+msgid ""
+"Define if the additional delay should be interpreted as a tal expression"
+msgstr ""
+"Choississez si le délai additionnel doit être interpreté comme une "
+"expression TAL"
+
 msgid "Define the calculation method for the additional delay"
 msgstr "Choisissez la méthode de calcul du délai aditionnel"
 
 msgid "Doable alone"
 msgstr "Réalisable seul"
 
 msgid "Done"
@@ -300,14 +312,17 @@
 
 msgid "Subtasks dependencies"
 msgstr "Réalisation distribuée"
 
 msgid "Sunday"
 msgstr "Dimanche"
 
+msgid "Task Closed"
+msgstr "Tâche cloturée"
+
 msgid "Task configuration."
 msgstr "Configuration de tâche"
 
 msgid "Task container creation state"
 msgstr "État de création de la tâche"
 
 msgid "Task container end states"
@@ -330,14 +345,17 @@
 
 msgid "Thaw"
 msgstr "Dégel"
 
 msgid "Thaw conditions"
 msgstr "Conditions de dégel de la tâche"
 
+msgid "The additional delay is not a valid integer"
+msgstr "Le délai supplémentaire n'est pas un entier"
+
 msgid ""
 "The orange value should be higher than the red one, as it is used as a first "
 "warning."
 msgstr ""
 "La limite pour l'orange doit être supérieure à la rouge, car l'orange est "
 "utilisé comme premier avertissement."
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/locales/fr/LC_MESSAGES/imio.schedule.po` & `imio.schedule-2.2.2/src/imio/schedule/locales/fr/LC_MESSAGES/imio.schedule.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2019-10-08 11:36+0000\n"
+"POT-Creation-Date: 2024-04-08 09:18+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
@@ -20,141 +20,155 @@
 msgid " to one of the following states"
 msgstr " vers l'un des états suivants"
 
 #: ../vocabularies.py:32
 msgid "Absolute"
 msgstr "Absolue"
 
-#: ../content/task_config.py:390
+#: ../content/task_config.py:422
 msgid "Activate recurrency"
 msgstr "Tache récurente"
 
-#: ../content/task_config.py:307
+#: ../content/task_config.py:322
 msgid "Additional delay"
 msgstr "Délai supplémentaire"
 
-#: ../content/task_config.py:314
+#: ../content/task_config.py:329
+msgid "Additional delay is a tal expression?"
+msgstr "Le délai supplémentaire est une expression TAL?"
+
+#: ../content/task_config.py:346
 msgid "Additional delay type"
-msgstr "Délai aditionnel"
+msgstr "Délai additionnel"
 
-#: ../events/dashboard_collection.py:16
+#: ../events/dashboard_collection.py:20
 msgid "All"
 msgstr "Tous"
 
-#: ../content/task_config.py:185
+#: ../content/task_config.py:196
 msgid "Assigned group"
 msgstr "Groupe responsable de la tâche"
 
 msgid "Assigned to"
 msgstr "Assigné à"
 
-#: ../content/task_config.py:192
+#: ../content/task_config.py:203
 msgid "Assigned user"
 msgstr "Responsable de la tâche"
 
+#: ../profiles/default/types/AutomatedMacroTask.xml
 msgid "AutomatedMacroTask"
 msgstr "Macro-tâche configurable"
 
 #: ../profiles/default/types/AutomatedTask.xml
 msgid "AutomatedTask"
 msgstr "Tâche configurable"
 
-#: ../content/task_config.py:276
+#: ../content/task_config.py:287
 msgid "Calculation delay"
 msgstr "Calcul du délai"
 
-#: ../content/task_config.py:297
+#: ../content/task_config.py:312
 msgid "Calculation delay method"
 msgstr "Calcul du délai"
 
 #: ../browser/templates/task_change_owner.pt:15
 msgid "Change the task owner"
 msgstr "Réassigner"
 
-#: ../content/task_config.py:47
+#: ../browser/templates/close_task.pt:15
+msgid "Close task"
+msgstr "Fermer la tâche"
 
 #: ../interfaces.py:237
 msgid "Color due date in orange if it comes close to X days"
 msgstr "Souligner l'échéance en ORANGE quand elle a atteint X jours restants"
 
 #: ../interfaces.py:245
 msgid "Color due date in red if it comes close to X days"
 msgstr "Souligner l'échéance en ROUGE quand elle a atteint X jours restants"
+
+#: ../content/task_config.py:58
 msgid "Condition"
 msgstr "Condition"
 
-#: ../content/task_config.py:222
+#: ../content/task_config.py:233
 msgid "Conditions"
 msgstr "Conditions"
 
+#: ../browser/close_task.py:22
 #: ../browser/task_owner.py:28
 msgid "Confirm"
 msgstr "Confirmer"
 
-#: ../content/task_config.py:207
+#: ../content/task_config.py:218
 msgid "Creation"
 msgstr "Création"
 
-#: ../content/task_config.py:219
+#: ../content/task_config.py:230
 msgid "Creation conditions"
 msgstr "Conditions de création de la tâche"
 
-#: ../content/task_config.py:200
+#: ../content/task_config.py:211
 msgid "Custom marker interfaces for this task."
 msgstr "Interfaces marqueurs"
 
-#: ../interfaces.py:218
+#: ../interfaces.py:226
 msgid "Day"
 msgstr "Jour"
 
-#: ../content/task_config.py:315
+#: ../content/task_config.py:330
+msgid "Define if the additional delay should be interpreted as a tal expression"
+msgstr "Choississez si le délai additionnel doit être interpreté comme une expression TAL"
+
+#: ../content/task_config.py:347
 msgid "Define the calculation method for the additional delay"
 msgstr "Choisissez la méthode de calcul du délai aditionnel"
 
 msgid "Doable alone"
 msgstr "Réalisable seul"
 
 #: ../browser/templates/task_completion.pt:53
 msgid "Done"
 msgstr "Fait"
 
-#: ../dashboard/columns.py:187
+#: ../dashboard/columns.py:218
 msgid "Due date"
 msgstr "Échéance"
 
-#: ../content/schedule_config.py:21
-#: ../content/task_config.py:179
+#: ../content/schedule_config.py:23
+#: ../content/task_config.py:190
 msgid "Enabled"
 msgstr "Activé"
 
-#: ../content/task_config.py:265
+#: ../content/task_config.py:276
 msgid "End conditions"
 msgstr "Conditions de clôture"
 
-#: ../content/task_config.py:253
+#: ../content/task_config.py:264
 msgid "Ending"
 msgstr "Fin"
 
-#: ../content/task_config.py:329
+#: ../content/task_config.py:361
 msgid "Freeze"
 msgstr "Gel"
 
-#: ../content/task_config.py:344
+#: ../content/task_config.py:376
 msgid "Freeze conditions"
 msgstr "Conditions de gel"
 
 #: ../vocabularies.py:22
 msgid "Friday"
 msgstr "Vendredi"
 
-#: ../content/task_config.py:171
+#: ../content/task_config.py:182
 msgid "General informations"
 msgstr "Paramètres"
 
-#: ../configure.zcml:31
+#: ../configure.zcml:32
 msgid "Installs the imio.schedule add-on."
 msgstr "Installe le produit 'échéancier'"
 
 #: ../interfaces.py:238
 msgid "Leave empty to disable"
 msgstr "Laissez le champ vide pour désactiver le surlignage"
 
@@ -166,107 +180,107 @@
 msgid "MacroTask configuration."
 msgstr "Configuration de macro-tâches"
 
 #: ../profiles/default/types/MacroTaskConfig.xml
 msgid "MacroTaskConfig"
 msgstr "Configuration de macro-tâches"
 
-#: ../content/task_config.py:199
+#: ../content/task_config.py:210
 msgid "Marker interfaces"
 msgstr "Interfaces marqueurs"
 
 #: ../vocabularies.py:18
 msgid "Monday"
 msgstr "Lundi"
 
 #: ../browser/task_owner.py:18
 msgid "New owner"
 msgstr "Nouveau propriétaire"
 
-#: ../content/vocabulary.py:435
+#: ../content/vocabulary.py:468
 msgid "Next Friday"
 msgstr "Vendredi suivant"
 
-#: ../content/vocabulary.py:431
+#: ../content/vocabulary.py:464
 msgid "Next Monday"
 msgstr "Lundi suivant"
 
-#: ../content/vocabulary.py:436
+#: ../content/vocabulary.py:469
 msgid "Next Saturday"
 msgstr "Samedi suivant"
 
-#: ../content/vocabulary.py:437
+#: ../content/vocabulary.py:470
 msgid "Next Sunday"
 msgstr "Dimanche suivant"
 
-#: ../content/vocabulary.py:434
+#: ../content/vocabulary.py:467
 msgid "Next Thursday"
 msgstr "Jeudi suivant"
 
-#: ../content/vocabulary.py:432
+#: ../content/vocabulary.py:465
 msgid "Next Tuesday"
 msgstr "Mardi suivant"
 
-#: ../content/vocabulary.py:433
+#: ../content/vocabulary.py:466
 msgid "Next Wednesday"
 msgstr "Mercredi suivant"
 
-#: ../content/vocabulary.py:430
+#: ../content/vocabulary.py:463
 msgid "None"
 msgstr ""
 
-#: ../content/task_config.py:53
+#: ../content/task_config.py:64
 msgid "Operator"
 msgstr "Opérateur"
 
 #: ../interfaces.py:246
 msgid "Overrides orange color, leave empty to disable"
 msgstr "Outrepasse la couleur orange; laissez le champ vide pour désactiver le surlignage"
 
 #: ../browser/task_owner.py:39
 msgid "Owner changed"
 msgstr "Propriétaire réassigné"
 
-#: ../content/vocabulary.py:442
+#: ../content/vocabulary.py:475
 msgid "Previous Friday"
 msgstr "Vendredi précédant"
 
-#: ../content/vocabulary.py:438
+#: ../content/vocabulary.py:471
 msgid "Previous Monday"
 msgstr "Lundi précédant"
 
-#: ../content/vocabulary.py:443
+#: ../content/vocabulary.py:476
 msgid "Previous Saturday"
 msgstr "Samedi précédant"
 
-#: ../content/vocabulary.py:444
+#: ../content/vocabulary.py:477
 msgid "Previous Sunday"
 msgstr "Dimanche précédant"
 
-#: ../content/vocabulary.py:441
+#: ../content/vocabulary.py:474
 msgid "Previous Thursday"
 msgstr "Jeudi précédant"
 
-#: ../content/vocabulary.py:439
+#: ../content/vocabulary.py:472
 msgid "Previous Tuesday"
 msgstr "Mardi précédant"
 
-#: ../content/vocabulary.py:440
+#: ../content/vocabulary.py:473
 msgid "Previous Wednesday"
 msgstr "Mercredi précédant"
 
-#: ../content/task_config.py:381
+#: ../content/task_config.py:413
 msgid "Recurrence"
 msgstr "Récurrence"
 
-#: ../content/task_config.py:403
+#: ../content/task_config.py:435
 msgid "Recurrence condition"
 msgstr "Conditions de récurente"
 
-#: ../content/task_config.py:321
+#: ../content/task_config.py:353
 msgid "Round to week day"
 msgstr "Arrondir au jour de la semaine"
 
 #: ../vocabularies.py:23
 msgid "Saturday"
 msgstr "Samedi"
 
@@ -282,155 +296,168 @@
 msgid "Schedule configuration."
 msgstr "Configuration d'échéances"
 
 #: ../profiles/default/types/ScheduleConfig.xml
 msgid "ScheduleConfig"
 msgstr "Configuration d'échéances"
 
-#: ../content/schedule_config.py:27
+#: ../content/schedule_config.py:29
 msgid "Scheduled content type"
 msgstr "Type de contenu associé"
 
-#: ../content/task_config.py:220
+#: ../content/task_config.py:231
 msgid "Select creation conditions of the task"
 msgstr "Sélectionnez les conditions de création de la tâche"
 
-#: ../content/task_config.py:186
+#: ../content/task_config.py:197
 msgid "Select default group assigned to this task."
 msgstr "Groupe assigné par défaut à cette tâche"
 
-#: ../content/task_config.py:193
+#: ../content/task_config.py:204
 msgid "Select default user assigned to this task."
 msgstr "Choisissez l'utisateur qui sera assigné par défaut à cette tâche"
 
-#: ../content/task_config.py:266
+#: ../content/task_config.py:277
 msgid "Select end conditions of the task."
 msgstr "Sélectionnez les conditions de clôture de la tâche"
 
-#: ../content/task_config.py:345
+#: ../content/task_config.py:377
 msgid "Select freeze conditions of the task."
 msgstr "Sélectionnez les conditions de gel de la tâche"
 
-#: ../content/task_config.py:404
+#: ../content/task_config.py:436
 msgid "Select recurrence conditions of the task."
 msgstr "Choisissez les conditions de récurence pour cette tâche"
 
-#: ../content/task_config.py:243
+#: ../content/task_config.py:254
 msgid "Select start conditions of the task"
 msgstr "Sélectionnez les conditions de démarrage de la tâche"
 
-#: ../content/task_config.py:371
+#: ../content/task_config.py:403
 msgid "Select thaw conditions of the task."
 msgstr "Sélectionnez les conditions de dégel de la tâche"
 
-#: ../content/schedule_config.py:28
+#: ../content/schedule_config.py:30
 msgid "Select the content type to apply schedule."
 msgstr "Sélectionnez le type de contenu de l'échéancier"
 
-#: ../content/task_config.py:286
+#: ../content/task_config.py:301
 msgid "Select the start date used to compute the due date."
 msgstr "Sélectionnez la date de départ pour la calcul de l'échéance"
 
-#: ../content/task_config.py:213
+#: ../content/task_config.py:224
 msgid "Select the state of the container where the task is automatically created."
 msgstr "Sélectionnez l'état du récipient pour lequel la tâche est automatiquement créée"
 
-#: ../content/task_config.py:236
+#: ../content/task_config.py:247
 msgid "Select the state of the container where the task is automatically started."
 msgstr "Sélectionnez l'état du récipient pour lequel la tâche est automatiquement démarrée"
 
-#: ../content/task_config.py:397
+#: ../content/task_config.py:429
 msgid "Select the state of the container where the task should be recurred"
 msgstr "Sélectionnez l'état pour lequel la tâche doit recommencer"
 
-#: ../content/task_config.py:259
+#: ../content/task_config.py:270
 msgid "Select the states of the container where the task is automatically closed."
 msgstr "Sélectionnez les états du récipient pour lequel la tâche est automatiquement clôturée"
 
 msgid "Should pass from actual state "
 msgstr "Changer l'état actuel "
 
-#: ../content/task_config.py:230
+#: ../content/task_config.py:241
 msgid "Start"
 msgstr "Démarrage"
 
-#: ../content/task_config.py:242
+#: ../content/task_config.py:253
 msgid "Start conditions"
 msgstr "Conditions de démarrage"
 
-#: ../content/task_config.py:285
+#: ../content/task_config.py:300
 msgid "Start date"
 msgstr "Date de départ"
 
 msgid "Started tasks"
 msgstr "Tâches en cours"
 
 msgid "State"
 msgstr "L'état"
 
 #: ../testing.zcml:16
 msgid "Steps to ease tests of imio.schedule"
 msgstr ""
 
-#: ../dashboard/columns.py:186
+#: ../dashboard/columns.py:217
 msgid "Subtask"
 msgstr "Sous-tâche"
 
+#. Default: "Subtasks:"
+#: ../browser/templates/taskmacros.pt:35
+msgid "Subtasks"
+msgstr "Sous-tâches"
+
 msgid "Subtasks dependencies"
 msgstr "Réalisation distribuée"
 
 #: ../vocabularies.py:24
 msgid "Sunday"
 msgstr "Dimanche"
 
+#: ../browser/close_task.py:32
+msgid "Task Closed"
+msgstr "Tâche cloturée"
+
 #: ../profiles/default/types/TaskConfig.xml
 msgid "Task configuration."
 msgstr "Configuration de tâche"
 
-#: ../content/task_config.py:212
+#: ../content/task_config.py:223
 msgid "Task container creation state"
 msgstr "État de création de la tâche"
 
-#: ../content/task_config.py:258
+#: ../content/task_config.py:269
 msgid "Task container end states"
 msgstr "État(s) de clôture de la tâche"
 
-#: ../content/task_config.py:337
+#: ../content/task_config.py:369
 msgid "Task container freeze states"
 msgstr "État(s) de gel de la tâche"
 
-#: ../content/task_config.py:396
+#: ../content/task_config.py:428
 msgid "Task container recurrence states"
 msgstr "État(s) de récurrence de la tâche"
 
-#: ../content/task_config.py:235
+#: ../content/task_config.py:246
 msgid "Task container start states"
 msgstr "État(s) de démarrage de la tâche"
 
-#: ../content/task_config.py:363
+#: ../content/task_config.py:395
 msgid "Task container thaw states"
 msgstr "État(s) de dégel de la tâche"
 
 #: ../profiles/default/types/TaskConfig.xml
 msgid "TaskConfig"
 msgstr "Configuration de tâche"
 
-#: ../content/task_config.py:355
+#: ../content/task_config.py:387
 msgid "Thaw"
 msgstr "Dégel"
 
-#: ../content/task_config.py:370
+#: ../content/task_config.py:402
 msgid "Thaw conditions"
 msgstr "Conditions de dégel de la tâche"
 
+#: ../content/task_config.py:343
+msgid "The additional delay is not a valid integer"
+msgstr "Le délai supplémentaire n'est pas un entier"
+
 #: ../interfaces.py:258
 msgid "The orange value should be higher than the red one, as it is used as a first warning."
 msgstr "La limite pour l'orange doit être supérieure à la rouge, car l'orange est utilisé comme premier avertissement."
 
-#: ../content/task_config.py:310
+#: ../content/task_config.py:323
 msgid "This delay is added to the due date of the task."
 msgstr "Délai (jours) supplémentaire additionné à la date d'échéance'"
 
 #: ../vocabularies.py:21
 msgid "Thursday"
 msgstr "Jeudi"
 
@@ -438,47 +465,47 @@
 msgid "To do"
 msgstr "À faire"
 
 #: ../vocabularies.py:19
 msgid "Tuesday"
 msgstr "Mardi"
 
-#: ../content/task_config.py:292
+#: ../content/task_config.py:307
 msgid "Warning delay"
 msgstr "Délai d'alerte"
 
 #: ../vocabularies.py:20
 msgid "Wednesday"
 msgstr "Mercredi"
 
 #: ../vocabularies.py:33
 msgid "Working days"
 msgstr "Jour ouvrables"
 
-#: ../content/vocabulary.py:419
+#: ../content/vocabulary.py:452
 msgid "and"
 msgstr "et"
 
 #: ../dashboard/vocabulary.py:27
 msgid "collective.task"
 msgstr ""
 
-#: ../content/task_config.py:59
+#: ../content/task_config.py:70
 msgid "display_status"
 msgstr "Statut"
 
-#: ../configure.zcml:31
+#: ../configure.zcml:32
 msgid "imio.schedule"
 msgstr ""
 
 #: ../testing.zcml:16
 msgid "imio.schedule tests"
 msgstr ""
 
-#: ../content/vocabulary.py:420
+#: ../content/vocabulary.py:453
 msgid "or"
 msgstr "ou"
 
 msgid "schedule.assign_current_user"
 msgstr "Utilisateur connecté"
 
 msgid "schedule.create_if_all_subtasks_can_be_created"
@@ -506,11 +533,7 @@
 msgstr "Condition de création TEST"
 
 msgid "schedule.test_end_condition"
 msgstr "Condition de fin TEST"
 
 msgid "schedule.test_start_condition"
 msgstr "Condition de démarrage TEST"
-
-#: ../../../browser/templates/taskmacros.pt:35
-msgid "Subtasks"
-msgstr "Sous-tâches"
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/locales/imio.schedule.pot` & `imio.schedule-2.2.2/src/imio/schedule/locales/imio.schedule.pot`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2019-10-08 11:36+0000\n"
+"POT-Creation-Date: 2024-04-08 09:18+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
@@ -23,143 +23,155 @@
 msgid " to one of the following states"
 msgstr ""
 
 #: ../vocabularies.py:32
 msgid "Absolute"
 msgstr ""
 
-#: ../content/task_config.py:390
+#: ../content/task_config.py:422
 msgid "Activate recurrency"
 msgstr ""
 
-#: ../content/task_config.py:307
+#: ../content/task_config.py:322
 msgid "Additional delay"
 msgstr ""
 
-#: ../content/task_config.py:314
+#: ../content/task_config.py:329
+msgid "Additional delay is a tal expression?"
+msgstr ""
+
+#: ../content/task_config.py:346
 msgid "Additional delay type"
 msgstr ""
 
-#: ../events/dashboard_collection.py:16
+#: ../events/dashboard_collection.py:20
 msgid "All"
 msgstr ""
 
-#: ../content/task_config.py:185
+#: ../content/task_config.py:196
 msgid "Assigned group"
 msgstr ""
 
 msgid "Assigned to"
 msgstr ""
 
-#: ../content/task_config.py:192
+#: ../content/task_config.py:203
 msgid "Assigned user"
 msgstr ""
 
 #: ../profiles/default/types/AutomatedMacroTask.xml
 msgid "AutomatedMacroTask"
 msgstr ""
 
 #: ../profiles/default/types/AutomatedTask.xml
 msgid "AutomatedTask"
 msgstr ""
 
-#: ../content/task_config.py:276
+#: ../content/task_config.py:287
 msgid "Calculation delay"
 msgstr ""
 
-#: ../content/task_config.py:297
+#: ../content/task_config.py:312
 msgid "Calculation delay method"
 msgstr ""
 
 #: ../browser/templates/task_change_owner.pt:15
 msgid "Change the task owner"
 msgstr ""
 
-#: ../content/task_config.py:47
+#: ../browser/templates/close_task.pt:15
+msgid "Close task"
+msgstr ""
+
 #: ../interfaces.py:237
 msgid "Color due date in orange if it comes close to X days"
 msgstr ""
 
 #: ../interfaces.py:245
 msgid "Color due date in red if it comes close to X days"
 msgstr ""
 
-#: ../content/task_config.py:49
+#: ../content/task_config.py:58
 msgid "Condition"
 msgstr ""
 
-#: ../content/task_config.py:222
+#: ../content/task_config.py:233
 msgid "Conditions"
 msgstr ""
 
+#: ../browser/close_task.py:22
 #: ../browser/task_owner.py:28
 msgid "Confirm"
 msgstr ""
 
-#: ../content/task_config.py:207
+#: ../content/task_config.py:218
 msgid "Creation"
 msgstr ""
 
-#: ../content/task_config.py:219
+#: ../content/task_config.py:230
 msgid "Creation conditions"
 msgstr ""
 
-#: ../content/task_config.py:200
+#: ../content/task_config.py:211
 msgid "Custom marker interfaces for this task."
 msgstr ""
 
-#: ../interfaces.py:218
+#: ../interfaces.py:226
 msgid "Day"
 msgstr ""
 
-#: ../content/task_config.py:315
+#: ../content/task_config.py:330
+msgid "Define if the additional delay should be interpreted as a tal expression"
+msgstr ""
+
+#: ../content/task_config.py:347
 msgid "Define the calculation method for the additional delay"
 msgstr ""
 
 msgid "Doable alone"
 msgstr ""
 
 #: ../browser/templates/task_completion.pt:53
 msgid "Done"
 msgstr ""
 
-#: ../dashboard/columns.py:187
+#: ../dashboard/columns.py:218
 msgid "Due date"
 msgstr ""
 
-#: ../content/schedule_config.py:21
-#: ../content/task_config.py:179
+#: ../content/schedule_config.py:23
+#: ../content/task_config.py:190
 msgid "Enabled"
 msgstr ""
 
-#: ../content/task_config.py:265
+#: ../content/task_config.py:276
 msgid "End conditions"
 msgstr ""
 
-#: ../content/task_config.py:253
+#: ../content/task_config.py:264
 msgid "Ending"
 msgstr ""
 
-#: ../content/task_config.py:329
+#: ../content/task_config.py:361
 msgid "Freeze"
 msgstr ""
 
-#: ../content/task_config.py:344
+#: ../content/task_config.py:376
 msgid "Freeze conditions"
 msgstr ""
 
 #: ../vocabularies.py:22
 msgid "Friday"
 msgstr ""
 
-#: ../content/task_config.py:171
+#: ../content/task_config.py:182
 msgid "General informations"
 msgstr ""
 
-#: ../configure.zcml:31
+#: ../configure.zcml:32
 msgid "Installs the imio.schedule add-on."
 msgstr ""
 
 #: ../interfaces.py:238
 msgid "Leave empty to disable"
 msgstr ""
 
@@ -171,107 +183,107 @@
 msgid "MacroTask configuration."
 msgstr ""
 
 #: ../profiles/default/types/MacroTaskConfig.xml
 msgid "MacroTaskConfig"
 msgstr ""
 
-#: ../content/task_config.py:199
+#: ../content/task_config.py:210
 msgid "Marker interfaces"
 msgstr ""
 
 #: ../vocabularies.py:18
 msgid "Monday"
 msgstr ""
 
 #: ../browser/task_owner.py:18
 msgid "New owner"
 msgstr ""
 
-#: ../content/vocabulary.py:435
+#: ../content/vocabulary.py:468
 msgid "Next Friday"
 msgstr ""
 
-#: ../content/vocabulary.py:431
+#: ../content/vocabulary.py:464
 msgid "Next Monday"
 msgstr ""
 
-#: ../content/vocabulary.py:436
+#: ../content/vocabulary.py:469
 msgid "Next Saturday"
 msgstr ""
 
-#: ../content/vocabulary.py:437
+#: ../content/vocabulary.py:470
 msgid "Next Sunday"
 msgstr ""
 
-#: ../content/vocabulary.py:434
+#: ../content/vocabulary.py:467
 msgid "Next Thursday"
 msgstr ""
 
-#: ../content/vocabulary.py:432
+#: ../content/vocabulary.py:465
 msgid "Next Tuesday"
 msgstr ""
 
-#: ../content/vocabulary.py:433
+#: ../content/vocabulary.py:466
 msgid "Next Wednesday"
 msgstr ""
 
-#: ../content/vocabulary.py:430
+#: ../content/vocabulary.py:463
 msgid "None"
 msgstr ""
 
-#: ../content/task_config.py:53
+#: ../content/task_config.py:64
 msgid "Operator"
 msgstr ""
 
 #: ../interfaces.py:246
 msgid "Overrides orange color, leave empty to disable"
 msgstr ""
 
 #: ../browser/task_owner.py:39
 msgid "Owner changed"
 msgstr ""
 
-#: ../content/vocabulary.py:442
+#: ../content/vocabulary.py:475
 msgid "Previous Friday"
 msgstr ""
 
-#: ../content/vocabulary.py:438
+#: ../content/vocabulary.py:471
 msgid "Previous Monday"
 msgstr ""
 
-#: ../content/vocabulary.py:443
+#: ../content/vocabulary.py:476
 msgid "Previous Saturday"
 msgstr ""
 
-#: ../content/vocabulary.py:444
+#: ../content/vocabulary.py:477
 msgid "Previous Sunday"
 msgstr ""
 
-#: ../content/vocabulary.py:441
+#: ../content/vocabulary.py:474
 msgid "Previous Thursday"
 msgstr ""
 
-#: ../content/vocabulary.py:439
+#: ../content/vocabulary.py:472
 msgid "Previous Tuesday"
 msgstr ""
 
-#: ../content/vocabulary.py:440
+#: ../content/vocabulary.py:473
 msgid "Previous Wednesday"
 msgstr ""
 
-#: ../content/task_config.py:381
+#: ../content/task_config.py:413
 msgid "Recurrence"
 msgstr ""
 
-#: ../content/task_config.py:403
+#: ../content/task_config.py:435
 msgid "Recurrence condition"
 msgstr ""
 
-#: ../content/task_config.py:321
+#: ../content/task_config.py:353
 msgid "Round to week day"
 msgstr ""
 
 #: ../vocabularies.py:23
 msgid "Saturday"
 msgstr ""
 
@@ -287,155 +299,168 @@
 msgid "Schedule configuration."
 msgstr ""
 
 #: ../profiles/default/types/ScheduleConfig.xml
 msgid "ScheduleConfig"
 msgstr ""
 
-#: ../content/schedule_config.py:27
+#: ../content/schedule_config.py:29
 msgid "Scheduled content type"
 msgstr ""
 
-#: ../content/task_config.py:220
+#: ../content/task_config.py:231
 msgid "Select creation conditions of the task"
 msgstr ""
 
-#: ../content/task_config.py:186
+#: ../content/task_config.py:197
 msgid "Select default group assigned to this task."
 msgstr ""
 
-#: ../content/task_config.py:193
+#: ../content/task_config.py:204
 msgid "Select default user assigned to this task."
 msgstr ""
 
-#: ../content/task_config.py:266
+#: ../content/task_config.py:277
 msgid "Select end conditions of the task."
 msgstr ""
 
-#: ../content/task_config.py:345
+#: ../content/task_config.py:377
 msgid "Select freeze conditions of the task."
 msgstr ""
 
-#: ../content/task_config.py:404
+#: ../content/task_config.py:436
 msgid "Select recurrence conditions of the task."
 msgstr ""
 
-#: ../content/task_config.py:243
+#: ../content/task_config.py:254
 msgid "Select start conditions of the task"
 msgstr ""
 
-#: ../content/task_config.py:371
+#: ../content/task_config.py:403
 msgid "Select thaw conditions of the task."
 msgstr ""
 
-#: ../content/schedule_config.py:28
+#: ../content/schedule_config.py:30
 msgid "Select the content type to apply schedule."
 msgstr ""
 
-#: ../content/task_config.py:286
+#: ../content/task_config.py:301
 msgid "Select the start date used to compute the due date."
 msgstr ""
 
-#: ../content/task_config.py:213
+#: ../content/task_config.py:224
 msgid "Select the state of the container where the task is automatically created."
 msgstr ""
 
-#: ../content/task_config.py:236
+#: ../content/task_config.py:247
 msgid "Select the state of the container where the task is automatically started."
 msgstr ""
 
-#: ../content/task_config.py:397
+#: ../content/task_config.py:429
 msgid "Select the state of the container where the task should be recurred"
 msgstr ""
 
-#: ../content/task_config.py:259
+#: ../content/task_config.py:270
 msgid "Select the states of the container where the task is automatically closed."
 msgstr ""
 
 msgid "Should pass from actual state "
 msgstr ""
 
-#: ../content/task_config.py:230
+#: ../content/task_config.py:241
 msgid "Start"
 msgstr ""
 
-#: ../content/task_config.py:242
+#: ../content/task_config.py:253
 msgid "Start conditions"
 msgstr ""
 
-#: ../content/task_config.py:285
+#: ../content/task_config.py:300
 msgid "Start date"
 msgstr ""
 
 msgid "Started tasks"
 msgstr ""
 
 msgid "State"
 msgstr ""
 
 #: ../testing.zcml:16
 msgid "Steps to ease tests of imio.schedule"
 msgstr ""
 
-#: ../dashboard/columns.py:186
+#: ../dashboard/columns.py:217
 msgid "Subtask"
 msgstr ""
 
+#. Default: "Subtasks:"
+#: ../browser/templates/taskmacros.pt:35
+msgid "Subtasks"
+msgstr ""
+
 msgid "Subtasks dependencies"
 msgstr ""
 
 #: ../vocabularies.py:24
 msgid "Sunday"
 msgstr ""
 
+#: ../browser/close_task.py:32
+msgid "Task Closed"
+msgstr ""
+
 #: ../profiles/default/types/TaskConfig.xml
 msgid "Task configuration."
 msgstr ""
 
-#: ../content/task_config.py:212
+#: ../content/task_config.py:223
 msgid "Task container creation state"
 msgstr ""
 
-#: ../content/task_config.py:258
+#: ../content/task_config.py:269
 msgid "Task container end states"
 msgstr ""
 
-#: ../content/task_config.py:337
+#: ../content/task_config.py:369
 msgid "Task container freeze states"
 msgstr ""
 
-#: ../content/task_config.py:396
+#: ../content/task_config.py:428
 msgid "Task container recurrence states"
 msgstr ""
 
-#: ../content/task_config.py:235
+#: ../content/task_config.py:246
 msgid "Task container start states"
 msgstr ""
 
-#: ../content/task_config.py:363
+#: ../content/task_config.py:395
 msgid "Task container thaw states"
 msgstr ""
 
 #: ../profiles/default/types/TaskConfig.xml
 msgid "TaskConfig"
 msgstr ""
 
-#: ../content/task_config.py:355
+#: ../content/task_config.py:387
 msgid "Thaw"
 msgstr ""
 
-#: ../content/task_config.py:370
+#: ../content/task_config.py:402
 msgid "Thaw conditions"
 msgstr ""
 
+#: ../content/task_config.py:343
+msgid "The additional delay is not a valid integer"
+msgstr ""
+
 #: ../interfaces.py:258
 msgid "The orange value should be higher than the red one, as it is used as a first warning."
 msgstr ""
 
-#: ../content/task_config.py:310
+#: ../content/task_config.py:323
 msgid "This delay is added to the due date of the task."
 msgstr ""
 
 #: ../vocabularies.py:21
 msgid "Thursday"
 msgstr ""
 
@@ -443,47 +468,47 @@
 msgid "To do"
 msgstr ""
 
 #: ../vocabularies.py:19
 msgid "Tuesday"
 msgstr ""
 
-#: ../content/task_config.py:292
+#: ../content/task_config.py:307
 msgid "Warning delay"
 msgstr ""
 
 #: ../vocabularies.py:20
 msgid "Wednesday"
 msgstr ""
 
 #: ../vocabularies.py:33
 msgid "Working days"
 msgstr ""
 
-#: ../content/vocabulary.py:419
+#: ../content/vocabulary.py:452
 msgid "and"
 msgstr ""
 
 #: ../dashboard/vocabulary.py:27
 msgid "collective.task"
 msgstr ""
 
-#: ../content/task_config.py:59
+#: ../content/task_config.py:70
 msgid "display_status"
 msgstr ""
 
-#: ../configure.zcml:31
+#: ../configure.zcml:32
 msgid "imio.schedule"
 msgstr ""
 
 #: ../testing.zcml:16
 msgid "imio.schedule tests"
 msgstr ""
 
-#: ../content/vocabulary.py:420
+#: ../content/vocabulary.py:453
 msgid "or"
 msgstr ""
 
 msgid "schedule.assign_current_user"
 msgstr ""
 
 msgid "schedule.create_if_all_subtasks_can_be_created"
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/locales/manual_translations.pot` & `imio.schedule-2.2.2/src/imio/schedule/locales/manual_translations.pot`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/locales/update.sh` & `imio.schedule-2.2.2/src/imio/schedule/locales/update.sh`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/migration/migrate_to_18.py` & `imio.schedule-2.2.2/src/imio/schedule/migration/migrate_to_18.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 
 from imio.schedule.workflow.freeze_task import FreezeTaskWorkflowAdaptation
 
 import logging
 
-logger = logging.getLogger('imio.schedule: migrations')
+logger = logging.getLogger("imio.schedule: migrations")
 
 
 def migrate_to_18(context):
     """ """
-    logger = logging.getLogger('imio.schedule: migrate to 1.8')
+    logger = logging.getLogger("imio.schedule: migrate to 1.8")
     logger.info("starting migration steps")
 
     logger.info("add freeze state to task workflow")
     adaptation = FreezeTaskWorkflowAdaptation()
-    adaptation.patch_workflow('task_workflow')
+    adaptation.patch_workflow("task_workflow")
 
     logger.info("reinstalling imio.schedule done!")
     logger.info("migration done!")
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/migration/upgrades.py` & `imio.schedule-2.2.2/src/imio/schedule/migration/upgrades.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,15 @@
             continue
         collection = brain.getObject()
         alsoProvides(collection, IScheduleCollection)
 
 
 def upgrade_3_set_showNumberOfItems(context):
     from collective.eeafaceted.collectionwidget.interfaces import IDashboardCollection
+
     brains = api.content.find(
         object_provides=IDashboardCollection.__identifier__,
         id="dashboard_collection",
     )
     for brain in brains:
         if "schedule" not in brain.getPath():
             continue
@@ -39,19 +40,21 @@
 def upgrade_4_add_due_date_reminders(context):
     from imio.schedule.interfaces import IDueDateSettings
 
     setup_tool = api.portal.get_tool("portal_setup")
     registry = getUtility(IRegistry)
 
     default_values = {
-        'color_orange_x_days_before_due_date': 10,
-        'color_red_x_days_before_due_date': 5,
+        "color_orange_x_days_before_due_date": 10,
+        "color_red_x_days_before_due_date": 5,
     }
 
-    base = 'imio.schedule.interfaces.IDueDateSettings'
+    base = "imio.schedule.interfaces.IDueDateSettings"
     for key, default_value in default_values.items():
         full_key = "{0}.{1}".format(base, key)
         if full_key not in registry.records:
-            registry_field = field.Int(title=IDueDateSettings[key].title, required=False, min=0)
+            registry_field = field.Int(
+                title=IDueDateSettings[key].title, required=False, min=0
+            )
             registry_record = Record(registry_field)
             registry_record.value = default_value
             registry.records[full_key] = registry_record
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/migration/upgrades.zcml` & `imio.schedule-2.2.2/src/imio/schedule/migration/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/profiles/default/catalog.xml` & `imio.schedule-2.2.2/src/imio/schedule/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/profiles/default/jsregistry.xml` & `imio.schedule-2.2.2/src/imio/schedule/profiles/default/jsregistry.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/profiles/default/registry.xml` & `imio.schedule-2.2.2/src/imio/schedule/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/profiles/default/types/AutomatedMacroTask.xml` & `imio.schedule-2.2.2/src/imio/schedule/profiles/default/types/AutomatedMacroTask.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/profiles/default/types/AutomatedTask.xml` & `imio.schedule-2.2.2/src/imio/schedule/profiles/default/types/AutomatedTask.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/profiles/default/types/MacroTaskConfig.xml` & `imio.schedule-2.2.2/src/imio/schedule/profiles/default/types/MacroTaskConfig.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/profiles/default/types/ScheduleConfig.xml` & `imio.schedule-2.2.2/src/imio/schedule/profiles/default/types/ScheduleConfig.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/profiles/default/types/TaskConfig.xml` & `imio.schedule-2.2.2/src/imio/schedule/profiles/default/types/TaskConfig.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/testing.py` & `imio.schedule-2.2.2/src/imio/schedule/testing.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,17 +8,20 @@
 from plone.app.testing import PLONE_FIXTURE
 from plone.app.testing import PloneSandboxLayer
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.app.testing import TEST_USER_NAME
 from plone.app.testing import TEST_USER_PASSWORD
 from plone.testing import z2
+from zope.globalrequest import setRequest
 
 from imio.schedule.events import zope_registration
-from imio.schedule.events.zope_registration import unsubscribe_task_configs_for_content_type
+from imio.schedule.events.zope_registration import (
+    unsubscribe_task_configs_for_content_type,
+)
 
 import transaction
 
 import unittest
 
 import imio.schedule
 
@@ -26,141 +29,129 @@
 class NakedPloneLayer(PloneSandboxLayer):
 
     defaultBases = (PLONE_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         """Set up Zope."""
         # Load ZCML
-        self.loadZCML(package=imio.schedule,
-                      name='testing.zcml')
+        self.loadZCML(package=imio.schedule, name="testing.zcml")
         # need to do this for archetypes products having 'initialize'
         # method for their content types in their __init__.py
-        z2.installProduct(app, 'imio.dashboard')
+        z2.installProduct(app, "imio.dashboard")
 
     def tearDownZope(self, app):
         """Tear down Zope."""
-        z2.uninstallProduct(app, 'imio.dashboard')
+        z2.uninstallProduct(app, "imio.dashboard")
 
-NAKED_PLONE_FIXTURE = NakedPloneLayer(
-    name='NAKED_PLONE_FIXTURE'
-)
+
+NAKED_PLONE_FIXTURE = NakedPloneLayer(name="NAKED_PLONE_FIXTURE")
 
 NAKED_PLONE_INTEGRATION = IntegrationTesting(
-    bases=(NAKED_PLONE_FIXTURE,),
-    name='NAKED_PLONE_INTEGRATION'
+    bases=(NAKED_PLONE_FIXTURE,), name="NAKED_PLONE_INTEGRATION"
 )
 
 
 class ScheduleLayer(NakedPloneLayer):
-
     def setUpPloneSite(self, portal):
-        applyProfile(portal, 'Products.CMFPlone:plone')
-        applyProfile(portal, 'imio.schedule:default')
+        setRequest(portal.REQUEST)
+        applyProfile(portal, "Products.CMFPlone:plone")
+        applyProfile(portal, "imio.schedule:default")
 
         # Login and create some test content
-        setRoles(portal, TEST_USER_ID, ['Manager'])
+        setRoles(portal, TEST_USER_ID, ["Manager"])
         login(portal, TEST_USER_NAME)
 
         # Commit so that the test browser sees these objects
         transaction.commit()
+        setRequest(portal.REQUEST)
 
 
-TEST_INSTALL_FIXTURE = ScheduleLayer(
-    name='TEST_INSTALL_FIXTURE'
-)
+TEST_INSTALL_FIXTURE = ScheduleLayer(name="TEST_INSTALL_FIXTURE")
 
 TEST_INSTALL_INTEGRATION = IntegrationTesting(
-    bases=(TEST_INSTALL_FIXTURE,),
-    name='TEST_INSTALL_INTEGRATION'
+    bases=(TEST_INSTALL_FIXTURE,), name="TEST_INSTALL_INTEGRATION"
 )
 
 
 TEST_INSTALL_FUNCTIONAL = FunctionalTesting(
-    bases=(TEST_INSTALL_FIXTURE,),
-    name='TEST_INSTALL_FUNCTIONAL'
+    bases=(TEST_INSTALL_FIXTURE,), name="TEST_INSTALL_FUNCTIONAL"
 )
 
 
 class ExampleScheduleLayer(ScheduleLayer):
-
     def setUpPloneSite(self, portal):
+        setRequest(portal.REQUEST)
         super(ExampleScheduleLayer, self).setUpPloneSite(portal)
 
-        applyProfile(portal, 'imio.schedule:testing')
+        applyProfile(portal, "imio.schedule:testing")
 
         # delete macro tasks
-        api.content.delete(
-            portal.config.test_scheduleconfig.test_macrotaskconfig
-        )
-        api.content.delete(
-            portal.test_taskcontainer.TASK_test_macrotaskconfig
-        )
+        api.content.delete(portal.config.test_scheduleconfig.test_macrotaskconfig)
+        api.content.delete(portal.test_taskcontainer.TASK_test_macrotaskconfig)
+        setRequest(portal.REQUEST)
 
 
-EXAMPLE_SCHEDULE_FIXTURE = ExampleScheduleLayer(
-    name='EXAMPLE_SCHEDULE_FIXTURE'
-)
+EXAMPLE_SCHEDULE_FIXTURE = ExampleScheduleLayer(name="EXAMPLE_SCHEDULE_FIXTURE")
 
 EXAMPLE_SCHEDULE_INTEGRATION = IntegrationTesting(
-    bases=(EXAMPLE_SCHEDULE_FIXTURE,),
-    name='EXAMPLE_SCHEDULE_INTEGRATION'
+    bases=(EXAMPLE_SCHEDULE_FIXTURE,), name="EXAMPLE_SCHEDULE_INTEGRATION"
 )
 
 
 EXAMPLE_SCHEDULE_FUNCTIONAL = FunctionalTesting(
-    bases=(EXAMPLE_SCHEDULE_FIXTURE,),
-    name='EXAMPLE_SCHEDULE_FUNCTIONAL'
+    bases=(EXAMPLE_SCHEDULE_FIXTURE,), name="EXAMPLE_SCHEDULE_FUNCTIONAL"
 )
 
 
 class BaseTest(unittest.TestCase):
     """
     Helper class for tests.
     """
 
     def setUp(self):
-        self.portal = self.layer['portal']
+        self.portal = self.layer["portal"]
 
 
 class BrowserTest(BaseTest):
     """
     Helper class for Browser tests.
     """
 
     def setUp(self):
         super(BrowserTest, self).setUp()
         self.browser = z2.Browser(self.portal)
         self.browser.handleErrors = False
 
     def browser_login(self, user, password):
         login(self.portal, user)
-        self.browser.open(self.portal.absolute_url() + '/logout')
-        self.browser.open(self.portal.absolute_url() + '/login_form')
-        self.browser.getControl(name='__ac_name').value = user
-        self.browser.getControl(name='__ac_password').value = password
-        self.browser.getControl(name='submit').click()
+        self.browser.open(self.portal.absolute_url() + "/logout")
+        self.browser.open(self.portal.absolute_url() + "/login_form")
+        self.browser.getControl(name="__ac_name").value = user
+        self.browser.getControl(name="__ac_password").value = password
+        self.browser.getControl(name="submit").click()
 
 
 class ExampleScheduleTestBase(BrowserTest):
-
     def setUp(self):
         super(ExampleScheduleTestBase, self).setUp()
+        setRequest(self.portal.REQUEST)
 
         # only keep simple tasks
         self.schedule_config = self.portal.config.test_scheduleconfig
         self.empty_schedule_config = self.portal.config.empty_scheduleconfig
         self.task_config = self.schedule_config.test_taskconfig
         self.empty_task_container = self.portal.test_empty_taskcontainer
         self.task_container = self.portal.test_taskcontainer
         self.task = self.task_container.TASK_test_taskconfig
 
         # commit to save the setup in the tests.
         transaction.commit()
 
         self.browser_login(TEST_USER_NAME, TEST_USER_PASSWORD)
+        setRequest(self.portal.REQUEST)
 
 
 class ExampleScheduleIntegrationTestCase(ExampleScheduleTestBase):
 
     layer = EXAMPLE_SCHEDULE_INTEGRATION
 
 
@@ -168,65 +159,60 @@
 
     layer = EXAMPLE_SCHEDULE_FUNCTIONAL
 
     def tearDown(self):
         """
         Unregister the adapters here since the zope instance never shut downs.
         """
+        setRequest(self.portal.REQUEST)
         unsubscribe_task_configs_for_content_type(self.task_config, None)
 
         api.content.delete(self.task_container)
         api.content.delete(self.empty_task_container)
         api.content.delete(self.portal.config)
         zope_registration._registered_sites = set([])
 
         transaction.commit()
 
         super(ExampleScheduleTestBase, self).tearDown()
+        setRequest(self.portal.REQUEST)
 
 
 class MacrotaskScheduleLayer(ScheduleLayer):
-
     def setUpPloneSite(self, portal):
+        setRequest(portal.REQUEST)
         super(MacrotaskScheduleLayer, self).setUpPloneSite(portal)
 
-        applyProfile(portal, 'Products.CMFPlone:dependencies')
+        applyProfile(portal, "Products.CMFPlone:dependencies")
         # ponr skin for robot tests
-        applyProfile(portal, 'plonetheme.sunburst:default')
-        applyProfile(portal, 'imio.schedule:testing')
+        applyProfile(portal, "plonetheme.sunburst:default")
+        applyProfile(portal, "imio.schedule:testing")
 
         # delete simple tasks
-        api.content.delete(
-            portal.config.test_scheduleconfig.test_taskconfig
-        )
-        api.content.delete(
-            portal.test_taskcontainer.TASK_test_taskconfig
-        )
+        api.content.delete(portal.config.test_scheduleconfig.test_taskconfig)
+        api.content.delete(portal.test_taskcontainer.TASK_test_taskconfig)
+        setRequest(portal.REQUEST)
 
 
-MACROTASK_SCHEDULE_FIXTURE = MacrotaskScheduleLayer(
-    name='MACROTASK_SCHEDULE_FIXTURE'
-)
+MACROTASK_SCHEDULE_FIXTURE = MacrotaskScheduleLayer(name="MACROTASK_SCHEDULE_FIXTURE")
 
 MACROTASK_SCHEDULE_INTEGRATION = IntegrationTesting(
-    bases=(MACROTASK_SCHEDULE_FIXTURE,),
-    name='MACROTASK_SCHEDULE_INTEGRATION'
+    bases=(MACROTASK_SCHEDULE_FIXTURE,), name="MACROTASK_SCHEDULE_INTEGRATION"
 )
 
 
 MACROTASK_SCHEDULE_FUNCTIONAL = FunctionalTesting(
-    bases=(MACROTASK_SCHEDULE_FIXTURE,),
-    name='MACROTASK_SCHEDULE_FUNCTIONAL'
+    bases=(MACROTASK_SCHEDULE_FIXTURE,), name="MACROTASK_SCHEDULE_FUNCTIONAL"
 )
 
 
 class MacroTaskScheduleTestBase(BrowserTest):
-
     def setUp(self):
         super(MacroTaskScheduleTestBase, self).setUp()
+        setRequest(self.portal.REQUEST)
 
         # recreate test objects
         self.portal.portal_workflow.setDefaultChain("simple_publication_workflow")
 
         # only keep macro tasks
         self.schedule_config = self.portal.config.test_scheduleconfig
         self.macrotask_config = self.schedule_config.test_macrotaskconfig
@@ -236,14 +222,15 @@
         self.macro_task = self.task_container.TASK_test_macrotaskconfig
         self.sub_task = self.macro_task.TASK_test_subtaskconfig
 
         # commit to save the setup in the tests.
         transaction.commit()
 
         self.browser_login(TEST_USER_NAME, TEST_USER_PASSWORD)
+        setRequest(self.portal.REQUEST)
 
 
 class MacroTaskScheduleIntegrationTestCase(MacroTaskScheduleTestBase):
 
     layer = MACROTASK_SCHEDULE_INTEGRATION
 
 
@@ -251,14 +238,15 @@
 
     layer = MACROTASK_SCHEDULE_FUNCTIONAL
 
     def tearDown(self):
         """
         Unregister the adapters here since the zope instance never shut downs.
         """
+        setRequest(self.portal.REQUEST)
         unsubscribe_task_configs_for_content_type(self.macrotask_config, None)
         unsubscribe_task_configs_for_content_type(self.subtask_config, None)
 
         api.content.delete(self.task_container)
         api.content.delete(self.empty_task_container)
         api.content.delete(self.portal.config)
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/testing.zcml` & `imio.schedule-2.2.2/src/imio/schedule/testing.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/tests/condition.py` & `imio.schedule-2.2.2/src/imio/schedule/tests/condition.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class TestCreationCondition(CreationCondition):
     """
     Test task start condition.
     """
 
     def evaluate(self):
-        return 'Should start'
+        return "Should start"
 
 
 class TestNegativeCreationCondition(CreationCondition):
     """
     Test task start condition.
     """
 
@@ -27,15 +27,15 @@
 
 class TestStartCondition(StartCondition):
     """
     Test task start condition.
     """
 
     def evaluate(self):
-        return 'Should start'
+        return "Should start"
 
 
 class TestNegativeStartCondition(StartCondition):
     """
     Test task start condition.
     """
 
@@ -45,15 +45,15 @@
 
 class TestEndCondition(EndCondition):
     """
     Test task end condition.
     """
 
     def evaluate(self):
-        return 'Should end'
+        return "Should end"
 
 
 class TestNegativeEndCondition(EndCondition):
     """
     Test task end condition.
     """
 
@@ -63,15 +63,15 @@
 
 class TestFreezeCondition(FreezeCondition):
     """
     Test task freeze condition.
     """
 
     def evaluate(self):
-        return 'Should freeze'
+        return "Should freeze"
 
 
 class TestNegativeFreezeCondition(FreezeCondition):
     """
     Test task freeze condition.
     """
 
@@ -81,15 +81,15 @@
 
 class TestThawCondition(ThawCondition):
     """
     Test task thaw condition.
     """
 
     def evaluate(self):
-        return 'Should thaw'
+        return "Should thaw"
 
 
 class TestNegativeThawCondition(ThawCondition):
     """
     Test task thaw condition.
     """
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/tests/conditions.zcml` & `imio.schedule-2.2.2/src/imio/schedule/tests/conditions.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/tests/robot/test_example.robot` & `imio.schedule-2.2.2/src/imio/schedule/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.2.1/src/imio/schedule/tests/setup.py` & `imio.schedule-2.2.2/src/imio/schedule/tests/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from imio.schedule.content.object_factories import ThawConditionObject
 
 
 def schedule_example_install(context):
     """
     Example schedule install script.
     """
-    if context.readDataFile('imioschedule_testing.txt') is None:
+    if context.readDataFile("imioschedule_testing.txt") is None:
         return
 
     monkey_patch_scheduled_conttentype_vocabulary(context)
     add_empty_task_container(context)
     add_schedule_config(context)
     add_task(context)
 
@@ -34,231 +34,223 @@
     Monkey patch the default vocabulary for the field 'scheduled_contenttype'
     to be able to select 'Folder' content type so we can test methods of this
     field.
     """
     from imio.schedule.content.vocabulary import ScheduledContentTypeVocabulary
 
     def monkey_allowed_types(self):
-        return{'Folder': IATFolder}
+        return {"Folder": IATFolder}
+
     ScheduledContentTypeVocabulary.content_types = monkey_allowed_types
 
 
 def add_empty_task_container(context):
     """
     Add dummy empty task container (ATFolder)
     """
     site = api.portal.get()
 
-    folder_id = 'test_empty_taskcontainer'
+    folder_id = "test_empty_taskcontainer"
     if folder_id not in site.objectIds():
         api.content.create(
-            container=site,
-            type='Folder',
-            id=folder_id,
-            title='Empty Task container'
+            container=site, type="Folder", id=folder_id, title="Empty Task container"
         )
 
 
 def add_schedule_config(context):
     """
     Add dummy ScheduleConfig, TaskConfig.
     """
     site = api.portal.get()
 
     # create config folder for schedule config
-    folder_id = 'config'
+    folder_id = "config"
     if folder_id not in site.objectIds():
         api.content.create(
-            container=site,
-            type='Folder',
-            id=folder_id,
-            title='Task configs'
+            container=site, type="Folder", id=folder_id, title="Task configs"
         )
     cfg_folder = getattr(site, folder_id)
 
     # create empty schedule config
-    schedule_cfg_id = 'empty_scheduleconfig'
+    schedule_cfg_id = "empty_scheduleconfig"
     if schedule_cfg_id not in cfg_folder.objectIds():
         api.content.create(
             container=cfg_folder,
-            type='ScheduleConfig',
+            type="ScheduleConfig",
             id=schedule_cfg_id,
-            title='Empty ScheduleConfig',
-            scheduled_contenttype=('Folder', (interface_to_tuple(IATFile),)),
+            title="Empty ScheduleConfig",
+            scheduled_contenttype=("Folder", (interface_to_tuple(IATFile),)),
         )
 
     # create schedule config
-    schedule_cfg_id = 'test_scheduleconfig'
+    schedule_cfg_id = "test_scheduleconfig"
     if schedule_cfg_id not in cfg_folder.objectIds():
         api.content.create(
             container=cfg_folder,
-            type='ScheduleConfig',
+            type="ScheduleConfig",
             id=schedule_cfg_id,
-            title='Test ScheduleConfig',
-            scheduled_contenttype=('Folder', (interface_to_tuple(IATFolder),)),
+            title="Test ScheduleConfig",
+            scheduled_contenttype=("Folder", (interface_to_tuple(IATFolder),)),
         )
     schedule_config = getattr(cfg_folder, schedule_cfg_id)
 
     # create task config
-    task_cfg_id = 'test_taskconfig'
+    task_cfg_id = "test_taskconfig"
     creation_conditions = CreationConditionObject()
     creation_conditions.__dict__ = {
-        'condition': u'schedule.test_creation_condition',
-        'operator': 'AND',
+        "condition": u"schedule.test_creation_condition",
+        "operator": "AND",
     }
     start_conditions = StartConditionObject()
     start_conditions.__dict__ = {
-        'condition': u'schedule.test_start_condition',
-        'operator': 'AND',
+        "condition": u"schedule.test_start_condition",
+        "operator": "AND",
     }
     end_conditions = EndConditionObject()
     end_conditions.__dict__ = {
-        'condition': u'schedule.test_end_condition',
-        'operator': 'AND',
+        "condition": u"schedule.test_end_condition",
+        "operator": "AND",
     }
     freeze_conditions = FreezeConditionObject()
     freeze_conditions.__dict__ = {
-        'condition': u'schedule.test_freeze_condition',
-        'operator': 'AND',
+        "condition": u"schedule.test_freeze_condition",
+        "operator": "AND",
     }
     thaw_conditions = ThawConditionObject()
     thaw_conditions.__dict__ = {
-        'condition': u'schedule.test_thaw_condition',
-        'operator': 'AND',
+        "condition": u"schedule.test_thaw_condition",
+        "operator": "AND",
     }
     macro_creation_conditions = MacroCreationConditionObject()
     macro_creation_conditions.__dict__ = creation_conditions.__dict__
     macro_start_conditions = MacroStartConditionObject()
     macro_start_conditions.__dict__ = start_conditions.__dict__
     macro_end_conditions = MacroEndConditionObject()
     macro_end_conditions.__dict__ = end_conditions.__dict__
 
     if task_cfg_id not in schedule_config.objectIds():
         api.content.create(
             container=schedule_config,
-            type='TaskConfig',
+            type="TaskConfig",
             id=task_cfg_id,
-            title='Test TaskConfig',
-            default_assigned_user='schedule.assign_current_user',
-            default_assigned_group='schedule.assign_authenticatedusers_group',
+            title="Test TaskConfig",
+            default_assigned_user="schedule.assign_current_user",
+            default_assigned_group="schedule.assign_authenticatedusers_group",
             creation_conditions=[creation_conditions],
             start_conditions=[start_conditions],
             end_conditions=[end_conditions],
             freeze_conditions=[freeze_conditions],
             thaw_conditions=[thaw_conditions],
-            creation_state='private',
-            starting_states=('pending',),
-            ending_states=('published',),
-            start_date='schedule.start_date.creation_date',
+            creation_state="private",
+            starting_states=("pending",),
+            ending_states=("published",),
+            start_date="schedule.start_date.creation_date",
             additional_delay=10,
         )
 
     # create macro task config
-    macrotask_cfg_id = 'test_macrotaskconfig'
+    macrotask_cfg_id = "test_macrotaskconfig"
     if macrotask_cfg_id not in schedule_config.objectIds():
         api.content.create(
             container=schedule_config,
-            type='MacroTaskConfig',
+            type="MacroTaskConfig",
             id=macrotask_cfg_id,
-            title='Test MacroTaskConfig',
-            default_assigned_user='schedule.assign_current_user',
-            default_assigned_group='schedule.assign_authenticatedusers_group',
+            title="Test MacroTaskConfig",
+            default_assigned_user="schedule.assign_current_user",
+            default_assigned_group="schedule.assign_authenticatedusers_group",
             creation_conditions=[macro_creation_conditions],
             start_conditions=[macro_start_conditions],
             end_conditions=[macro_end_conditions],
-            creation_state='private',
-            starting_states=('pending',),
-            ending_states=('published',),
-            start_date='schedule.start_date.subtask_highest_due_date',
+            creation_state="private",
+            starting_states=("pending",),
+            ending_states=("published",),
+            start_date="schedule.start_date.subtask_highest_due_date",
             additional_delay=17,
         )
     macrotask_config = getattr(schedule_config, macrotask_cfg_id)
 
     # create sub task config
-    subtask_cfg_id = 'test_subtaskconfig'
+    subtask_cfg_id = "test_subtaskconfig"
     if subtask_cfg_id not in macrotask_config.objectIds():
         api.content.create(
             container=macrotask_config,
-            type='TaskConfig',
+            type="TaskConfig",
             id=subtask_cfg_id,
-            title='Test SubTaskConfig',
-            default_assigned_user='schedule.assign_current_user',
-            default_assigned_group='schedule.assign_authenticatedusers_group',
+            title="Test SubTaskConfig",
+            default_assigned_user="schedule.assign_current_user",
+            default_assigned_group="schedule.assign_authenticatedusers_group",
             creation_conditions=[creation_conditions],
             start_conditions=[start_conditions],
             end_conditions=[end_conditions],
-            creation_state='private',
-            starting_states=('pending',),
-            ending_states=('published',),
-            start_date='schedule.start_date.creation_date',
+            creation_state="private",
+            starting_states=("pending",),
+            ending_states=("published",),
+            start_date="schedule.start_date.creation_date",
             additional_delay=13,
         )
 
 
 def add_task(context):
     """
     Add dummy task container (ATFolder) and create
     a AutomatedTask in it
     """
     site = api.portal.get()
 
-    task_container_id = 'test_taskcontainer'
+    task_container_id = "test_taskcontainer"
     if task_container_id not in site.objectIds():
         api.content.create(
-            container=site,
-            type='Folder',
-            id=task_container_id,
-            title='Task container'
+            container=site, type="Folder", id=task_container_id, title="Task container"
         )
     task_container = getattr(site, task_container_id)
 
     # If no task was created automatically, create the task manually
     # to keep AutomatedTask tests alive
-    task_id = 'TASK_test_taskconfig'
+    task_id = "TASK_test_taskconfig"
     if task_id not in task_container.objectIds():
-        portal_types = api.portal.get_tool('portal_types')
-        type_info = portal_types.getTypeInfo('AutomatedTask')
+        portal_types = api.portal.get_tool("portal_types")
+        type_info = portal_types.getTypeInfo("AutomatedTask")
         schedule_config = site.config.test_scheduleconfig
         task_config = schedule_config.test_taskconfig
 
         type_info._constructInstance(
             container=task_container,
             id=task_id,
             title=task_config.Title(),
             schedule_config_UID=schedule_config.UID(),
-            task_config_UID=task_config.UID()
+            task_config_UID=task_config.UID(),
         )
 
     # If no task was created automatically, create the macrotask manually
     # to keep AutomatedMacroTask tests alive
-    macrotask_id = 'TASK_test_macrotaskconfig'
+    macrotask_id = "TASK_test_macrotaskconfig"
     if macrotask_id not in task_container.objectIds():
-        portal_types = api.portal.get_tool('portal_types')
-        type_info = portal_types.getTypeInfo('AutomatedMacroTask')
+        portal_types = api.portal.get_tool("portal_types")
+        type_info = portal_types.getTypeInfo("AutomatedMacroTask")
         schedule_config = site.config.test_scheduleconfig
         task_config = schedule_config.test_macrotaskconfig
 
         type_info._constructInstance(
             container=task_container,
             id=macrotask_id,
             title=task_config.Title(),
             schedule_config_UID=schedule_config.UID(),
-            task_config_UID=task_config.UID()
+            task_config_UID=task_config.UID(),
         )
     macro_task = getattr(task_container, macrotask_id)
 
     # If no task was created automatically, create the subtask manually
     # to keep AutomatedMacroTask tests alive
-    subtask_id = 'TASK_test_subtaskconfig'
+    subtask_id = "TASK_test_subtaskconfig"
     if subtask_id not in macro_task.objectIds():
-        portal_types = api.portal.get_tool('portal_types')
-        type_info = portal_types.getTypeInfo('AutomatedTask')
+        portal_types = api.portal.get_tool("portal_types")
+        type_info = portal_types.getTypeInfo("AutomatedTask")
         schedule_config = site.config.test_scheduleconfig
         task_config = schedule_config.test_macrotaskconfig.test_subtaskconfig
 
         type_info._constructInstance(
             container=macro_task,
             id=subtask_id,
             title=task_config.Title(),
             schedule_config_UID=schedule_config.UID(),
-            task_config_UID=task_config.UID()
+            task_config_UID=task_config.UID(),
         )
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/tests/test_dashboardcollection.py` & `imio.schedule-2.2.2/src/imio/schedule/tests/test_dashboardcollection.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,26 +5,25 @@
 from plone import api
 
 from zope.event import notify
 from zope.lifecycleevent import ObjectModifiedEvent
 
 
 class TestDashboardCollectionFunctional(ExampleScheduleFunctionalTestCase):
-    """
-    """
+    """ """
 
     def test_update_title(self):
         """
         DashboardCollection title should always be the same as the parent task.
         """
         task_config = self.task_config
         collection = self.task_config.dashboard_collection
         self.assertEquals(task_config.title, collection.title)
 
-        task_config.title = 'my new title'
+        task_config.title = "my new title"
         notify(ObjectModifiedEvent(task_config))
         self.assertEquals(task_config.title, collection.title)
 
-        msg = 'collection title should be reindexed when updated'
-        catalog = api.portal.get_tool('portal_catalog')
-        brains = catalog(portal_type='DashboardCollection', Title=task_config.title)
+        msg = "collection title should be reindexed when updated"
+        catalog = api.portal.get_tool("portal_catalog")
+        brains = catalog(portal_type="DashboardCollection", Title=task_config.title)
         self.assertEquals(len(brains), 1, msg)
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/tests/test_delay.py` & `imio.schedule-2.2.2/src/imio/schedule/tests/test_delay.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from imio.schedule.content.delay import CalculationDefaultDelay
 from imio.schedule.testing import ExampleScheduleFunctionalTestCase
 from imio.schedule.tests.due_date import ContainerCreationDate
 
 
 class TestCalculationDelay(ExampleScheduleFunctionalTestCase):
-
     def setUp(self):
         super(TestCalculationDelay, self).setUp()
         self._start_date = ContainerCreationDate.start_date
 
     def tearDown(self):
         ContainerCreationDate.start_date = self._start_date
         super(TestCalculationDelay, self).tearDown()
@@ -46,21 +45,23 @@
 
         adapter.calculate_delay = Mock(return_value=10)
         self.assertEqual(10, adapter.delta)
 
     def test_due_date(self):
         """Test 'due_date' property"""
         adapter = self.delay_adapter
-        ContainerCreationDate.start_date = Mock(return_value=datetime(2016, 1, 1).date())
+        ContainerCreationDate.start_date = Mock(
+            return_value=datetime(2016, 1, 1).date()
+        )
         due_date = datetime(2016, 1, 11).date()
         adapter.calculate_delay = Mock(return_value=10)
 
         self.assertEqual(due_date, adapter.due_date)
 
     def test_compute_due_date(self):
         """Test 'compute_due_date' method"""
         adapter = self.delay_adapter
         base_date = datetime(2016, 1, 1).date()
         due_date = datetime(2016, 1, 11).date()
         adapter.calculate_delay = Mock(return_value=10)
 
-        self.assertEqual(due_date, adapter.compute_due_date(base_date))
+        self.assertEqual(due_date, adapter.compute_due_date(base_date))
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/tests/test_indexes.py` & `imio.schedule-2.2.2/src/imio/schedule/tests/test_indexes.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 
     def test_schedule_config_UID_index(self):
         """
         Check is schedule config UID is indexed in tasks.
         """
         schedule_config = self.schedule_config
         task = self.task
-        catalog = api.portal.get_tool('portal_catalog')
+        catalog = api.portal.get_tool("portal_catalog")
 
         task_brains = catalog(schedule_config_UID=schedule_config.UID())
         msg = "should have found at least one indexed task"
         self.assertEquals(len(task_brains), 1, msg)
         self.assertEquals(task_brains[0].getObject(), task)
 
     def test_task_config_UID_index(self):
         """
         Check is task config UID is indexed in tasks.
         """
         task_config = self.task_config
         task = self.task
-        catalog = api.portal.get_tool('portal_catalog')
+        catalog = api.portal.get_tool("portal_catalog")
 
         task_brains = catalog(task_config_UID=task_config.UID())
         msg = "should have found at least one indexed task"
         self.assertEquals(len(task_brains), 1, msg)
         self.assertEquals(task_brains[0].getObject(), task)
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/tests/test_logic.py` & `imio.schedule-2.2.2/src/imio/schedule/tests/test_logic.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,71 +16,63 @@
     Test some logic for tasks.
     """
 
     def test_task_starting_date_registration(self):
         """
         Content types voc factory should be registered as a named utility.
         """
-        logic_name = 'schedule.start_date.task_starting_date'
+        logic_name = "schedule.start_date.task_starting_date"
 
         duedate_adapter = queryMultiAdapter(
-            (self.task_container, self.task),
-            IStartDate,
-            name=logic_name
+            (self.task_container, self.task), IStartDate, name=logic_name
         )
         self.assertTrue(duedate_adapter)
 
     def test_task_starting_date_logic(self):
         """
         Check if the SubtaskHighestDueDate adapter return the highest
         due date amongst all the subtasks of a AutomatedMacroTask.
         """
         task_config = self.task_config
         task = self.task
-        logic_name = 'schedule.start_date.task_starting_date'
+        logic_name = "schedule.start_date.task_starting_date"
 
         duedate_adapter = getMultiAdapter(
-            (self.task_container, task),
-            IStartDate,
-            name=logic_name
+            (self.task_container, task), IStartDate, name=logic_name
         )
 
         task_config.start_task(task)
         due_date = duedate_adapter.start_date()
-        expected_date = task.workflow_history.values()[0][-1]['time']
+        expected_date = task.workflow_history.values()[0][-1]["time"]
         self.assertEquals(due_date, expected_date)
 
 
 class TestMacroTaskLogicIntegration(MacroTaskScheduleIntegrationTestCase):
     """
     Test MacroTaskConfig methods.
     """
 
     def test_subtask_highest_due_date_registration(self):
         """
         Content types voc factory should be registered as a named utility.
         """
-        logic_name = 'schedule.start_date.subtask_highest_due_date'
+        logic_name = "schedule.start_date.subtask_highest_due_date"
 
         duedate_adapter = queryMultiAdapter(
-            (self.task_container, self.macro_task),
-            IMacroTaskStartDate,
-            name=logic_name
+            (self.task_container, self.macro_task), IMacroTaskStartDate, name=logic_name
         )
         self.assertTrue(duedate_adapter)
 
     def test_subtask_highest_due_date_logic(self):
         """
         Check if the SubtaskHighestDueDate adapter return the highest
         due date amongst all the subtasks of a AutomatedMacroTask.
         """
-        logic_name = 'schedule.start_date.subtask_highest_due_date'
+        logic_name = "schedule.start_date.subtask_highest_due_date"
 
         duedate_adapter = getMultiAdapter(
-            (self.task_container, self.macro_task),
-            IMacroTaskStartDate,
-            name=logic_name
+            (self.task_container, self.macro_task), IMacroTaskStartDate, name=logic_name
         )
 
         highest_due_date = duedate_adapter.start_date()
         expected_date = DateTime(str(self.sub_task.due_date))
         self.assertEquals(highest_due_date, expected_date)
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/tests/test_registration_events.py` & `imio.schedule-2.2.2/src/imio/schedule/tests/test_registration_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,17 +37,15 @@
         a new adapter should be registered with:
             for: ATFolder (type selected on the ScheduleConfig of this TaskConfig)
             provides: IToTaskConfig
             name: this TaskConfig UID
         """
 
         task_config = api.content.create(
-            type='TaskConfig',
-            id='task_config_2',
-            container=self.schedule_config
+            type="TaskConfig", id="task_config_2", container=self.schedule_config
         )
 
         folder = self.portal.config
         adapter = queryAdapter(folder, IToTaskConfig, task_config.UID())
         msg = "an adapter should have been registered when creating a new TaskConfig"
         self.assertTrue(adapter is not None, msg)
 
@@ -57,17 +55,15 @@
 
     def test_unregistration_on_TaskConfig_deletion(self):
         """
         When deleting a TaskConfig, its IToTaskConfig adapter should be unregistered
         """
 
         task_config = api.content.create(
-            type='TaskConfig',
-            id='task_config_2',
-            container=self.schedule_config
+            type="TaskConfig", id="task_config_2", container=self.schedule_config
         )
 
         # to test unregistration, we have to be sure something was registered
         folder = self.portal.config
         adapter = getAdapter(folder, IToTaskConfig, task_config.UID())
         msg = "an adapter providing IToTaskConfig should have been registered for IATFolder"
         self.assertTrue(adapter is not None, msg)
@@ -83,28 +79,31 @@
         of a ScheduleConfig, we have to unregister all the IToTaskConfig adapter of
         each TaskConfig of this ScheduleConfig and register them back for the new
         portal_type.
         """
         schedule_config = self.schedule_config
         task_config = self.task_config
         folder = self.portal.config
-        document = api.content.create(type='Document', id='doc', container=self.portal)
+        document = api.content.create(type="Document", id="doc", container=self.portal)
 
         # the adapter should be registered for IATFolder
         adapter = getAdapter(folder, IToTaskConfig, task_config.UID())
         msg = "an adapter providing IToTaskConfig should have been registered for IATFolder"
         self.assertTrue(adapter is not None, msg)
 
-        #... but not for IATDocument
+        # ... but not for IATDocument
         adapter = queryAdapter(document, IToTaskConfig, task_config.UID())
         msg = "not adapter should have been registered for IATDocument yet..."
         self.assertTrue(adapter is None, msg)
 
         # modify 'scheduled_contenttype' then manually trigger the modification event
-        schedule_config.scheduled_contenttype = ('Document', interface_to_tuple(IATDocument))
+        schedule_config.scheduled_contenttype = (
+            "Document",
+            interface_to_tuple(IATDocument),
+        )
         notify(ObjectModifiedEvent(schedule_config))
 
         # old IToTaskConfig adapter should be unregistered for IATFolder
         adapter = queryAdapter(folder, IToTaskConfig, task_config.UID())
         msg = "the adapter should have been unregistered when modifying the ScheduleConfig"
         self.assertTrue(adapter is None, msg)
 
@@ -123,36 +122,40 @@
     def test_criterion_registration_on_ScheduleConfig_creation(self):
         """
         When creating a new ScheduleConfig,
         A vocabulary, named with the ScheduleConfig title, listing all its subtasks
         should be registered.
         """
         adapter = queryAdapter(
-            self.portal,
-            ICompoundCriterionFilter,
-            self.schedule_config.UID()
+            self.portal, ICompoundCriterionFilter, self.schedule_config.UID()
         )
         msg = "an criterion adapter should have been registered when creating a new ScheduleConfig"
         self.assertTrue(adapter is not None, msg)
 
     def test_criterion_unregistration_on_ScheduleConfig_deletion(self):
         """
         When deleting a ScheduleConfig, its IVocabularyFactory should be
         unregistered.
         """
         schedule_config = api.content.create(
-            type='ScheduleConfig',
-            id='schedule_config_2',
+            type="ScheduleConfig",
+            id="schedule_config_2",
             container=self.portal.config,
             scheduled_contenttype=self.schedule_config.scheduled_contenttype,
         )
 
         # to test unregistration, we have to be sure something was registered
-        adapter = queryAdapter(self.portal, ICompoundCriterionFilter, schedule_config.UID())
-        msg = "an adapter providing ICompoundCriterionFilter should have been registered"
+        adapter = queryAdapter(
+            self.portal, ICompoundCriterionFilter, schedule_config.UID()
+        )
+        msg = (
+            "an adapter providing ICompoundCriterionFilter should have been registered"
+        )
         self.assertTrue(adapter is not None, msg)
 
         schedule_config_UID = schedule_config.UID()
         api.content.delete(schedule_config)
-        adapter = queryAdapter(self.portal, ICompoundCriterionFilter, schedule_config_UID)
+        adapter = queryAdapter(
+            self.portal, ICompoundCriterionFilter, schedule_config_UID
+        )
         msg = "the ICompoundCriterionFilter adapter should have been unregistered when deleting the ScheduleConfig"
         self.assertTrue(adapter is None, msg)
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/tests/test_scheduleconfig.py` & `imio.schedule-2.2.2/src/imio/schedule/tests/test_scheduleconfig.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,112 +14,113 @@
     """
     Test ScheduleConfig content type.
     """
 
     layer = TEST_INSTALL_INTEGRATION
 
     def test_ScheduleConfig_portal_type_is_registered(self):
-        portal_types = api.portal.get_tool('portal_types')
+        portal_types = api.portal.get_tool("portal_types")
         registered_types = portal_types.listContentTypes()
-        self.assertTrue('ScheduleConfig' in registered_types)
+        self.assertTrue("ScheduleConfig" in registered_types)
 
 
 class TestScheduleConfigFields(ExampleScheduleIntegrationTestCase):
     """
     Test schema fields declaration.
     """
 
     def test_class_registration(self):
         """
         Check if the class of the content type ScheduleConfig is the
         correct one.
         """
         from imio.schedule.content.schedule_config import ScheduleConfig
+
         self.assertTrue(self.schedule_config.__class__ == ScheduleConfig)
 
     def test_schema_registration(self):
         """
         Check if the schema Interface of the content type ScheduleConfig is the
         correct one.
         """
-        portal_types = api.portal.get_tool('portal_types')
+        portal_types = api.portal.get_tool("portal_types")
         scheduleconfig_type = portal_types.get(self.schedule_config.portal_type)
-        self.assertTrue('IScheduleConfig' in scheduleconfig_type.schema)
+        self.assertTrue("IScheduleConfig" in scheduleconfig_type.schema)
 
     def test_enabled_attribute(self):
         task_config = aq_base(self.task_config)
-        self.assertTrue(hasattr(task_config, 'enabled'))
+        self.assertTrue(hasattr(task_config, "enabled"))
 
     def test_enabled_field_display(self):
         self.browser.open(self.task_config.absolute_url())
         contents = self.browser.contents
         msg = "field 'enabled' is not displayed"
         self.assertTrue('id="form-widgets-enabled"' in contents, msg)
         msg = "field 'enabled' is not translated"
-        self.assertTrue('Activé' in contents, msg)
+        self.assertTrue("Activé" in contents, msg)
 
     def test_enabled_field_edit(self):
-        self.browser.open(self.task_config.absolute_url() + '/edit')
+        self.browser.open(self.task_config.absolute_url() + "/edit")
         contents = self.browser.contents
         msg = "field 'enabled' is not editable"
-        self.assertTrue('Activé' in contents, msg)
+        self.assertTrue("Activé" in contents, msg)
 
     def test_scheduled_contenttype_attribute(self):
         schedule_config = aq_base(self.schedule_config)
-        self.assertTrue(hasattr(schedule_config, 'scheduled_contenttype'))
+        self.assertTrue(hasattr(schedule_config, "scheduled_contenttype"))
 
     def test_scheduled_contenttype_field_display(self):
         self.browser.open(self.schedule_config.absolute_url())
         contents = self.browser.contents
         msg = "field 'scheduled_contenttype' is not displayed"
         self.assertTrue('id="form-widgets-scheduled_contenttype"' in contents, msg)
         msg = "field 'scheduled_contenttype' is not translated"
-        self.assertTrue('Type de contenu associé' in contents, msg)
+        self.assertTrue("Type de contenu associé" in contents, msg)
 
     def test_scheduled_contenttype_field_edit(self):
-        self.browser.open(self.schedule_config.absolute_url() + '/edit')
+        self.browser.open(self.schedule_config.absolute_url() + "/edit")
         contents = self.browser.contents
         msg = "field 'scheduled_contenttype' is not editable"
-        self.assertTrue('Type de contenu associé' in contents, msg)
+        self.assertTrue("Type de contenu associé" in contents, msg)
 
 
 class TestScheduleConfigIntegration(ExampleScheduleIntegrationTestCase):
     """
     Test ScheduleConfig methods.
     """
 
     def test_get_all_task_configs(self):
         """
         Should return all TaskConfig contained in the ScheduleConfig.
         """
         expected_taskconfigs = [self.task_config]
         task_configs = self.schedule_config.get_all_task_configs()
-        msg = 'expected {} but got {}'.format(expected_taskconfigs, task_configs)
+        msg = "expected {} but got {}".format(expected_taskconfigs, task_configs)
         self.assertTrue(task_configs == expected_taskconfigs, msg)
 
     def test_get_scheduled_portal_type(self):
         """
         Should return the portal_type of the content type selected on the field
         'scheduled_contenttype'.
         """
         portal_type = self.schedule_config.get_scheduled_portal_type()
-        expected_type = 'Folder'
-        msg = 'expected {} but got {}'.format(expected_type, portal_type)
+        expected_type = "Folder"
+        msg = "expected {} but got {}".format(expected_type, portal_type)
         self.assertTrue(portal_type == expected_type, msg)
 
     def test_get_scheduled_interfaces(self):
         """
         Should return the Interface (or a class) of the content type selected
         on the field 'scheduled_contenttype'.
         """
         from Products.ATContentTypes.interfaces import IATFolder
 
         type_interface = self.schedule_config.get_scheduled_interfaces()
         expected_interface = (IATFolder,)
-        msg = 'expected {} but got {}'.format(expected_interface, type_interface)
+        msg = "expected {} but got {}".format(expected_interface, type_interface)
         self.assertTrue(type_interface == expected_interface, msg)
 
     def test_is_empty(self):
         """
         Should return True if the schedule_config has no TaskConfig.
         """
         self.assertTrue(not self.schedule_config.is_empty())
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/tests/test_setup.py` & `imio.schedule-2.2.2/src/imio/schedule/tests/test_setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,84 +10,88 @@
 
 
 class TestInstallDependencies(unittest.TestCase):
 
     layer = NAKED_PLONE_INTEGRATION
 
     def setUp(self):
-        self.portal = self.layer['portal']
-        self.installer = api.portal.get_tool('portal_quickinstaller')
+        self.portal = self.layer["portal"]
+        self.installer = api.portal.get_tool("portal_quickinstaller")
 
     def test_dexterity_is_dependency_of_imio_schedule(self):
         """
         dexterity should be installed when we install imio.schedule
         """
-        self.assertTrue(not self.installer.isProductInstalled('plone.app.dexterity'))
-        applyProfile(self.portal, 'imio.schedule:default')
-        self.assertTrue(self.installer.isProductInstalled('plone.app.dexterity'))
+        self.assertTrue(not self.installer.isProductInstalled("plone.app.dexterity"))
+        applyProfile(self.portal, "imio.schedule:default")
+        self.assertTrue(self.installer.isProductInstalled("plone.app.dexterity"))
 
     def test_z3cformdatagridfield_is_dependency_of_imio_schedule(self):
         """
         z3cform.datagridfield should be installed when we install imio.schedule
         """
-        self.assertTrue(not self.installer.isProductInstalled('collective.z3cform.datagridfield'))
-        applyProfile(self.portal, 'imio.schedule:default')
-        self.assertTrue(self.installer.isProductInstalled('collective.z3cform.datagridfield'))
+        self.assertTrue(
+            not self.installer.isProductInstalled("collective.z3cform.datagridfield")
+        )
+        applyProfile(self.portal, "imio.schedule:default")
+        self.assertTrue(
+            self.installer.isProductInstalled("collective.z3cform.datagridfield")
+        )
 
     def test_collectivetask_is_dependency_of_imio_schedule(self):
         """
         collective.task should be installed when we install imio.schedule
         """
-        self.assertTrue(not self.installer.isProductInstalled('collective.task'))
-        applyProfile(self.portal, 'imio.schedule:default')
-        self.assertTrue(self.installer.isProductInstalled('collective.task'))
+        self.assertTrue(not self.installer.isProductInstalled("collective.task"))
+        applyProfile(self.portal, "imio.schedule:default")
+        self.assertTrue(self.installer.isProductInstalled("collective.task"))
 
 
 class TestSetup(unittest.TestCase):
     """
     Test that imio.schedule is properly installed.
     """
 
     layer = TEST_INSTALL_INTEGRATION
 
     def setUp(self):
-        self.portal = self.layer['portal']
-        self.installer = api.portal.get_tool('portal_quickinstaller')
+        self.portal = self.layer["portal"]
+        self.installer = api.portal.get_tool("portal_quickinstaller")
 
     def test_product_installed(self):
         """
         Test if imio.schedule is installed.
         """
-        self.assertTrue(self.installer.isProductInstalled('imio.schedule'))
+        self.assertTrue(self.installer.isProductInstalled("imio.schedule"))
 
     def test_browserlayer(self):
         """
         Test that IImioScheduleLayer is registered.
         """
         from imio.schedule.interfaces import IImioScheduleLayer
         from plone.browserlayer import utils
+
         self.assertIn(IImioScheduleLayer, utils.registered_layers())
 
     def test_testing_profile_is_registered(self):
         """
         Test testing profile is registered.
         """
-        portal_setup = api.portal.get_tool(name='portal_setup')
-        demo_profile_name = u'imio.schedule:testing'
-        profile_ids = [info['id'] for info in portal_setup.listProfileInfo()]
-        msg = 'testing profile is not registered'
+        portal_setup = api.portal.get_tool(name="portal_setup")
+        demo_profile_name = u"imio.schedule:testing"
+        profile_ids = [info["id"] for info in portal_setup.listProfileInfo()]
+        msg = "testing profile is not registered"
         self.assertTrue(demo_profile_name in profile_ids, msg)
 
 
 class TestUninstall(unittest.TestCase):
 
     layer = TEST_INSTALL_INTEGRATION
 
     def setUp(self):
-        self.portal = self.layer['portal']
-        self.installer = api.portal.get_tool('portal_quickinstaller')
-        self.installer.uninstallProducts(['imio.schedule'])
+        self.portal = self.layer["portal"]
+        self.installer = api.portal.get_tool("portal_quickinstaller")
+        self.installer.uninstallProducts(["imio.schedule"])
 
     def test_product_uninstalled(self):
         """Test if imio.schedule is cleanly uninstalled."""
-        self.assertFalse(self.installer.isProductInstalled(
-            'imio.schedule'))
+        self.assertFalse(self.installer.isProductInstalled("imio.schedule"))
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/tests/test_task.py` & `imio.schedule-2.2.2/src/imio/schedule/tests/test_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,50 +10,52 @@
 from imio.schedule.testing import ExampleScheduleIntegrationTestCase
 from imio.schedule.testing import MacroTaskScheduleIntegrationTestCase
 from imio.schedule.testing import TEST_INSTALL_INTEGRATION
 
 from plone import api
 
 import unittest
+import transaction
 
 
 class TestAutomatedTask(unittest.TestCase):
     """
     Test AutomatedTask content type.
     """
 
     layer = TEST_INSTALL_INTEGRATION
 
     def test_AutomatedTask_portal_type_is_registered(self):
-        portal_types = api.portal.get_tool('portal_types')
+        portal_types = api.portal.get_tool("portal_types")
         registered_types = portal_types.listContentTypes()
-        self.assertTrue('AutomatedTask' in registered_types)
+        self.assertTrue("AutomatedTask" in registered_types)
 
 
 class TestAutomatedTaskFields(ExampleScheduleIntegrationTestCase):
     """
     Test schema fields declaration.
     """
 
     def test_class_registration(self):
         """
         Check if the class of the content type AutomatedTask is the
         correct one.
         """
         from imio.schedule.content.task import AutomatedTask
+
         self.assertTrue(self.task.__class__ == AutomatedTask)
 
     def test_schema_registration(self):
         """
         Check if the schema Interface of the content type AutomatedTask is the
         correct one.
         """
-        portal_types = api.portal.get_tool('portal_types')
+        portal_types = api.portal.get_tool("portal_types")
         taskconfig_type = portal_types.get(self.task.portal_type)
-        self.assertTrue('IAutomatedTask' in taskconfig_type.schema)
+        self.assertTrue("IAutomatedTask" in taskconfig_type.schema)
 
 
 class TestAutomatedTaskIntegration(ExampleScheduleFunctionalTestCase):
     """
     Test AutomatedTask methods.
     """
 
@@ -86,14 +88,15 @@
         task = self.task
 
         config = task.get_task_config()
         expected_config = self.task_config
         self.assertEquals(config, expected_config)
 
         api.content.delete(self.task_config)
+        task.id = "{0}_test".format(task.id)  # This reset the cache
         with self.assertRaises(TaskConfigNotFound):
             task.get_task_config()
 
     def test_get_status(self):
         """
         Should return CREATION, STARTED or DONE depending
         on the task workflow state.
@@ -191,93 +194,94 @@
 
     def test_start(self):
         """
         Should start a task.
         """
         task = self.task
         msg = "task should not be started yet (for the sake of the test..)"
-        self.assertEquals(api.content.get_state(task), 'created', msg)
+        self.assertEquals(api.content.get_state(task), "created", msg)
         task._start()
         msg = "task should have been started"
-        self.assertEquals(api.content.get_state(task), 'to_do', msg)
+        self.assertEquals(api.content.get_state(task), "to_do", msg)
 
     def test_end(self):
         """
         Should end a task.
         """
         task = self.task
         msg = "task should not be ended yet (for the sake of the test..)"
-        self.assertEquals(api.content.get_state(task), 'created', msg)
+        self.assertEquals(api.content.get_state(task), "created", msg)
         task._end()
         msg = "task should have been ended"
-        self.assertEquals(api.content.get_state(task), 'closed', msg)
+        self.assertEquals(api.content.get_state(task), "closed", msg)
 
     def test_freeze(self):
         """
         Should freeze a task.
         """
         task = self.task
         msg = "task should not be frozen yet (for the sake of the test..)"
-        self.assertEquals(api.content.get_state(task), 'created', msg)
+        self.assertEquals(api.content.get_state(task), "created", msg)
         task._freeze()
         msg = "task should have been frozen"
-        self.assertEquals(api.content.get_state(task), 'frozen', msg)
+        self.assertEquals(api.content.get_state(task), "frozen", msg)
 
     def test_thaw(self):
         """
         Should thaw a task.
         """
         task = self.task
         msg = "task should be in created state"
-        self.assertEquals(api.content.get_state(task), 'created', msg)
+        self.assertEquals(api.content.get_state(task), "created", msg)
         # freeze task befor thaw tests
         task._freeze()
         msg = "task should not be thawed yet (for the sake of the test..)"
-        self.assertEquals(api.content.get_state(task), 'frozen', msg)
+        self.assertEquals(api.content.get_state(task), "frozen", msg)
 
         task._thaw()
 
         msg = "task should have been thawed and put back in its original state"
-        self.assertEquals(api.content.get_state(task), 'created', msg)
+        self.assertEquals(api.content.get_state(task), "created", msg)
 
 
 class TestAutomatedMacroTask(unittest.TestCase):
     """
     Test AutomatedMacroTask content type.
     """
 
     layer = TEST_INSTALL_INTEGRATION
 
     def test_AutomatedMacroTask_portal_type_is_registered(self):
-        portal_types = api.portal.get_tool('portal_types')
+        portal_types = api.portal.get_tool("portal_types")
         registered_types = portal_types.listContentTypes()
-        self.assertTrue('AutomatedMacroTask' in registered_types)
+        self.assertTrue("AutomatedMacroTask" in registered_types)
 
 
 class TestAutomatedMacroTaskFields(MacroTaskScheduleIntegrationTestCase):
     """
     Test schema fields declaration.
     """
 
     def test_class_registration(self):
         """
         Check if the class of the content type AutomatedMacroTask is the
         correct one.
         """
         from imio.schedule.content.task import AutomatedMacroTask
+
         self.assertTrue(self.macro_task.__class__ == AutomatedMacroTask)
 
     def test_schema_registration(self):
         """
         Check if the schema Interface of the content type AutomatedMacroTask is the
         correct one.
         """
-        portal_types = api.portal.get_tool('portal_types')
+        portal_types = api.portal.get_tool("portal_types")
         taskconfig_type = portal_types.get(self.macro_task.portal_type)
-        self.assertTrue('IAutomatedTask' in taskconfig_type.schema)
+        self.assertTrue("IAutomatedTask" in taskconfig_type.schema)
 
 
 class TestAutomatedMacroTaskIntegration(MacroTaskScheduleIntegrationTestCase):
     """
     Test AutomatedMacroTask methods.
     """
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/tests/test_task_events.py` & `imio.schedule-2.2.2/src/imio/schedule/tests/test_task_events.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 
 from mock import Mock
 
 from plone import api
 
 from zope.event import notify
 from zope.lifecycleevent import ObjectModifiedEvent
+from zope.globalrequest import setRequest
 
 
 class TestTaskCreation(ExampleScheduleFunctionalTestCase):
     """
     Test task creation with different changes of TaskContainer.
     """
 
     def setUp(self):
         super(TestTaskCreation, self).setUp()
         self._adapter_computed_due_date = CalculationDefaultDelay.compute_due_date
+        setRequest(self.portal.REQUEST)
 
     def tearDown(self):
         CalculationDefaultDelay.compute_due_date = self._adapter_computed_due_date
         super(TestTaskCreation, self).tearDown()
 
     def test_task_creation_on_container_modification(self):
         """
@@ -60,16 +62,16 @@
         and starting_states.
         """
         empty_task_container = self.empty_task_container
         msg = "so far, no task should have been created"
         self.assertEquals(len(empty_task_container.objectValues()), 0, msg)
 
         # do workflow change
-        api.content.transition(empty_task_container, transition='submit')
-        api.content.transition(empty_task_container, transition='retract')
+        api.content.transition(empty_task_container, transition="submit")
+        api.content.transition(empty_task_container, transition="retract")
 
         created = empty_task_container.objectValues()
         created = created and created[0]
 
         # a task should have been created
         msg = "A task should have been created"
         self.assertTrue(created, msg)
@@ -82,17 +84,15 @@
     def test_task_creation_on_container_creation(self):
         """
         When creating a contentype scheduled with a ScheduleConfig
         Task should created automatically depending on start conditions
         and starting_states.
         """
         new_task_container = api.content.create(
-            type='Folder',
-            id='new_task_container',
-            container=self.portal
+            type="Folder", id="new_task_container", container=self.portal
         )
 
         created = new_task_container.objectValues()
         created = created and created[0]
 
         # a task should have been created
         msg = "A task should have been created"
@@ -104,23 +104,23 @@
         self.assertTrue(IAutomatedTask.providedBy(created), msg)
 
     def test_assigned_user_is_set_on_created_task(self):
         """
         Check that the assigned user is set on an
         automatically created task.
         """
-        msg = 'default assigned user should have been admin'
-        self.assertEquals(self.task.assigned_user, 'admin', msg)
+        msg = "default assigned user should have been admin"
+        self.assertEquals(self.task.assigned_user, "admin", msg)
 
     def test_due_date_is_set_on_created_task(self):
         """
         Check that the computed due date is set on an
         automatically created task.
         """
-        msg = 'default du date should have been today + 10 days'
+        msg = "default du date should have been today + 10 days"
         due_date = self.task.due_date
         expected_date = self.task_container.creation_date
         delay = relativedelta(days=self.task_config.additional_delay)
         expected_date = expected_date.asdatetime().date() + delay
         self.assertEquals(due_date, expected_date, msg)
 
     def test_schedule_config_UID_is_set_on_created_task(self):
@@ -155,47 +155,47 @@
         Task should started automatically depending on start conditions
         and starting_states.
         """
         task_container = self.task_container
         task = self.task
 
         # put the task container on 'pending' state to match 'starting states'
-        api.content.transition(task_container, transition='submit')
+        api.content.transition(task_container, transition="submit")
         # reopen the task to be sure it was not closed before the container
         # modification
-        if api.content.get_state(task) == 'to_do':
-            api.content.transition(task, 'back_in_to_assign')
+        if api.content.get_state(task) == "to_do":
+            api.content.transition(task, "back_in_to_assign")
         msg = "The task should not be started yet ! (for the sake of the test)"
-        self.assertNotEquals(api.content.get_state(task), 'to_do', msg)
+        self.assertNotEquals(api.content.get_state(task), "to_do", msg)
 
         # simulate modification
         notify(ObjectModifiedEvent(task_container))
 
         # the task should have been started
         msg = "The task should have been started"
-        self.assertEquals(api.content.get_state(task), 'to_do', msg)
+        self.assertEquals(api.content.get_state(task), "to_do", msg)
 
     def test_task_starting_on_container_workflow_modification(self):
         """
         When changing state a contentype scheduled with a ScheduleConfig
         Task should started automatically depending on start conditions
         and starting_states.
         """
         task_container = self.task_container
         task = self.task
 
         msg = "The task should not be closed yet ! (for the sake of the test)"
-        self.assertNotEquals(api.content.get_state(task), 'to_do', msg)
+        self.assertNotEquals(api.content.get_state(task), "to_do", msg)
 
         # do workflow change
-        api.content.transition(task_container, transition='submit')
+        api.content.transition(task_container, transition="submit")
 
         # the task should have been started
         msg = "The task should have been started"
-        self.assertEquals(api.content.get_state(task), 'to_do', msg)
+        self.assertEquals(api.content.get_state(task), "to_do", msg)
 
 
 class TestTaskUpdate(ExampleScheduleFunctionalTestCase):
     """
     Test task update with different changes of TaskContainer.
     """
 
@@ -232,51 +232,55 @@
         CalculationDefaultDelay.calculate_delay = Mock(return_value=42)
         msg = "The task due date should not have changed"
         self.assertEquals(task.due_date, old_due_date)
 
         # simulate modification
         notify(ObjectModifiedEvent(task_container))
 
-        catalog = api.portal.get_tool('portal_catalog')
-        msg = 'catalog should not find anything with old due date'
+        catalog = api.portal.get_tool("portal_catalog")
+        msg = "catalog should not find anything with old due date"
         task_brain = catalog(due_date=old_due_date, UID=task.UID())
         self.assertFalse(task_brain, msg)
-        msg = 'new due date should have been reindexed'
+        msg = "new due date should have been reindexed"
         task_brain = catalog(due_date=task.due_date, UID=task.UID())
         self.assertTrue(task_brain, msg)
 
 
 class TestMacroTaskUpdate(MacroTaskScheduleFunctionalTestCase):
     """
     Test task update with different changes of TaskContainer.
     """
 
     def tearDown(self):
-        api.content.transition(obj=self.macro_task, to_state='created')
+        api.content.transition(obj=self.macro_task, to_state="created")
 
     def test_update_recurrence_handler(self):
         """
         When modifying a contenttype the recurrence should be evaluated
         """
-        transitions = ['do_to_assign', 'do_realized', 'do_closed']
+        transitions = ["do_to_assign", "do_realized", "do_closed"]
         self.macrotask_config.activate_recurrency = True
-        self.macrotask_config.recurrence_conditions = self.macrotask_config.creation_conditions
-        self.macrotask_config.recurrence_states = ('private', )
+        self.macrotask_config.recurrence_conditions = (
+            self.macrotask_config.creation_conditions
+        )
+        self.macrotask_config.recurrence_states = ("private",)
 
         self.subtask_config.activate_recurrency = True
-        self.subtask_config.recurrence_conditions = self.subtask_config.creation_conditions
-        self.subtask_config.recurrence_states = ('private', )
+        self.subtask_config.recurrence_conditions = (
+            self.subtask_config.creation_conditions
+        )
+        self.subtask_config.recurrence_states = ("private",)
 
         for transition in transitions:
             api.content.transition(obj=self.macro_task, transition=transition)
         notify(ObjectModifiedEvent(self.task_container))
 
-        self.assertTrue('TASK_test_macrotaskconfig-1' in self.task_container)
-        macro_task = self.task_container['TASK_test_macrotaskconfig-1']
-        self.assertTrue('TASK_test_subtaskconfig' in macro_task)
+        self.assertTrue("TASK_test_macrotaskconfig-1" in self.task_container)
+        macro_task = self.task_container["TASK_test_macrotaskconfig-1"]
+        self.assertTrue("TASK_test_subtaskconfig" in macro_task)
         for transition in transitions:
             api.content.transition(obj=macro_task, transition=transition)
 
 
 class TestTaskEnding(ExampleScheduleFunctionalTestCase):
     """
     Test task ending with different changes of TaskContainer.
@@ -288,47 +292,47 @@
         Task should ended automatically depending on end conditions
         and ending_states.
         """
         task_container = self.task_container
         task = self.task
 
         # put the task container on 'published' state to match 'ending states'
-        api.content.transition(task_container, transition='publish')
+        api.content.transition(task_container, transition="publish")
         # reopen the task to be sure it was not closed before the container
         # modification
-        if api.content.get_state(task) == 'closed':
-            api.content.transition(task, 'back_in_realized')
+        if api.content.get_state(task) == "closed":
+            api.content.transition(task, "back_in_realized")
         msg = "The task should not be closed yet ! (for the sake of the test)"
-        self.assertNotEquals(api.content.get_state(task), 'closed', msg)
+        self.assertNotEquals(api.content.get_state(task), "closed", msg)
 
         # simulate modification
         notify(ObjectModifiedEvent(task_container))
 
         # the task should have been ended
         msg = "The task should have been ended"
-        self.assertEquals(api.content.get_state(task), 'closed', msg)
+        self.assertEquals(api.content.get_state(task), "closed", msg)
 
     def test_task_ending_on_container_workflow_modification(self):
         """
         When changing state a contentype scheduled with a ScheduleConfig
         Task should ended automatically depending on end conditions
         and ending_states.
         """
         task_container = self.task_container
         task = self.task
 
         msg = "The task should not be closed yet ! (for the sake of the test)"
-        self.assertNotEquals(api.content.get_state(task), 'closed', msg)
+        self.assertNotEquals(api.content.get_state(task), "closed", msg)
 
         # do workflow change
-        api.content.transition(task_container, transition='publish')
+        api.content.transition(task_container, transition="publish")
 
         # the task should have been ended
         msg = "The task should have been ended"
-        self.assertEquals(api.content.get_state(task), 'closed', msg)
+        self.assertEquals(api.content.get_state(task), "closed", msg)
 
 
 class TestTaskFreezing(ExampleScheduleFunctionalTestCase):
     """
     Test task freezing with different changes of TaskContainer.
     """
 
@@ -337,52 +341,52 @@
         When modifying a contentype scheduled with a ScheduleConfig
         Task should froze automatically depending on freeze conditions
         and freezing_states.
         """
         task_container = self.task_container
         task = self.task
         task_config = self.task_config
-        task_config.ending_states = ['published']
-        task_config.freeze_states = ['private']
+        task_config.ending_states = ["published"]
+        task_config.freeze_states = ["private"]
 
         msg = "The task should not be closed or frozen yet ! (for the sake of the test)"
-        self.assertNotEquals(task.get_state(), 'closed', msg)
-        self.assertNotEquals(task.get_state(), 'frozen', msg)
+        self.assertNotEquals(task.get_state(), "closed", msg)
+        self.assertNotEquals(task.get_state(), "frozen", msg)
         msg = "The task container should  be in private state"
-        self.assertEquals(api.content.get_state(task_container), 'private', msg)
+        self.assertEquals(api.content.get_state(task_container), "private", msg)
 
         # simulate modification
         notify(ObjectModifiedEvent(task_container))
 
         # the task should have been frozen
         msg = "The task should have been frozen"
-        self.assertEquals(api.content.get_state(task), 'frozen', msg)
+        self.assertEquals(api.content.get_state(task), "frozen", msg)
 
     def test_task_freezing_on_container_workflow_modification(self):
         """
         When changing state a contentype scheduled with a ScheduleConfig
         Task should froze automatically depending on freeze conditions
         and freezing_states.
         """
         task_container = self.task_container
         task = self.task
         task_config = self.task_config
-        task_config.ending_states = ['private']
-        task_config.freeze_states = ['published']
+        task_config.ending_states = ["private"]
+        task_config.freeze_states = ["published"]
 
         msg = "The task should not be closed or frozen yet ! (for the sake of the test)"
-        self.assertNotEquals(task.get_state(), 'closed', msg)
-        self.assertNotEquals(task.get_state(), 'frozen', msg)
+        self.assertNotEquals(task.get_state(), "closed", msg)
+        self.assertNotEquals(task.get_state(), "frozen", msg)
 
         # do workflow change
-        api.content.transition(task_container, transition='publish')
+        api.content.transition(task_container, transition="publish")
 
         # the task should have been frozen
         msg = "The task should have been frozen"
-        self.assertEquals(task.get_state(), 'frozen', msg)
+        self.assertEquals(task.get_state(), "frozen", msg)
 
 
 class TestTaskThawing(ExampleScheduleFunctionalTestCase):
     """
     Test task thawing with different changes of TaskContainer.
     """
 
@@ -391,26 +395,26 @@
         When modifying a contentype scheduled with a ScheduleConfig
         Task should froze automatically depending on thaw conditions
         and thawing_states.
         """
         task_container = self.task_container
         task = self.task
         task_config = self.task_config
-        task_config.ending_states = ['published']
-        task_config.thaw_states = ['private']
+        task_config.ending_states = ["published"]
+        task_config.thaw_states = ["private"]
 
         task_original_state = task.get_state()
         msg = "The task original state should not be frozen! (for the sake of the test)"
-        self.assertNotEquals(task_original_state, 'frozen', msg)
+        self.assertNotEquals(task_original_state, "frozen", msg)
         msg = "The task container should  be in private state"
-        self.assertEquals(api.content.get_state(task_container), 'private', msg)
+        self.assertEquals(api.content.get_state(task_container), "private", msg)
 
         # freeze task
         task_config.freeze_task(task)
-        self.assertEquals(task.get_state(), 'frozen', msg)
+        self.assertEquals(task.get_state(), "frozen", msg)
         # simulate modification
         notify(ObjectModifiedEvent(task_container))
 
         # the task should have been thawed
         msg = "The task should have been thawed"
         self.assertEquals(api.content.get_state(task), task_original_state, msg)
 
@@ -419,23 +423,23 @@
         When changing state a contentype scheduled with a ScheduleConfig
         Task should froze automatically depending on thaw conditions
         and thawing_states.
         """
         task_container = self.task_container
         task = self.task
         task_config = self.task_config
-        task_config.freeze_states = ['private']
-        task_config.thaw_states = ['published']
+        task_config.freeze_states = ["private"]
+        task_config.thaw_states = ["published"]
 
         task_original_state = task.get_state()
         msg = "The task original state should not be frozen! (for the sake of the test)"
-        self.assertNotEquals(task_original_state, 'frozen', msg)
+        self.assertNotEquals(task_original_state, "frozen", msg)
 
         # freeze task
         task_config.freeze_task(task)
-        self.assertEquals(task.get_state(), 'frozen', msg)
+        self.assertEquals(task.get_state(), "frozen", msg)
         # do workflow change
-        api.content.transition(task_container, transition='publish')
+        api.content.transition(task_container, transition="publish")
 
         # the task should have been thawed
         msg = "The task should have been thawed"
         self.assertEquals(task.get_state(), task_original_state, msg)
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/tests/test_taskconfig.py` & `imio.schedule-2.2.2/src/imio/schedule/tests/test_taskconfig.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,365 +1,369 @@
 # -*- coding: utf-8 -*-
 
 from Acquisition import aq_base
 from DateTime import DateTime
 from datetime import datetime
 from dateutil.relativedelta import relativedelta
-
 from imio.schedule.config import DONE
 from imio.schedule.content.delay import CalculationDefaultDelay
 from imio.schedule.content.task import AutomatedMacroTask
 from imio.schedule.content.task import AutomatedTask
 from imio.schedule.testing import ExampleScheduleIntegrationTestCase
 from imio.schedule.testing import MacroTaskScheduleIntegrationTestCase
 from imio.schedule.testing import TEST_INSTALL_INTEGRATION
-
 from mock import Mock
 from plone import api
-
 from zope.annotation import IAnnotations
+from zope.globalrequest import setRequest
 
 import unittest
 
 
 class TestTaskConfig(unittest.TestCase):
     """
     Test TaskConfig content type.
     """
 
     layer = TEST_INSTALL_INTEGRATION
 
     def test_TaskConfig_portal_type_is_registered(self):
-        portal_types = api.portal.get_tool('portal_types')
+        portal_types = api.portal.get_tool("portal_types")
         registered_types = portal_types.listContentTypes()
-        self.assertTrue('TaskConfig' in registered_types)
+        self.assertTrue("TaskConfig" in registered_types)
 
 
 class TestTaskConfigFields(ExampleScheduleIntegrationTestCase):
     """
     Test schema fields declaration.
     """
 
     def test_class_registration(self):
         """
         Check if the class of the content type TaskConfig is the
         correct one.
         """
         from imio.schedule.content.task_config import TaskConfig
+
         self.assertTrue(self.task_config.__class__ == TaskConfig)
 
     def test_schema_registration(self):
         """
         Check if the schema Interface of the content type TaskConfig is the
         correct one.
         """
-        portal_types = api.portal.get_tool('portal_types')
+        portal_types = api.portal.get_tool("portal_types")
         taskconfig_type = portal_types.get(self.task_config.portal_type)
-        self.assertTrue('ITaskConfig' in taskconfig_type.schema)
+        self.assertTrue("ITaskConfig" in taskconfig_type.schema)
 
     def test_enabled_attribute(self):
         task_config = aq_base(self.task_config)
-        self.assertTrue(hasattr(task_config, 'enabled'))
+        self.assertTrue(hasattr(task_config, "enabled"))
 
     def test_enabled_field_display(self):
         self.browser.open(self.task_config.absolute_url())
         contents = self.browser.contents
         msg = "field 'enabled' is not displayed"
         self.assertTrue('id="form-widgets-enabled"' in contents, msg)
         msg = "field 'enabled' is not translated"
-        self.assertTrue('Activé' in contents, msg)
+        self.assertTrue("Activé" in contents, msg)
 
     def test_enabled_field_edit(self):
-        self.browser.open(self.task_config.absolute_url() + '/edit')
+        self.browser.open(self.task_config.absolute_url() + "/edit")
         contents = self.browser.contents
         msg = "field 'enabled' is not editable"
-        self.assertTrue('Activé' in contents, msg)
+        self.assertTrue("Activé" in contents, msg)
 
     def test_default_assigned_user_attribute(self):
         task_config = aq_base(self.task_config)
-        self.assertTrue(hasattr(task_config, 'default_assigned_user'))
+        self.assertTrue(hasattr(task_config, "default_assigned_user"))
 
     def test_default_assigned_user_field_display(self):
         self.browser.open(self.task_config.absolute_url())
         contents = self.browser.contents
         msg = "field 'default_assigned_user' is not displayed"
         self.assertTrue('id="form-widgets-default_assigned_user"' in contents, msg)
         msg = "field 'default_assigned_user' is not translated"
-        self.assertTrue('Responsable de la tâche' in contents, msg)
+        self.assertTrue("Responsable de la tâche" in contents, msg)
 
     def test_default_assigned_user_field_edit(self):
-        self.browser.open(self.task_config.absolute_url() + '/edit')
+        self.browser.open(self.task_config.absolute_url() + "/edit")
         contents = self.browser.contents
         msg = "field 'default_assigned_user' is not editable"
-        self.assertTrue('Responsable de la tâche' in contents, msg)
+        self.assertTrue("Responsable de la tâche" in contents, msg)
 
     def test_creation_conditions_attribute(self):
         task_config = aq_base(self.task_config)
-        self.assertTrue(hasattr(task_config, 'creation_conditions'))
+        self.assertTrue(hasattr(task_config, "creation_conditions"))
 
     def test_creation_conditions_field_display(self):
         self.browser.open(self.task_config.absolute_url())
         contents = self.browser.contents
         msg = "field 'creation_conditions' is not displayed"
         self.assertTrue('id="form-widgets-creation_conditions"' in contents, msg)
         msg = "field 'creation_conditions' is not translated"
-        self.assertTrue('Conditions de création' in contents, msg)
+        self.assertTrue("Conditions de création" in contents, msg)
 
     def test_creation_conditions_field_edit(self):
-        self.browser.open(self.task_config.absolute_url() + '/edit')
+        self.browser.open(self.task_config.absolute_url() + "/edit")
         contents = self.browser.contents
         msg = "field 'creation_conditions' is not editable"
-        self.assertTrue('Conditions de création' in contents, msg)
+        self.assertTrue("Conditions de création" in contents, msg)
 
     def test_creation_state_attribute(self):
         task_config = aq_base(self.task_config)
-        self.assertTrue(hasattr(task_config, 'creation_state'))
+        self.assertTrue(hasattr(task_config, "creation_state"))
 
     def test_creation_state_field_display(self):
         self.browser.open(self.task_config.absolute_url())
         contents = self.browser.contents
         msg = "field 'creation_state' is not displayed"
         self.assertTrue('id="form-widgets-creation_state"' in contents, msg)
         msg = "field 'creation_state' is not translated"
-        self.assertTrue('État de création de la tâche' in contents, msg)
+        self.assertTrue("État de création de la tâche" in contents, msg)
 
     def test_creation_state_field_edit(self):
-        self.browser.open(self.task_config.absolute_url() + '/edit')
+        self.browser.open(self.task_config.absolute_url() + "/edit")
         contents = self.browser.contents
         msg = "field 'creation_state' is not editable"
-        self.assertTrue('État de création de la tâche' in contents, msg)
+        self.assertTrue("État de création de la tâche" in contents, msg)
 
     def test_start_conditions_attribute(self):
         task_config = aq_base(self.task_config)
-        self.assertTrue(hasattr(task_config, 'start_conditions'))
+        self.assertTrue(hasattr(task_config, "start_conditions"))
 
     def test_start_conditions_field_display(self):
         self.browser.open(self.task_config.absolute_url())
         contents = self.browser.contents
         msg = "field 'start_conditions' is not displayed"
         self.assertTrue('id="form-widgets-start_conditions"' in contents, msg)
         msg = "field 'start_conditions' is not translated"
-        self.assertTrue('Conditions de création' in contents, msg)
+        self.assertTrue("Conditions de création" in contents, msg)
 
     def test_start_conditions_field_edit(self):
-        self.browser.open(self.task_config.absolute_url() + '/edit')
+        self.browser.open(self.task_config.absolute_url() + "/edit")
         contents = self.browser.contents
         msg = "field 'start_conditions' is not editable"
-        self.assertTrue('Conditions de création' in contents, msg)
+        self.assertTrue("Conditions de création" in contents, msg)
 
     def test_starting_states_attribute(self):
         task_config = aq_base(self.task_config)
-        self.assertTrue(hasattr(task_config, 'starting_states'))
+        self.assertTrue(hasattr(task_config, "starting_states"))
 
     def test_starting_states_field_display(self):
         self.browser.open(self.task_config.absolute_url())
         contents = self.browser.contents
         msg = "field 'starting_states' is not displayed"
         self.assertTrue('id="form-widgets-starting_states"' in contents, msg)
         msg = "field 'starting_states' is not translated"
-        self.assertTrue('État(s) de démarrage de la tâche' in contents, msg)
+        self.assertTrue("État(s) de démarrage de la tâche" in contents, msg)
 
     def test_starting_states_field_edit(self):
-        self.browser.open(self.task_config.absolute_url() + '/edit')
+        self.browser.open(self.task_config.absolute_url() + "/edit")
         contents = self.browser.contents
         msg = "field 'starting_states' is not editable"
-        self.assertTrue('État(s) de démarrage de la tâche' in contents, msg)
+        self.assertTrue("État(s) de démarrage de la tâche" in contents, msg)
 
     def test_end_conditions_attribute(self):
         task_config = aq_base(self.task_config)
-        self.assertTrue(hasattr(task_config, 'end_conditions'))
+        self.assertTrue(hasattr(task_config, "end_conditions"))
 
     def test_end_conditions_field_display(self):
         self.browser.open(self.task_config.absolute_url())
         contents = self.browser.contents
         msg = "field 'end_conditions' is not displayed"
         self.assertTrue('id="form-widgets-end_conditions"' in contents, msg)
         msg = "field 'end_conditions' is not translated"
-        self.assertTrue('Conditions de clôture' in contents, msg)
+        self.assertTrue("Conditions de clôture" in contents, msg)
 
     def test_end_conditions_field_edit(self):
-        self.browser.open(self.task_config.absolute_url() + '/edit')
+        self.browser.open(self.task_config.absolute_url() + "/edit")
         contents = self.browser.contents
         msg = "field 'end_conditions' is not editable"
-        self.assertTrue('Conditions de clôture' in contents, msg)
+        self.assertTrue("Conditions de clôture" in contents, msg)
 
     def test_ending_states_attribute(self):
         task_config = aq_base(self.task_config)
-        self.assertTrue(hasattr(task_config, 'ending_states'))
+        self.assertTrue(hasattr(task_config, "ending_states"))
 
     def test_ending_states_field_display(self):
         self.browser.open(self.task_config.absolute_url())
         contents = self.browser.contents
         msg = "field 'ending_states' is not displayed"
         self.assertTrue('id="form-widgets-ending_states"' in contents, msg)
         msg = "field 'ending_states' is not translated"
-        self.assertTrue('État(s) de clôture de la tâche' in contents, msg)
+        self.assertTrue("État(s) de clôture de la tâche" in contents, msg)
 
     def test_ending_states_field_edit(self):
-        self.browser.open(self.task_config.absolute_url() + '/edit')
+        self.browser.open(self.task_config.absolute_url() + "/edit")
         contents = self.browser.contents
         msg = "field 'ending_states' is not editable"
-        self.assertTrue('État(s) de clôture de la tâche' in contents, msg)
+        self.assertTrue("État(s) de clôture de la tâche" in contents, msg)
 
     def test_freeze_conditions_attribute(self):
         task_config = aq_base(self.task_config)
-        self.assertTrue(hasattr(task_config, 'freeze_conditions'))
+        self.assertTrue(hasattr(task_config, "freeze_conditions"))
 
     def test_freeze_conditions_field_display(self):
         self.browser.open(self.task_config.absolute_url())
         contents = self.browser.contents
         msg = "field 'freeze_conditions' is not displayed"
         self.assertTrue('id="form-widgets-freeze_conditions"' in contents, msg)
         msg = "field 'freeze_conditions' is not translated"
-        self.assertTrue('Conditions de gel' in contents, msg)
+        self.assertTrue("Conditions de gel" in contents, msg)
 
     def test_freeze_conditions_field_edit(self):
-        self.browser.open(self.task_config.absolute_url() + '/edit')
+        self.browser.open(self.task_config.absolute_url() + "/edit")
         contents = self.browser.contents
         msg = "field 'freeze_conditions' is not editable"
-        self.assertTrue('Conditions de gel' in contents, msg)
+        self.assertTrue("Conditions de gel" in contents, msg)
 
     def test_freeze_states_attribute(self):
         task_config = aq_base(self.task_config)
-        self.assertTrue(hasattr(task_config, 'freeze_states'))
+        self.assertTrue(hasattr(task_config, "freeze_states"))
 
     def test_freeze_states_field_display(self):
         self.browser.open(self.task_config.absolute_url())
         contents = self.browser.contents
         msg = "field 'freeze_states' is not displayed"
         self.assertTrue('id="form-widgets-freeze_states"' in contents, msg)
         msg = "field 'freeze_states' is not translated"
-        self.assertTrue('État(s) de gel de la tâche' in contents, msg)
+        self.assertTrue("État(s) de gel de la tâche" in contents, msg)
 
     def test_freeze_states_field_edit(self):
-        self.browser.open(self.task_config.absolute_url() + '/edit')
+        self.browser.open(self.task_config.absolute_url() + "/edit")
         contents = self.browser.contents
         msg = "field 'freeze_states' is not editable"
-        self.assertTrue('État(s) de gel de la tâche' in contents, msg)
+        self.assertTrue("État(s) de gel de la tâche" in contents, msg)
 
     def test_thaw_conditions_attribute(self):
         task_config = aq_base(self.task_config)
-        self.assertTrue(hasattr(task_config, 'thaw_conditions'))
+        self.assertTrue(hasattr(task_config, "thaw_conditions"))
 
     def test_thaw_conditions_field_display(self):
         self.browser.open(self.task_config.absolute_url())
         contents = self.browser.contents
         msg = "field 'thaw_conditions' is not displayed"
         self.assertTrue('id="form-widgets-thaw_conditions"' in contents, msg)
         msg = "field 'thaw_conditions' is not translated"
-        self.assertTrue('Conditions de dégel' in contents, msg)
+        self.assertTrue("Conditions de dégel" in contents, msg)
 
     def test_thaw_conditions_field_edit(self):
-        self.browser.open(self.task_config.absolute_url() + '/edit')
+        self.browser.open(self.task_config.absolute_url() + "/edit")
         contents = self.browser.contents
         msg = "field 'thaw_conditions' is not editable"
-        self.assertTrue('Conditions de dégel' in contents, msg)
+        self.assertTrue("Conditions de dégel" in contents, msg)
 
     def test_thaw_states_attribute(self):
         task_config = aq_base(self.task_config)
-        self.assertTrue(hasattr(task_config, 'thaw_states'))
+        self.assertTrue(hasattr(task_config, "thaw_states"))
 
     def test_thaw_states_field_display(self):
         self.browser.open(self.task_config.absolute_url())
         contents = self.browser.contents
         msg = "field 'thaw_states' is not displayed"
         self.assertTrue('id="form-widgets-thaw_states"' in contents, msg)
         msg = "field 'thaw_states' is not translated"
-        self.assertTrue('État(s) de dégel de la tâche' in contents, msg)
+        self.assertTrue("État(s) de dégel de la tâche" in contents, msg)
 
     def test_thaw_states_field_edit(self):
-        self.browser.open(self.task_config.absolute_url() + '/edit')
+        self.browser.open(self.task_config.absolute_url() + "/edit")
         contents = self.browser.contents
         msg = "field 'thaw_states' is not editable"
-        self.assertTrue('État(s) de dégel de la tâche' in contents, msg)
+        self.assertTrue("État(s) de dégel de la tâche" in contents, msg)
 
     def test_start_date_attribute(self):
         task_config = aq_base(self.task_config)
-        self.assertTrue(hasattr(task_config, 'start_date'))
+        self.assertTrue(hasattr(task_config, "start_date"))
 
     def test_start_date_field_display(self):
         self.browser.open(self.task_config.absolute_url())
         contents = self.browser.contents
         msg = "field 'start_date' is not displayed"
         self.assertTrue('id="form-widgets-start_date"' in contents, msg)
         msg = "field 'start_date' is not translated"
-        self.assertTrue('Date de départ' in contents, msg)
+        self.assertTrue("Date de départ" in contents, msg)
 
     def test_start_date_field_edit(self):
-        self.browser.open(self.task_config.absolute_url() + '/edit')
+        self.browser.open(self.task_config.absolute_url() + "/edit")
         contents = self.browser.contents
         msg = "field 'start_date' is not editable"
-        self.assertTrue('Date de départ' in contents, msg)
+        self.assertTrue("Date de départ" in contents, msg)
 
     def test_calculation_delay_attribute(self):
         task_config = aq_base(self.task_config)
-        self.assertTrue(hasattr(task_config, 'additional_delay'))
+        self.assertTrue(hasattr(task_config, "additional_delay"))
 
     def test_calculation_delay_field_display(self):
         self.browser.open(self.task_config.absolute_url())
         contents = self.browser.contents
         msg = "field 'calculation_delay' is not displayed"
         self.assertTrue('id="form-widgets-calculation_delay"' in contents, msg)
         msg = "field 'calculation_delay' is not translated"
-        self.assertTrue('Calcul du délai' in contents, msg)
+        self.assertTrue("Calcul du délai" in contents, msg)
 
     def test_calculation_delay_field_edit(self):
-        self.browser.open(self.task_config.absolute_url() + '/edit')
+        self.browser.open(self.task_config.absolute_url() + "/edit")
         contents = self.browser.contents
         msg = "field 'calculation_delay' is not editable"
-        self.assertTrue('Calcul du délai' in contents, msg)
+        self.assertTrue("Calcul du délai" in contents, msg)
 
     def test_additional_delay_attribute(self):
         task_config = aq_base(self.task_config)
-        self.assertTrue(hasattr(task_config, 'additional_delay'))
+        self.assertTrue(hasattr(task_config, "additional_delay"))
 
     def test_additional_delay_field_display(self):
         self.browser.open(self.task_config.absolute_url())
         contents = self.browser.contents
         msg = "field 'additional_delay' is not displayed"
         self.assertTrue('id="form-widgets-additional_delay"' in contents, msg)
         msg = "field 'additional_delay' is not translated"
-        self.assertTrue('Délai supplémentaire' in contents, msg)
+        self.assertTrue("Délai supplémentaire" in contents, msg)
 
     def test_additional_delay_field_edit(self):
-        self.browser.open(self.task_config.absolute_url() + '/edit')
+        self.browser.open(self.task_config.absolute_url() + "/edit")
         contents = self.browser.contents
         msg = "field 'additional_delay' is not editable"
-        self.assertTrue('Délai supplémentaire' in contents, msg)
+        self.assertTrue("Délai supplémentaire" in contents, msg)
 
 
 class TestTaskConfigMethodsIntegration(ExampleScheduleIntegrationTestCase):
     """
     Test TaskConfig methods.
     """
 
     def setUp(self):
         super(TestTaskConfigMethodsIntegration, self).setUp()
         self._evaluate_one_condition = self.task_config.evaluate_one_condition
         self._evaluate_conditions = self.task_config.evaluate_conditions
         self._match_recurrence_states = self.task_config.match_recurrence_states
         self._create_task = self.task_config.create_task
+        self._additional_delay = self.task_config.additional_delay
+        self._additional_delay_tal = self.task_config.additional_delay_tal
         self._api_get_state = api.content.get_state
         self._adapter_computed_due_date = CalculationDefaultDelay.compute_due_date
+        setRequest(self.portal.REQUEST)
 
     def tearDown(self):
         self.task_config.evaluate_one_condition = self._evaluate_one_condition
         self.task_config.evaluate_conditions = self._evaluate_conditions
         self.task_config.match_recurrence_states = self._match_recurrence_states
         self.task_config.create_task = self._create_task
+        self.task_config.additional_delay = self._additional_delay
+        self.task_config.additional_delay_tal = self._additional_delay_tal
         api.content.get_state = self._api_get_state
         CalculationDefaultDelay.compute_due_date = self._adapter_computed_due_date
         super(TestTaskConfigMethodsIntegration, self).tearDown()
 
     def test_get_task_type(self):
         """
         Should return 'AutomatedTask'
         """
         task_type = self.task_config.get_task_type()
-        expected_type = 'AutomatedTask'
+        expected_type = "AutomatedTask"
         self.assertEquals(task_type, expected_type)
 
     def test_is_main_taskconfig(self):
         """
         Tells wheter a task config is a subtaskconfig or not
         """
         msg = "this simple task config should be considered as a main task config"
@@ -375,15 +379,15 @@
 
     def test_get_scheduled_portal_type(self):
         """
         Sould return the portal_type of the content type selected on the field
         'scheduled_contenttype' of the parent ScheduleConfig.
         """
         portal_type = self.task_config.get_scheduled_portal_type()
-        expected_type = 'Folder'
+        expected_type = "Folder"
         self.assertEquals(portal_type, expected_type)
 
     def test_get_scheduled_interfaces(self):
         """
         Should return the Interface (or a class) of the content type selected
         on the field 'scheduled_contenttype' of the parent ScheduleConfig.
         """
@@ -398,15 +402,15 @@
         Should return a user to assign on a task.
         """
         task_config = self.task_config
         task_container = self.task_container
         task = self.task
 
         user = task_config.user_to_assign(task_container, task)
-        expected_user = 'test-user'
+        expected_user = "test-user"
         msg = "should have return '{}' user id".format(expected_user)
         self.assertEquals(user, expected_user, msg)
 
     def test_get_task_instances(self):
         """
         Should return AutomatedTask brains in a container created from a given TaskConfig.
         """
@@ -459,15 +463,15 @@
         task = self.task
 
         # so far nothing should be found
         task_found = task_config.get_started_task(task_container)
         self.assertFalse(task_found)
 
         # start the task
-        api.content.transition(obj=task, transition='do_to_assign')
+        api.content.transition(obj=task, transition="do_to_assign")
 
         task_found = task_config.get_started_task(task_container)
         msg = "should have found the started task"
         self.assertEquals(task_found, task, msg)
 
     def test_get_open_task(self):
         """
@@ -479,15 +483,15 @@
         task = self.task
 
         task_found = task_config.get_open_task(task_container)
         msg = "should have found the created task"
         self.assertEquals(task_found, task, msg)
 
         # start the task
-        api.content.transition(obj=task, transition='do_to_assign')
+        api.content.transition(obj=task, transition="do_to_assign")
 
         task_found = task_config.get_open_task(task_container)
         msg = "should have found the started task"
         self.assertEquals(task_found, task, msg)
 
         # close the task
         task_config.end_task(task)
@@ -597,28 +601,40 @@
         task_config.enabled = False
         msg = "Task should not be created because the creation condition is not matched"
         self.assertFalse(task_config.should_create_task(empty_task_container), msg)
 
         # set the task_config field 'creation_conditions' with a negative condition
         # => task should not be created
         task_config.enabled = True
-        task_config.creation_conditions = [type('condition', (object, ), {
-            'condition': 'schedule.negative_creation_condition',
-            'operator': 'AND',
-        })()]
+        task_config.creation_conditions = [
+            type(
+                "condition",
+                (object,),
+                {
+                    "condition": "schedule.negative_creation_condition",
+                    "operator": "AND",
+                },
+            )()
+        ]
         msg = "Task should not be created because the creation condition is not matched"
         self.assertFalse(task_config.should_create_task(empty_task_container), msg)
 
         # set the task_config starting_states field to a state different from
         # the task_container state => task should not be created
-        task_config.creation_conditions = [type('condition', (object, ), {
-            'condition': 'schedule.test_creation_condition',
-            'operator': 'AND',
-        })()]
-        task_config.creation_state = 'pending'
+        task_config.creation_conditions = [
+            type(
+                "condition",
+                (object,),
+                {
+                    "condition": "schedule.test_creation_condition",
+                    "operator": "AND",
+                },
+            )()
+        ]
+        task_config.creation_state = "pending"
         msg = "Task should not be created because the creation state does not match container state"
         self.assertFalse(task_config.should_create_task(empty_task_container), msg)
 
     def test_should_start_task(self):
         """
         Test different cases for the 'should_start_task' method.
         """
@@ -628,15 +644,15 @@
 
         # task container state is different from the states selected on
         # task_config 'starting_states' => task should not start
         msg = "Task should not be started because the starting state does not match container state"
         self.assertFalse(task_config.should_start_task(task_container, task), msg)
 
         # normal case
-        api.content.transition(obj=task_container, transition='submit')
+        api.content.transition(obj=task_container, transition="submit")
         msg = "Task should be started"
         start = task_config.should_start_task(task_container, task)
         self.assertTrue(start, msg)
 
         # no starting creation states given means any state allow task start
         task_config.starting_states = None
         start = task_config.should_start_task(task_container, task)
@@ -646,51 +662,73 @@
         # => task should not start
         task.assigned_user = None
         msg = "Task should not be started because no user is defined on the task"
         self.assertFalse(task_config.should_start_task(task_container, task), msg)
 
         # set the task_config field 'start_conditions' with a negative condition
         # => task should not start
-        task.assigned_user = 'user'
-        task_config.start_conditions = [type('condition', (object, ), {
-            'condition': 'schedule.negative_start_condition',
-            'operator': 'AND',
-        })()]
+        task.assigned_user = "user"
+        task_config.start_conditions = [
+            type(
+                "condition",
+                (object,),
+                {
+                    "condition": "schedule.negative_start_condition",
+                    "operator": "AND",
+                },
+            )()
+        ]
         msg = "Task should not be started because the start condition is not matched"
         self.assertFalse(task_config.should_start_task(task_container, task), msg)
 
         # set the task_config starting_states field to a state different from
         # the task_container state => task should not start
-        task_config.start_conditions = [type('condition', (object, ), {
-            'condition': 'schedule.test_start_condition',
-            'operator': 'AND',
-        })()]
-        task_config.starting_states = ('published',)
+        task_config.start_conditions = [
+            type(
+                "condition",
+                (object,),
+                {
+                    "condition": "schedule.test_start_condition",
+                    "operator": "AND",
+                },
+            )()
+        ]
+        task_config.starting_states = ("published",)
         msg = "Task should not be started because the starting state does not match container state"
         self.assertFalse(task_config.should_start_task(task_container, task), msg)
 
     def test_start_conditions_status(self):
         """
         Test different cases for the 'start_conditions_status' method.
         """
         task_config = self.task_config
         task_container = self.task_container
         task = self.task
 
-        matched_conditions, unmatched_conditions = task_config.start_conditions_status(task_container, task)
-        self.assertTrue(matched_conditions == ['schedule.test_start_condition'])
+        matched_conditions, unmatched_conditions = task_config.start_conditions_status(
+            task_container, task
+        )
+        self.assertTrue(matched_conditions == ["schedule.test_start_condition"])
         self.assertTrue(unmatched_conditions == [])
 
-        task_config.start_conditions = [type('condition', (object, ), {
-            'condition': 'schedule.negative_start_condition',
-            'operator': 'AND',
-        })()]
-        matched_conditions, unmatched_conditions = task_config.start_conditions_status(task_container, task)
+        task_config.start_conditions = [
+            type(
+                "condition",
+                (object,),
+                {
+                    "condition": "schedule.negative_start_condition",
+                    "operator": "AND",
+                },
+            )()
+        ]
+        matched_conditions, unmatched_conditions = task_config.start_conditions_status(
+            task_container, task
+        )
         self.assertTrue(matched_conditions == [])
-        self.assertTrue(unmatched_conditions == ['schedule.negative_start_condition'])
+        self.assertTrue(unmatched_conditions == ["schedule.negative_start_condition"])
 
     def test_should_end_task(self):
         """
         Test different cases for the 'should_end_task' method.
         """
         task_config = self.task_config
         task_container = self.task_container
@@ -698,58 +736,74 @@
 
         # task container state is different from the states selected on
         # task_config 'ending_states' => task should not end
         msg = "Task should not be ended because the ending state does not match container state"
         self.assertFalse(task_config.should_end_task(task_container, task), msg)
 
         # normal case
-        api.content.transition(obj=task_container, transition='publish')
+        api.content.transition(obj=task_container, transition="publish")
         msg = "Task should be ended"
         end = task_config.should_end_task(task_container, task)
         self.assertTrue(end, msg)
 
         # no ending creation states given means any state allow task end
         task_config.ending_states = None
         end = task_config.should_end_task(task_container, task)
         self.assertTrue(end, msg)
 
         # set the task_config field 'end_conditions' with a negative condition
         # => task should not end
-        task_config.end_conditions = [type('object', (object, ), {
-            'condition': 'schedule.negative_end_condition',
-            'operator': 'AND',
-        })()]
+        task_config.end_conditions = [
+            type(
+                "object",
+                (object,),
+                {
+                    "condition": "schedule.negative_end_condition",
+                    "operator": "AND",
+                },
+            )()
+        ]
         msg = "Task should not be ended because the end condition is not matched"
         self.assertFalse(task_config.should_end_task(task_container, task), msg)
 
         # set the task_config ending_states field to a state different from
         # the task_container state => task should not end
-        task_config.ending_states = ('pending',)
+        task_config.ending_states = ("pending",)
         msg = "Task should not be ended because the ending state does not match container state"
         self.assertFalse(task_config.should_end_task(task_container, task), msg)
 
     def test_end_conditions_status(self):
         """
         Test different cases for the 'end_conditions_status' method.
         """
         task_config = self.task_config
         task_container = self.task_container
         task = self.task
 
-        matched_conditions, unmatched_conditions = task_config.end_conditions_status(task_container, task)
-        self.assertTrue(matched_conditions == ['schedule.test_end_condition'])
+        matched_conditions, unmatched_conditions = task_config.end_conditions_status(
+            task_container, task
+        )
+        self.assertTrue(matched_conditions == ["schedule.test_end_condition"])
         self.assertTrue(unmatched_conditions == [])
 
-        task_config.end_conditions = [type('condition', (object, ), {
-            'condition': 'schedule.negative_end_condition',
-            'operator': 'AND',
-        })()]
-        matched_conditions, unmatched_conditions = task_config.end_conditions_status(task_container, task)
+        task_config.end_conditions = [
+            type(
+                "condition",
+                (object,),
+                {
+                    "condition": "schedule.negative_end_condition",
+                    "operator": "AND",
+                },
+            )()
+        ]
+        matched_conditions, unmatched_conditions = task_config.end_conditions_status(
+            task_container, task
+        )
         self.assertTrue(matched_conditions == [])
-        self.assertTrue(unmatched_conditions == ['schedule.negative_end_condition'])
+        self.assertTrue(unmatched_conditions == ["schedule.negative_end_condition"])
 
     def test_should_freeze_task(self):
         """
         Test different cases for the 'should_freeze_task' method.
         """
         task_config = self.task_config
         task_container = self.task_container
@@ -759,243 +813,284 @@
 
         # task container state is different from the states selected on
         # task_config 'freeze_states' => task should not freeze
         msg = "Task should not be frozen because the freeze state does not match container state"
         self.assertFalse(task_config.should_freeze_task(task_container, task), msg)
 
         # normal case
-        task_config.freeze_states = ['private']
+        task_config.freeze_states = ["private"]
         msg = "Task should be frozen"
         freeze = task_config.should_freeze_task(task_container, task)
         self.assertTrue(freeze, msg)
 
         # no freeze creation states given means the task should never be frozen
         task_config.freeze_states = None
         freeze = task_config.should_freeze_task(task_container, task)
         self.assertFalse(freeze, msg)
 
         # set the task_config field 'freeze_conditions' with a negative condition
         # => task should not freeze
-        task_config.freeze_states = ['private']
-        task_config.freeze_conditions = [type('object', (object, ), {
-            'condition': 'schedule.negative_freeze_condition',
-            'operator': 'AND',
-        })()]
+        task_config.freeze_states = ["private"]
+        task_config.freeze_conditions = [
+            type(
+                "object",
+                (object,),
+                {
+                    "condition": "schedule.negative_freeze_condition",
+                    "operator": "AND",
+                },
+            )()
+        ]
         msg = "Task should not be frozen because the freeze condition is not matched"
         freeze = task_config.should_freeze_task(task_container, task)
         self.assertFalse(freeze, msg)
 
         # set the task_config freeze_states field to a state different from
         # the task_container state => task should not freeze
         task_config.freeze_conditions = []
-        task_config.freeze_states = ('pending',)
+        task_config.freeze_states = ("pending",)
         msg = "Task should not be frozen because the freeze state does not match container state"
         freeze = task_config.should_freeze_task(task_container, task)
         self.assertFalse(freeze, msg)
 
     def test_freeze_conditions_status(self):
         """
         Test different cases for the 'freeze_conditions_status' method.
         """
         task_config = self.task_config
         task_container = self.task_container
         task = self.task
 
-        matched_conditions, unmatched_conditions = task_config.freeze_conditions_status(task_container, task)
-        self.assertTrue(matched_conditions == ['schedule.test_freeze_condition'])
+        matched_conditions, unmatched_conditions = task_config.freeze_conditions_status(
+            task_container, task
+        )
+        self.assertTrue(matched_conditions == ["schedule.test_freeze_condition"])
         self.assertTrue(unmatched_conditions == [])
 
-        task_config.freeze_conditions = [type('condition', (object, ), {
-            'condition': 'schedule.negative_freeze_condition',
-            'operator': 'AND',
-        })()]
-        matched_conditions, unmatched_conditions = task_config.freeze_conditions_status(task_container, task)
+        task_config.freeze_conditions = [
+            type(
+                "condition",
+                (object,),
+                {
+                    "condition": "schedule.negative_freeze_condition",
+                    "operator": "AND",
+                },
+            )()
+        ]
+        matched_conditions, unmatched_conditions = task_config.freeze_conditions_status(
+            task_container, task
+        )
         self.assertTrue(matched_conditions == [])
-        self.assertTrue(unmatched_conditions == ['schedule.negative_freeze_condition'])
+        self.assertTrue(unmatched_conditions == ["schedule.negative_freeze_condition"])
 
     def test_should_thaw_task(self):
         """
         Test different cases for the 'should_thaw_task' method.
         """
         task_config = self.task_config
         task_container = self.task_container
         task = self.task
         # freeze task befor thaw tests
         task_config.freeze_task(task)
-        self.assertEquals(api.content.get_state(task), 'frozen', 'task should be frozen')
+        self.assertEquals(
+            api.content.get_state(task), "frozen", "task should be frozen"
+        )
 
         # task container state is different from the states selected on
         # task_config 'thaw_states' => task should not thaw
         msg = "Task should not be thawed because the thaw state does not match container state"
         self.assertFalse(task_config.should_thaw_task(task_container, task), msg)
 
         # normal case
-        task_config.thaw_states = ['private']
+        task_config.thaw_states = ["private"]
         msg = "Task should be thawed"
         thaw = task_config.should_thaw_task(task_container, task)
         self.assertTrue(thaw, msg)
 
         # no thaw creation states given means the task should never be thawed
         task_config.thaw_states = None
         thaw = task_config.should_thaw_task(task_container, task)
         self.assertFalse(thaw, msg)
 
         # set the task_config field 'thaw_conditions' with a negative condition
         # => task should not thaw
-        task_config.thaw_states = ['private']
-        task_config.thaw_conditions = [type('object', (object, ), {
-            'condition': 'schedule.negative_thaw_condition',
-            'operator': 'AND',
-        })()]
+        task_config.thaw_states = ["private"]
+        task_config.thaw_conditions = [
+            type(
+                "object",
+                (object,),
+                {
+                    "condition": "schedule.negative_thaw_condition",
+                    "operator": "AND",
+                },
+            )()
+        ]
         msg = "Task should not be thawed because the thaw condition is not matched"
         thaw = task_config.should_thaw_task(task_container, task)
         self.assertFalse(thaw, msg)
 
         # set the task_config thaw_states field to a state different from
         # the task_container state => task should not thaw
         task_config.thaw_conditions = []
-        task_config.thaw_states = ('pending',)
+        task_config.thaw_states = ("pending",)
         msg = "Task should not be thawed because the thaw state does not match container state"
         thaw = task_config.should_thaw_task(task_container, task)
         self.assertFalse(thaw, msg)
 
     def test_thaw_conditions_status(self):
         """
         Test different cases for the 'thaw_conditions_status' method.
         """
         task_config = self.task_config
         task_container = self.task_container
         task = self.task
         # freeze task befor thaw tests
         task_config.freeze_task(task)
-        self.assertEquals(api.content.get_state(task), 'frozen', 'task should be frozen')
-
-        matched_conditions, unmatched_conditions = task_config.thaw_conditions_status(task_container, task)
-        self.assertTrue(matched_conditions == ['schedule.test_thaw_condition'])
+        self.assertEquals(
+            api.content.get_state(task), "frozen", "task should be frozen"
+        )
+
+        matched_conditions, unmatched_conditions = task_config.thaw_conditions_status(
+            task_container, task
+        )
+        self.assertTrue(matched_conditions == ["schedule.test_thaw_condition"])
         self.assertTrue(unmatched_conditions == [])
 
-        task_config.thaw_conditions = [type('condition', (object, ), {
-            'condition': 'schedule.negative_thaw_condition',
-            'operator': 'AND',
-        })()]
-        matched_conditions, unmatched_conditions = task_config.thaw_conditions_status(task_container, task)
+        task_config.thaw_conditions = [
+            type(
+                "condition",
+                (object,),
+                {
+                    "condition": "schedule.negative_thaw_condition",
+                    "operator": "AND",
+                },
+            )()
+        ]
+        matched_conditions, unmatched_conditions = task_config.thaw_conditions_status(
+            task_container, task
+        )
         self.assertTrue(matched_conditions == [])
-        self.assertTrue(unmatched_conditions == ['schedule.negative_thaw_condition'])
+        self.assertTrue(unmatched_conditions == ["schedule.negative_thaw_condition"])
 
     def test_create_task(self):
         """
         Should create a task.
         """
         task_container = self.empty_task_container
         task_config = self.task_config
 
         created_task = task_config.create_task(task_container)
 
         self.assertTrue(isinstance(created_task, AutomatedTask))
 
         # should raise TaskAlreadyExists when trying to use same task id
         from imio.schedule.interfaces import TaskAlreadyExists
-        kwargs = {'task_container': task_container, 'task_id': created_task.id}
+
+        kwargs = {"task_container": task_container, "task_id": created_task.id}
         self.assertRaises(TaskAlreadyExists, task_config.create_task, **kwargs)
 
     def test_start_task(self):
         """
         Should start a task.
         """
         task_config = self.task_config
         task = self.task
 
         msg = "task should not be started yet (for the sake of the test..)"
-        self.assertEquals(api.content.get_state(task), 'created', msg)
+        self.assertEquals(api.content.get_state(task), "created", msg)
 
         task_config.start_task(task)
 
         msg = "task should have been started"
-        self.assertEquals(api.content.get_state(task), 'to_do', msg)
+        self.assertEquals(api.content.get_state(task), "to_do", msg)
 
     def test_end_task(self):
         """
         Should end a task.
         """
         task_config = self.task_config
         task = self.task
 
         msg = "task should not be ended yet (for the sake of the test..)"
-        self.assertEquals(api.content.get_state(task), 'created', msg)
+        self.assertEquals(api.content.get_state(task), "created", msg)
 
         task_config.end_task(task)
 
         msg = "task should have been ended"
-        self.assertEquals(api.content.get_state(task), 'closed', msg)
+        self.assertEquals(api.content.get_state(task), "closed", msg)
 
     def test_freeze_task(self):
         """
         Should freeze a task.
         """
         task_config = self.task_config
         task = self.task
 
         msg = "task should not be frozen yet (for the sake of the test..)"
-        self.assertEquals(api.content.get_state(task), 'created', msg)
+        self.assertEquals(api.content.get_state(task), "created", msg)
 
         task_config.freeze_task(task)
 
         msg = "task should have been frozen"
-        self.assertEquals(api.content.get_state(task), 'frozen', msg)
+        self.assertEquals(api.content.get_state(task), "frozen", msg)
 
     def test_thaw_task(self):
         """
         Should thaw a task.
         """
         task_config = self.task_config
         task = self.task
 
         msg = "task should be in created state"
-        self.assertEquals(api.content.get_state(task), 'created', msg)
+        self.assertEquals(api.content.get_state(task), "created", msg)
 
         # freeze task befor thaw tests
         task_config.freeze_task(task)
         msg = "task should not be thawed yet (for the sake of the test..)"
-        self.assertEquals(api.content.get_state(task), 'frozen', msg)
+        self.assertEquals(api.content.get_state(task), "frozen", msg)
 
         task_config.thaw_task(task)
 
         msg = "task should have been thawed and put back in its original state"
-        self.assertEquals(api.content.get_state(task), 'created', msg)
+        self.assertEquals(api.content.get_state(task), "created", msg)
 
     def test_thaw_task_stack_freeze_periods(self):
         """
         Verify that a task accumulate multiple frozen periods correctly.
         Multiple freeze periods should stack.
         """
         task_config = self.task_config
         task = self.task
 
         msg = "task should be in created state"
-        self.assertEquals(api.content.get_state(task), 'created', msg)
+        self.assertEquals(api.content.get_state(task), "created", msg)
 
         # freeze task befor thaw tests
         task_config.freeze_task(task)
         msg = "task should not be thawed yet (for the sake of the test..)"
-        self.assertEquals(api.content.get_state(task), 'frozen', msg)
+        self.assertEquals(api.content.get_state(task), "frozen", msg)
 
         # mock a previous freeze period of 5 days and mockput the current freeze date
         # as 10 days earlier to simulate a new 10 days freeze period
         annotations = IAnnotations(task)
-        freeze_infos = annotations['imio.schedule.freeze_task']
-        freeze_infos['previous_freeze_duration'] = 5
-        freeze_infos['freeze_date'] = str(datetime.now().date() + relativedelta(days=-10))
-        annotations['imio.schedule.freeze_task'] = freeze_infos
+        freeze_infos = annotations["imio.schedule.freeze_task"]
+        freeze_infos["previous_freeze_duration"] = 5
+        freeze_infos["freeze_date"] = str(
+            datetime.now().date() + relativedelta(days=-10)
+        )
+        annotations["imio.schedule.freeze_task"] = freeze_infos
 
         task_config.thaw_task(task)
 
         msg = "task should have been thawed and put back in its original state"
-        self.assertEquals(api.content.get_state(task), 'created', msg)
+        self.assertEquals(api.content.get_state(task), "created", msg)
         msg = "task freeze duration should be the sum of the two freeze periods: 5 + 10"
-        freeze_period = annotations['imio.schedule.freeze_task']['previous_freeze_duration']
+        freeze_period = annotations["imio.schedule.freeze_task"][
+            "previous_freeze_duration"
+        ]
         self.assertEquals(freeze_period, 15, msg)
 
     def test_compute_due_date(self):
         """
         Due date should be the date computed by the adapter of
         start_date field + the value in additional_delay (10)
         + the computed delay (15).
@@ -1010,28 +1105,70 @@
 
         expected_date = task_container.creation_date + computed_delay + additional_delay
         expected_date = expected_date.asdatetime().date()
 
         due_date = task_config.compute_due_date(task_container, task)
         self.assertEquals(due_date, expected_date)
 
+    def test_compute_due_date_additional_delay_basic(self):
+        """Ensure that basic (string/int) additional delay is working properly"""
+        task_config = self.task_config
+        task_container = self.task_container
+        task = self.task
+
+        CalculationDefaultDelay.calculate_delay = Mock(return_value=0)
+
+        expected_date = task_container.creation_date + 10
+        expected_date = expected_date.asdatetime().date()
+
+        task_config.additional_delay = 10
+        due_date = task_config.compute_due_date(task_container, task)
+        self.assertEquals(due_date, expected_date)
+
+        task_config.additional_delay = "10"
+        due_date = task_config.compute_due_date(task_container, task)
+        self.assertEquals(due_date, expected_date)
+
+    def test_compute_due_date_additional_delay_tal(self):
+        """Ensure that TAL expression are correctly interpreted"""
+        task_config = self.task_config
+        task_container = self.task_container
+        task = self.task
+
+        CalculationDefaultDelay.calculate_delay = Mock(return_value=0)
+
+        expected_date = task_container.creation_date + 10
+        expected_date = expected_date.asdatetime().date()
+
+        task_config.additional_delay = "python: 1 == 1 and 10 or 20"
+        task_config.additional_delay_tal = True
+        due_date = task_config.compute_due_date(task_container, task)
+        self.assertEquals(due_date, expected_date)
+
+        expected_date = task_container.creation_date + 20
+        expected_date = expected_date.asdatetime().date()
+
+        task_config.additional_delay = "python: 1 == 0 and 10 or 20"
+        due_date = task_config.compute_due_date(task_container, task)
+        self.assertEquals(due_date, expected_date)
+
     def test_compute_due_date_working_days(self):
         """
         Due date should handle the working days
         start date (2017-03-01) + 10 additional days = 2017-03-11
         + 4 weekend days = 2017-03-15
         """
         task_config = self.task_config
         task_container = self.task_container
         task_container.creation_date = DateTime(2017, 3, 1)
         task = self.task
 
         CalculationDefaultDelay.calculate_delay = Mock(return_value=0)
 
-        task_config.additional_delay_type = 'working_days'
+        task_config.additional_delay_type = "working_days"
         due_date = task_config.compute_due_date(task_container, task)
         self.assertEquals(due_date, datetime(2017, 3, 15).date())
 
     def test_compute_due_date_holidays(self):
         """
         Due date whould handle the holidays and working days
         start date (2017-04-14) + 10 additional days = 2017-04-25
@@ -1041,15 +1178,15 @@
         task_config = self.task_config
         task_container = self.task_container
         task_container.creation_date = DateTime(2017, 4, 14)
         task = self.task
 
         CalculationDefaultDelay.calculate_delay = Mock(return_value=0)
 
-        task_config.additional_delay_type = 'working_days'
+        task_config.additional_delay_type = "working_days"
         due_date = task_config.compute_due_date(task_container, task)
         self.assertEquals(due_date, datetime(2017, 5, 2).date())
 
     def test_compute_due_date_with_freeze_period(self):
         """
         Test 'compute_due_date' method for a task who had been frozen.
         start date (2017-04-01) + 10 additional days = 2017-04-11
@@ -1059,46 +1196,46 @@
         task_container = self.task_container
         task_container.creation_date = DateTime(2017, 4, 1)
         task = self.task
 
         CalculationDefaultDelay.calculate_delay = Mock(return_value=0)
 
         annotations = IAnnotations(task)
-        annotations['imio.schedule.freeze_task'] = {
-            'freeze_date': None,
-            'previous_state': task.get_state(),
-            'previous_freeze_duration': 10
+        annotations["imio.schedule.freeze_task"] = {
+            "freeze_date": None,
+            "previous_state": task.get_state(),
+            "previous_freeze_duration": 10,
         }
 
         due_date = task_config.compute_due_date(task_container, task)
         self.assertEquals(due_date, datetime(2017, 4, 21).date())
 
     def test_evaluate_conditions_and(self):
         """
         Evaluate conditions with AND operator
         """
         conditions = [
-            type('condition', (object, ), {'condition': 1, 'operator': 'AND'})(),
-            type('condition', (object, ), {'condition': 2, 'operator': 'AND'})(),
+            type("condition", (object,), {"condition": 1, "operator": "AND"})(),
+            type("condition", (object,), {"condition": 2, "operator": "AND"})(),
         ]
         self.task_config.evaluate_one_condition = Mock(return_value=True)
         result = self.task_config.evaluate_conditions(conditions, None, None)
         self.assertTrue(result)
 
         self.task_config.evaluate_one_condition = Mock(side_effect=[True, False])
         result = self.task_config.evaluate_conditions(conditions, None, None)
         self.assertFalse(result)
 
     def test_evaluate_conditions_or(self):
         """
         Evaluate conditions with OR operator
         """
         conditions = [
-            type('condition', (object, ), {'condition': 1, 'operator': 'OR'})(),
-            type('condition', (object, ), {'condition': 2, 'operator': 'OR'})(),
+            type("condition", (object,), {"condition": 1, "operator": "OR"})(),
+            type("condition", (object,), {"condition": 2, "operator": "OR"})(),
         ]
         self.task_config.evaluate_one_condition = Mock(return_value=True)
         result = self.task_config.evaluate_conditions(conditions, None, None)
         self.assertTrue(result)
 
         self.task_config.evaluate_one_condition = Mock(side_effect=[True, False])
         result = self.task_config.evaluate_conditions(conditions, None, None)
@@ -1113,34 +1250,34 @@
         self.assertFalse(result)
 
     def test_evaluate_conditions_and_or(self):
         """
         Evaluate conditions with AND and OR operators
         """
         conditions = [
-            type('condition', (object, ), {'condition': 1, 'operator': 'OR'})(),
-            type('condition', (object, ), {'condition': 2, 'operator': 'AND'})(),
-            type('condition', (object, ), {'condition': 3, 'operator': 'AND'})(),
+            type("condition", (object,), {"condition": 1, "operator": "OR"})(),
+            type("condition", (object,), {"condition": 2, "operator": "AND"})(),
+            type("condition", (object,), {"condition": 3, "operator": "AND"})(),
         ]
         self.task_config.evaluate_one_condition = Mock(side_effect=[True, False, False])
         result = self.task_config.evaluate_conditions(conditions, None, None)
         self.assertTrue(result)
 
         self.task_config.evaluate_one_condition = Mock(side_effect=[False, False, True])
         result = self.task_config.evaluate_conditions(conditions, None, None)
         self.assertFalse(result)
 
         self.task_config.evaluate_one_condition = Mock(side_effect=[False, True, True])
         result = self.task_config.evaluate_conditions(conditions, None, None)
         self.assertTrue(result)
 
         conditions = [
-            type('condition', (object, ), {'condition': 1, 'operator': 'OR'})(),
-            type('condition', (object, ), {'condition': 2, 'operator': 'AND'})(),
-            type('condition', (object, ), {'condition': 3, 'operator': 'OR'})(),
+            type("condition", (object,), {"condition": 1, "operator": "OR"})(),
+            type("condition", (object,), {"condition": 2, "operator": "AND"})(),
+            type("condition", (object,), {"condition": 3, "operator": "OR"})(),
         ]
         self.task_config.evaluate_one_condition = Mock(side_effect=[False, False, True])
         result = self.task_config.evaluate_conditions(conditions, None, None)
         self.assertFalse(result)
 
     def test_should_recurred(self):
         """
@@ -1155,81 +1292,88 @@
 
         task_config.match_recurrence_states = Mock(return_value=True)
         self.assertFalse(task_config.should_recurred(None))
 
         task_config.activate_recurrency = True
         self.assertTrue(task_config.should_recurred(None))
 
-        task_config.recurrence_conditions = ['foo']
+        task_config.recurrence_conditions = ["foo"]
         task_config.evaluate_conditions = Mock(return_value=True)
         self.assertTrue(task_config.should_recurred(None))
 
     def test_match_recurrence_states(self):
         """
         Test method 'match_recurrence_states'
         """
         self.task_config.recurrence_states = []
         self.assertTrue(self.task_config.match_recurrence_states(None))
 
-        self.task_config.recurrence_states = ['foo']
-        api.content.get_state = Mock(return_value='foo')
+        self.task_config.recurrence_states = ["foo"]
+        api.content.get_state = Mock(return_value="foo")
         self.assertTrue(self.task_config.match_recurrence_states(None))
 
-        self.task_config.recurrence_states = ['bar']
+        self.task_config.recurrence_states = ["bar"]
         self.assertFalse(self.task_config.match_recurrence_states(None))
 
     def test_create_recurring_task(self):
         """
         Test different cases for the 'create_recurring_task' method
         """
-        container = type('container', (dict, ), {})()
-        container['TASK_test_taskconfig'] = None
-        api.content.get_state = Mock(return_value='foo')
-        container.objectIds = Mock(return_value=['TASK_test_taskconfig'])
-        self.assertIsNone(self.task_config.create_recurring_task(
-            container,
-            creation_place=container,
-        ))
+        container = type("container", (dict,), {})()
+        container["TASK_test_taskconfig"] = type("task", (dict,), {
+            "get_task_config": Mock(return_value=self.task_config),
+        })
+        api.content.get_state = Mock(return_value="foo")
+        container.objectIds = Mock(return_value=["TASK_test_taskconfig"])
+        self.assertIsNone(
+            self.task_config.create_recurring_task(
+                container,
+                creation_place=container,
+            )
+        )
 
         container.objectIds = Mock(return_value=[])
         self.task_config.create_task = Mock(return_value=True)
-        self.assertTrue(self.task_config.create_recurring_task(
-            container,
-            creation_place=container,
-        ))
+        self.assertTrue(
+            self.task_config.create_recurring_task(
+                container,
+                creation_place=container,
+            )
+        )
 
-        container.objectIds = Mock(return_value=['TASK_test_taskconfig'])
-        api.content.get_state = Mock(return_value='closed')
+        container.objectIds = Mock(return_value=["TASK_test_taskconfig"])
+        api.content.get_state = Mock(return_value="closed")
         self.assertTrue(self.task_config.create_recurring_task(container))
 
 
 class TestMacroTaskConfig(unittest.TestCase):
     """
     Test MacroTaskConfig content type.
     """
 
     layer = TEST_INSTALL_INTEGRATION
 
     def test_MacroTaskConfig_portal_type_is_registered(self):
-        portal_types = api.portal.get_tool('portal_types')
+        portal_types = api.portal.get_tool("portal_types")
         registered_types = portal_types.listContentTypes()
-        self.assertTrue('MacroTaskConfig' in registered_types)
+        self.assertTrue("MacroTaskConfig" in registered_types)
 
 
 class TestMacroTaskConfigMethodsIntegration(MacroTaskScheduleIntegrationTestCase):
     """
     Test MacroTaskConfig methods.
     """
 
     def setUp(self):
         super(TestMacroTaskConfigMethodsIntegration, self).setUp()
         self._mt_match_recurrence_states = self.macrotask_config.match_recurrence_states
         self._mt_evaluate_conditions = self.macrotask_config.evaluate_conditions
         self._st_match_recurrence_states = self.subtask_config.match_recurrence_states
         self._st_evaluate_conditions = self.subtask_config.evaluate_conditions
+        setRequest(self.portal.REQUEST)
 
     def tearDown(self):
         self.macrotask_config.match_recurrence_states = self._mt_match_recurrence_states
         self.macrotask_config.evaluate_conditions = self._mt_evaluate_conditions
         self.subtask_config.match_recurrence_states = self._st_match_recurrence_states
         self.subtask_config.evaluate_conditions = self._st_evaluate_conditions
         super(TestMacroTaskConfigMethodsIntegration, self).tearDown()
@@ -1239,23 +1383,24 @@
         MacroTaskConfig implements ITaskConfig and should implements all
         the methods defined in TaskConfig.
         As long MacroTaskConfig inherits from BaseTaskConfig, we test the inherited
         methods only in TaskConfig test cases to avoid test code duplication.
         """
         from imio.schedule.content.task_config import MacroTaskConfig
         from imio.schedule.content.task_config import BaseTaskConfig
+
         msg = "MacroTaskConfig should inherits BaseTaskConfig"
         self.assertTrue(issubclass(MacroTaskConfig, BaseTaskConfig), msg)
 
     def test_get_task_type(self):
         """
         Should return 'AutomatedMacroTask'
         """
         task_type = self.macrotask_config.get_task_type()
-        expected_type = 'AutomatedMacroTask'
+        expected_type = "AutomatedMacroTask"
         self.assertEquals(task_type, expected_type)
 
     def test_get_subtask_configs(self):
         """
         Should return all the subtasks configs of a macro task.
         """
         subtasks_configs = self.macrotask_config.get_subtask_configs()
@@ -1292,28 +1437,28 @@
         macrotask_config = self.macrotask_config
         subtask_config = self.subtask_config
         task_container = self.task_container
         macrotask = self.macro_task
         subtask = self.sub_task
 
         # normal case
-        api.content.transition(obj=task_container, transition='publish')
+        api.content.transition(obj=task_container, transition="publish")
 
         msg = "SubTask should be ended"
         end = subtask_config.should_end_task(task_container, macrotask)
         self.assertTrue(end, msg)
 
         msg = "MacroTask should be ended"
         end = macrotask_config.should_end_task(task_container, subtask)
         self.assertTrue(end, msg)
 
         # re open the subtask => the macro task should not be ended as long
         # the subtask is open
 
-        api.content.transition(obj=subtask, transition='back_in_realized')
+        api.content.transition(obj=subtask, transition="back_in_realized")
         self.assertFalse(subtask.get_status() == DONE)
 
         msg = "MacroTask should not be ended as long its subtask is open"
         end = macrotask_config.should_end_task(task_container, macrotask)
         self.assertFalse(end, msg)
 
     def test_should_recurred_macrotask(self):
@@ -1329,46 +1474,46 @@
 
         task_config.match_recurrence_states = Mock(return_value=True)
         self.assertFalse(task_config.should_recurred(None))
 
         task_config.activate_recurrency = True
         self.assertTrue(task_config.should_recurred(None))
 
-        task_config.recurrence_conditions = ['foo']
+        task_config.recurrence_conditions = ["foo"]
         task_config.evaluate_conditions = Mock(return_value=True)
         self.assertTrue(task_config.should_recurred(None))
 
     def test_freeze_macrotask(self):
         macrotask_config = self.macrotask_config
         macrotask = self.macro_task
         subtask = self.sub_task
 
         # normal case
         macrotask_config.freeze_task(macrotask)
 
         msg = "MacroTask should be frozen"
-        self.assertEquals(macrotask.get_state(), 'frozen', msg)
+        self.assertEquals(macrotask.get_state(), "frozen", msg)
 
         msg = "SubTask should be frozen"
-        self.assertEquals(subtask.get_state(), 'frozen', msg)
+        self.assertEquals(subtask.get_state(), "frozen", msg)
 
     def test_thaw_macrotask(self):
         macrotask_config = self.macrotask_config
         macrotask = self.macro_task
         subtask = self.sub_task
 
         original_macrotask_state = macrotask.get_state()
         original_subtask_state = subtask.get_state()
         # freeze task before trying to thaw it
         macrotask_config.freeze_task(macrotask)
 
         msg = "MacroTask should be frozen"
-        self.assertEquals(macrotask.get_state(), 'frozen', msg)
+        self.assertEquals(macrotask.get_state(), "frozen", msg)
         msg = "SubTask should be frozen"
-        self.assertEquals(subtask.get_state(), 'frozen', msg)
+        self.assertEquals(subtask.get_state(), "frozen", msg)
 
         # thaw macro task
         macrotask_config.thaw_task(macrotask)
 
         msg = "MacroTask should be thawed"
         self.assertEquals(macrotask.get_state(), original_macrotask_state, msg)
         msg = "SubTask should be thawed"
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/tests/test_utils.py` & `imio.schedule-2.2.2/src/imio/schedule/tests/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,78 +19,81 @@
         """
         Test the method get_all_schedule_configs.
         """
         from imio.schedule.utils import get_all_schedule_configs
 
         self.assertEquals(
             [self.empty_schedule_config, self.schedule_config],
-            get_all_schedule_configs()
+            get_all_schedule_configs(),
         )
 
     def test_get_task_configs(self):
         """
         Test the method get_task_configs.
         """
         from imio.schedule.utils import get_task_configs
 
-        expected_UIDS = [task_config.UID() for task_config in self.schedule_config.get_all_task_configs()]
+        expected_UIDS = [
+            task_config.UID()
+            for task_config in self.schedule_config.get_all_task_configs()
+        ]
         folder = self.portal.config
         task_configs = get_task_configs(folder)
         task_config_UIDS = [task_config.UID() for task_config in task_configs]
         self.assertEqual(set(task_config_UIDS), set(expected_UIDS))
 
     def test_get_container_open_tasks(self):
         """
         Test the method get_container_open_tasks.
         """
         from imio.schedule.utils import get_container_open_tasks
 
         task_state = api.content.get_state(self.task)
-        self.assertEqual(status_by_state[task_state] in [CREATION, STARTED])
+        self.assertTrue(status_by_state[task_state] in [CREATION, STARTED])
         expected = [self.task]
         open_tasks = get_container_open_tasks(self.task_container)
         self.assertEqual(expected, open_tasks)
 
     def test_end_all_open_tasks(self):
         """
         Test the method end_all_open_tasks.
         """
         from imio.schedule.utils import end_all_open_tasks
 
         open_tasks = end_all_open_tasks(self.task_container)
         end_all_open_tasks(self.task_container)
         for task in open_tasks:
-            self.assertEqual(status_by_state[api.content.get_state()], DONE)
+            self.assertEqual(status_by_state[api.content.get_state(obj=task)], DONE)
 
     def test_tuple_to_interface(self):
         """
         Should turn a tuple ('interface.module.path', 'Interface') into
         Interface class.
         """
         from imio.schedule.utils import tuple_to_interface
 
         expected_interface = IATFolder
-        interface_tuple = ('Products.ATContentTypes.interfaces.folder', 'IATFolder')
+        interface_tuple = ("Products.ATContentTypes.interfaces.folder", "IATFolder")
         interface = tuple_to_interface(interface_tuple)
         self.assertEqual(interface, expected_interface)
 
     def test_interface_to_tuple(self):
         """
         Should turn an Interface class into a tuple:
         ('interface.module.path', 'Interface')
         """
         from imio.schedule.utils import interface_to_tuple
 
-        expected_tuple = ('Products.ATContentTypes.interfaces.folder', 'IATFolder')
+        expected_tuple = ("Products.ATContentTypes.interfaces.folder", "IATFolder")
         interface_tuple = interface_to_tuple(IATFolder)
         self.assertEqual(interface_tuple, expected_tuple)
 
 
 def TestWorkingDaysCalendar(ExampleScheduleIntegrationTestCase):
-
     def test_is_working_day(self):
         from imio.schedule.utils import WorkingDaysCalendar
+
         calendar = WorkingDaysCalendar()
         # Basic holiday
         self.assertTrue(calendar.is_working_day(date(2017, 1, 1)))
         # Test holiday from CalendarExtraHolidays utility
         self.assertTrue(calendar.is_working_day(date(2017, 2, 1)))
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/tests/test_vocabulary.py` & `imio.schedule-2.2.2/src/imio/schedule/tests/test_vocabulary.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,291 +17,319 @@
     Test dashboard vocabularies registration and values.
     """
 
     def test_task_workflow_vocabulary_factory_registration(self):
         """
         Content types voc factory should be registered as a named utility.
         """
-        factory_name = 'schedule.TaskWorkflowStates'
+        factory_name = "schedule.TaskWorkflowStates"
         self.assertTrue(queryUtility(IVocabularyFactory, factory_name))
 
     def test_task_workflow_vocabulary_values(self):
         """
         Test task workflow vocabulary values.
         """
 
-        voc_name = 'schedule.TaskWorkflowStates'
+        voc_name = "schedule.TaskWorkflowStates"
         voc_factory = getUtility(IVocabularyFactory, voc_name)
         vocabulary = voc_factory(self.schedule_config)
-        expected_keys = ['created', 'to_do', 'closed']
+        expected_keys = ["created", "to_do", "closed"]
         for expected_key in expected_keys:
-            msg = 'expected key:\n{expected}\nwas not found in voc_keys:\n{voc}'.format(
-                expected=expected_key,
-                voc=vocabulary.by_token.keys()
+            msg = "expected key:\n{expected}\nwas not found in voc_keys:\n{voc}".format(
+                expected=expected_key, voc=vocabulary.by_token.keys()
             )
             self.assertTrue(expected_key in vocabulary.by_token.keys(), msg)
 
 
 class TestVocabularies(ExampleScheduleIntegrationTestCase):
     """
     Test field vocabularies registration and values.
     """
 
     def _get_fti(self, portal_type):
         """
         Helper method to return the fti of a content type.
         """
-        portal_types = api.portal.get_tool('portal_types')
+        portal_types = api.portal.get_tool("portal_types")
         fti = portal_types.getTypeInfo(portal_type)
         return fti
 
     def test_content_types_vocabulary_factory_registration(self):
         """
         Content types voc factory should be registered as a named utility.
         """
-        factory_name = 'schedule.scheduled_contenttype'
+        factory_name = "schedule.scheduled_contenttype"
         self.assertTrue(queryUtility(IVocabularyFactory, factory_name))
 
     def test_content_types_default_vocabulary_registration(self):
         """
         Voc values should be registered as a named adapter on the task
         config fti and name should be the fti portal_type.
         """
         from imio.schedule.interfaces import IScheduledContentTypeVocabulary
 
         portal_type = self.schedule_config.portal_type
 
         voc_adapter = queryAdapter(
-            self._get_fti(portal_type),
-            IScheduledContentTypeVocabulary,
-            portal_type
+            self._get_fti(portal_type), IScheduledContentTypeVocabulary, portal_type
         )
         self.assertTrue(voc_adapter)
 
     def test_content_types_vocabulary_values(self):
         """
         Test some content_types values.
         """
 
-        voc_name = 'schedule.scheduled_contenttype'
+        voc_name = "schedule.scheduled_contenttype"
         voc_factory = getUtility(IVocabularyFactory, voc_name)
         vocabulary = voc_factory(self.schedule_config)
-        expected_key = "('Folder', (('Products.ATContentTypes.interfaces.folder', 'IATFolder'),))"
-        msg = 'expected key:\n{expected}\nwas not found in voc_keys:\n{voc}'.format(
-            expected=expected_key,
-            voc=vocabulary.by_token.keys()
+        expected_key = (
+            "('Folder', (('Products.ATContentTypes.interfaces.folder', 'IATFolder'),))"
+        )
+        msg = "expected key:\n{expected}\nwas not found in voc_keys:\n{voc}".format(
+            expected=expected_key, voc=vocabulary.by_token.keys()
         )
         self.assertTrue(expected_key in vocabulary.by_token.keys(), msg)
 
     def test_assigned_user_vocabulary_factory_registration(self):
         """
         Content types voc factory should be registered as a named utility.
         """
-        factory_name = 'schedule.assigned_user'
+        factory_name = "schedule.assigned_user"
         self.assertTrue(queryUtility(IVocabularyFactory, factory_name))
 
     def test_assigned_user_vocabulary_values(self):
         """
         Test some assigned_user values.
         """
-        voc_name = 'schedule.assigned_user'
+        voc_name = "schedule.assigned_user"
         voc_factory = getUtility(IVocabularyFactory, voc_name)
         vocabulary = voc_factory(self.task_config)
-        self.assertTrue('schedule.assign_current_user' in vocabulary)
+        self.assertTrue("schedule.assign_current_user" in vocabulary)
 
-        term = vocabulary.getTerm('schedule.assign_current_user')
-        translation = translate(term.title, context=self.portal.REQUEST, target_language='fr')
-        msg = 'Condition title was not translated'
-        self.assertEquals(translation, u'Utilisateur connecté', msg)
+        term = vocabulary.getTerm("schedule.assign_current_user")
+        translation = translate(
+            term.title, context=self.portal.REQUEST, target_language="fr"
+        )
+        msg = "Condition title was not translated"
+        self.assertEquals(translation, u"Utilisateur connecté", msg)
 
     def test_creation_conditions_vocabulary_factory_registration(self):
         """
         Content types voc factory should be registered as a named utility.
         """
-        factory_name = 'schedule.creation_conditions'
+        factory_name = "schedule.creation_conditions"
         self.assertTrue(queryUtility(IVocabularyFactory, factory_name))
 
     def test_creation_conditions_vocabulary_values(self):
         """
         Test some creation_conditions values.
         """
-        voc_name = 'schedule.creation_conditions'
+        voc_name = "schedule.creation_conditions"
         voc_factory = getUtility(IVocabularyFactory, voc_name)
         vocabulary = voc_factory(self.task_config)
-        self.assertTrue('schedule.test_creation_condition' in vocabulary)
+        self.assertTrue("schedule.test_creation_condition" in vocabulary)
 
-        term = vocabulary.getTerm('schedule.test_creation_condition')
-        translation = translate(term.title, context=self.portal.REQUEST, target_language='fr')
-        msg = 'Condition title was not translated'
-        self.assertEquals(translation, u'Condition de création TEST', msg)
+        term = vocabulary.getTerm("schedule.test_creation_condition")
+        translation = translate(
+            term.title, context=self.portal.REQUEST, target_language="fr"
+        )
+        msg = "Condition title was not translated"
+        self.assertEquals(translation, u"Condition de création TEST", msg)
 
     def test_start_conditions_vocabulary_factory_registration(self):
         """
         Content types voc factory should be registered as a named utility.
         """
-        factory_name = 'schedule.start_conditions'
+        factory_name = "schedule.start_conditions"
         self.assertTrue(queryUtility(IVocabularyFactory, factory_name))
 
     def test_start_conditions_vocabulary_values(self):
         """
         Test some start_conditions values.
         """
-        voc_name = 'schedule.start_conditions'
+        voc_name = "schedule.start_conditions"
         voc_factory = getUtility(IVocabularyFactory, voc_name)
         vocabulary = voc_factory(self.task_config)
-        self.assertTrue('schedule.test_start_condition' in vocabulary)
+        self.assertTrue("schedule.test_start_condition" in vocabulary)
 
-        term = vocabulary.getTerm('schedule.test_start_condition')
-        translation = translate(term.title, context=self.portal.REQUEST, target_language='fr')
-        msg = 'Condition title was not translated'
-        self.assertEquals(translation, u'Condition de démarrage TEST', msg)
+        term = vocabulary.getTerm("schedule.test_start_condition")
+        translation = translate(
+            term.title, context=self.portal.REQUEST, target_language="fr"
+        )
+        msg = "Condition title was not translated"
+        self.assertEquals(translation, u"Condition de démarrage TEST", msg)
 
     def test_end_conditions_vocabulary_factory_registration(self):
         """
         Content types voc factory should be registered as a named utility.
         """
-        factory_name = 'schedule.end_conditions'
+        factory_name = "schedule.end_conditions"
         self.assertTrue(queryUtility(IVocabularyFactory, factory_name))
 
     def test_end_conditions_vocabulary_values(self):
         """
         Test some end_conditions values.
         """
-        voc_name = 'schedule.end_conditions'
+        voc_name = "schedule.end_conditions"
         voc_factory = getUtility(IVocabularyFactory, voc_name)
         vocabulary = voc_factory(self.task_config)
-        self.assertTrue('schedule.test_end_condition' in vocabulary)
+        self.assertTrue("schedule.test_end_condition" in vocabulary)
 
-        term = vocabulary.getTerm('schedule.test_end_condition')
-        translation = translate(term.title, context=self.portal.REQUEST, target_language='fr')
-        msg = 'Condition title was not translated'
-        self.assertEquals(translation, u'Condition de fin TEST', msg)
+        term = vocabulary.getTerm("schedule.test_end_condition")
+        translation = translate(
+            term.title, context=self.portal.REQUEST, target_language="fr"
+        )
+        msg = "Condition title was not translated"
+        self.assertEquals(translation, u"Condition de fin TEST", msg)
 
     def test_start_date_vocabulary_factory_registration(self):
         """
         Content types voc factory should be registered as a named utility.
         """
-        factory_name = 'schedule.start_date'
+        factory_name = "schedule.start_date"
         self.assertTrue(queryUtility(IVocabularyFactory, factory_name))
 
     def test_start_date_vocabulary_values(self):
         """
         Test some due_date values.
         """
-        voc_name = 'schedule.start_date'
+        voc_name = "schedule.start_date"
         voc_factory = getUtility(IVocabularyFactory, voc_name)
         vocabulary = voc_factory(self.task_config)
-        self.assertTrue('schedule.start_date.creation_date' in vocabulary)
+        self.assertTrue("schedule.start_date.creation_date" in vocabulary)
 
-        term = vocabulary.getTerm('schedule.start_date.creation_date')
-        translation = translate(term.title, context=self.portal.REQUEST, target_language='fr')
-        msg = 'Condition title was not translated'
-        self.assertEquals(translation, u'Date de création du dossier', msg)
+        term = vocabulary.getTerm("schedule.start_date.creation_date")
+        translation = translate(
+            term.title, context=self.portal.REQUEST, target_language="fr"
+        )
+        msg = "Condition title was not translated"
+        self.assertEquals(translation, u"Date de création du dossier", msg)
 
     def test_task_owner_vocabulary_factory_registration(self):
         """
         Content types voc factory should be registered as a named utility.
         """
-        factory_name = 'schedule.task_owner'
+        factory_name = "schedule.task_owner"
         self.assertTrue(queryUtility(IVocabularyFactory, factory_name))
 
 
 class TestMacroTaskVocabularies(MacroTaskScheduleIntegrationTestCase):
     """
     Test AutomatedMacroTask field vocabularies registration and values.
     """
 
     def test_macrotask_creation_conditions_vocabulary_factory_registration(self):
         """
         Content types voc factory should be registered as a named utility.
         """
-        factory_name = 'schedule.macrotask_creation_conditions'
+        factory_name = "schedule.macrotask_creation_conditions"
         self.assertTrue(queryUtility(IVocabularyFactory, factory_name))
 
     def test_macrotask_creation_conditions_vocabulary_values(self):
         """
         Test some creation_conditions values.
         """
-        voc_name = 'schedule.macrotask_creation_conditions'
+        voc_name = "schedule.macrotask_creation_conditions"
         voc_factory = getUtility(IVocabularyFactory, voc_name)
         vocabulary = voc_factory(self.macrotask_config)
-        self.assertTrue('schedule.create_if_subtask_can_be_created' in vocabulary)
-        self.assertTrue('schedule.create_if_all_subtasks_can_be_created' in vocabulary)
+        self.assertTrue("schedule.create_if_subtask_can_be_created" in vocabulary)
+        self.assertTrue("schedule.create_if_all_subtasks_can_be_created" in vocabulary)
 
-        term = vocabulary.getTerm('schedule.create_if_subtask_can_be_created')
-        translation = translate(term.title, context=self.portal.REQUEST, target_language='fr')
-        msg = 'Condition title was not translated'
+        term = vocabulary.getTerm("schedule.create_if_subtask_can_be_created")
+        translation = translate(
+            term.title, context=self.portal.REQUEST, target_language="fr"
+        )
+        msg = "Condition title was not translated"
         self.assertEquals(translation, u"Créer dès qu'une sous-tâche est créable", msg)
 
-        term = vocabulary.getTerm('schedule.create_if_all_subtasks_can_be_created')
-        translation = translate(term.title, context=self.portal.REQUEST, target_language='fr')
-        msg = 'Condition title was not translated'
-        self.assertEquals(translation, u"Créer si toutes les sous-tâche sont créables", msg)
+        term = vocabulary.getTerm("schedule.create_if_all_subtasks_can_be_created")
+        translation = translate(
+            term.title, context=self.portal.REQUEST, target_language="fr"
+        )
+        msg = "Condition title was not translated"
+        self.assertEquals(
+            translation, u"Créer si toutes les sous-tâche sont créables", msg
+        )
 
     def test_macrotask_start_conditions_vocabulary_factory_registration(self):
         """
         Content types voc factory should be registered as a named utility.
         """
-        factory_name = 'schedule.macrotask_start_conditions'
+        factory_name = "schedule.macrotask_start_conditions"
         self.assertTrue(queryUtility(IVocabularyFactory, factory_name))
 
     def test_macrotask_start_conditions_vocabulary_values(self):
         """
         Test some start_conditions values.
         """
-        voc_name = 'schedule.macrotask_start_conditions'
+        voc_name = "schedule.macrotask_start_conditions"
         voc_factory = getUtility(IVocabularyFactory, voc_name)
         vocabulary = voc_factory(self.macrotask_config)
-        self.assertTrue('schedule.start_if_subtask_started' in vocabulary)
-        self.assertTrue('schedule.start_if_all_subtasks_started' in vocabulary)
+        self.assertTrue("schedule.start_if_subtask_started" in vocabulary)
+        self.assertTrue("schedule.start_if_all_subtasks_started" in vocabulary)
 
-        term = vocabulary.getTerm('schedule.start_if_subtask_started')
-        translation = translate(term.title, context=self.portal.REQUEST, target_language='fr')
-        msg = 'Condition title was not translated'
-        self.assertEquals(translation, u"Démarrer dès qu'une sous-tâche est démarrée", msg)
-
-        term = vocabulary.getTerm('schedule.start_if_all_subtasks_started')
-        translation = translate(term.title, context=self.portal.REQUEST, target_language='fr')
-        msg = 'Condition title was not translated'
-        self.assertEquals(translation, u"Démarrer si toutes les sous-tâche sont démarrées", msg)
+        term = vocabulary.getTerm("schedule.start_if_subtask_started")
+        translation = translate(
+            term.title, context=self.portal.REQUEST, target_language="fr"
+        )
+        msg = "Condition title was not translated"
+        self.assertEquals(
+            translation, u"Démarrer dès qu'une sous-tâche est démarrée", msg
+        )
+
+        term = vocabulary.getTerm("schedule.start_if_all_subtasks_started")
+        translation = translate(
+            term.title, context=self.portal.REQUEST, target_language="fr"
+        )
+        msg = "Condition title was not translated"
+        self.assertEquals(
+            translation, u"Démarrer si toutes les sous-tâche sont démarrées", msg
+        )
 
     def test_macrotask_end_conditions_vocabulary_factory_registration(self):
         """
         Content types voc factory should be registered as a named utility.
         """
-        factory_name = 'schedule.macrotask_end_conditions'
+        factory_name = "schedule.macrotask_end_conditions"
         self.assertTrue(queryUtility(IVocabularyFactory, factory_name))
 
     def test_macrotask_end_conditions_vocabulary_values(self):
         """
         Test some end_conditions values.
         """
-        voc_name = 'schedule.macrotask_end_conditions'
+        voc_name = "schedule.macrotask_end_conditions"
         voc_factory = getUtility(IVocabularyFactory, voc_name)
         vocabulary = voc_factory(self.macrotask_config)
-        self.assertTrue('schedule.test_end_condition' in vocabulary)
+        self.assertTrue("schedule.test_end_condition" in vocabulary)
 
-        term = vocabulary.getTerm('schedule.test_end_condition')
-        translation = translate(term.title, context=self.portal.REQUEST, target_language='fr')
-        msg = 'Condition title was not translated'
-        self.assertEquals(translation, u'Condition de fin TEST', msg)
+        term = vocabulary.getTerm("schedule.test_end_condition")
+        translation = translate(
+            term.title, context=self.portal.REQUEST, target_language="fr"
+        )
+        msg = "Condition title was not translated"
+        self.assertEquals(translation, u"Condition de fin TEST", msg)
 
     def test_macrotask_start_date_vocabulary_factory_registration(self):
         """
         Content types voc factory should be registered as a named utility.
         """
-        factory_name = 'schedule.macrotask_start_date'
+        factory_name = "schedule.macrotask_start_date"
         self.assertTrue(queryUtility(IVocabularyFactory, factory_name))
 
     def test_macrotask_start_date_vocabulary_values(self):
         """
         Test some due_date values.
         """
-        voc_name = 'schedule.macrotask_start_date'
+        voc_name = "schedule.macrotask_start_date"
         voc_factory = getUtility(IVocabularyFactory, voc_name)
         vocabulary = voc_factory(self.macrotask_config)
-        self.assertTrue('schedule.start_date.subtask_highest_due_date' in vocabulary)
+        self.assertTrue("schedule.start_date.subtask_highest_due_date" in vocabulary)
 
-        term = vocabulary.getTerm('schedule.start_date.subtask_highest_due_date')
-        translation = translate(term.title, context=self.portal.REQUEST, target_language='fr')
-        msg = 'Condition title was not translated'
-        self.assertEquals(translation, u"La plus haute date d'échéance parmi les sous-tâches", msg)
+        term = vocabulary.getTerm("schedule.start_date.subtask_highest_due_date")
+        translation = translate(
+            term.title, context=self.portal.REQUEST, target_language="fr"
+        )
+        msg = "Condition title was not translated"
+        self.assertEquals(
+            translation, u"La plus haute date d'échéance parmi les sous-tâches", msg
+        )
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/utils.py` & `imio.schedule-2.2.2/src/imio/schedule/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 def get_all_schedule_configs():
     """
     Return all the ScheduleConfig of the site.
     """
     # nested import to avoid recursive imports
     from imio.schedule.content.schedule_config import IScheduleConfig
 
-    catalog = api.portal.get_tool('portal_catalog')
+    catalog = api.portal.get_tool("portal_catalog")
     brains = catalog(object_provides=IScheduleConfig.__identifier__)
     configs = [brain.getObject() for brain in brains]
 
     return configs
 
 
 def get_task_configs(task_container, descending=False):
@@ -85,15 +85,15 @@
     while to_explore:
         current = to_explore.pop()
         if IAutomatedTask.providedBy(current):
             if not states:
                 open_tasks.append(current)
             elif api.content.get_state(current) in states:
                 open_tasks.append(current)
-        if hasattr(current, 'objectValues'):
+        if hasattr(current, "objectValues"):
             to_explore.extend(current.objectValues())
     return open_tasks
 
 
 def tuple_to_interface(interface_tuple):
     """
     Turn a tuple of strings:
@@ -111,72 +111,73 @@
     """
     Turn an Interface class into a tuple of strings:
     ('interface.module.path', 'Interface')
     """
     return (interface.__module__, interface.__name__)
 
 
-def set_schedule_view(folder, faceted_config_path, schedule_configs, default_collection=None):
+def set_schedule_view(
+    folder, faceted_config_path, schedule_configs, default_collection=None
+):
     """
     Boilerplate code to set up the schedule view on a folderish context.
     """
 
     if type(schedule_configs) not in [list, tuple]:
         schedule_configs = [schedule_configs]
 
     _set_faceted_view(folder, faceted_config_path, schedule_configs, default_collection)
     _set_collection_portlet(folder)
 
 
-def _set_faceted_view(folder, faceted_config_path, schedule_configs, default_collection=None):
-    """
-    """
+def _set_faceted_view(
+    folder, faceted_config_path, schedule_configs, default_collection=None
+):
+    """ """
     annotations = IAnnotations(folder)
-    key = 'imio.schedule.schedule_configs'
+    key = "imio.schedule.schedule_configs"
     annotations[key] = [cfg.UID() for cfg in schedule_configs]
 
-    subtyper = folder.restrictedTraverse('@@faceted_subtyper')
+    subtyper = folder.restrictedTraverse("@@faceted_subtyper")
     if not subtyper.is_faceted:
         subtyper.enable()
-        folder.restrictedTraverse('@@faceted_settings').toggle_left_column()
-        IFacetedLayout(folder).update_layout('faceted-table-items')
-        folder.unrestrictedTraverse('@@faceted_exportimport').import_xml(
+        folder.restrictedTraverse("@@faceted_settings").toggle_left_column()
+        IFacetedLayout(folder).update_layout("faceted-table-items")
+        folder.unrestrictedTraverse("@@faceted_exportimport").import_xml(
             import_file=open(faceted_config_path)
         )
 
     default_collection = default_collection or schedule_configs[0].dashboard_collection
     _updateDefaultCollectionFor(folder, default_collection.UID())
 
 
 def _set_collection_portlet(folder):
-    """
-    """
+    """ """
     # block parent portlets
-    manager = getUtility(IPortletManager, name='plone.leftcolumn')
+    manager = getUtility(IPortletManager, name="plone.leftcolumn")
     blacklist = getMultiAdapter((folder, manager), ILocalPortletAssignmentManager)
     blacklist.setBlacklistStatus(CONTEXT_CATEGORY, True)
 
     # assign collection portlet
-    manager = getUtility(IPortletManager, name='plone.leftcolumn', context=folder)
+    manager = getUtility(IPortletManager, name="plone.leftcolumn", context=folder)
     mapping = getMultiAdapter((folder, manager), IPortletAssignmentMapping)
-    if 'schedules' not in mapping.keys():
-        mapping['schedules'] = Assignment('schedules')
+    if "schedules" not in mapping.keys():
+        mapping["schedules"] = Assignment("schedules")
 
 
 def dict_list_2_vocabulary(dict_list):
     """dict_list_2_vocabulary
     Converts a dictionary list to a SimpleVocabulary
 
     :param dict_list: dictionary list
     """
     terms = []
     for item in dict_list:
         for key in sorted([k for k in item]):
-            terms.append(SimpleVocabulary.createTerm(
-                key, str(key), item[key]))
+            terms.append(SimpleVocabulary.createTerm(key, str(key), item[key]))
     return SimpleVocabulary(terms)
 
 
 def round_to_weekday(date, weekday):
     direction = weekday / abs(weekday)  # -1 => past, +1 => future
     weekday = abs(weekday) - 1
     days_delta = weekday - date.weekday()
@@ -194,40 +195,41 @@
     """
     today = datetime.date.today()
     limit_date = date - datetime.timedelta(days=by_days)
     return today >= limit_date
 
 
 class WorkingDaysCalendar(Belgium):
-
     def __init__(self, *args, **kwargs):
         super(WorkingDaysCalendar, self).__init__(*args, **kwargs)
         self.working_days = self._get_working_days()
 
     def is_working_day(self, date, *args, **kwargs):
-        result = super(WorkingDaysCalendar, self).is_working_day(
-            date, *args, **kwargs)
+        result = super(WorkingDaysCalendar, self).is_working_day(date, *args, **kwargs)
         if result is True:
             result = date.isoweekday() in self.working_days
         return result
 
     def get_calendar_holidays(self, year):
         result = super(WorkingDaysCalendar, self).get_calendar_holidays(year)
         for name, utility in getUtilitiesFor(ICalendarExtraHolidays):
             result += utility.get_holidays(year)
         return result
 
     def _get_working_days(self):
         """Return the working days configured in the registry"""
         matching = {
-            'monday': 1,
-            'tuesday': 2,
-            'wednesday': 3,
-            'thursday': 4,
-            'friday': 5,
-            'saturday': 6,
-            'sunday': 7,
+            "monday": 1,
+            "tuesday": 2,
+            "wednesday": 3,
+            "thursday": 4,
+            "friday": 5,
+            "saturday": 6,
+            "sunday": 7,
         }
-        days = api.portal.get_registry_record(
-            'imio.schedule.interfaces.ISettings.working_days'
-        ) or []
+        days = (
+            api.portal.get_registry_record(
+                "imio.schedule.interfaces.ISettings.working_days"
+            )
+            or []
+        )
         return [matching[d] for d in days]
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/vocabularies.py` & `imio.schedule-2.2.2/src/imio/schedule/vocabularies.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,27 +8,29 @@
 """
 
 from imio.schedule import utils
 from imio.schedule import _
 
 
 class WorkingDaysVocabularyFactory(object):
-
     def __call__(self, context):
-        return utils.dict_list_2_vocabulary([
-            {'monday': _(u'Monday')},
-            {'tuesday': _(u'Tuesday')},
-            {'wednesday': _(u'Wednesday')},
-            {'thursday': _(u'Thursday')},
-            {'friday': _(u'Friday')},
-            {'saturday': _(u'Saturday')},
-            {'sunday': _(u'Sunday')},
-        ])
+        return utils.dict_list_2_vocabulary(
+            [
+                {"monday": _(u"Monday")},
+                {"tuesday": _(u"Tuesday")},
+                {"wednesday": _(u"Wednesday")},
+                {"thursday": _(u"Thursday")},
+                {"friday": _(u"Friday")},
+                {"saturday": _(u"Saturday")},
+                {"sunday": _(u"Sunday")},
+            ]
+        )
 
 
 class AdditionalDelayTypeVocabularyFactory(object):
-
     def __call__(self, context):
-        return utils.dict_list_2_vocabulary([
-            {'absolute': _(u'Absolute')},
-            {'working_days': _(u'Working days')},
-        ])
+        return utils.dict_list_2_vocabulary(
+            [
+                {"absolute": _(u"Absolute")},
+                {"working_days": _(u"Working days")},
+            ]
+        )
```

### Comparing `imio.schedule-2.2.1/src/imio/schedule/workflow/freeze_task.py` & `imio.schedule-2.2.2/src/imio/schedule/workflow/freeze_task.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,29 +16,29 @@
 
     implements(IWorkflowAdaptation)
 
     schema = None
 
     def patch_workflow(self, workflow_name, **parameters):
 
-        wtool = api.portal.get_tool('portal_workflow')
+        wtool = api.portal.get_tool("portal_workflow")
         workflow = wtool[workflow_name]
 
         self.create_frozen_state(workflow, **parameters)
 
         message = "patched '{}' workflow with frozen state".format(workflow_name)
         return True, message
 
     def create_frozen_state(self, workflow, **parameters):
         """
         create a 'frozen' state
         """
-        if 'frozen' not in workflow.states:
-            workflow.states.addState('frozen')
+        if "frozen" not in workflow.states:
+            workflow.states.addState("frozen")
 
-        frozen_state = workflow.states['frozen']
+        frozen_state = workflow.states["frozen"]
         default_mapping = workflow.states.objectValues()[0].permission_roles.copy()
-        frozen_state.title = 'frozen'
+        frozen_state.title = "frozen"
         frozen_state.permission_roles = default_mapping
         frozen_state.group_roles = PersistentMapping()
         frozen_state.var_values = PersistentMapping()
         frozen_state.transitions = ()
```

### Comparing `imio.schedule-2.2.1/src/imio.schedule.egg-info/PKG-INFO` & `imio.schedule-2.2.2/src/imio.schedule.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.schedule
-Version: 2.2.1
+Version: 2.2.2
 Summary: Schedule for imio products
 Home-page: https://pypi.python.org/pypi/imio.schedule
 Author: Simon Delcourt
 Author-email: simon.delcourt@imio.be
 License: GPL version 2
 Keywords: Python Plone
 Classifier: Environment :: Web Environment
@@ -94,14 +94,39 @@
 ============
 
 - Simon Delcourt, simon.delcourt@imio.be
 
 Changelog
 =========
 
+.. You should *NOT* be adding new change log entries to this file.
+   You should create a file in the news directory instead.
+   For helpful instructions, please see:
+   https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
+
+.. towncrier release notes start
+
+2.2.2 (2024-04-25)
+------------------
+
+New features:
+
+
+- Allow additional delay to be a TAL expression
+  [mpeeters] (URB-3005)
+
+
+Internal:
+
+
+- Black
+  [mpeeters] (SUP-27104)
+- Fix tests
+  [mpeeters] (URB-3005)
+
 
 2.2.1 (2024-04-10)
 ------------------
 
 - Fix object deserializer
   [jchandelle]
```

### Comparing `imio.schedule-2.2.1/src/imio.schedule.egg-info/SOURCES.txt` & `imio.schedule-2.2.2/src/imio.schedule.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 CHANGES.rst
 CONTRIBUTORS.rst
 MANIFEST.in
 Makefile
 README.rst
 bootstrap.py
+pyproject.toml
+requirements.txt
 setup.cfg
 setup.py
 docs/LICENSE.GPL
 docs/LICENSE.rst
 docs/index.rst
 src/imio/__init__.py
 src/imio.schedule.egg-info/PKG-INFO
```


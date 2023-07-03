# Comparing `tmp/imio.schedule-1.8.tar.gz` & `tmp/imio.schedule-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imio.schedule-1.8.tar", last modified: Thu Apr  6 09:22:10 2023, max compression
+gzip compressed data, was "dist/imio.schedule-1.9.0.tar", last modified: Mon Jul  3 09:37:50 2023, max compression
```

## Comparing `imio.schedule-1.8.tar` & `imio.schedule-1.9.0.tar`

### file list

```diff
@@ -1,163 +1,165 @@
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/docs/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      658 2023-04-06 09:22:09.000000 imio.schedule-1.8/docs/LICENSE.rst
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)       76 2023-04-06 09:22:09.000000 imio.schedule-1.8/docs/index.rst
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)    18092 2023-04-06 09:22:09.000000 imio.schedule-1.8/docs/LICENSE.GPL
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)       80 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/__init__.py
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio/schedule/
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio/schedule/collectionwidget/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      638 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/collectionwidget/configure.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      439 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/collectionwidget/views.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1264 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/collectionwidget/vocabulary.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/collectionwidget/__init__.py
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio/schedule/collectionwidget/templates/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1569 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/collectionwidget/templates/term.pt
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      461 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/vocabularies.zcml
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio/schedule/tests/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     4809 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/tests/test_scheduleconfig.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     3056 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/tests/conditions.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)    10523 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/tests/test_task.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1003 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/tests/test_dashboardcollection.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      396 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/tests/configure.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)    17095 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/tests/test_task_events.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     3361 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/tests/test_utils.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      391 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/tests/due_date.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     9742 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/tests/setup.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      426 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/tests/logic.py
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio/schedule/tests/robot/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1542 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/tests/robot/test_example.robot
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     6586 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/tests/test_registration_events.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     2292 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/tests/test_delay.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      318 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/tests/holidays.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)    13257 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/tests/test_vocabulary.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)    57639 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/tests/test_taskconfig.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/tests/__init__.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      279 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/tests/due_date.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      455 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/tests/logic.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1774 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/tests/condition.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1197 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/tests/test_indexes.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     2792 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/tests/test_logic.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     3294 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/tests/test_setup.py
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio/schedule/content/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)    46099 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/content/task_config.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1641 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/content/subform_context_choice.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     2177 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/content/conditions.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     3432 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/content/object_factories.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      362 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/content/configure.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)    16202 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/content/vocabulary.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     4054 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/content/logic.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      304 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/content/view.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      592 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/content/delay.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     5614 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/content/vocabulary.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      616 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/content/widget.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     2273 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/content/delay.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/content/__init__.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1276 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/content/logic.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     6337 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/content/object_factories.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     5091 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/content/condition.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     2764 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/content/schedule_config.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      460 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/content/view.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     8001 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/content/task.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     4626 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/interfaces.py
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio/schedule/locales/
--rwxrwxr-x   0 fngaha    (1000) fngaha    (1000)      686 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/locales/update.sh
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      774 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/locales/collective.eeafaceted.z3ctable.pot
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1575 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/locales/manual_translations.pot
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio/schedule/locales/fr/
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio/schedule/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)    12139 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/locales/fr/LC_MESSAGES/imio.schedule.po
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      708 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.po
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     9239 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/locales/imio.schedule.pot
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1281 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/configure.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      222 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/setuphandlers.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      847 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/vocabularies.py
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio/schedule/events/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     7941 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/events/update_tasks.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     2174 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/events/task_config.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     5177 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/events/configure.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     8333 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/events/zope_registration.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     2587 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/events/dashboard_collection.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/events/__init__.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1810 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/events/create_task.py
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio/schedule/workflow/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      404 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/workflow/configure.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1286 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/workflow/freeze_task.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/workflow/__init__.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     7829 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/testing.py
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio/schedule/migration/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      244 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/migration/configure.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      393 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/migration/upgrades.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      561 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/migration/migrate_to_18.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/migration/__init__.py
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio/schedule/browser/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1806 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/browser/configure.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1071 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/browser/close_task.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/browser/__init__.py
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio/schedule/browser/templates/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      577 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/browser/templates/task_change_owner.pt
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     3167 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/browser/templates/task_completion.pt
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      566 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/browser/templates/close_task.pt
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     5112 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/browser/templates/taskmacros.pt
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1324 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/browser/task_owner.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     3696 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/browser/task_completion.py
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio/schedule/browser/overrides/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/browser/overrides/.gitkeep
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio/schedule/browser/static/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1023 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/browser/static/schedule.css
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/browser/static/.gitkeep
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      175 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/browser/static/overlay.js
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio/schedule/profiles/
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio/schedule/profiles/default/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      369 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/profiles/default/workflows.xml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      148 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/profiles/default/browserlayer.xml
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio/schedule/profiles/default/types/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     2193 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/profiles/default/types/ScheduleConfig.xml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1955 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/profiles/default/types/AutomatedTask.xml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     2087 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/profiles/default/types/TaskConfig.xml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     2193 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/profiles/default/types/MacroTaskConfig.xml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     2134 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/profiles/default/types/AutomatedMacroTask.xml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      554 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/profiles/default/catalog.xml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/profiles/default/imioschedule_default.txt
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      655 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/profiles/default/jsregistry.xml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1595 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/profiles/default/registry.xml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      490 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/profiles/default/cssregistry.xml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      488 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/profiles/default/types.xml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      231 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/profiles/default/propertiestool.xml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      369 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/profiles/default/metadata.xml
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio/schedule/profiles/testing/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/profiles/testing/imioschedule_testing.txt
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      164 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/profiles/testing/metadata.xml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     7336 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/utils.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      611 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/indexes.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      130 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/__init__.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      661 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/config.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      782 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/testing.zcml
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio/schedule/dashboard/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     7287 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/dashboard/columns.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      624 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/dashboard/interfaces.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      178 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/dashboard/configure.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1386 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/dashboard/vocabulary.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      534 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/dashboard/vocabulary.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     2647 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/dashboard/columns.zcml
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/dashboard/__init__.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      378 2023-04-06 09:22:09.000000 imio.schedule-1.8/src/imio/schedule/indexes.zcml
-drwxrwxr-x   0 fngaha    (1000) fngaha    (1000)        0 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio.schedule.egg-info/
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      201 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio.schedule.egg-info/requires.txt
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     4673 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio.schedule.egg-info/PKG-INFO
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        1 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio.schedule.egg-info/not-zip-safe
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        5 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio.schedule.egg-info/namespace_packages.txt
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        1 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio.schedule.egg-info/dependency_links.txt
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)        5 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio.schedule.egg-info/top_level.txt
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)       53 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio.schedule.egg-info/entry_points.txt
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     5506 2023-04-06 09:22:10.000000 imio.schedule-1.8/src/imio.schedule.egg-info/SOURCES.txt
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     4673 2023-04-06 09:22:10.000000 imio.schedule-1.8/PKG-INFO
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      140 2023-04-06 09:22:10.000000 imio.schedule-1.8/setup.cfg
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1758 2023-04-06 09:22:09.000000 imio.schedule-1.8/setup.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     7458 2023-04-06 09:22:09.000000 imio.schedule-1.8/bootstrap.py
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)       41 2023-04-06 09:22:09.000000 imio.schedule-1.8/CONTRIBUTORS.rst
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)       91 2023-04-06 09:22:09.000000 imio.schedule-1.8/MANIFEST.in
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1218 2023-04-06 09:22:09.000000 imio.schedule-1.8/CHANGES.rst
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)     1543 2023-04-06 09:22:09.000000 imio.schedule-1.8/README.rst
--rw-rw-r--   0 fngaha    (1000) fngaha    (1000)      703 2023-04-06 09:22:09.000000 imio.schedule-1.8/Makefile
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1320 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/CHANGES.rst
+-rw-r--r--   0 mpeeters   (501) staff       (20)       41 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/CONTRIBUTORS.rst
+-rw-r--r--   0 mpeeters   (501) staff       (20)       91 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/MANIFEST.in
+-rw-r--r--   0 mpeeters   (501) staff       (20)      703 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/Makefile
+-rw-r--r--   0 mpeeters   (501) staff       (20)     4857 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/PKG-INFO
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1543 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/README.rst
+-rw-r--r--   0 mpeeters   (501) staff       (20)     7458 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/bootstrap.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/docs/
+-rw-r--r--   0 mpeeters   (501) staff       (20)    18092 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/docs/LICENSE.GPL
+-rw-r--r--   0 mpeeters   (501) staff       (20)      658 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/docs/LICENSE.rst
+-rw-r--r--   0 mpeeters   (501) staff       (20)       76 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/docs/index.rst
+-rw-r--r--   0 mpeeters   (501) staff       (20)      140 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/setup.cfg
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1760 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/setup.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/
+-rw-r--r--   0 mpeeters   (501) staff       (20)       80 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/__init__.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/schedule/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      130 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/__init__.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/schedule/browser/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/browser/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1071 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/browser/close_task.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1806 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/browser/configure.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/schedule/browser/overrides/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/browser/overrides/.gitkeep
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/schedule/browser/static/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/browser/static/.gitkeep
+-rw-r--r--   0 mpeeters   (501) staff       (20)      175 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/browser/static/overlay.js
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1016 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/browser/static/schedule.css
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3696 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/browser/task_completion.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1324 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/browser/task_owner.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/schedule/browser/templates/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      566 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/browser/templates/close_task.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)      577 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/browser/templates/task_change_owner.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3167 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/browser/templates/task_completion.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5112 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/browser/templates/taskmacros.pt
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/schedule/collectionwidget/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/collectionwidget/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      638 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/collectionwidget/configure.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/schedule/collectionwidget/templates/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1569 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/collectionwidget/templates/term.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)      439 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/collectionwidget/views.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1264 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/collectionwidget/vocabulary.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      661 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/config.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1281 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/configure.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/schedule/content/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/content/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5091 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/content/condition.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2177 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/content/conditions.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      362 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/content/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2273 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/content/delay.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      592 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/content/delay.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     4054 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/content/logic.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1276 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/content/logic.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     6337 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/content/object_factories.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3432 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/content/object_factories.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2764 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/content/schedule_config.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1641 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/content/subform_context_choice.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     8001 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/content/task.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)    46099 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/content/task_config.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      460 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/content/view.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      304 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/content/view.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)    16202 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/content/vocabulary.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5614 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/content/vocabulary.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      616 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/content/widget.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/schedule/dashboard/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/dashboard/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     7287 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/dashboard/columns.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2640 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/dashboard/columns.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      178 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/dashboard/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      624 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/dashboard/interfaces.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1386 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/dashboard/vocabulary.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      534 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/dashboard/vocabulary.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/schedule/events/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/events/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5177 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/events/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1810 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/events/create_task.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2573 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/events/dashboard_collection.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2174 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/events/task_config.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     7941 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/events/update_tasks.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     8333 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/events/zope_registration.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      611 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/indexes.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      378 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/indexes.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     4626 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/interfaces.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/schedule/locales/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      767 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/locales/collective.eeafaceted.z3ctable.pot
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/schedule/locales/fr/
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/schedule/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      666 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/schedule/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.mo
+-rw-r--r--   0 mpeeters   (501) staff       (20)      701 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.po
+-rw-r--r--   0 mpeeters   (501) staff       (20)     8147 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/schedule/locales/fr/LC_MESSAGES/imio.schedule.mo
+-rw-r--r--   0 mpeeters   (501) staff       (20)    12139 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/locales/fr/LC_MESSAGES/imio.schedule.po
+-rw-r--r--   0 mpeeters   (501) staff       (20)     9239 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/locales/imio.schedule.pot
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1575 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/locales/manual_translations.pot
+-rwxr-xr-x   0 mpeeters   (501) staff       (20)      686 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/locales/update.sh
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/schedule/migration/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/migration/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      244 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/migration/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      561 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/migration/migrate_to_18.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      393 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/migration/upgrades.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/schedule/profiles/
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/schedule/profiles/default/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      148 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/profiles/default/browserlayer.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      554 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/profiles/default/catalog.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      490 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/profiles/default/cssregistry.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/profiles/default/imioschedule_default.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)      655 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/profiles/default/jsregistry.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      369 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/profiles/default/metadata.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      231 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/profiles/default/propertiestool.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1595 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/profiles/default/registry.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/schedule/profiles/default/types/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2134 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/profiles/default/types/AutomatedMacroTask.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1955 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/profiles/default/types/AutomatedTask.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2193 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/profiles/default/types/MacroTaskConfig.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2193 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/profiles/default/types/ScheduleConfig.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2087 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/profiles/default/types/TaskConfig.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      488 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/profiles/default/types.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      369 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/profiles/default/workflows.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/schedule/profiles/testing/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/profiles/testing/imioschedule_testing.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)      164 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/profiles/testing/metadata.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      222 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/setuphandlers.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     7829 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/testing.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      782 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/testing.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/schedule/tests/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/tests/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1774 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/tests/condition.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3056 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/tests/conditions.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      396 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/tests/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      279 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/tests/due_date.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      391 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/tests/due_date.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      318 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/tests/holidays.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      426 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/tests/logic.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      455 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/tests/logic.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/schedule/tests/robot/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1542 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/tests/robot/test_example.robot
+-rw-r--r--   0 mpeeters   (501) staff       (20)     9742 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/tests/setup.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1003 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/tests/test_dashboardcollection.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2292 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/tests/test_delay.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1197 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/tests/test_indexes.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2792 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/tests/test_logic.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     6586 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/tests/test_registration_events.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     4809 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/tests/test_scheduleconfig.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3294 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/tests/test_setup.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)    10523 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/tests/test_task.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)    17095 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/tests/test_task_events.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)    57639 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/tests/test_taskconfig.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3361 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/tests/test_utils.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)    13257 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/tests/test_vocabulary.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     7336 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/utils.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      847 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/vocabularies.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      461 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/vocabularies.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio/schedule/workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/workflow/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      404 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/workflow/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1286 2023-07-03 09:37:49.000000 imio.schedule-1.9.0/src/imio/schedule/workflow/freeze_task.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio.schedule.egg-info/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     4857 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio.schedule.egg-info/PKG-INFO
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5639 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio.schedule.egg-info/SOURCES.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)        1 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio.schedule.egg-info/dependency_links.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)       53 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio.schedule.egg-info/entry_points.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)        5 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio.schedule.egg-info/namespace_packages.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)        1 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio.schedule.egg-info/not-zip-safe
+-rw-r--r--   0 mpeeters   (501) staff       (20)      201 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio.schedule.egg-info/requires.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)        5 2023-07-03 09:37:50.000000 imio.schedule-1.9.0/src/imio.schedule.egg-info/top_level.txt
```

### Comparing `imio.schedule-1.8/docs/LICENSE.rst` & `imio.schedule-1.9.0/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/docs/LICENSE.GPL` & `imio.schedule-1.9.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/collectionwidget/configure.zcml` & `imio.schedule-1.9.0/src/imio/schedule/collectionwidget/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/collectionwidget/vocabulary.py` & `imio.schedule-1.9.0/src/imio/schedule/collectionwidget/vocabulary.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/collectionwidget/templates/term.pt` & `imio.schedule-1.9.0/src/imio/schedule/collectionwidget/templates/term.pt`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/tests/test_scheduleconfig.py` & `imio.schedule-1.9.0/src/imio/schedule/tests/test_scheduleconfig.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/tests/conditions.zcml` & `imio.schedule-1.9.0/src/imio/schedule/tests/conditions.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/tests/test_task.py` & `imio.schedule-1.9.0/src/imio/schedule/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/tests/test_dashboardcollection.py` & `imio.schedule-1.9.0/src/imio/schedule/tests/test_dashboardcollection.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/tests/test_task_events.py` & `imio.schedule-1.9.0/src/imio/schedule/tests/test_task_events.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/tests/test_utils.py` & `imio.schedule-1.9.0/src/imio/schedule/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/tests/setup.py` & `imio.schedule-1.9.0/src/imio/schedule/tests/setup.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/tests/robot/test_example.robot` & `imio.schedule-1.9.0/src/imio/schedule/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/tests/test_registration_events.py` & `imio.schedule-1.9.0/src/imio/schedule/tests/test_registration_events.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/tests/test_delay.py` & `imio.schedule-1.9.0/src/imio/schedule/tests/test_delay.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/tests/test_vocabulary.py` & `imio.schedule-1.9.0/src/imio/schedule/tests/test_vocabulary.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/tests/test_taskconfig.py` & `imio.schedule-1.9.0/src/imio/schedule/tests/test_taskconfig.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/tests/condition.py` & `imio.schedule-1.9.0/src/imio/schedule/tests/condition.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/tests/test_indexes.py` & `imio.schedule-1.9.0/src/imio/schedule/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/tests/test_logic.py` & `imio.schedule-1.9.0/src/imio/schedule/tests/test_logic.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/tests/test_setup.py` & `imio.schedule-1.9.0/src/imio/schedule/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/content/task_config.py` & `imio.schedule-1.9.0/src/imio/schedule/content/task_config.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/content/subform_context_choice.py` & `imio.schedule-1.9.0/src/imio/schedule/content/subform_context_choice.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/content/conditions.zcml` & `imio.schedule-1.9.0/src/imio/schedule/content/conditions.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/content/object_factories.zcml` & `imio.schedule-1.9.0/src/imio/schedule/content/object_factories.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/content/vocabulary.py` & `imio.schedule-1.9.0/src/imio/schedule/content/vocabulary.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/content/logic.py` & `imio.schedule-1.9.0/src/imio/schedule/content/logic.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/content/delay.zcml` & `imio.schedule-1.9.0/src/imio/schedule/content/delay.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/content/vocabulary.zcml` & `imio.schedule-1.9.0/src/imio/schedule/content/vocabulary.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/content/widget.zcml` & `imio.schedule-1.9.0/src/imio/schedule/content/widget.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/content/delay.py` & `imio.schedule-1.9.0/src/imio/schedule/content/delay.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/content/logic.zcml` & `imio.schedule-1.9.0/src/imio/schedule/content/logic.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/content/object_factories.py` & `imio.schedule-1.9.0/src/imio/schedule/content/object_factories.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/content/condition.py` & `imio.schedule-1.9.0/src/imio/schedule/content/condition.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/content/schedule_config.py` & `imio.schedule-1.9.0/src/imio/schedule/content/schedule_config.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/content/task.py` & `imio.schedule-1.9.0/src/imio/schedule/content/task.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/interfaces.py` & `imio.schedule-1.9.0/src/imio/schedule/interfaces.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/locales/update.sh` & `imio.schedule-1.9.0/src/imio/schedule/locales/update.sh`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/locales/collective.eeafaceted.z3ctable.pot` & `imio.schedule-1.9.0/src/imio/schedule/locales/collective.eeafaceted.z3ctable.pot`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: collective.eeafaceted.z3ctable\n"
 
-msgid "header_assigned_user_column"
+msgid "header_assigned_user"
 msgstr ""
 
 msgid "header_due_date"
 msgstr ""
 
 msgid "header_status"
 msgstr ""
```

### Comparing `imio.schedule-1.8/src/imio/schedule/locales/manual_translations.pot` & `imio.schedule-1.9.0/src/imio/schedule/locales/manual_translations.pot`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/locales/fr/LC_MESSAGES/imio.schedule.po` & `imio.schedule-1.9.0/src/imio/schedule/locales/fr/LC_MESSAGES/imio.schedule.po`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.po` & `imio.schedule-1.9.0/src/imio/schedule/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.po`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: DOMAIN\n"
 
-msgid "header_assigned_user_column"
+msgid "header_assigned_user"
 msgstr "Assigné à"
 
 msgid "header_due_date"
 msgstr "Échéance"
 
 msgid "header_simple_status"
 msgstr "Statut"
```

### Comparing `imio.schedule-1.8/src/imio/schedule/locales/imio.schedule.pot` & `imio.schedule-1.9.0/src/imio/schedule/locales/imio.schedule.pot`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/configure.zcml` & `imio.schedule-1.9.0/src/imio/schedule/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/vocabularies.py` & `imio.schedule-1.9.0/src/imio/schedule/vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/events/update_tasks.py` & `imio.schedule-1.9.0/src/imio/schedule/events/update_tasks.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/events/task_config.py` & `imio.schedule-1.9.0/src/imio/schedule/events/task_config.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/events/configure.zcml` & `imio.schedule-1.9.0/src/imio/schedule/events/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/events/zope_registration.py` & `imio.schedule-1.9.0/src/imio/schedule/events/zope_registration.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/events/dashboard_collection.py` & `imio.schedule-1.9.0/src/imio/schedule/events/dashboard_collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,28 +28,28 @@
                 {
                     'i': 'review_state',
                     'o': 'plone.app.querystring.operation.selection.is',
                     'v': ['to_do']
                 }
             ],
             'customViewFields': (
-                u'assigned_user_column',
+                u'assigned_user',
                 u'status',
                 u'due_date'
             ),
             'sort_on': u'due_date',
             'sort_reversed': True,
             'b_size': 30
         }
 
         if IScheduleConfig.providedBy(schedule_container):
             factory_args['customViewFields'] = (
                 u'pretty_link',
                 u'sortable_title',
-                u'assigned_user_column',
+                u'assigned_user',
                 u'status',
                 u'due_date'
             )
 
         kwargs = {}
         additional_queries = kwargs.pop('query', [])
         for query in additional_queries:
```

### Comparing `imio.schedule-1.8/src/imio/schedule/events/create_task.py` & `imio.schedule-1.9.0/src/imio/schedule/events/create_task.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/workflow/freeze_task.py` & `imio.schedule-1.9.0/src/imio/schedule/workflow/freeze_task.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/testing.py` & `imio.schedule-1.9.0/src/imio/schedule/testing.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/migration/migrate_to_18.py` & `imio.schedule-1.9.0/src/imio/schedule/migration/migrate_to_18.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/browser/configure.zcml` & `imio.schedule-1.9.0/src/imio/schedule/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/browser/close_task.py` & `imio.schedule-1.9.0/src/imio/schedule/browser/close_task.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/browser/templates/task_change_owner.pt` & `imio.schedule-1.9.0/src/imio/schedule/browser/templates/task_change_owner.pt`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/browser/templates/task_completion.pt` & `imio.schedule-1.9.0/src/imio/schedule/browser/templates/task_completion.pt`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/browser/templates/close_task.pt` & `imio.schedule-1.9.0/src/imio/schedule/browser/templates/close_task.pt`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/browser/templates/taskmacros.pt` & `imio.schedule-1.9.0/src/imio/schedule/browser/templates/taskmacros.pt`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/browser/task_owner.py` & `imio.schedule-1.9.0/src/imio/schedule/browser/task_owner.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/browser/task_completion.py` & `imio.schedule-1.9.0/src/imio/schedule/browser/task_completion.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/browser/static/schedule.css` & `imio.schedule-1.9.0/src/imio/schedule/browser/static/schedule.css`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     text-align: center;
 }
 
 td.td_cell_status {
     text-align: left;
 }
 
-td.td_cell_assigned_user_column {
+td.td_cell_assigned_user {
     text-align: center;
 }
 
 span.schedule_created {
     background-color: #ff9000;
 }
```

### Comparing `imio.schedule-1.8/src/imio/schedule/profiles/default/types/ScheduleConfig.xml` & `imio.schedule-1.9.0/src/imio/schedule/profiles/default/types/ScheduleConfig.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/profiles/default/types/AutomatedTask.xml` & `imio.schedule-1.9.0/src/imio/schedule/profiles/default/types/AutomatedTask.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/profiles/default/types/TaskConfig.xml` & `imio.schedule-1.9.0/src/imio/schedule/profiles/default/types/TaskConfig.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/profiles/default/types/MacroTaskConfig.xml` & `imio.schedule-1.9.0/src/imio/schedule/profiles/default/types/MacroTaskConfig.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/profiles/default/types/AutomatedMacroTask.xml` & `imio.schedule-1.9.0/src/imio/schedule/profiles/default/types/AutomatedMacroTask.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/profiles/default/catalog.xml` & `imio.schedule-1.9.0/src/imio/schedule/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/profiles/default/jsregistry.xml` & `imio.schedule-1.9.0/src/imio/schedule/profiles/default/jsregistry.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/profiles/default/registry.xml` & `imio.schedule-1.9.0/src/imio/schedule/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/utils.py` & `imio.schedule-1.9.0/src/imio/schedule/utils.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/indexes.py` & `imio.schedule-1.9.0/src/imio/schedule/indexes.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/config.py` & `imio.schedule-1.9.0/src/imio/schedule/config.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/testing.zcml` & `imio.schedule-1.9.0/src/imio/schedule/testing.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/dashboard/columns.py` & `imio.schedule-1.9.0/src/imio/schedule/dashboard/columns.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/dashboard/interfaces.py` & `imio.schedule-1.9.0/src/imio/schedule/dashboard/interfaces.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/dashboard/vocabulary.py` & `imio.schedule-1.9.0/src/imio/schedule/dashboard/vocabulary.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/dashboard/vocabulary.zcml` & `imio.schedule-1.9.0/src/imio/schedule/dashboard/vocabulary.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/src/imio/schedule/dashboard/columns.zcml` & `imio.schedule-1.9.0/src/imio/schedule/dashboard/columns.zcml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
   <adapter
      for="zope.interface.Interface
           zope.publisher.interfaces.browser.IBrowserRequest
           collective.eeafaceted.z3ctable.interfaces.IFacetedTable"
      factory=".columns.AssignedUserColumn"
      provides="collective.eeafaceted.z3ctable.interfaces.IFacetedColumn"
-     name="assigned_user_column"
+     name="assigned_user"
   />
 
   <adapter
      for="zope.interface.Interface
           zope.publisher.interfaces.browser.IBrowserRequest
           collective.eeafaceted.z3ctable.interfaces.IFacetedTable"
      factory=".columns.StatusColum"
```

### Comparing `imio.schedule-1.8/src/imio.schedule.egg-info/PKG-INFO` & `imio.schedule-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.schedule
-Version: 1.8
+Version: 1.9.0
 Summary: Schedule for imio products
 Home-page: https://pypi.python.org/pypi/imio.schedule
 Author: Simon Delcourt
 Author-email: simon.delcourt@imio.be
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide_addons.html
@@ -84,23 +84,33 @@
         
         - Simon Delcourt, simon.delcourt@imio.be
         
         Changelog
         =========
         
         
+        1.9.0 (2023-07-03)
+        ------------------
+        
+        - URB-1537 - Change collection column name
+          [jchandelle]
+        
+        
         1.8 (2023-04-06)
         ----------------
         
         - Allow multiple interfaces to be registered on schedule config.
           [sdelcourt]
+        
         - Get tasks and subtasks attribute exploration rather than catalog.
           [sdelcourt]
+        
         - Add method 'get_closed_tasks' on TaskConfig.
           [sdelcourt]
+        
         - Add util method 'end_all_open_tasks' of a container.
           [sdelcourt]
         
         
         1.6 (2018-08-30)
         ----------------
```

### Comparing `imio.schedule-1.8/src/imio.schedule.egg-info/SOURCES.txt` & `imio.schedule-1.9.0/src/imio.schedule.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,17 @@
 src/imio/schedule/events/task_config.py
 src/imio/schedule/events/update_tasks.py
 src/imio/schedule/events/zope_registration.py
 src/imio/schedule/locales/collective.eeafaceted.z3ctable.pot
 src/imio/schedule/locales/imio.schedule.pot
 src/imio/schedule/locales/manual_translations.pot
 src/imio/schedule/locales/update.sh
+src/imio/schedule/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.mo
 src/imio/schedule/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.po
+src/imio/schedule/locales/fr/LC_MESSAGES/imio.schedule.mo
 src/imio/schedule/locales/fr/LC_MESSAGES/imio.schedule.po
 src/imio/schedule/migration/__init__.py
 src/imio/schedule/migration/configure.zcml
 src/imio/schedule/migration/migrate_to_18.py
 src/imio/schedule/migration/upgrades.zcml
 src/imio/schedule/profiles/default/browserlayer.xml
 src/imio/schedule/profiles/default/catalog.xml
```

### Comparing `imio.schedule-1.8/PKG-INFO` & `imio.schedule-1.9.0/src/imio.schedule.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.schedule
-Version: 1.8
+Version: 1.9.0
 Summary: Schedule for imio products
 Home-page: https://pypi.python.org/pypi/imio.schedule
 Author: Simon Delcourt
 Author-email: simon.delcourt@imio.be
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide_addons.html
@@ -84,23 +84,33 @@
         
         - Simon Delcourt, simon.delcourt@imio.be
         
         Changelog
         =========
         
         
+        1.9.0 (2023-07-03)
+        ------------------
+        
+        - URB-1537 - Change collection column name
+          [jchandelle]
+        
+        
         1.8 (2023-04-06)
         ----------------
         
         - Allow multiple interfaces to be registered on schedule config.
           [sdelcourt]
+        
         - Get tasks and subtasks attribute exploration rather than catalog.
           [sdelcourt]
+        
         - Add method 'get_closed_tasks' on TaskConfig.
           [sdelcourt]
+        
         - Add util method 'end_all_open_tasks' of a container.
           [sdelcourt]
         
         
         1.6 (2018-08-30)
         ----------------
```

### Comparing `imio.schedule-1.8/setup.py` & `imio.schedule-1.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     '\n' +
     open('CHANGES.rst').read() +
     '\n')
 
 
 setup(
     name='imio.schedule',
-    version='1.8',
+    version='1.9.0',
     description="Schedule for imio products",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 4.3",
```

### Comparing `imio.schedule-1.8/bootstrap.py` & `imio.schedule-1.9.0/bootstrap.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/CHANGES.rst` & `imio.schedule-1.9.0/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 Changelog
 =========
 
 
+1.9.0 (2023-07-03)
+------------------
+
+- URB-1537 - Change collection column name
+  [jchandelle]
+
+
 1.8 (2023-04-06)
 ----------------
 
 - Allow multiple interfaces to be registered on schedule config.
   [sdelcourt]
+
 - Get tasks and subtasks attribute exploration rather than catalog.
   [sdelcourt]
+
 - Add method 'get_closed_tasks' on TaskConfig.
   [sdelcourt]
+
 - Add util method 'end_all_open_tasks' of a container.
   [sdelcourt]
 
 
 1.6 (2018-08-30)
 ----------------
```

### Comparing `imio.schedule-1.8/README.rst` & `imio.schedule-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `imio.schedule-1.8/Makefile` & `imio.schedule-1.9.0/Makefile`

 * *Files identical despite different names*


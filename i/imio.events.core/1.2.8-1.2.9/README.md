# Comparing `tmp/imio.events.core-1.2.8.tar.gz` & `tmp/imio.events.core-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imio.events.core-1.2.8.tar", last modified: Tue Mar 12 09:34:19 2024, max compression
+gzip compressed data, was "imio.events.core-1.2.9.tar", last modified: Wed Mar 13 12:04:34 2024, max compression
```

## Comparing `imio.events.core-1.2.8.tar` & `imio.events.core-1.2.9.tar`

### file list

```diff
@@ -1,162 +1,164 @@
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.806571 imio.events.core-1.2.8/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5967 2024-03-12 09:34:18.000000 imio.events.core-1.2.8/CHANGES.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       64 2024-03-12 09:34:18.000000 imio.events.core-1.2.8/CONTRIBUTORS.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      522 2024-03-12 09:34:18.000000 imio.events.core-1.2.8/DEVELOP.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2024-03-12 09:34:18.000000 imio.events.core-1.2.8/LICENSE.GPL
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      651 2024-03-12 09:34:18.000000 imio.events.core-1.2.8/LICENSE.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       61 2024-03-12 09:34:18.000000 imio.events.core-1.2.8/MANIFEST.in
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9021 2024-03-12 09:34:19.806571 imio.events.core-1.2.8/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1993 2024-03-12 09:34:18.000000 imio.events.core-1.2.8/README.rst
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.790571 imio.events.core-1.2.8/docs/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7958 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/docs/conf.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       71 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/docs/index.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2024-03-12 09:34:19.806571 imio.events.core-1.2.8/setup.cfg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2536 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/setup.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.782571 imio.events.core-1.2.8/src/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.790571 imio.events.core-1.2.8/src/imio/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.794571 imio.events.core-1.2.8/src/imio/events/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.794571 imio.events.core-1.2.8/src/imio/events/core/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      267 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.798571 imio.events.core-1.2.8/src/imio/events/core/browser/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/browser/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.798571 imio.events.core-1.2.8/src/imio/events/core/browser/bring_event_into_agendas/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/browser/bring_event_into_agendas/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3147 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/browser/bring_event_into_agendas/agendas.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      319 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/browser/bring_event_into_agendas/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1779 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/browser/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2485 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/browser/forms.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      760 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/browser/json_recurrence.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.798571 imio.events.core-1.2.8/src/imio/events/core/browser/overrides/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/browser/overrides/.gitkeep
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.798571 imio.events.core-1.2.8/src/imio/events/core/browser/static/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/browser/static/.gitkeep
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1472 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/browser/utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      884 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.798571 imio.events.core-1.2.8/src/imio/events/core/contents/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/contents/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.798571 imio.events.core-1.2.8/src/imio/events/core/contents/agenda/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/contents/agenda/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/contents/agenda/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1264 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/contents/agenda/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      198 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/contents/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.798571 imio.events.core-1.2.8/src/imio/events/core/contents/entity/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/contents/entity/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/contents/entity/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1153 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/contents/entity/content.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.798571 imio.events.core-1.2.8/src/imio/events/core/contents/event/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/contents/event/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      682 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/contents/event/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6728 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/contents/event/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2785 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/contents/event/serializer.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8451 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/contents/event/view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4315 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/contents/event/views.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.798571 imio.events.core-1.2.8/src/imio/events/core/contents/folder/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/contents/folder/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/contents/folder/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      314 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/contents/folder/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      487 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/converters.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.786571 imio.events.core-1.2.8/src/imio/events/core/faceted/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.798571 imio.events.core-1.2.8/src/imio/events/core/faceted/config/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8038 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/faceted/config/events.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5107 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/indexers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1795 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/indexers.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      201 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/interfaces.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      343 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/overrides.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      520 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/permissions.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.786571 imio.events.core-1.2.8/src/imio/events/core/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.802571 imio.events.core-1.2.8/src/imio/events/core/profiles/default/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      173 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/profiles/default/browserlayer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2525 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/profiles/default/catalog.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2833 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/profiles/default/contentrules.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      203 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/profiles/default/diff_tool.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      590 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/profiles/default/metadata.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1299 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/profiles/default/registry.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      251 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/profiles/default/repositorytool.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      840 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/profiles/default/rolemap.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.802571 imio.events.core-1.2.8/src/imio/events/core/profiles/default/taxonomies/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      316 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/profiles/default/taxonomies/event_public.cfg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4154 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/profiles/default/taxonomies/event_public.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.802571 imio.events.core-1.2.8/src/imio/events/core/profiles/default/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      297 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/profiles/default/types/Plone_Site.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1422 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/profiles/default/types/imio.events.Agenda.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1619 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/profiles/default/types/imio.events.Entity.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1735 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/profiles/default/types/imio.events.Event.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1381 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/profiles/default/types/imio.events.Folder.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      362 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/profiles/default/types.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.802571 imio.events.core-1.2.8/src/imio/events/core/profiles/uninstall/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      126 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      890 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/profiles.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.802571 imio.events.core-1.2.8/src/imio/events/core/rest/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/rest/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      395 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/rest/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6486 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/rest/endpoint.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      667 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/setuphandlers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6564 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/subscribers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1308 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/subscribers.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1873 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/testing.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.802571 imio.events.core-1.2.8/src/imio/events/core/tests/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/tests/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.806571 imio.events.core-1.2.8/src/imio/events/core/tests/resources/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    24753 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/tests/resources/plone.png
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.806571 imio.events.core-1.2.8/src/imio/events/core/tests/robot/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2876 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/tests/robot/test_ct_imio_events_agenda.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2852 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/tests/robot/test_ct_imio_events_event.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2876 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/tests/robot/test_ct_imio_events_folder.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1995 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/tests/robot/test_example.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8078 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/tests/test_agenda.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4412 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/tests/test_bring_event_into_agendas.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1597 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/tests/test_cropping.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3566 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/tests/test_entity.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18914 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/tests/test_event.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4202 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/tests/test_folder.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9739 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/tests/test_indexes.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2204 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/tests/test_local_roles.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7860 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/tests/test_multilingual.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5919 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/tests/test_rest.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      935 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/tests/test_robot.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1971 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/tests/test_setup.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8718 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/tests/test_utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5147 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/tests/test_vocabularies.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      273 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/tests/utils.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.806571 imio.events.core-1.2.8/src/imio/events/core/upgrades/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/upgrades/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5392 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/upgrades/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.786571 imio.events.core-1.2.8/src/imio/events/core/upgrades/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.806571 imio.events.core-1.2.8/src/imio/events/core/upgrades/profiles/1002_to_1003/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      183 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/upgrades/profiles/1002_to_1003/types.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.806571 imio.events.core-1.2.8/src/imio/events/core/upgrades/profiles/1005_to_1006/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1066 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/upgrades/profiles/1005_to_1006/catalog.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.806571 imio.events.core-1.2.8/src/imio/events/core/upgrades/profiles/1010_to_1011/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2833 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/upgrades/profiles/1010_to_1011/contentrules.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      203 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/upgrades/profiles/1010_to_1011/diff_tool.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      251 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/upgrades/profiles/1010_to_1011/repositorytool.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.806571 imio.events.core-1.2.8/src/imio/events/core/upgrades/profiles/1010_to_1011/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      281 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/upgrades/profiles/1010_to_1011/types/imio.events.Event.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.806571 imio.events.core-1.2.8/src/imio/events/core/upgrades/profiles/1011_to_1012/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      743 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/upgrades/profiles/1011_to_1012/registry.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.786571 imio.events.core-1.2.8/src/imio/events/core/upgrades/profiles/1012_to_1013/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.806571 imio.events.core-1.2.8/src/imio/events/core/upgrades/profiles/1012_to_1013/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      307 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/upgrades/profiles/1012_to_1013/types/imio.events.Agenda.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      307 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/upgrades/profiles/1012_to_1013/types/imio.events.Entity.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      306 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/upgrades/profiles/1012_to_1013/types/imio.events.Event.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      307 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/upgrades/profiles/1012_to_1013/types/imio.events.Folder.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3666 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/upgrades/upgrades.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3504 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/utils.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.806571 imio.events.core-1.2.8/src/imio/events/core/viewlets/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/viewlets/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      527 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/viewlets/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.806571 imio.events.core-1.2.8/src/imio/events/core/viewlets/event/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      339 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/viewlets/event/button_to_bring_event.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      420 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/viewlets/event.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5533 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/vocabularies.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1180 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio/events/core/vocabularies.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-12 09:34:19.794571 imio.events.core-1.2.8/src/imio.events.core.egg-info/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9021 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio.events.core.egg-info/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5640 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio.events.core.egg-info/SOURCES.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio.events.core.egg-info/dependency_links.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       17 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio.events.core.egg-info/namespace_packages.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio.events.core.egg-info/not-zip-safe
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      352 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio.events.core.egg-info/requires.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2024-03-12 09:34:19.000000 imio.events.core-1.2.8/src/imio.events.core.egg-info/top_level.txt
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.813291 imio.events.core-1.2.9/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6114 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/CHANGES.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       64 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/CONTRIBUTORS.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      522 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/DEVELOP.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/LICENSE.GPL
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      651 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/LICENSE.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       61 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/MANIFEST.in
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9168 2024-03-13 12:04:34.813291 imio.events.core-1.2.9/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1993 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/README.rst
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.801291 imio.events.core-1.2.9/docs/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7958 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/docs/conf.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       71 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/docs/index.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2024-03-13 12:04:34.813291 imio.events.core-1.2.9/setup.cfg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2536 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/setup.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.797291 imio.events.core-1.2.9/src/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.801291 imio.events.core-1.2.9/src/imio/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.805291 imio.events.core-1.2.9/src/imio/events/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.805291 imio.events.core-1.2.9/src/imio/events/core/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      267 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.805291 imio.events.core-1.2.9/src/imio/events/core/browser/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/browser/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.805291 imio.events.core-1.2.9/src/imio/events/core/browser/bring_event_into_agendas/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/browser/bring_event_into_agendas/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3618 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/browser/bring_event_into_agendas/agendas.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      319 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/browser/bring_event_into_agendas/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1779 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/browser/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2485 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/browser/forms.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      760 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/browser/json_recurrence.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.805291 imio.events.core-1.2.9/src/imio/events/core/browser/overrides/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/browser/overrides/.gitkeep
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.805291 imio.events.core-1.2.9/src/imio/events/core/browser/static/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/browser/static/.gitkeep
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1472 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/browser/utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      884 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.805291 imio.events.core-1.2.9/src/imio/events/core/contents/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/contents/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.805291 imio.events.core-1.2.9/src/imio/events/core/contents/agenda/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/contents/agenda/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/contents/agenda/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1264 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/contents/agenda/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      198 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/contents/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.805291 imio.events.core-1.2.9/src/imio/events/core/contents/entity/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/contents/entity/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/contents/entity/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1736 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/contents/entity/content.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.809291 imio.events.core-1.2.9/src/imio/events/core/contents/event/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/contents/event/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      682 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/contents/event/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6728 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/contents/event/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2785 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/contents/event/serializer.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8451 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/contents/event/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4315 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/contents/event/views.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.809291 imio.events.core-1.2.9/src/imio/events/core/contents/folder/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/contents/folder/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/contents/folder/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      314 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/contents/folder/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      487 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/converters.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.801291 imio.events.core-1.2.9/src/imio/events/core/faceted/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.809291 imio.events.core-1.2.9/src/imio/events/core/faceted/config/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8038 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/faceted/config/events.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5107 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/indexers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1795 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/indexers.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      201 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/interfaces.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      343 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/overrides.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      668 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/permissions.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.801291 imio.events.core-1.2.9/src/imio/events/core/profiles/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.809291 imio.events.core-1.2.9/src/imio/events/core/profiles/default/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      173 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/profiles/default/browserlayer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2525 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/profiles/default/catalog.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2833 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/profiles/default/contentrules.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      203 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/profiles/default/diff_tool.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      590 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/profiles/default/metadata.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1299 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/profiles/default/registry.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      251 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/profiles/default/repositorytool.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      979 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/profiles/default/rolemap.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.809291 imio.events.core-1.2.9/src/imio/events/core/profiles/default/taxonomies/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      316 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/profiles/default/taxonomies/event_public.cfg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4154 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/profiles/default/taxonomies/event_public.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.809291 imio.events.core-1.2.9/src/imio/events/core/profiles/default/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      297 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/profiles/default/types/Plone_Site.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1422 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/profiles/default/types/imio.events.Agenda.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1619 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/profiles/default/types/imio.events.Entity.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1735 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/profiles/default/types/imio.events.Event.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1381 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/profiles/default/types/imio.events.Folder.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      362 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/profiles/default/types.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.809291 imio.events.core-1.2.9/src/imio/events/core/profiles/uninstall/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      126 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      890 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/profiles.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.809291 imio.events.core-1.2.9/src/imio/events/core/rest/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/rest/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      395 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/rest/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6486 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/rest/endpoint.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      667 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/setuphandlers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6564 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/subscribers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1308 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/subscribers.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1873 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/testing.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.813291 imio.events.core-1.2.9/src/imio/events/core/tests/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/tests/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.813291 imio.events.core-1.2.9/src/imio/events/core/tests/resources/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    24753 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/tests/resources/plone.png
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.813291 imio.events.core-1.2.9/src/imio/events/core/tests/robot/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2876 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/tests/robot/test_ct_imio_events_agenda.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2852 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/tests/robot/test_ct_imio_events_event.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2876 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/tests/robot/test_ct_imio_events_folder.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1995 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/tests/robot/test_example.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8078 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/tests/test_agenda.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4412 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/tests/test_bring_event_into_agendas.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1597 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/tests/test_cropping.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3566 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/tests/test_entity.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18914 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/tests/test_event.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4202 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/tests/test_folder.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9739 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/tests/test_indexes.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2204 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/tests/test_local_roles.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7860 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/tests/test_multilingual.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5919 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/tests/test_rest.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      935 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/tests/test_robot.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1971 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/tests/test_setup.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8718 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/tests/test_utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5147 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/tests/test_vocabularies.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      273 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/tests/utils.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.813291 imio.events.core-1.2.9/src/imio/events/core/upgrades/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/upgrades/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6069 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/upgrades/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.801291 imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.813291 imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/1002_to_1003/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      183 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/1002_to_1003/types.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.813291 imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/1005_to_1006/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1066 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/1005_to_1006/catalog.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.813291 imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/1010_to_1011/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2833 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/1010_to_1011/contentrules.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      203 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/1010_to_1011/diff_tool.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      251 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/1010_to_1011/repositorytool.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.813291 imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/1010_to_1011/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      281 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/1010_to_1011/types/imio.events.Event.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.813291 imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/1011_to_1012/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      743 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/1011_to_1012/registry.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.801291 imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/1012_to_1013/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.813291 imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/1012_to_1013/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      307 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/1012_to_1013/types/imio.events.Agenda.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      307 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/1012_to_1013/types/imio.events.Entity.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      306 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/1012_to_1013/types/imio.events.Event.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      307 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/1012_to_1013/types/imio.events.Folder.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.813291 imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/1013_to_1014/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      216 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/1013_to_1014/rolemap.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3666 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/upgrades/upgrades.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3504 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/utils.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.813291 imio.events.core-1.2.9/src/imio/events/core/viewlets/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/viewlets/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      527 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/viewlets/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.813291 imio.events.core-1.2.9/src/imio/events/core/viewlets/event/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      339 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/viewlets/event/button_to_bring_event.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      616 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/viewlets/event.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5533 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/vocabularies.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1180 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio/events/core/vocabularies.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2024-03-13 12:04:34.805291 imio.events.core-1.2.9/src/imio.events.core.egg-info/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9168 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio.events.core.egg-info/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5704 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio.events.core.egg-info/SOURCES.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio.events.core.egg-info/dependency_links.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       17 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio.events.core.egg-info/namespace_packages.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio.events.core.egg-info/not-zip-safe
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      352 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio.events.core.egg-info/requires.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2024-03-13 12:04:34.000000 imio.events.core-1.2.9/src/imio.events.core.egg-info/top_level.txt
```

### Comparing `imio.events.core-1.2.8/CHANGES.rst` & `imio.events.core-1.2.9/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+1.2.9 (2024-03-13)
+------------------
+
+- WEB-4068 : Add field to limit the new feature "adding events in any agenda" to some entities
+  [boulch]
+
+
 1.2.8 (2024-03-12)
 ------------------
 
 - WEB-4068 : Refactor "adding events in any agenda" : (update translations, add feature : "remove agenda")
   [boulch]
```

### Comparing `imio.events.core-1.2.8/DEVELOP.rst` & `imio.events.core-1.2.9/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/LICENSE.GPL` & `imio.events.core-1.2.9/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/LICENSE.rst` & `imio.events.core-1.2.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/PKG-INFO` & `imio.events.core-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.events.core
-Version: 1.2.8
+Version: 1.2.9
 Summary: Core product for iMio events website
 Home-page: https://github.com/collective/imio.events.core
 Author: iMio
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.events.core
 Project-URL: Source, https://github.com/collective/imio.events.core
@@ -119,14 +119,21 @@
 - iMio, christophe.boulanger@imio.be
 
 
 Changelog
 =========
 
 
+1.2.9 (2024-03-13)
+------------------
+
+- WEB-4068 : Add field to limit the new feature "adding events in any agenda" to some entities
+  [boulch]
+
+
 1.2.8 (2024-03-12)
 ------------------
 
 - WEB-4068 : Refactor "adding events in any agenda" : (update translations, add feature : "remove agenda")
   [boulch]
```

### Comparing `imio.events.core-1.2.8/README.rst` & `imio.events.core-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/docs/conf.py` & `imio.events.core-1.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/setup.cfg` & `imio.events.core-1.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/setup.py` & `imio.events.core-1.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="imio.events.core",
-    version="1.2.8",
+    version="1.2.9",
     description="Core product for iMio events website",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `imio.events.core-1.2.8/src/imio/events/core/browser/bring_event_into_agendas/agendas.py` & `imio.events.core-1.2.9/src/imio/events/core/browser/bring_event_into_agendas/agendas.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 
+from imio.events.core.utils import get_entity_for_obj
 from imio.smartweb.common.utils import get_vocabulary
 from imio.smartweb.locales import SmartwebMessageFactory as _
 from plone import api
 from plone.autoform import directives
 from plone.autoform.form import AutoExtensibleForm
 from plone.app.z3cform.widget import AjaxSelectFieldWidget
 from zope import schema
@@ -35,14 +36,24 @@
     """ """
 
     schema = IBringEventIntoAgendasForm
     ignoreContext = True
     enable_autofocus = False
     label = _("Add/Remove agenda(s)")
 
+    def update(self):
+        entity = get_entity_for_obj(self.context)
+        if entity.authorize_to_bring_event_anywhere is False:
+            api.portal.show_message(
+                _("You don't have rights to access this page."), self.request
+            )
+            self.request.response.redirect(self.context.absolute_url())
+            return False
+        super(BringEventIntoAgendasForm, self).update()
+
     def updateWidgets(self):
         agendas_to_display = []
         vocabulary = get_vocabulary("imio.events.vocabulary.UserAgendas")
         # Loop to display only agenda where user has the permission (ex : to remove these agendas out of event)
         for agenda_uid in self.context.selected_agendas:
             if vocabulary.by_token.get(agenda_uid) is None:
                 # user can't remove this agenda because he has no permission on it so we don't display it
```

### Comparing `imio.events.core-1.2.8/src/imio/events/core/browser/configure.zcml` & `imio.events.core-1.2.9/src/imio/events/core/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/browser/forms.py` & `imio.events.core-1.2.9/src/imio/events/core/browser/forms.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/browser/json_recurrence.py` & `imio.events.core-1.2.9/src/imio/events/core/browser/json_recurrence.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/browser/utils.py` & `imio.events.core-1.2.9/src/imio/events/core/browser/utils.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/configure.zcml` & `imio.events.core-1.2.9/src/imio/events/core/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/contents/agenda/content.py` & `imio.events.core-1.2.9/src/imio/events/core/contents/agenda/content.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/contents/event/configure.zcml` & `imio.events.core-1.2.9/src/imio/events/core/contents/event/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/contents/event/content.py` & `imio.events.core-1.2.9/src/imio/events/core/contents/event/content.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/contents/event/serializer.py` & `imio.events.core-1.2.9/src/imio/events/core/contents/event/serializer.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/contents/event/view.pt` & `imio.events.core-1.2.9/src/imio/events/core/contents/event/view.pt`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/contents/event/views.py` & `imio.events.core-1.2.9/src/imio/events/core/contents/event/views.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/faceted/config/events.xml` & `imio.events.core-1.2.9/src/imio/events/core/faceted/config/events.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/indexers.py` & `imio.events.core-1.2.9/src/imio/events/core/indexers.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/indexers.zcml` & `imio.events.core-1.2.9/src/imio/events/core/indexers.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/profiles/default/catalog.xml` & `imio.events.core-1.2.9/src/imio/events/core/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/profiles/default/contentrules.xml` & `imio.events.core-1.2.9/src/imio/events/core/profiles/default/contentrules.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/profiles/default/metadata.xml` & `imio.events.core-1.2.9/src/imio/events/core/profiles/default/metadata.xml`

 * *Files 14% similar despite different names*

#### Comparing `imio.events.core-1.2.8/src/imio/events/core/profiles/default/metadata.xml` & `imio.events.core-1.2.9/src/imio/events/core/profiles/default/metadata.xml`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <metadata>
-  <version>1013</version>
+  <version>1014</version>
   <dependencies>
     <dependency>profile-plone.app.dexterity:default</dependency>
     <dependency>profile-plone.gallery:default</dependency>
     <dependency>profile-plone.app.imagecropping:default</dependency>
     <dependency>profile-collective.geolocationbehavior:default</dependency>
     <dependency>profile-collective.taxonomy:default</dependency>
     <dependency>profile-imio.smartweb.common:default</dependency>
```

### Comparing `imio.events.core-1.2.8/src/imio/events/core/profiles/default/registry.xml` & `imio.events.core-1.2.9/src/imio/events/core/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/profiles/default/rolemap.xml` & `imio.events.core-1.2.9/src/imio/events/core/profiles/default/rolemap.xml`

 * *Files 8% similar despite different names*

#### Comparing `imio.events.core-1.2.8/src/imio/events/core/profiles/default/rolemap.xml` & `imio.events.core-1.2.9/src/imio/events/core/profiles/default/rolemap.xml`

```diff
@@ -18,9 +18,12 @@
     </permission>
     <permission name="imio.events.core: Add Event" acquire="True">
       <role name="Manager"/>
       <role name="Site Administrator"/>
       <role name="Owner"/>
       <role name="Contributor"/>
     </permission>
+    <permission name="imio.events.core: Bring Event into personnal agenda" acquire="True">
+      <role name="Manager"/>
+    </permission>
   </permissions>
 </rolemap>
```

### Comparing `imio.events.core-1.2.8/src/imio/events/core/profiles/default/taxonomies/event_public.xml` & `imio.events.core-1.2.9/src/imio/events/core/profiles/default/taxonomies/event_public.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/profiles/default/types/imio.events.Agenda.xml` & `imio.events.core-1.2.9/src/imio/events/core/profiles/default/types/imio.events.Agenda.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/profiles/default/types/imio.events.Entity.xml` & `imio.events.core-1.2.9/src/imio/events/core/profiles/default/types/imio.events.Entity.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/profiles/default/types/imio.events.Event.xml` & `imio.events.core-1.2.9/src/imio/events/core/profiles/default/types/imio.events.Event.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/profiles/default/types/imio.events.Folder.xml` & `imio.events.core-1.2.9/src/imio/events/core/profiles/default/types/imio.events.Folder.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/profiles.zcml` & `imio.events.core-1.2.9/src/imio/events/core/profiles.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/rest/endpoint.py` & `imio.events.core-1.2.9/src/imio/events/core/rest/endpoint.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/setuphandlers.py` & `imio.events.core-1.2.9/src/imio/events/core/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/subscribers.py` & `imio.events.core-1.2.9/src/imio/events/core/subscribers.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/subscribers.zcml` & `imio.events.core-1.2.9/src/imio/events/core/subscribers.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/testing.py` & `imio.events.core-1.2.9/src/imio/events/core/testing.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/tests/resources/plone.png` & `imio.events.core-1.2.9/src/imio/events/core/tests/resources/plone.png`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/tests/robot/test_ct_imio_events_agenda.robot` & `imio.events.core-1.2.9/src/imio/events/core/tests/robot/test_ct_imio_events_agenda.robot`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/tests/robot/test_ct_imio_events_event.robot` & `imio.events.core-1.2.9/src/imio/events/core/tests/robot/test_ct_imio_events_event.robot`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/tests/robot/test_ct_imio_events_folder.robot` & `imio.events.core-1.2.9/src/imio/events/core/tests/robot/test_ct_imio_events_folder.robot`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/tests/robot/test_example.robot` & `imio.events.core-1.2.9/src/imio/events/core/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/tests/test_agenda.py` & `imio.events.core-1.2.9/src/imio/events/core/tests/test_agenda.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/tests/test_bring_event_into_agendas.py` & `imio.events.core-1.2.9/src/imio/events/core/tests/test_bring_event_into_agendas.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/tests/test_cropping.py` & `imio.events.core-1.2.9/src/imio/events/core/tests/test_cropping.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/tests/test_entity.py` & `imio.events.core-1.2.9/src/imio/events/core/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/tests/test_event.py` & `imio.events.core-1.2.9/src/imio/events/core/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/tests/test_folder.py` & `imio.events.core-1.2.9/src/imio/events/core/tests/test_folder.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/tests/test_indexes.py` & `imio.events.core-1.2.9/src/imio/events/core/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/tests/test_local_roles.py` & `imio.events.core-1.2.9/src/imio/events/core/tests/test_local_roles.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/tests/test_multilingual.py` & `imio.events.core-1.2.9/src/imio/events/core/tests/test_multilingual.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/tests/test_rest.py` & `imio.events.core-1.2.9/src/imio/events/core/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/tests/test_robot.py` & `imio.events.core-1.2.9/src/imio/events/core/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/tests/test_setup.py` & `imio.events.core-1.2.9/src/imio/events/core/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/tests/test_utils.py` & `imio.events.core-1.2.9/src/imio/events/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/tests/test_vocabularies.py` & `imio.events.core-1.2.9/src/imio/events/core/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/upgrades/configure.zcml` & `imio.events.core-1.2.9/src/imio/events/core/upgrades/configure.zcml`

 * *Files 8% similar despite different names*

```diff
@@ -31,22 +31,30 @@
       name="upgrade_1011_to_1012"
       title="Upgrade core from 1011 to 1012"
       directory="profiles/1011_to_1012"
       description="Exclude some content_types from search results"
       provides="Products.GenericSetup.interfaces.EXTENSION"
       />
 
-    <genericsetup:registerProfile
+  <genericsetup:registerProfile
       name="upgrade_1012_to_1013"
       title="Upgrade core from 1012 to 1013"
       directory="profiles/1012_to_1013"
       description="Add solr.fields behavior to some content types"
       provides="Products.GenericSetup.interfaces.EXTENSION"
       />
 
+  <genericsetup:registerProfile
+      name="upgrade_1013_to_1014"
+      title="Upgrade core from 1013 to 1014"
+      directory="profiles/1013_to_1014"
+      description="Add new permission to manager : imio.events.core.BringEventIntoPersonnalAgenda"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      />
+
   <genericsetup:upgradeStep
       title="Refresh faceted"
       description="Refresh faceted configurations on all entities / agendas"
       source="1000"
       destination="1001"
       handler=".upgrades.refresh_objects_faceted"
       profile="imio.events.core:default"
@@ -165,8 +173,18 @@
       profile="imio.events.core:default">
     <genericsetup:upgradeDepends
         title="Add solr.fields behavior to some content types"
         import_profile="imio.events.core.upgrades:upgrade_1012_to_1013"
         />
   </genericsetup:upgradeSteps>
 
+  <genericsetup:upgradeSteps
+      source="1013"
+      destination="1014"
+      profile="imio.events.core:default">
+    <genericsetup:upgradeDepends
+        title="Add new permission to manager : imio.events.core.BringEventIntoPersonnalAgenda"
+        import_profile="imio.events.core.upgrades:upgrade_1013_to_1014"
+        />
+  </genericsetup:upgradeSteps>
+
 </configure>
```

### Comparing `imio.events.core-1.2.8/src/imio/events/core/upgrades/profiles/1005_to_1006/catalog.xml` & `imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/1005_to_1006/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/upgrades/profiles/1010_to_1011/contentrules.xml` & `imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/1010_to_1011/contentrules.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/upgrades/profiles/1011_to_1012/registry.xml` & `imio.events.core-1.2.9/src/imio/events/core/upgrades/profiles/1011_to_1012/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/upgrades/upgrades.py` & `imio.events.core-1.2.9/src/imio/events/core/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/utils.py` & `imio.events.core-1.2.9/src/imio/events/core/utils.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/viewlets/configure.zcml` & `imio.events.core-1.2.9/src/imio/events/core/viewlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/vocabularies.py` & `imio.events.core-1.2.9/src/imio/events/core/vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio/events/core/vocabularies.zcml` & `imio.events.core-1.2.9/src/imio/events/core/vocabularies.zcml`

 * *Files identical despite different names*

### Comparing `imio.events.core-1.2.8/src/imio.events.core.egg-info/PKG-INFO` & `imio.events.core-1.2.9/src/imio.events.core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.events.core
-Version: 1.2.8
+Version: 1.2.9
 Summary: Core product for iMio events website
 Home-page: https://github.com/collective/imio.events.core
 Author: iMio
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.events.core
 Project-URL: Source, https://github.com/collective/imio.events.core
@@ -119,14 +119,21 @@
 - iMio, christophe.boulanger@imio.be
 
 
 Changelog
 =========
 
 
+1.2.9 (2024-03-13)
+------------------
+
+- WEB-4068 : Add field to limit the new feature "adding events in any agenda" to some entities
+  [boulch]
+
+
 1.2.8 (2024-03-12)
 ------------------
 
 - WEB-4068 : Refactor "adding events in any agenda" : (update translations, add feature : "remove agenda")
   [boulch]
```

### Comparing `imio.events.core-1.2.8/src/imio.events.core.egg-info/SOURCES.txt` & `imio.events.core-1.2.9/src/imio.events.core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -113,11 +113,12 @@
 src/imio/events/core/upgrades/profiles/1010_to_1011/repositorytool.xml
 src/imio/events/core/upgrades/profiles/1010_to_1011/types/imio.events.Event.xml
 src/imio/events/core/upgrades/profiles/1011_to_1012/registry.xml
 src/imio/events/core/upgrades/profiles/1012_to_1013/types/imio.events.Agenda.xml
 src/imio/events/core/upgrades/profiles/1012_to_1013/types/imio.events.Entity.xml
 src/imio/events/core/upgrades/profiles/1012_to_1013/types/imio.events.Event.xml
 src/imio/events/core/upgrades/profiles/1012_to_1013/types/imio.events.Folder.xml
+src/imio/events/core/upgrades/profiles/1013_to_1014/rolemap.xml
 src/imio/events/core/viewlets/__init__.py
 src/imio/events/core/viewlets/configure.zcml
 src/imio/events/core/viewlets/event.py
 src/imio/events/core/viewlets/event/button_to_bring_event.pt
```


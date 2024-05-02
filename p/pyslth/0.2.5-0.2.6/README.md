# Comparing `tmp/pyslth-0.2.5.tar.gz` & `tmp/pyslth-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.2.5.tar", last modified: Wed May  1 17:49:31 2024, max compression
+gzip compressed data, was "pyslth-0.2.6.tar", last modified: Wed May  1 21:27:08 2024, max compression
```

## Comparing `pyslth-0.2.5.tar` & `pyslth-0.2.6.tar`

### file list

```diff
@@ -1,81 +1,80 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.895048 pyslth-0.2.5/
--rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.2.5/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-01 17:49:31.894636 pyslth-0.2.5/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.850502 pyslth-0.2.5/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-01 17:49:31.000000 pyslth-0.2.5/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)     1784 2024-05-01 17:49:31.000000 pyslth-0.2.5/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-01 17:49:31.000000 pyslth-0.2.5/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-01 17:49:31.000000 pyslth-0.2.5/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-01 17:49:31.000000 pyslth-0.2.5/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.2.5/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-01 17:49:31.895332 pyslth-0.2.5/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-01 17:47:12.000000 pyslth-0.2.5/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.856976 pyslth-0.2.5/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3774 2024-04-28 09:42:58.000000 pyslth-0.2.5/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6945 2024-04-30 16:46:55.000000 pyslth-0.2.5/slth/components.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.857639 pyslth-0.2.5/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.2.5/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.2.5/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    20556 2024-05-01 15:37:13.000000 pyslth-0.2.5/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.2.5/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)     2527 2024-05-01 13:30:46.000000 pyslth-0.2.5/slth/factory.py
--rw-r--r--   0 breno      (501) staff       (20)    25521 2024-05-01 15:36:17.000000 pyslth-0.2.5/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.857976 pyslth-0.2.5/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.5/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.858643 pyslth-0.2.5/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.5/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.2.5/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.2.5/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.862043 pyslth-0.2.5/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.2.5/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.2.5/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.2.5/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
--rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.2.5/slth/migrations/0004_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.2.5/slth/migrations/0005_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.2.5/slth/migrations/0006_user.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.5/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6441 2024-05-01 14:04:01.000000 pyslth-0.2.5/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.2.5/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.2.5/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    19351 2024-05-01 11:31:08.000000 pyslth-0.2.5/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.2.5/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.862807 pyslth-0.2.5/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.2.5/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.2.5/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    14408 2024-05-01 13:49:16.000000 pyslth-0.2.5/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.863366 pyslth-0.2.5/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.866807 pyslth-0.2.5/slth/static/css/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.2.5/slth/static/css/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.2.5/slth/static/css/fontawesome.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.872744 pyslth-0.2.5/slth/static/css/fonts/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.2.5/slth/static/css/fonts/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.2.5/slth/static/css/fonts/fa-solid-900.woff2
--rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.2.5/slth/static/css/fonts/rawline-400.woff
--rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.2.5/slth/static/css/fonts/rawline-500i.woff
--rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.2.5/slth/static/css/fonts/rawline-700.woff
--rw-r--r--   0 breno      (501) staff       (20)      752 2024-05-01 13:59:41.000000 pyslth-0.2.5/slth/static/css/slth.css
--rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.2.5/slth/static/css/solid.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.874314 pyslth-0.2.5/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.2.5/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.2.5/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.2.5/slth/static/images/user.png
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.2.5/slth/static/index.html
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.892283 pyslth-0.2.5/slth/static/js/
--rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.2.5/slth/static/js/echarts.min.js
--rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-01 17:47:42.000000 pyslth-0.2.5/slth/static/js/index.min.js
--rw-r--r--   0 breno      (501) staff       (20)    83233 2024-05-01 17:36:19.000000 pyslth-0.2.5/slth/static/js/lib.min.js
--rw-r--r--   0 breno      (501) staff       (20)   117723 2024-04-27 15:01:32.000000 pyslth-0.2.5/slth/static/js/peerjs.min.js
--rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.2.5/slth/static/js/qrcode.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.2.5/slth/static/js/react-trigger-change.js
--rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-01 17:47:42.000000 pyslth-0.2.5/slth/static/js/react.min.js
--rw-r--r--   0 breno      (501) staff       (20)    83233 2024-05-01 17:47:42.000000 pyslth-0.2.5/slth/static/js/slth.min.js
--rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.2.5/slth/static/js/vanilla-masker.js
--rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.2.5/slth/static/js/vanilla-masker.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.2.5/slth/statistics.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 17:49:31.893416 pyslth-0.2.5/slth/templates/
--rw-r--r--   0 breno      (501) staff       (20)     2282 2024-05-01 17:36:48.000000 pyslth-0.2.5/slth/templates/index.html
--rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.2.5/slth/templates/service-worker.js
--rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.2.5/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.2.5/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1000 2024-04-27 19:14:01.000000 pyslth-0.2.5/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     2425 2024-05-01 13:07:02.000000 pyslth-0.2.5/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 21:27:08.660575 pyslth-0.2.6/
+-rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.2.6/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-01 21:27:08.660372 pyslth-0.2.6/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 21:27:08.629376 pyslth-0.2.6/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-01 21:27:08.000000 pyslth-0.2.6/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)     1758 2024-05-01 21:27:08.000000 pyslth-0.2.6/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-01 21:27:08.000000 pyslth-0.2.6/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-01 21:27:08.000000 pyslth-0.2.6/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-01 21:27:08.000000 pyslth-0.2.6/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.2.6/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-01 21:27:08.660633 pyslth-0.2.6/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-01 21:25:51.000000 pyslth-0.2.6/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 21:27:08.635611 pyslth-0.2.6/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3774 2024-04-28 09:42:58.000000 pyslth-0.2.6/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6945 2024-04-30 16:46:55.000000 pyslth-0.2.6/slth/components.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 21:27:08.636249 pyslth-0.2.6/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.2.6/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.2.6/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    20556 2024-05-01 15:37:13.000000 pyslth-0.2.6/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.2.6/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)     2527 2024-05-01 13:30:46.000000 pyslth-0.2.6/slth/factory.py
+-rw-r--r--   0 breno      (501) staff       (20)    25521 2024-05-01 15:36:17.000000 pyslth-0.2.6/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 21:27:08.636565 pyslth-0.2.6/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.6/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 21:27:08.637197 pyslth-0.2.6/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.6/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.2.6/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.2.6/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 21:27:08.639950 pyslth-0.2.6/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.2.6/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.2.6/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.2.6/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+-rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.2.6/slth/migrations/0004_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.2.6/slth/migrations/0005_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.2.6/slth/migrations/0006_user.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.2.6/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6441 2024-05-01 14:04:01.000000 pyslth-0.2.6/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.2.6/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.2.6/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    19351 2024-05-01 11:31:08.000000 pyslth-0.2.6/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.2.6/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 21:27:08.640422 pyslth-0.2.6/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.2.6/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.2.6/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    14408 2024-05-01 13:49:16.000000 pyslth-0.2.6/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 21:27:08.640785 pyslth-0.2.6/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 21:27:08.642402 pyslth-0.2.6/slth/static/css/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.2.6/slth/static/css/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.2.6/slth/static/css/fontawesome.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 21:27:08.646642 pyslth-0.2.6/slth/static/css/fonts/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.2.6/slth/static/css/fonts/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.2.6/slth/static/css/fonts/fa-solid-900.woff2
+-rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.2.6/slth/static/css/fonts/rawline-400.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.2.6/slth/static/css/fonts/rawline-500i.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.2.6/slth/static/css/fonts/rawline-700.woff
+-rw-r--r--   0 breno      (501) staff       (20)      752 2024-05-01 13:59:41.000000 pyslth-0.2.6/slth/static/css/slth.css
+-rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.2.6/slth/static/css/solid.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 21:27:08.648020 pyslth-0.2.6/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.2.6/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.2.6/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.2.6/slth/static/images/user.png
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.2.6/slth/static/index.html
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 21:27:08.658449 pyslth-0.2.6/slth/static/js/
+-rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.2.6/slth/static/js/echarts.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-01 21:26:48.000000 pyslth-0.2.6/slth/static/js/index.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   117723 2024-04-27 15:01:32.000000 pyslth-0.2.6/slth/static/js/peerjs.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.2.6/slth/static/js/qrcode.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.2.6/slth/static/js/react-trigger-change.js
+-rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-01 21:26:48.000000 pyslth-0.2.6/slth/static/js/react.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    86890 2024-05-01 21:26:48.000000 pyslth-0.2.6/slth/static/js/slth.min.js
+-rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.2.6/slth/static/js/vanilla-masker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.2.6/slth/static/js/vanilla-masker.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.2.6/slth/statistics.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-01 21:27:08.660084 pyslth-0.2.6/slth/templates/
+-rw-r--r--   0 breno      (501) staff       (20)     2282 2024-05-01 17:36:48.000000 pyslth-0.2.6/slth/templates/index.html
+-rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.2.6/slth/templates/service-worker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.2.6/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.2.6/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1000 2024-04-27 19:14:01.000000 pyslth-0.2.6/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     2425 2024-05-01 13:07:02.000000 pyslth-0.2.6/slth/views.py
```

### Comparing `pyslth-0.2.5/PKG-INFO` & `pyslth-0.2.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.2.5
+Version: 0.2.6
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.2.5/pyslth.egg-info/PKG-INFO` & `pyslth-0.2.6/pyslth.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.2.5
+Version: 0.2.6
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.2.5/pyslth.egg-info/SOURCES.txt` & `pyslth-0.2.6/pyslth.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 slth/static/css/fonts/rawline-500i.woff
 slth/static/css/fonts/rawline-700.woff
 slth/static/images/logo.png
 slth/static/images/logo.svg
 slth/static/images/user.png
 slth/static/js/echarts.min.js
 slth/static/js/index.min.js
-slth/static/js/lib.min.js
 slth/static/js/peerjs.min.js
 slth/static/js/qrcode.min.js
 slth/static/js/react-trigger-change.js
 slth/static/js/react.min.js
 slth/static/js/slth.min.js
 slth/static/js/vanilla-masker.js
 slth/static/js/vanilla-masker.min.js
```

### Comparing `pyslth-0.2.5/setup.py` & `pyslth-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.2.5',
+    version='0.2.6',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.2.5/slth/__init__.py` & `pyslth-0.2.6/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/components.py` & `pyslth-0.2.6/slth/components.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/db/models.py` & `pyslth-0.2.6/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/endpoints.py` & `pyslth-0.2.6/slth/endpoints.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/factory.py` & `pyslth-0.2.6/slth/factory.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/forms.py` & `pyslth-0.2.6/slth/forms.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/management/commands/integration_test.py` & `pyslth-0.2.6/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/management/commands/sync.py` & `pyslth-0.2.6/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/migrations/0001_initial.py` & `pyslth-0.2.6/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.2.6/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/migrations/0003_rename_photo_profile_alter_profile_options.py` & `pyslth-0.2.6/slth/migrations/0003_rename_photo_profile_alter_profile_options.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/migrations/0006_user.py` & `pyslth-0.2.6/slth/migrations/0006_user.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/models.py` & `pyslth-0.2.6/slth/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/permissions.py` & `pyslth-0.2.6/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/queryset.py` & `pyslth-0.2.6/slth/queryset.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/roles.py` & `pyslth-0.2.6/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/selenium/__init__.py` & `pyslth-0.2.6/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/selenium/browser.py` & `pyslth-0.2.6/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/serializer.py` & `pyslth-0.2.6/slth/serializer.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/static/css/.DS_Store` & `pyslth-0.2.6/slth/static/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/static/css/fontawesome.min.css` & `pyslth-0.2.6/slth/static/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/static/css/fonts/.DS_Store` & `pyslth-0.2.6/slth/static/css/fonts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/static/css/fonts/fa-solid-900.woff2` & `pyslth-0.2.6/slth/static/css/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/static/css/fonts/rawline-400.woff` & `pyslth-0.2.6/slth/static/css/fonts/rawline-400.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/static/css/fonts/rawline-500i.woff` & `pyslth-0.2.6/slth/static/css/fonts/rawline-500i.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/static/css/fonts/rawline-700.woff` & `pyslth-0.2.6/slth/static/css/fonts/rawline-700.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/static/css/slth.css` & `pyslth-0.2.6/slth/static/css/slth.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/static/css/solid.min.css` & `pyslth-0.2.6/slth/static/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/static/images/logo.png` & `pyslth-0.2.6/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/static/images/logo.svg` & `pyslth-0.2.6/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/static/images/user.png` & `pyslth-0.2.6/slth/static/images/user.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/static/js/echarts.min.js` & `pyslth-0.2.6/slth/static/js/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/static/js/index.min.js` & `pyslth-0.2.6/slth/static/js/index.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/static/js/lib.min.js` & `pyslth-0.2.6/slth/static/js/slth.min.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,53 +1,53 @@
 import {
     j as t,
-    c as W,
-    r as C,
+    c as P,
+    r as M,
     R as Ie
 } from "./react.min.js";
 
-function De(e) {
+function Be(e) {
     function n(r) {
         navigator.clipboard.writeText(r), ee('Icon "' + r + '" copied to clipboard!')
     }
     const a = {
         display: "inline-block",
         width: 150,
         textAlign: "center",
         cursor: "pointer"
     };
     return t.jsx("div", {
         style: {
             marginTop: 30
         },
-        children: qe.map(r => t.jsxs("div", {
+        children: Le.map(r => t.jsxs("div", {
             className: "icon-box",
             onClick: () => n(r),
             style: a,
             children: [t.jsx("i", {
                 className: "fa-solid fa-fw fa-" + r
             }), t.jsx("div", {
                 className: "icon-text",
                 children: r
             })]
         }, Math.random()))
     })
 }
 
-function Be(e) {
+function De(e) {
     function n() {
         return t.jsx("i", {
             style: e.style,
             className: "fa-solid fa-circle-notch fa-spin fa-1x spin"
         })
     }
     return n()
 }
 
-function b(e) {
+function k(e) {
     var n = "fa-solid fa-" + e.icon;
     return e.className && (n += " " + e.className), (e.onClick || e.clickable) && (n += " clickable"), t.jsx("i", {
         style: e.style,
         className: n,
         onClick: e.onClick
     })
 }
@@ -65,50 +65,50 @@
         };
         return e.primary && (a.backgroundColor = "#1351b4", a.color = "white"), e.default && (a.color = "#1351b4", a.border = "solid 1px #1351b4"), t.jsx("a", {
             id: e.id,
             style: a,
             onClick: r => {
                 r.preventDefault(), e.onClick()
             },
-            children: t.jsx(b, {
+            children: t.jsx(k, {
                 icon: e.icon
             })
         })
     }
     return n()
 }
-const qe = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "fill-drip", "arrows-to-circle", "circle-chevron-right", "at", "trash-can", "text-height", "user-xmark", "stethoscope", "message", "info", "down-left-and-up-right-to-center", "explosion", "file-text", "wave-square", "ring", "building-un", "dice-three", "calendar-days", "anchor-circle-check", "building-circle-arrow-right", "volleyball", "arrows-up-to-line", "sort-down", "minus-circle", "door-open", "sign-out-alt", "atom", "soap", "icons", "microphone-lines-slash", "bridge-circle-check", "pump-medical", "fingerprint", "hand-point-right", "search-location", "step-forward", "smile-beam", "flag-checkered", "football", "school-circle-exclamation", "crop", "angles-down", "users-rectangle", "people-roof", "people-line", "beer", "diagram-predecessor", "long-arrow-up", "fire-flame-simple", "person", "laptop", "file-csv", "menorah", "truck-plane", "record-vinyl", "grin-stars", "bong", "spaghetti-monster-flying", "arrow-down-up-across-line", "utensil-spoon", "jar-wheat", "mail-bulk", "file-circle-exclamation", "hospital-symbol", "pager", "contact-book", "strikethrough", "k", "landmark-flag", "pencil", "backward", "caret-right", "comments", "paste", "code-pull-request", "clipboard-list", "truck-ramp-box", "user-check", "vial-virus", "sheet-plastic", "blog", "user-ninja", "person-arrow-up-from-line", "torah", "quidditch", "toggle-off", "box-archive", "person-drowning", "sort-numeric-down-alt", "grin-tongue-squint", "spray-can", "truck-monster", "w", "globe-africa", "rainbow", "circle-notch", "tablet-screen-button", "paw", "cloud", "trowel-bricks", "flushed", "hospital-user", "tent-arrow-left-right", "legal", "binoculars", "microphone-slash", "box-tissue", "motorcycle", "concierge-bell", "pencil-ruler", "people-arrows", "mars-and-venus-burst", "square-caret-right", "scissors", "sun-plant-wilt", "toilets-portable", "hockey-puck", "table", "magnifying-glass-arrow-right", "tachograph-digital", "users-slash", "clover", "reply", "star-and-crescent", "house-fire", "square-minus", "helicopter", "compass", "square-caret-down", "file-circle-question", "laptop-code", "swatchbook", "prescription-bottle", "navicon", "people-group", "hourglass-end", "heart-crack", "square-up-right", "kiss-beam", "film", "ruler-horizontal", "people-robbery", "lightbulb", "caret-left", "exclamation-circle", "school-circle-xmark", "sign-out", "circle-chevron-down", "unlock-keyhole", "cloud-showers-heavy", "headphones-simple", "sitemap", "donate", "memory", "road-spikes", "fire-burner", "flag", "hanukiah", "feather", "volume-low", "comment-slash", "cloud-sun-rain", "compress", "wheat-awn", "ankh", "hands-holding-child", "asterisk", "square-check", "peseta-sign", "heading", "ghost", "list", "square-phone-flip", "cart-plus", "gamepad", "dot-circle", "face-dizzy", "egg", "house-medical-circle-xmark", "campground", "folder-plus", "soccer-ball", "paintbrush", "lock", "gas-pump", "hot-tub", "map-marked", "house-flood-water", "tree", "bridge-lock", "sack-dollar", "pen-to-square", "car-side", "share-nodes", "heart-circle-minus", "hourglass-half", "microscope", "sink", "shopping-bag", "sort-alpha-down-alt", "mitten", "person-rays", "users", "eye-slash", "flask-vial", "hand", "om", "worm", "house-circle-xmark", "plug", "chevron-up", "hand-spock", "stopwatch", "kiss", "bridge-circle-xmark", "grin-tongue", "chess-bishop", "grin-wink", "hard-of-hearing", "road-circle-check", "dice-five", "square-rss", "land-mine-on", "i-cursor", "stamp", "stairs", "i", "hryvnia", "pills", "grin-alt", "tooth", "v", "bangladeshi-taka-sign", "bicycle", "staff-snake", "head-side-cough-slash", "truck-medical", "wheat-awn-circle-exclamation", "snowman", "mortar-pestle", "road-barrier", "school", "igloo", "joint", "angle-right", "horse", "q", "g", "notes-medical", "thermometer-half", "dong-sign", "capsules", "poo-storm", "frown-open", "hand-point-up", "money-bill", "bookmark", "align-justify", "umbrella-beach", "helmet-un", "bullseye", "bacon", "hand-point-down", "arrow-up-from-bracket", "folder", "file-waveform", "radiation", "chart-simple", "mars-stroke", "vial", "tachometer-alt-average", "wand-magic-sparkles", "e", "pen-clip", "bridge-circle-exclamation", "user", "school-circle-check", "dumpster", "van-shuttle", "building-user", "square-caret-left", "highlighter", "key", "bullhorn", "globe", "synagogue", "person-half-dress", "road-bridge", "location-arrow", "c", "tablet-button", "building-lock", "pizza-slice", "money-bill-wave", "chart-area", "house-flag", "person-circle-minus", "cancel", "camera-rotate", "spray-can-sparkles", "star", "repeat", "cross", "box", "venus-mars", "mouse-pointer", "maximize", "charging-station", "triangle-circle-square", "shuffle", "running", "mobile-retro", "grip-lines-vertical", "spider", "hands-bound", "file-invoice-dollar", "plane-circle-exclamation", "x-ray", "spell-check", "slash", "mouse", "sign-in", "store-alt-slash", "server", "virus-covid-slash", "shop-lock", "hourglass-start", "blender-phone", "building-wheat", "person-breastfeeding", "sign-in-alt", "venus", "passport", "heartbeat", "people-carry", "temperature-high", "microchip", "crown", "weight-hanging", "xmarks-lines", "file-prescription", "weight", "user-group", "sort-alpha-up", "chess-knight", "laugh-squint", "wheelchair", "circle-arrow-up", "toggle-on", "walking", "l", "fire", "procedures", "space-shuttle", "laugh", "folder-open", "heart-circle-plus", "code-fork", "city", "microphone-lines", "pepper-hot", "unlock", "colon-sign", "headset", "store-slash", "road-circle-xmark", "user-minus", "mars-stroke-v", "glass-cheers", "clipboard", "house-circle-exclamation", "file-upload", "wifi", "bathtub", "underline", "user-pen", "signature", "stroopwafel", "bold", "anchor-lock", "building-ngo", "manat-sign", "not-equal", "border-top-left", "map-marked-alt", "jedi", "square-poll-vertical", "mug-hot", "car-battery", "gift", "dice-two", "chess-queen", "glasses", "chess-board", "building-circle-check", "person-chalkboard", "mars-stroke-right", "hand-rock", "square-caret-up", "cloud-showers-water", "chart-bar", "hands-wash", "less-than-equal", "train", "low-vision", "crow", "sailboat", "window-restore", "square-plus", "torii-gate", "frog", "bucket", "image", "microphone", "cow", "caret-up", "screwdriver", "folder-closed", "house-tsunami", "square-nfi", "arrow-up-from-ground-water", "martini-glass", "undo-alt", "table-columns", "lemon", "head-side-mask", "handshake", "gem", "dolly", "smoking", "minimize", "monument", "snowplow", "angles-right", "cannabis", "play-circle", "tablets", "ethernet", "euro", "chair", "circle-check", "stop-circle", "drafting-compass", "plate-wheat", "icicles", "person-shelter", "neuter", "id-badge", "marker", "laugh-beam", "helicopter-symbol", "universal-access", "circle-chevron-up", "lari-sign", "volcano", "person-walking-dashed-line-arrow-right", "sterling-sign", "viruses", "square-person-confined", "user-tie", "long-arrow-down", "tent-arrow-down-to-line", "certificate", "reply-all", "suitcase", "skating", "funnel-dollar", "camera-retro", "circle-arrow-down", "file-import", "square-arrow-up-right", "box-open", "scroll", "spa", "location-pin-lock", "pause", "hill-avalanche", "thermometer-empty", "bomb", "registered", "vcard", "scale-unbalanced-flip", "subscript", "directions", "burst", "laptop-house", "tired", "money-bills", "smog", "crutch", "cloud-upload", "palette", "arrows-turn-right", "vest", "ferry", "arrows-down-to-people", "sprout", "left-right", "boxes-packing", "circle-arrow-left", "group-arrows-rotate", "bowl-food", "candy-cane", "sort-amount-down", "thunderstorm", "text-slash", "smile-wink", "file-word", "file-powerpoint", "arrows-left-right", "house-lock", "cloud-download", "children", "chalkboard", "user-large-slash", "envelope-open", "handshake-simple-slash", "mattress-pillow", "guarani-sign", "sync", "fire-extinguisher", "cruzeiro-sign", "greater-than-equal", "shield-halved", "book-atlas", "virus", "envelope-circle-check", "layer-group", "arrows-to-dot", "archway", "heart-circle-check", "house-damage", "file-zipper", "square", "martini-glass-empty", "couch", "cedi-sign", "italic", "church", "comments-dollar", "democrat", "z", "skiing", "road-lock", "a", "temperature-down", "feather-pointed", "p", "snowflake", "newspaper", "rectangle-ad", "circle-arrow-right", "filter-circle-xmark", "locust", "unsorted", "list-ol", "person-dress-burst", "money-check-dollar", "vector-square", "bread-slice", "language", "kiss-wink-heart", "filter", "question", "file-signature", "up-down-left-right", "house-chimney-user", "hand-holding-heart", "puzzle-piece", "money-check", "star-half-stroke", "code", "whiskey-glass", "building-circle-exclamation", "magnifying-glass-chart", "external-link", "cubes-stacked", "won", "virus-covid", "austral-sign", "f", "leaf", "road", "taxi", "person-circle-plus", "pie-chart", "bolt-lightning", "sack-xmark", "file-excel", "file-contract", "fish-fins", "building-flag", "grin-beam", "object-ungroup", "poop", "map-marker", "kaaba", "toilet-paper", "helmet-safety", "eject", "circle-right", "plane-circle-check", "meh-rolling-eyes", "object-group", "line-chart", "mask-ventilator", "arrow-right", "signs-post", "cash-register", "person-circle-question", "h", "tarp", "tools", "arrows-to-eye", "plug-circle-bolt", "heart", "mars-and-venus", "house-user", "dumpster-fire", "house-crack", "martini-glass-citrus", "surprise", "bottle-water", "pause-circle", "toilet-paper-slash", "apple-whole", "kitchen-set", "r", "thermometer-quarter", "cube", "bitcoin-sign", "shield-dog", "solar-panel", "lock-open", "elevator", "money-bill-transfer", "money-bill-trend-up", "house-flood-water-circle-arrow-right", "square-poll-horizontal", "circle", "fast-backward", "recycle", "user-astronaut", "plane-slash", "trademark", "basketball", "satellite-dish", "circle-up", "mobile-screen-button", "volume-up", "users-rays", "wallet", "clipboard-check", "file-audio", "hamburger", "wrench", "bugs", "rupee", "file-image", "question-circle", "plane-departure", "handshake-slash", "book-bookmark", "code-branch", "hat-cowboy", "bridge", "phone-flip", "truck-front", "cat", "anchor-circle-exclamation", "truck-field", "route", "clipboard-question", "panorama", "comment-medical", "teeth-open", "file-circle-minus", "tags", "wine-glass", "fast", "meh-blank", "square-parking", "house-signal", "tasks-alt", "faucet-drip", "dolly-flatbed", "smoking-ban", "terminal", "mobile-button", "house-medical-flag", "shopping-basket", "tape", "bus-simple", "eye", "sad-cry", "audio-description", "person-military-to-person", "file-shield", "user-slash", "pen", "tower-observation", "file-code", "signal", "bus", "heart-circle-xmark", "house-chimney", "window-maximize", "frown", "prescription", "store-alt", "save", "vihara", "scale-unbalanced", "sort-up", "commenting", "plant-wilt", "diamond", "grin-squint", "hand-holding-usd", "bacterium", "hand-pointer", "drum-steelpan", "hand-scissors", "praying-hands", "redo", "biohazard", "location", "mars-double", "child-dress", "users-between-lines", "lungs-virus", "grin-tears", "phone", "calendar-xmark", "child-reaching", "head-side-virus", "user-gear", "sort-numeric-up", "door-closed", "shield-virus", "dice-six", "mosquito-net", "bridge-water", "person-booth", "text-width", "hat-wizard", "fancy", "person-digging", "trash", "tachometer-average", "book-medical", "poo", "quote-right", "tshirt", "cubes", "divide", "tenge", "headphones", "hands-holding", "hands-clapping", "republican", "arrow-left", "person-circle-xmark", "ruler", "align-left", "dice-d6", "restroom", "j", "users-viewfinder", "file-video", "up-right-from-square", "th", "file-pdf", "book-bible", "o", "suitcase-medical", "user-secret", "otter", "person-dress", "comment-dollar", "business-time", "th-large", "tanakh", "volume-control-phone", "hat-cowboy-side", "clipboard-user", "child", "lira-sign", "satellite", "plane-lock", "tag", "comment", "cake", "envelope", "angles-up", "paperclip", "arrow-right-to-city", "ribbon", "lungs", "sort-numeric-up-alt", "litecoin-sign", "border-none", "circle-nodes", "parachute-box", "indent", "truck-field-un", "hourglass", "mountain", "user-md", "info-circle", "cloud-meatball", "camera", "square-virus", "meteor", "car-on", "sleigh", "sort-numeric-down", "hand-holding-water", "water", "calendar-check", "braille", "prescription-bottle-medical", "landmark", "truck", "crosshairs", "person-cane", "tent", "vest-patches", "check-double", "sort-alpha-down", "money-bill-wheat", "cookie", "undo", "hdd", "grin-squint-tears", "dumbbell", "rectangle-list", "tarp-droplet", "house-medical-circle-check", "skiing-nordic", "calendar-plus", "plane-arrival", "circle-left", "train-subway", "chart-gantt", "inr", "crop-simple", "money-bill-alt", "long-arrow-alt-left", "dna", "virus-slash", "subtract", "chess", "long-arrow-left", "plug-circle-check", "street-view", "franc-sign", "volume-off", "hands-asl-interpreting", "gear", "tint-slash", "mosque", "mosquito", "star-of-david", "person-military-rifle", "shopping-cart", "vials", "plug-circle-plus", "place-of-worship", "grip-vertical", "level-up", "u", "square-root-variable", "clock", "step-backward", "pallet", "faucet", "baseball-bat-ball", "s", "timeline", "keyboard", "caret-down", "house-chimney-medical", "thermometer-three-quarters", "mobile-screen", "plane-up", "piggy-bank", "battery-half", "mountain-city", "coins", "khanda", "sliders", "folder-tree", "network-wired", "map-pin", "hamsa", "cent-sign", "flask", "person-pregnant", "wand-sparkles", "ellipsis-vertical", "ticket", "power-off", "right-long", "flag-usa", "laptop-file", "tty", "diagram-next", "person-rifle", "house-medical-circle-exclamation", "closed-captioning", "person-hiking", "venus-double", "images", "calculator", "people-pulling", "n", "tram", "cloud-rain", "building-circle-xmark", "ship", "arrows-down-to-line", "download", "grin", "delete-left", "eyedropper", "file-circle-check", "forward", "mobile", "meh", "align-center", "book-skull", "id-card", "outdent", "heart-circle-exclamation", "house", "calendar-week", "laptop-medical", "b", "file-medical", "dice-one", "kiwi-bird", "exchange", "rotate-right", "utensils", "sort-amount-up", "mill-sign", "bowl-rice", "skull", "tower-broadcast", "truck-pickup", "up-long", "stop", "code-merge", "upload", "hurricane", "mound", "toilet-portable", "compact-disc", "file-download", "caravan", "shield-cat", "zap", "glass-water", "oil-well", "vault", "mars", "toilet", "plane-circle-xmark", "yen", "ruble", "sun", "guitar", "laugh-wink", "horse-head", "bore-hole", "industry", "circle-down", "arrows-turn-to-dots", "florin-sign", "sort-amount-down-alt", "less-than", "angle-down", "car-tunnel", "head-side-cough", "grip-lines", "thumbs-down", "user-lock", "long-arrow-right", "anchor-circle-xmark", "ellipsis", "chess-pawn", "kit-medical", "person-through-window", "toolbox", "hands-holding-circle", "bug", "credit-card", "car", "hand-holding-hand", "book-reader", "mountain-sun", "arrows-left-right-to-line", "dice-d20", "truck-droplet", "file-circle-xmark", "temperature-up", "medal", "bed", "square-h", "podcast", "thermometer-full", "bell", "superscript", "plug-circle-xmark", "star-of-life", "phone-slash", "paint-roller", "handshake-angle", "map-marker-alt", "file", "greater-than", "swimmer", "arrow-down", "tint", "eraser", "globe-americas", "person-burst", "dove", "battery-empty", "socks", "inbox", "section", "tachometer-alt", "envelope-open-text", "hospital", "wine-bottle", "chess-rook", "stream", "dharmachakra", "hotdog", "person-walking-with-cane", "drum", "ice-cream", "heart-circle-bolt", "fax", "paragraph", "vote-yea", "star-half", "boxes", "link", "ear-listen", "tree-city", "play", "font", "rupiah-sign", "search", "table-tennis", "person-dots-from-line", "trash-restore-alt", "naira-sign", "cart-arrow-down", "walkie-talkie", "file-pen", "receipt", "square-pen", "suitcase-rolling", "person-circle-exclamation", "chevron-down", "battery", "skull-crossbones", "code-compare", "list-ul", "school-lock", "tower-cell", "long-arrow-alt-down", "ranking-star", "chess-king", "person-harassing", "brazilian-real-sign", "landmark-dome", "arrow-up", "tv", "shrimp", "tasks", "jug-detergent", "user-circle", "user-shield", "wind", "car-crash", "y", "snowboarding", "fast", "fish", "user-graduate", "circle-half-stroke", "clapperboard", "radiation-alt", "baseball", "jet-fighter-up", "project-diagram", "copy", "volume-xmark", "hand-sparkles", "grip", "share-square", "child-rifle", "gun", "square-phone", "plus", "expand", "computer", "xmark", "arrows", "chalkboard-user", "peso-sign", "building-shield", "baby", "users-line", "quote-left", "tractor", "trash-restore", "arrow-down-up-lock", "lines-leaning", "ruler-combined", "copyright", "equals", "blender", "teeth", "sheqel", "map", "rocket", "photo-video", "folder-minus", "store", "arrow-trend-up", "plug-circle-minus", "sign", "bezier-curve", "bell-slash", "tablet", "school-flag", "fill", "angle-up", "drumstick-bite", "holly-berry", "chevron-left", "bacteria", "hand-lizard", "notdef", "disease", "briefcase-medical", "genderless", "chevron-right", "retweet", "car-rear", "pump-soap", "video-slash", "battery-quarter", "radio", "carriage-baby", "traffic-light", "thermometer", "vr-cardboard", "hand-middle-finger", "percentage", "truck-moving", "glass-water-droplet", "display", "smile", "thumbtack", "trophy", "pray", "hammer", "hand-peace", "sync-alt", "spinner", "robot", "peace", "gears", "warehouse", "arrow-up-right-dots", "splotch", "grin-hearts", "dice-four", "sim-card", "transgender", "mercury", "level-down", "falling-burst", "award", "ticket-simple", "building", "angles-left", "qrcode", "history", "grin-beam-sweat", "file-export", "shield", "sort-amount-up-alt", "house-medical", "golf-ball", "circle-chevron-left", "house-chimney-window", "pen-nib", "tent-arrow-turn-left", "tents", "wand-magic", "dog", "carrot", "moon", "wine-glass-empty", "cheese", "yin-yang", "music", "code-commit", "temperature-low", "person-biking", "broom", "shield-heart", "gopuram", "globe-oceania", "xmark-square", "hashtag", "up-right-and-down-left-from-center", "oil-can", "t", "hippo", "chart-column", "infinity", "vial-circle-check", "person-arrow-down-to-line", "voicemail", "fan", "person-walking-luggage", "up-down", "cloud-moon-rain", "calendar", "trailer", "haykal", "sd-card", "dragon", "shoe-prints", "plus-circle", "grin-tongue-wink", "hand-holding", "plug-circle-exclamation", "unlink", "clone", "person-walking-arrow-loop-left", "sort-alpha-up-alt", "fire-flame-curved", "tornado", "file-circle-plus", "quran", "anchor", "border-all", "face-angry", "cookie-bite", "arrow-trend-down", "rss", "draw-polygon", "scale-balanced", "tachometer", "shower", "desktop", "m", "th-list", "sms", "book", "user-plus", "check", "battery-three-quarters", "house-circle-check", "angle-left", "diagram-successor", "truck-arrow-right", "arrows-split-up-and-left", "hand-fist", "cloud-moon", "briefcase", "falling", "portrait", "user-tag", "rug", "globe-europe", "luggage-cart", "window-close", "baht-sign", "book-open", "journal-whills", "handcuffs", "warning", "database", "share", "bottle-droplet", "face", "hill-rockslide", "right-left", "paper-plane", "road-circle-exclamation", "dungeon", "align-right", "money-bill-wave-alt", "life-ring", "signing", "calendar-day", "water-ladder", "arrows-v", "grimace", "wheelchair-move", "turn-down", "person-walking-arrow-right", "square-envelope", "dice", "bowling-ball", "brain", "bandage", "calendar-minus", "xmark-circle", "gifts", "hotel", "globe-asia", "id-card-clip", "search-plus", "thumbs-up", "user-clock", "hand-dots", "file-invoice", "window-minimize", "mug-saucer", "brush", "mask", "search-minus", "ruler-vertical", "user-large", "train-tram", "user-nurse", "syringe", "cloud-sun", "stopwatch-20", "square-full", "magnet", "jar", "sticky-note", "bug-slash", "arrow-up-from-water-pump", "bone", "user-injured", "sad-tear", "plane", "tent-arrows-down", "exclamation", "arrows-spin", "print", "turkish-lira", "usd", "x", "search-dollar", "users-gear", "person-military-pointing", "university", "umbrella", "trowel", "d", "stapler", "theater-masks", "kip-sign", "hand-point-left", "handshake-simple", "jet-fighter", "square-share-nodes", "barcode", "plus-minus", "video", "mortar-board", "hand-holding-medical", "person-circle-check", "turn-up"];
+const Le = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "fill-drip", "arrows-to-circle", "circle-chevron-right", "at", "trash-can", "text-height", "user-xmark", "stethoscope", "message", "info", "down-left-and-up-right-to-center", "explosion", "file-text", "wave-square", "ring", "building-un", "dice-three", "calendar-days", "anchor-circle-check", "building-circle-arrow-right", "volleyball", "arrows-up-to-line", "sort-down", "minus-circle", "door-open", "sign-out-alt", "atom", "soap", "icons", "microphone-lines-slash", "bridge-circle-check", "pump-medical", "fingerprint", "hand-point-right", "search-location", "step-forward", "smile-beam", "flag-checkered", "football", "school-circle-exclamation", "crop", "angles-down", "users-rectangle", "people-roof", "people-line", "beer", "diagram-predecessor", "long-arrow-up", "fire-flame-simple", "person", "laptop", "file-csv", "menorah", "truck-plane", "record-vinyl", "grin-stars", "bong", "spaghetti-monster-flying", "arrow-down-up-across-line", "utensil-spoon", "jar-wheat", "mail-bulk", "file-circle-exclamation", "hospital-symbol", "pager", "contact-book", "strikethrough", "k", "landmark-flag", "pencil", "backward", "caret-right", "comments", "paste", "code-pull-request", "clipboard-list", "truck-ramp-box", "user-check", "vial-virus", "sheet-plastic", "blog", "user-ninja", "person-arrow-up-from-line", "torah", "quidditch", "toggle-off", "box-archive", "person-drowning", "sort-numeric-down-alt", "grin-tongue-squint", "spray-can", "truck-monster", "w", "globe-africa", "rainbow", "circle-notch", "tablet-screen-button", "paw", "cloud", "trowel-bricks", "flushed", "hospital-user", "tent-arrow-left-right", "legal", "binoculars", "microphone-slash", "box-tissue", "motorcycle", "concierge-bell", "pencil-ruler", "people-arrows", "mars-and-venus-burst", "square-caret-right", "scissors", "sun-plant-wilt", "toilets-portable", "hockey-puck", "table", "magnifying-glass-arrow-right", "tachograph-digital", "users-slash", "clover", "reply", "star-and-crescent", "house-fire", "square-minus", "helicopter", "compass", "square-caret-down", "file-circle-question", "laptop-code", "swatchbook", "prescription-bottle", "navicon", "people-group", "hourglass-end", "heart-crack", "square-up-right", "kiss-beam", "film", "ruler-horizontal", "people-robbery", "lightbulb", "caret-left", "exclamation-circle", "school-circle-xmark", "sign-out", "circle-chevron-down", "unlock-keyhole", "cloud-showers-heavy", "headphones-simple", "sitemap", "donate", "memory", "road-spikes", "fire-burner", "flag", "hanukiah", "feather", "volume-low", "comment-slash", "cloud-sun-rain", "compress", "wheat-awn", "ankh", "hands-holding-child", "asterisk", "square-check", "peseta-sign", "heading", "ghost", "list", "square-phone-flip", "cart-plus", "gamepad", "dot-circle", "face-dizzy", "egg", "house-medical-circle-xmark", "campground", "folder-plus", "soccer-ball", "paintbrush", "lock", "gas-pump", "hot-tub", "map-marked", "house-flood-water", "tree", "bridge-lock", "sack-dollar", "pen-to-square", "car-side", "share-nodes", "heart-circle-minus", "hourglass-half", "microscope", "sink", "shopping-bag", "sort-alpha-down-alt", "mitten", "person-rays", "users", "eye-slash", "flask-vial", "hand", "om", "worm", "house-circle-xmark", "plug", "chevron-up", "hand-spock", "stopwatch", "kiss", "bridge-circle-xmark", "grin-tongue", "chess-bishop", "grin-wink", "hard-of-hearing", "road-circle-check", "dice-five", "square-rss", "land-mine-on", "i-cursor", "stamp", "stairs", "i", "hryvnia", "pills", "grin-alt", "tooth", "v", "bangladeshi-taka-sign", "bicycle", "staff-snake", "head-side-cough-slash", "truck-medical", "wheat-awn-circle-exclamation", "snowman", "mortar-pestle", "road-barrier", "school", "igloo", "joint", "angle-right", "horse", "q", "g", "notes-medical", "thermometer-half", "dong-sign", "capsules", "poo-storm", "frown-open", "hand-point-up", "money-bill", "bookmark", "align-justify", "umbrella-beach", "helmet-un", "bullseye", "bacon", "hand-point-down", "arrow-up-from-bracket", "folder", "file-waveform", "radiation", "chart-simple", "mars-stroke", "vial", "tachometer-alt-average", "wand-magic-sparkles", "e", "pen-clip", "bridge-circle-exclamation", "user", "school-circle-check", "dumpster", "van-shuttle", "building-user", "square-caret-left", "highlighter", "key", "bullhorn", "globe", "synagogue", "person-half-dress", "road-bridge", "location-arrow", "c", "tablet-button", "building-lock", "pizza-slice", "money-bill-wave", "chart-area", "house-flag", "person-circle-minus", "cancel", "camera-rotate", "spray-can-sparkles", "star", "repeat", "cross", "box", "venus-mars", "mouse-pointer", "maximize", "charging-station", "triangle-circle-square", "shuffle", "running", "mobile-retro", "grip-lines-vertical", "spider", "hands-bound", "file-invoice-dollar", "plane-circle-exclamation", "x-ray", "spell-check", "slash", "mouse", "sign-in", "store-alt-slash", "server", "virus-covid-slash", "shop-lock", "hourglass-start", "blender-phone", "building-wheat", "person-breastfeeding", "sign-in-alt", "venus", "passport", "heartbeat", "people-carry", "temperature-high", "microchip", "crown", "weight-hanging", "xmarks-lines", "file-prescription", "weight", "user-group", "sort-alpha-up", "chess-knight", "laugh-squint", "wheelchair", "circle-arrow-up", "toggle-on", "walking", "l", "fire", "procedures", "space-shuttle", "laugh", "folder-open", "heart-circle-plus", "code-fork", "city", "microphone-lines", "pepper-hot", "unlock", "colon-sign", "headset", "store-slash", "road-circle-xmark", "user-minus", "mars-stroke-v", "glass-cheers", "clipboard", "house-circle-exclamation", "file-upload", "wifi", "bathtub", "underline", "user-pen", "signature", "stroopwafel", "bold", "anchor-lock", "building-ngo", "manat-sign", "not-equal", "border-top-left", "map-marked-alt", "jedi", "square-poll-vertical", "mug-hot", "car-battery", "gift", "dice-two", "chess-queen", "glasses", "chess-board", "building-circle-check", "person-chalkboard", "mars-stroke-right", "hand-rock", "square-caret-up", "cloud-showers-water", "chart-bar", "hands-wash", "less-than-equal", "train", "low-vision", "crow", "sailboat", "window-restore", "square-plus", "torii-gate", "frog", "bucket", "image", "microphone", "cow", "caret-up", "screwdriver", "folder-closed", "house-tsunami", "square-nfi", "arrow-up-from-ground-water", "martini-glass", "undo-alt", "table-columns", "lemon", "head-side-mask", "handshake", "gem", "dolly", "smoking", "minimize", "monument", "snowplow", "angles-right", "cannabis", "play-circle", "tablets", "ethernet", "euro", "chair", "circle-check", "stop-circle", "drafting-compass", "plate-wheat", "icicles", "person-shelter", "neuter", "id-badge", "marker", "laugh-beam", "helicopter-symbol", "universal-access", "circle-chevron-up", "lari-sign", "volcano", "person-walking-dashed-line-arrow-right", "sterling-sign", "viruses", "square-person-confined", "user-tie", "long-arrow-down", "tent-arrow-down-to-line", "certificate", "reply-all", "suitcase", "skating", "funnel-dollar", "camera-retro", "circle-arrow-down", "file-import", "square-arrow-up-right", "box-open", "scroll", "spa", "location-pin-lock", "pause", "hill-avalanche", "thermometer-empty", "bomb", "registered", "vcard", "scale-unbalanced-flip", "subscript", "directions", "burst", "laptop-house", "tired", "money-bills", "smog", "crutch", "cloud-upload", "palette", "arrows-turn-right", "vest", "ferry", "arrows-down-to-people", "sprout", "left-right", "boxes-packing", "circle-arrow-left", "group-arrows-rotate", "bowl-food", "candy-cane", "sort-amount-down", "thunderstorm", "text-slash", "smile-wink", "file-word", "file-powerpoint", "arrows-left-right", "house-lock", "cloud-download", "children", "chalkboard", "user-large-slash", "envelope-open", "handshake-simple-slash", "mattress-pillow", "guarani-sign", "sync", "fire-extinguisher", "cruzeiro-sign", "greater-than-equal", "shield-halved", "book-atlas", "virus", "envelope-circle-check", "layer-group", "arrows-to-dot", "archway", "heart-circle-check", "house-damage", "file-zipper", "square", "martini-glass-empty", "couch", "cedi-sign", "italic", "church", "comments-dollar", "democrat", "z", "skiing", "road-lock", "a", "temperature-down", "feather-pointed", "p", "snowflake", "newspaper", "rectangle-ad", "circle-arrow-right", "filter-circle-xmark", "locust", "unsorted", "list-ol", "person-dress-burst", "money-check-dollar", "vector-square", "bread-slice", "language", "kiss-wink-heart", "filter", "question", "file-signature", "up-down-left-right", "house-chimney-user", "hand-holding-heart", "puzzle-piece", "money-check", "star-half-stroke", "code", "whiskey-glass", "building-circle-exclamation", "magnifying-glass-chart", "external-link", "cubes-stacked", "won", "virus-covid", "austral-sign", "f", "leaf", "road", "taxi", "person-circle-plus", "pie-chart", "bolt-lightning", "sack-xmark", "file-excel", "file-contract", "fish-fins", "building-flag", "grin-beam", "object-ungroup", "poop", "map-marker", "kaaba", "toilet-paper", "helmet-safety", "eject", "circle-right", "plane-circle-check", "meh-rolling-eyes", "object-group", "line-chart", "mask-ventilator", "arrow-right", "signs-post", "cash-register", "person-circle-question", "h", "tarp", "tools", "arrows-to-eye", "plug-circle-bolt", "heart", "mars-and-venus", "house-user", "dumpster-fire", "house-crack", "martini-glass-citrus", "surprise", "bottle-water", "pause-circle", "toilet-paper-slash", "apple-whole", "kitchen-set", "r", "thermometer-quarter", "cube", "bitcoin-sign", "shield-dog", "solar-panel", "lock-open", "elevator", "money-bill-transfer", "money-bill-trend-up", "house-flood-water-circle-arrow-right", "square-poll-horizontal", "circle", "fast-backward", "recycle", "user-astronaut", "plane-slash", "trademark", "basketball", "satellite-dish", "circle-up", "mobile-screen-button", "volume-up", "users-rays", "wallet", "clipboard-check", "file-audio", "hamburger", "wrench", "bugs", "rupee", "file-image", "question-circle", "plane-departure", "handshake-slash", "book-bookmark", "code-branch", "hat-cowboy", "bridge", "phone-flip", "truck-front", "cat", "anchor-circle-exclamation", "truck-field", "route", "clipboard-question", "panorama", "comment-medical", "teeth-open", "file-circle-minus", "tags", "wine-glass", "fast", "meh-blank", "square-parking", "house-signal", "tasks-alt", "faucet-drip", "dolly-flatbed", "smoking-ban", "terminal", "mobile-button", "house-medical-flag", "shopping-basket", "tape", "bus-simple", "eye", "sad-cry", "audio-description", "person-military-to-person", "file-shield", "user-slash", "pen", "tower-observation", "file-code", "signal", "bus", "heart-circle-xmark", "house-chimney", "window-maximize", "frown", "prescription", "store-alt", "save", "vihara", "scale-unbalanced", "sort-up", "commenting", "plant-wilt", "diamond", "grin-squint", "hand-holding-usd", "bacterium", "hand-pointer", "drum-steelpan", "hand-scissors", "praying-hands", "redo", "biohazard", "location", "mars-double", "child-dress", "users-between-lines", "lungs-virus", "grin-tears", "phone", "calendar-xmark", "child-reaching", "head-side-virus", "user-gear", "sort-numeric-up", "door-closed", "shield-virus", "dice-six", "mosquito-net", "bridge-water", "person-booth", "text-width", "hat-wizard", "fancy", "person-digging", "trash", "tachometer-average", "book-medical", "poo", "quote-right", "tshirt", "cubes", "divide", "tenge", "headphones", "hands-holding", "hands-clapping", "republican", "arrow-left", "person-circle-xmark", "ruler", "align-left", "dice-d6", "restroom", "j", "users-viewfinder", "file-video", "up-right-from-square", "th", "file-pdf", "book-bible", "o", "suitcase-medical", "user-secret", "otter", "person-dress", "comment-dollar", "business-time", "th-large", "tanakh", "volume-control-phone", "hat-cowboy-side", "clipboard-user", "child", "lira-sign", "satellite", "plane-lock", "tag", "comment", "cake", "envelope", "angles-up", "paperclip", "arrow-right-to-city", "ribbon", "lungs", "sort-numeric-up-alt", "litecoin-sign", "border-none", "circle-nodes", "parachute-box", "indent", "truck-field-un", "hourglass", "mountain", "user-md", "info-circle", "cloud-meatball", "camera", "square-virus", "meteor", "car-on", "sleigh", "sort-numeric-down", "hand-holding-water", "water", "calendar-check", "braille", "prescription-bottle-medical", "landmark", "truck", "crosshairs", "person-cane", "tent", "vest-patches", "check-double", "sort-alpha-down", "money-bill-wheat", "cookie", "undo", "hdd", "grin-squint-tears", "dumbbell", "rectangle-list", "tarp-droplet", "house-medical-circle-check", "skiing-nordic", "calendar-plus", "plane-arrival", "circle-left", "train-subway", "chart-gantt", "inr", "crop-simple", "money-bill-alt", "long-arrow-alt-left", "dna", "virus-slash", "subtract", "chess", "long-arrow-left", "plug-circle-check", "street-view", "franc-sign", "volume-off", "hands-asl-interpreting", "gear", "tint-slash", "mosque", "mosquito", "star-of-david", "person-military-rifle", "shopping-cart", "vials", "plug-circle-plus", "place-of-worship", "grip-vertical", "level-up", "u", "square-root-variable", "clock", "step-backward", "pallet", "faucet", "baseball-bat-ball", "s", "timeline", "keyboard", "caret-down", "house-chimney-medical", "thermometer-three-quarters", "mobile-screen", "plane-up", "piggy-bank", "battery-half", "mountain-city", "coins", "khanda", "sliders", "folder-tree", "network-wired", "map-pin", "hamsa", "cent-sign", "flask", "person-pregnant", "wand-sparkles", "ellipsis-vertical", "ticket", "power-off", "right-long", "flag-usa", "laptop-file", "tty", "diagram-next", "person-rifle", "house-medical-circle-exclamation", "closed-captioning", "person-hiking", "venus-double", "images", "calculator", "people-pulling", "n", "tram", "cloud-rain", "building-circle-xmark", "ship", "arrows-down-to-line", "download", "grin", "delete-left", "eyedropper", "file-circle-check", "forward", "mobile", "meh", "align-center", "book-skull", "id-card", "outdent", "heart-circle-exclamation", "house", "calendar-week", "laptop-medical", "b", "file-medical", "dice-one", "kiwi-bird", "exchange", "rotate-right", "utensils", "sort-amount-up", "mill-sign", "bowl-rice", "skull", "tower-broadcast", "truck-pickup", "up-long", "stop", "code-merge", "upload", "hurricane", "mound", "toilet-portable", "compact-disc", "file-download", "caravan", "shield-cat", "zap", "glass-water", "oil-well", "vault", "mars", "toilet", "plane-circle-xmark", "yen", "ruble", "sun", "guitar", "laugh-wink", "horse-head", "bore-hole", "industry", "circle-down", "arrows-turn-to-dots", "florin-sign", "sort-amount-down-alt", "less-than", "angle-down", "car-tunnel", "head-side-cough", "grip-lines", "thumbs-down", "user-lock", "long-arrow-right", "anchor-circle-xmark", "ellipsis", "chess-pawn", "kit-medical", "person-through-window", "toolbox", "hands-holding-circle", "bug", "credit-card", "car", "hand-holding-hand", "book-reader", "mountain-sun", "arrows-left-right-to-line", "dice-d20", "truck-droplet", "file-circle-xmark", "temperature-up", "medal", "bed", "square-h", "podcast", "thermometer-full", "bell", "superscript", "plug-circle-xmark", "star-of-life", "phone-slash", "paint-roller", "handshake-angle", "map-marker-alt", "file", "greater-than", "swimmer", "arrow-down", "tint", "eraser", "globe-americas", "person-burst", "dove", "battery-empty", "socks", "inbox", "section", "tachometer-alt", "envelope-open-text", "hospital", "wine-bottle", "chess-rook", "stream", "dharmachakra", "hotdog", "person-walking-with-cane", "drum", "ice-cream", "heart-circle-bolt", "fax", "paragraph", "vote-yea", "star-half", "boxes", "link", "ear-listen", "tree-city", "play", "font", "rupiah-sign", "search", "table-tennis", "person-dots-from-line", "trash-restore-alt", "naira-sign", "cart-arrow-down", "walkie-talkie", "file-pen", "receipt", "square-pen", "suitcase-rolling", "person-circle-exclamation", "chevron-down", "battery", "skull-crossbones", "code-compare", "list-ul", "school-lock", "tower-cell", "long-arrow-alt-down", "ranking-star", "chess-king", "person-harassing", "brazilian-real-sign", "landmark-dome", "arrow-up", "tv", "shrimp", "tasks", "jug-detergent", "user-circle", "user-shield", "wind", "car-crash", "y", "snowboarding", "fast", "fish", "user-graduate", "circle-half-stroke", "clapperboard", "radiation-alt", "baseball", "jet-fighter-up", "project-diagram", "copy", "volume-xmark", "hand-sparkles", "grip", "share-square", "child-rifle", "gun", "square-phone", "plus", "expand", "computer", "xmark", "arrows", "chalkboard-user", "peso-sign", "building-shield", "baby", "users-line", "quote-left", "tractor", "trash-restore", "arrow-down-up-lock", "lines-leaning", "ruler-combined", "copyright", "equals", "blender", "teeth", "sheqel", "map", "rocket", "photo-video", "folder-minus", "store", "arrow-trend-up", "plug-circle-minus", "sign", "bezier-curve", "bell-slash", "tablet", "school-flag", "fill", "angle-up", "drumstick-bite", "holly-berry", "chevron-left", "bacteria", "hand-lizard", "notdef", "disease", "briefcase-medical", "genderless", "chevron-right", "retweet", "car-rear", "pump-soap", "video-slash", "battery-quarter", "radio", "carriage-baby", "traffic-light", "thermometer", "vr-cardboard", "hand-middle-finger", "percentage", "truck-moving", "glass-water-droplet", "display", "smile", "thumbtack", "trophy", "pray", "hammer", "hand-peace", "sync-alt", "spinner", "robot", "peace", "gears", "warehouse", "arrow-up-right-dots", "splotch", "grin-hearts", "dice-four", "sim-card", "transgender", "mercury", "level-down", "falling-burst", "award", "ticket-simple", "building", "angles-left", "qrcode", "history", "grin-beam-sweat", "file-export", "shield", "sort-amount-up-alt", "house-medical", "golf-ball", "circle-chevron-left", "house-chimney-window", "pen-nib", "tent-arrow-turn-left", "tents", "wand-magic", "dog", "carrot", "moon", "wine-glass-empty", "cheese", "yin-yang", "music", "code-commit", "temperature-low", "person-biking", "broom", "shield-heart", "gopuram", "globe-oceania", "xmark-square", "hashtag", "up-right-and-down-left-from-center", "oil-can", "t", "hippo", "chart-column", "infinity", "vial-circle-check", "person-arrow-down-to-line", "voicemail", "fan", "person-walking-luggage", "up-down", "cloud-moon-rain", "calendar", "trailer", "haykal", "sd-card", "dragon", "shoe-prints", "plus-circle", "grin-tongue-wink", "hand-holding", "plug-circle-exclamation", "unlink", "clone", "person-walking-arrow-loop-left", "sort-alpha-up-alt", "fire-flame-curved", "tornado", "file-circle-plus", "quran", "anchor", "border-all", "face-angry", "cookie-bite", "arrow-trend-down", "rss", "draw-polygon", "scale-balanced", "tachometer", "shower", "desktop", "m", "th-list", "sms", "book", "user-plus", "check", "battery-three-quarters", "house-circle-check", "angle-left", "diagram-successor", "truck-arrow-right", "arrows-split-up-and-left", "hand-fist", "cloud-moon", "briefcase", "falling", "portrait", "user-tag", "rug", "globe-europe", "luggage-cart", "window-close", "baht-sign", "book-open", "journal-whills", "handcuffs", "warning", "database", "share", "bottle-droplet", "face", "hill-rockslide", "right-left", "paper-plane", "road-circle-exclamation", "dungeon", "align-right", "money-bill-wave-alt", "life-ring", "signing", "calendar-day", "water-ladder", "arrows-v", "grimace", "wheelchair-move", "turn-down", "person-walking-arrow-right", "square-envelope", "dice", "bowling-ball", "brain", "bandage", "calendar-minus", "xmark-circle", "gifts", "hotel", "globe-asia", "id-card-clip", "search-plus", "thumbs-up", "user-clock", "hand-dots", "file-invoice", "window-minimize", "mug-saucer", "brush", "mask", "search-minus", "ruler-vertical", "user-large", "train-tram", "user-nurse", "syringe", "cloud-sun", "stopwatch-20", "square-full", "magnet", "jar", "sticky-note", "bug-slash", "arrow-up-from-water-pump", "bone", "user-injured", "sad-tear", "plane", "tent-arrows-down", "exclamation", "arrows-spin", "print", "turkish-lira", "usd", "x", "search-dollar", "users-gear", "person-military-pointing", "university", "umbrella", "trowel", "d", "stapler", "theater-masks", "kip-sign", "hand-point-left", "handshake-simple", "jet-fighter", "square-share-nodes", "barcode", "plus-minus", "video", "mortar-board", "hand-holding-medical", "person-circle-check", "turn-up"];
 
 function Ae(e) {
     function n() {
         const a = {
             position: "fixed",
             color: "white",
             backgroundColor: e.isError ? "#e52207" : "#1151b3",
             width: 300,
             top: 10,
             left: (window.innerWidth - 320) / 2,
             padding: 15
         };
         return t.jsxs("div", {
             style: a,
-            children: [t.jsx(b, {
+            children: [t.jsx(k, {
                 icon: e.isError ? "xmark-circle" : "circle-check",
                 style: {
                     marginRight: 5
                 }
             }), e.text]
         })
     }
     return n()
 }
 
 function ee(e, n = !1) {
     const a = document.createElement("div");
-    a.classList.add("message"), W.createRoot(document.body.appendChild(a)).render(t.jsx(Ae, {
+    a.classList.add("message"), P.createRoot(document.body.appendChild(a)).render(t.jsx(Ae, {
         text: e,
         isError: n
     })), setTimeout(function() {
         a.remove()
     }, 3e3)
 }
 
@@ -137,33 +137,33 @@
                 children: e.children
             })]
         })
     }
     return n()
 }
 
-function Le(e) {
+function qe(e) {
     return ye(e.data)
 }
 
-function A(e) {
+function q(e) {
     return e.replace("/app/", "/api/")
 }
 
 function H(e) {
     return e.replace("/api/", "/app/")
 }
 
-function E(e, n, a, r) {
+function I(e, n, a, r) {
     const d = localStorage.getItem("token");
     var i = {
         Accept: "application/json"
     };
     d && (i.Authorization = "Token " + d);
-    const o = A(n);
+    const o = q(n);
     var s = {
         method: e,
         headers: new Headers(i),
         ajax: 1
     };
     r && (s.body = r);
     var c = null,
@@ -176,16 +176,16 @@
         if (u == "application/json") {
             var m = JSON.parse(l || "{}");
             typeof m == "object" && m.type == "redirect" ? document.location.href = H(m.url) : a && a(m, c)
         } else if (u.indexOf("text") < 0 || u.indexOf("csv") >= 0) {
             var x = window.URL.createObjectURL(new Blob([new Uint8Array(l)], {
                     type: u
                 })),
-                v = document.createElement("a");
-            v.href = x, u.indexOf("excel") >= 0 ? v.download = "Download.xls" : u.indexOf("pdf") >= 0 ? v.download = "Download.pdf" : u.indexOf("zip") >= 0 ? v.download = "Download.zip" : u.indexOf("json") >= 0 ? v.download = "Download.json" : u.indexOf("csv") >= 0 ? v.download = "Download.csv" : u.indexOf("png") >= 0 && (v.download = "Download.png"), document.body.appendChild(v), v.click(), a && a({}, c)
+                w = document.createElement("a");
+            w.href = x, u.indexOf("excel") >= 0 ? w.download = "Download.xls" : u.indexOf("pdf") >= 0 ? w.download = "Download.pdf" : u.indexOf("zip") >= 0 ? w.download = "Download.zip" : u.indexOf("json") >= 0 ? w.download = "Download.json" : u.indexOf("csv") >= 0 ? w.download = "Download.csv" : u.indexOf("png") >= 0 && (w.download = "Download.png"), document.body.appendChild(w), w.click(), a && a({}, c)
         } else a && a(l, c)
     })
 }
 
 function ye(e) {
     e.store && Object.keys(e.store).map(function(n) {
         e.store[n] ? localStorage.setItem(n, e.store[n]) : localStorage.removeItem(n, e.store[n])
@@ -197,70 +197,70 @@
     if (e === !0) return "Sim";
     if (e === !1) return "Não";
     if (typeof e == "number") {
         var n = e.toString().split(".");
         return n.length == 1 ? e.toString().replace(/\B(?=(\d{3})+(?!\d))/g, ".") : (n[0] = n[0].toString().replace(/\B(?=(\d{3})+(?!\d))/g, "."), n[1] = n[1].substring(0, 2), n[1].length == 1 && (n[1] = n[1] + "0"), n[0] + "," + n[1])
     }
     if (typeof e == "string") {
-        if (e.length == 7 && e[0] == "#") return t.jsx(y, {
+        if (e.length == 7 && e[0] == "#") return t.jsx(p, {
             data: {
                 type: "color",
                 value: e
             }
         });
         if (e.length == 19 && e[13] == ":" && e[16] == ":") {
             var n = e.split(" "),
                 a = n[0],
                 r = n[1];
             return r == "00:00:00" ? a : a + " " + r
         }
         return e
     }
-    return typeof e == "object" && e.type ? t.jsx(y, {
+    return typeof e == "object" && e.type ? t.jsx(p, {
         data: e
     }) : typeof e == "object" && Array.isArray(e) ? e.length == 0 ? "-" : t.jsx("ul", {
         style: {
             padding: 0
         },
         children: e.map(function(d) {
             return t.jsx("li", {
                 children: d
             }, Math.random())
         })
     }) : typeof e == "object" && JSON.stringify(Object.keys(e)) == JSON.stringify(["id", "text"]) ? e.text : JSON.stringify(e)
 }
 
 function pe() {
-    document.querySelector(".layer") == null && W.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Ne, {}))
+    document.querySelector(".layer") == null && P.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Re, {}))
 }
 
 function ve(e, n) {
     xe(), pe(), window.reloader = n;
     for (var a = document.getElementsByTagName("dialog"), r = 0; r < a.length; r++) a[r].style.display = "none";
-    W.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Oe, {
-        url: A(e)
+    P.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Ne, {
+        url: q(e)
     }))
 }
 
-function Re(e) {
-    xe(), pe(), W.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(_e, {
-        url: A(e)
+function Oe(e) {
+    xe(), pe(), P.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(_e, {
+        url: q(e)
     }))
 }
 
 function V(e) {
     e != null && showMessage(e);
     for (var n = document.getElementsByTagName("dialog"), a = 0; a < n.length; a++)
         if (a == n.length - 1) {
             var r = n[a];
             r.close(), r.classList.remove("opened"), r.remove(), a == 0 ? (document.querySelector(".layer").style.display = "none", window.reloader && window.reloader()) : n[a - 1].style.display = "block"
         }
 }
 
-function Ne(e) {
+function Re(e) {
     const n = {
         backgroundColor: "black",
         bottom: 0,
         left: 0,
         position: "fixed",
         right: 0,
         top: 0,
@@ -272,22 +272,22 @@
         onClick: function() {
             V()
         },
         style: n
     })
 }
 
-function Oe(e) {
-    const [n, a] = C.useState(null), [r, d] = C.useState(0);
-    C.useEffect(() => {
-        i(A(e.url)), document.querySelector(".layer").style.display = "block"
+function Ne(e) {
+    const [n, a] = M.useState(null), [r, d] = M.useState(0);
+    M.useEffect(() => {
+        i(q(e.url)), document.querySelector(".layer").style.display = "block"
     }, []);
 
     function i(c) {
-        E("GET", A(c), function(u) {
+        I("GET", q(c), function(u) {
             a(u), d(r + 1)
         })
     }
 
     function o() {
         const c = {
                 maxWidth: 800
@@ -296,19 +296,19 @@
                 textAlign: "right",
                 cursor: "pointer"
             };
         if (n) return t.jsxs("div", {
             style: c,
             children: [t.jsx("div", {
                 style: u,
-                children: t.jsx(b, {
+                children: t.jsx(k, {
                     icon: "x",
                     onClick: () => V()
                 })
-            }), t.jsx(y, {
+            }), t.jsx(p, {
                 data: n
             })]
         })
     }
     const s = {
         minWidth: "50%",
         display: n ? "block" : "none",
@@ -319,15 +319,15 @@
         style: s,
         children: o()
     }, r)
 }
 
 function _e(e) {
     var n = Math.random();
-    C.useEffect(() => {
+    M.useEffect(() => {
         document.querySelector(".layer").style.display = "block";
         var r = document.getElementById(n);
         r.style.top = document.documentElement.scrollTop + 100
     }, []);
 
     function a() {
         const r = {
@@ -342,48 +342,48 @@
                 marginTop: -20
             };
         return t.jsxs("dialog", {
             style: r,
             id: n,
             children: [t.jsx("div", {
                 style: d,
-                children: t.jsx(b, {
+                children: t.jsx(k, {
                     icon: "x",
                     onClick: () => V()
                 })
             }), t.jsx("iframe", {
-                src: A(e.url),
+                src: q(e.url),
                 width: "100%",
                 height: 500,
                 style: {
                     border: 0
                 }
             })]
         })
     }
     return a()
 }
 
-function w(e) {
+function C(e) {
     return e != null && (e = e.toString().replace("-", "").normalize("NFD").replace("_", "").toLowerCase()), e
 }
 
 function N(e) {
     const n = e.id || Math.random(),
-        [a, r] = C.useState(e.data.name);
+        [a, r] = M.useState(e.data.name);
 
     function d(s) {
         s.preventDefault(), e.onClick ? (a && r("Aguarde...."), e.onClick(s)) : e.data.modal == !1 ? window.load(H(e.data.url)) : ve(e.data.url)
     }
 
     function i() {
-        return e.data.icon ? e.compact || !e.data.name || window.innerWidth < 800 ? t.jsx(b, {
+        return e.data.icon ? e.compact || !e.data.name || window.innerWidth < 800 ? t.jsx(k, {
             icon: e.data.icon
         }) : t.jsxs(t.Fragment, {
-            children: [t.jsx(b, {
+            children: [t.jsx(k, {
                 icon: e.data.icon,
                 style: {
                     paddingRight: 10
                 }
             }), e.data.name || ""]
         }) : e.data.name
     }
@@ -398,15 +398,15 @@
         return e.primary && (s.backgroundColor = "#1351b4", s.color = "white"), e.default && (s.border = "solid 1px #1351b4", s.color = "#1351b4"), e.style && Object.keys(e.style).map(function(c) {
             s[c] = e.style[c]
         }), t.jsx("a", {
             id: n,
             href: H(e.data.url) || "#",
             onClick: d,
             style: s,
-            "data-label": w(e.data.name),
+            "data-label": C(e.data.name),
             children: i()
         })
     }
     return o()
 }
 
 function X(e) {
@@ -443,15 +443,15 @@
             };
         return t.jsxs(t.Fragment, {
             children: [t.jsx("div", {
                 onClick: a,
                 style: {
                     cursor: "pointer"
                 },
-                "data-label": w(e.dataLabel),
+                "data-label": C(e.dataLabel),
                 children: e.children
             }), e.actions && e.actions.length > 0 && t.jsx("ul", {
                 style: i,
                 onMouseLeave: r,
                 className: "dropdown",
                 children: e.actions.map(s => t.jsx("li", {
                     style: o,
@@ -464,36 +464,36 @@
                 }, Math.random()))
             })]
         })
     }
     return d()
 }
 
-function P({
+function W({
     id: e,
     href: n,
     modal: a,
     imodal: r,
     children: d,
     onClick: i,
     dataLabel: o,
     style: s
 }) {
     const c = n && n.indexOf("/media/") < 0 ? H(n) : n;
 
     function u(m) {
-        m.preventDefault(), a ? ve(c) : r ? Re(c) : window.load(c)
+        m.preventDefault(), a ? ve(c) : r ? Oe(c) : window.load(c)
     }
 
     function l() {
         return t.jsx("a", {
             id: e,
             onClick: i || u,
             href: c || "#",
-            "data-label": w(o),
+            "data-label": C(o),
             style: s,
             children: d
         })
     }
     return l()
 }
 
@@ -539,18 +539,18 @@
         })
     }
     return n()
 }
 
 function Fe(e) {
     const n = Math.random(),
-        [a, r] = C.useState(e.data);
+        [a, r] = M.useState(e.data);
 
     function d(o) {
-        E("GET", o, function(s) {
+        I("GET", o, function(s) {
             r(s)
         })
     }
 
     function i() {
         return window[n] = () => d(e.data.url), t.jsx("div", {
             className: e.data.url && "reloadable",
@@ -722,17 +722,17 @@
                 children: [n(), a(), d()]
             })]
         })
     }
     return i()
 }
 
-function Pe(e) {
+function We(e) {
     const n = Math.random(),
-        [a, r] = C.useState(e.data);
+        [a, r] = M.useState(e.data);
 
     function d() {
         return t.jsx(ke, {
             data: a
         })
     }
 
@@ -760,21 +760,21 @@
                 }, Math.random()))
             }, Math.random()) : t.jsx("div", {
                 children: t.jsx(J, {
                     data: u,
                     width: 100
                 })
             }, Math.random())
-        }) : t.jsx(y, {
+        }) : t.jsx(p, {
             data: a.data
         })
     }
 
     function s(u) {
-        E("GET", u, function(l) {
+        I("GET", u, function(l) {
             r(l)
         })
     }
 
     function c() {
         return e.data.url ? (window[n] = () => s(e.data.url), t.jsxs("div", {
             className: e.data.url && "reloadable",
@@ -783,25 +783,25 @@
         })) : t.jsxs("div", {
             children: [d(), i()]
         })
     }
     return c()
 }
 
-function We(e) {
+function Pe(e) {
     const n = Math.random(),
-        [a, r] = C.useState(e.data.actions);
+        [a, r] = M.useState(e.data.actions);
 
     function d() {
         const s = e.data.url.indexOf("?") < 0 ? "?" : "&";
         return e.data.url + s + "only=actions"
     }
 
     function i() {
-        E("GET", d(), function(s) {
+        I("GET", d(), function(s) {
             r(s)
         })
     }
 
     function o() {
         return window[n] = () => i(), t.jsx("div", {
             className: "reloadable",
@@ -827,17 +827,17 @@
             r = {
                 margin: 0
             };
         return t.jsxs("div", {
             style: a,
             children: [e.data.title && t.jsx("h1", {
                 style: r,
-                "data-label": w(e.data.title),
+                "data-label": C(e.data.title),
                 children: e.data.title
-            }), t.jsx(We, {
+            }), t.jsx(Pe, {
                 data: e.data
             })]
         })
     }
     return n()
 }
 
@@ -852,15 +852,15 @@
                 marginBottom: 0,
                 marginTop: 15
             };
         return t.jsxs("div", {
             style: a,
             children: [e.data.title && t.jsx("h2", {
                 style: r,
-                "data-label": w(e.data.title),
+                "data-label": C(e.data.title),
                 children: e.data.title
             }), e.data.actions.length > 0 && t.jsx("div", {
                 children: e.data.actions.map(function(d) {
                     return t.jsx(N, {
                         data: d,
                         default: !0
                     }, Math.random())
@@ -876,15 +876,15 @@
         return t.jsx(Ge, {
             data: e.data
         })
     }
 
     function a() {
         return e.data.data.map(function(d, i) {
-            return t.jsx(y, {
+            return t.jsx(p, {
                 data: d
             }, Math.random())
         })
     }
 
     function r() {
         return t.jsxs(t.Fragment, {
@@ -904,15 +904,15 @@
     function a() {
         const d = {
             backgroundColor: "white"
         };
         return e.data.data.map(function(i, o) {
             return t.jsx("div", {
                 style: d,
-                children: t.jsx(y, {
+                children: t.jsx(p, {
                     data: i
                 }, Math.random())
             })
         })
     }
 
     function r() {
@@ -920,55 +920,55 @@
             children: [n(), a()]
         })
     }
     return r()
 }
 
 function $e(e) {
-    const [n, a] = C.useState(0);
+    const [n, a] = M.useState(0);
 
     function r() {
         return t.jsx("div", {
             style: {
                 display: "inline-block",
                 textAlign: "center",
                 width: "100%",
                 margin: "auto",
                 marginBottom: 20
             },
             children: e.data.map(function(d, i) {
-                return t.jsx(P, {
+                return t.jsx(W, {
                     href: d.url,
                     style: {
                         padding: 5,
                         fontWeight: n == i ? "bold" : "normal",
                         borderBottom: n == i ? "solid 3px #2670e8" : "solid 3px inherite",
                         textDecoration: "none",
                         color: "#0c326f",
                         margin: 15
                     },
                     onClick: function(o) {
                         o.preventDefault(), a(i), e.loadContent(d.url)
                     },
-                    dataLabel: w(d.title),
+                    dataLabel: C(d.title),
                     children: d.title
                 }, Math.random())
             })
         })
     }
     return r()
 }
 
 function Je(e) {
     var n = Math.random();
-    const [a, r] = C.useState(e.data.data[0]);
+    const [a, r] = M.useState(e.data.data[0]);
 
     function d() {
         return e.data.title != "Top" && t.jsx("h2", {
-            "data-label": w(e.data.title),
+            "data-label": C(e.data.title),
             children: e.data.title
         })
     }
 
     function i() {
         return t.jsx($e, {
             data: e.data.data,
@@ -982,15 +982,15 @@
         };
         l.title = null;
         const m = {
             padding: 0
         };
         return t.jsx("div", {
             style: m,
-            children: t.jsx(y, {
+            children: t.jsx(p, {
                 data: l
             }, Math.random())
         })
     }
 
     function s() {
         const l = {
@@ -1002,15 +1002,15 @@
         };
         return t.jsx("div", {
             style: l
         })
     }
 
     function c(l) {
-        E("GET", l, function(m) {
+        I("GET", l, function(m) {
             r(m)
         })
     }
 
     function u() {
         return window[n] = () => c(a.url), e.data.data.length > 0 && t.jsxs("div", {
             className: "reloadable",
@@ -1023,34 +1023,34 @@
 
 function Ye() {
     document.querySelectorAll(".reloadable").forEach(function(e) {
         window[e.id]()
     })
 }
 
-function B({
+function A({
     id: e,
     onClick: n,
     icon: a,
     label: r,
     display: d,
     primary: i,
     compact: o,
     spin: s
 }) {
     function c() {
-        return a ? o || !r ? t.jsx(b, {
+        return a ? o || !r ? t.jsx(k, {
             icon: a
         }) : t.jsxs(t.Fragment, {
-            children: [t.jsx(Be, {
+            children: [t.jsx(De, {
                 style: {
                     marginRight: 10,
                     display: "none"
                 }
-            }), t.jsx(b, {
+            }), t.jsx(k, {
                 icon: a,
                 style: {
                     marginRight: 10
                 }
             }), r || ""]
         }) : r
     }
@@ -1066,15 +1066,15 @@
             display: d || "block",
             width: "fit-content",
             textWrap: "nowrap"
         };
         return i ? (l.backgroundColor = "#1351b4", l.color = "white") : (l.border = "solid 1px #1351b4", l.color = "#1351b4"), t.jsx("a", {
             id: e,
             style: l,
-            "data-label": w(r || a),
+            "data-label": C(r || a),
             onClick: m => {
                 m.preventDefault(), a && s && (m.target.dataset.spinning = a, m.target.querySelector("i.fa-spin").style.display = "inline-block", m.target.querySelector("i.fa-" + a).style.display = "none"), n(m)
             },
             children: c()
         })
     }
     return u()
@@ -1092,15 +1092,15 @@
         for (var n = 0; n < a.length; n++)
             if (e.toLowerCase().indexOf(a[n]) > 0) return !0
     }
 }
 
 function Se(e, n) {
     var a = new FormData(e);
-    E("POST", n, et, a)
+    I("POST", n, et, a)
 }
 
 function Xe(e) {
     if (e) {
         var n = document.querySelector(".form-fieldset." + e);
         n && (n.style.display = "none");
         var a = document.querySelector(".form-group." + e);
@@ -1154,15 +1154,15 @@
             justifyContent: "space-between",
             marginTop: 10,
             marginBottom: 10
         };
         return t.jsxs("div", {
             style: a,
             children: [t.jsxs("div", {
-                children: [t.jsx(b, {
+                children: [t.jsx(k, {
                     icon: "circle-check",
                     style: {
                         color: "#155bcb",
                         marginRight: 20
                     }
                 }), e.data.text]
             }), e.children && t.jsx("div", {
@@ -1182,15 +1182,15 @@
             marginTop: 2,
             marginBottom: 2,
             padding: 8
         };
         return t.jsxs("div", {
             style: a,
             id: e.id,
-            children: [t.jsx(b, {
+            children: [t.jsx(k, {
                 icon: "xmark-circle",
                 style: {
                     marginRight: 5
                 }
             }), t.jsx("span", {})]
         })
     }
@@ -1292,20 +1292,20 @@
     }
     return o()
 }
 
 function he(e) {
     var n = "";
     const a = e.data.name + Math.random();
-    e.data.mask == "decimal" && (n = "decimal", e.data.value && (e.data.value = Math.round(parseFloat(e.data.value)).toFixed(2).replace(".", ","))), C.useEffect(() => {
+    e.data.mask == "decimal" && (n = "decimal", e.data.value && (e.data.value = Math.round(parseFloat(e.data.value)).toFixed(2).replace(".", ","))), M.useEffect(() => {
         function o(u, l, m) {
             var x = m.target,
-                v = x.value.replace(/\D/g, ""),
-                j = x.value.length > l ? 1 : 0;
-            VMasker(x).unMask(), VMasker(x).maskPattern(u[j]), x.value = VMasker.toPattern(v, u[j])
+                w = x.value.replace(/\D/g, ""),
+                S = x.value.length > l ? 1 : 0;
+            VMasker(x).unMask(), VMasker(x).maskPattern(u[S]), x.value = VMasker.toPattern(w, u[S])
         }
         if (e.data.mask) {
             var s = document.getElementById(a);
             if (e.data.mask == "decimal") VMasker(s).maskMoney({
                 precision: 2,
                 separator: ",",
                 delimiter: "."
@@ -1323,29 +1323,29 @@
 
     function d(o) {
         if (e.data.type == "file" && o.target.files) {
             let c = o.target.files[0];
             var s = new FileReader;
             s.onload = function(u) {
                 if (re(c.name)) {
-                    const v = "display" + a;
+                    const w = "display" + a;
                     var l = document.createElement("img");
-                    l.id = o.target.id + "img", l.style.width = "200px", l.style.display = "block", l.style.margin = "auto", l.style.marginTop = "20px", l.onload = function(j) {
-                        const I = e.data.width > e.data.height ? e.data.width / l.width : e.data.height / l.height;
-                        var M = document.createElement("canvas");
-                        const q = M.getContext("2d");
-                        M.height = M.width * (l.height / l.width);
-                        const S = document.createElement("canvas"),
-                            F = S.getContext("2d");
-                        S.width = l.width * I, S.height = l.height * I, F.drawImage(l, 0, 0, S.width, S.height), q.drawImage(S, 0, 0, S.width * I, S.height * I, 0, 0, M.width, M.height), S.toBlob(function(h) {
+                    l.id = o.target.id + "img", l.style.width = "200px", l.style.display = "block", l.style.margin = "auto", l.style.marginTop = "20px", l.onload = function(S) {
+                        const B = e.data.width > e.data.height ? e.data.width / l.width : e.data.height / l.height;
+                        var y = document.createElement("canvas");
+                        const j = y.getContext("2d");
+                        y.height = y.width * (l.height / l.width);
+                        const v = document.createElement("canvas"),
+                            L = v.getContext("2d");
+                        v.width = l.width * B, v.height = l.height * B, L.drawImage(l, 0, 0, v.width, v.height), j.drawImage(v, 0, 0, v.width * B, v.height * B, 0, 0, y.width, y.height), v.toBlob(function(h) {
                             const f = new DataTransfer;
                             f.items.add(new File([h], c.name)), o.target.files = f.files
                         });
-                        var D = document.getElementById(v);
-                        D == null ? (D = document.createElement("div"), D.id = v) : D.removeChild(D.childNodes[0]), D.appendChild(l), o.target.parentNode.appendChild(D)
+                        var D = document.getElementById(w);
+                        D == null ? (D = document.createElement("div"), D.id = w) : D.removeChild(D.childNodes[0]), D.appendChild(l), o.target.parentNode.appendChild(D)
                     }, l.src = u.target.result
                 }
                 const m = document.getElementById("fileinfo" + a);
                 var x = c.size / 1024;
                 x < 1024 ? x = parseInt(x) + " Kb" : x = (x / 1024).toFixed(2) + " Mb", m.innerHTML = c.name + " / " + x, e.data.max_size && c.size / 1024 / 1024 > e.data.max_size && alert("O limite de tamanho é " + e.data.max_size + "Mb. O arquivo informado possui " + x + ". Por favor, adicione um arquivo menor.")
             }, s.readAsDataURL(c)
         }
@@ -1370,15 +1370,15 @@
                         backgroundColor: "rgba(15, 145, 210, 0.05)",
                         border: "1px dashed rgba(15, 145, 210, 0.4)",
                         borderRadius: 10,
                         textAlign: "center"
                     },
                     children: [t.jsx("div", {
                         style: u,
-                        children: t.jsx(b, {
+                        children: t.jsx(k, {
                             icon: "cloud-upload",
                             style: {
                                 fontSize: "2.5rem",
                                 color: "#1351b4"
                             }
                         })
                     }), t.jsxs("div", {
@@ -1400,25 +1400,25 @@
                             className: "bold",
                             id: "fileinfo" + a,
                             children: ["O arquivo", e.data.max_size && "deve possuir até " + e.data.max_size + " Mb e ", "deve ter extensão", " ", e.data.extensions.map(l => "." + l).join(" ou "), "."]
                         })]
                     }), t.jsx("div", {
                         style: u,
                         align: "center",
-                        children: t.jsx(B, {
+                        children: t.jsx(A, {
                             label: "Selecionar Arquivo",
                             onClick: () => document.getElementById(a).click()
                         })
                     })]
                 }), t.jsx("input", {
                     className: "form-control " + n,
                     type: o,
                     name: e.data.name,
                     id: a,
-                    "data-label": w(e.data.label),
+                    "data-label": C(e.data.label),
                     readOnly: e.data.read_only,
                     onBlur: e.data.onchange ? r : null,
                     onChange: d,
                     style: {
                         zIndex: "-1",
                         marginTop: -20
                     },
@@ -1431,15 +1431,15 @@
                 ...Y
             }, c.width = "100%", c.backgroundColor = "white", c.height = 47.5), t.jsx("input", {
                 className: "form-control " + n,
                 type: o,
                 name: e.data.name,
                 id: a,
                 defaultValue: e.data.value,
-                "data-label": w(e.data.label),
+                "data-label": C(e.data.label),
                 readOnly: e.data.read_only,
                 onBlur: e.data.onchange ? r : null,
                 onChange: d,
                 style: c
             })
         }
     }
@@ -1456,82 +1456,82 @@
     }) : e.data.value != null && n.push({
         id: e.data.value.id,
         value: e.data.value.label
     }), e.data.id == null && (e.data.id = Math.random()), e.data.id2 == null && (e.data.id2 = e.data.id + "__autocomplete");
     const a = e.data.id,
         r = e.data.id2,
         d = Array.isArray(e.data.value),
-        [i, o] = C.useState(!1),
-        [s, c] = C.useState(null);
+        [i, o] = M.useState(!1),
+        [s, c] = M.useState(null);
     var u = !1;
     let l;
-    C.useEffect(() => {
-        S(n), document.getElementById(a).addEventListener("customchange", function(h) {
-            S(h.detail.value), reactTriggerChange(document.getElementById(e.data.name))
+    M.useEffect(() => {
+        v(n), document.getElementById(a).addEventListener("customchange", function(h) {
+            v(h.detail.value), reactTriggerChange(document.getElementById(e.data.name))
         })
     }, []);
 
     function m() {
         const h = document.getElementById(a);
         if (d) {
             const f = {
                     padding: 5,
                     display: "inline"
                 },
                 g = {
                     cursor: "pointer",
                     marginRight: 5
                 },
-                p = {
+                b = {
                     fontSize: "0.8rem"
                 };
             return t.jsxs("div", {
-                children: [h == null && n.map((k, R) => t.jsxs("div", {
+                children: [h == null && n.map((T, R) => t.jsxs("div", {
                     style: f,
                     children: [t.jsx("span", {
-                        onClick: () => F(R),
+                        onClick: () => L(R),
                         style: g,
-                        children: t.jsx(b, {
+                        children: t.jsx(k, {
                             icon: "trash-can",
-                            style: p
+                            style: b
                         })
-                    }), k.value]
-                }, Math.random())), h != null && Array.from(h.options).map((k, R) => t.jsxs("div", {
+                    }), T.value]
+                }, Math.random())), h != null && Array.from(h.options).map((T, R) => t.jsxs("div", {
                     style: f,
                     children: [t.jsx("span", {
-                        onClick: () => F(R),
+                        onClick: () => L(R),
                         style: g,
-                        children: t.jsx(b, {
+                        children: t.jsx(k, {
                             icon: "trash-can",
-                            style: p
+                            style: b
                         })
-                    }), k.innerHTML]
+                    }), T.innerHTML]
                 }, Math.random()))]
             })
         }
     }
 
     function x(h) {
         c([])
     }
 
-    function v() {
+    function w() {
         return t.jsx("select", {
             onChange: x,
             id: a,
             name: e.data.name,
             multiple: d,
             readOnly: !0,
             style: {
                 display: "contents"
             }
         })
     }
 
-    function j() {
+    function S() {
         const h = {
                 ...Y,
                 ...e.style || {}
             },
             f = {
                 padding: 0,
                 margin: 0,
@@ -1540,120 +1540,120 @@
                 borderRadius: 5,
                 maxHeight: 150,
                 overflowY: "auto"
             };
         f.position = "absolute", f.backgroundColor = "white";
         const g = document.getElementById(r);
         if (g) {
-            let T = null,
+            let E = null,
                 z = g,
                 G = null;
             for (; !G && (z = z.parentElement) instanceof HTMLElement;) z.matches("dialog") && (G = z);
-            T = G;
-            const O = g.getBoundingClientRect();
-            var p = O.top + O.height,
-                k = O.left;
-            if (T) {
-                const Q = T.getBoundingClientRect();
-                p = p - Q.top, k = k - Q.left
-            } else p += window.scrollY, k += window.scrollX;
-            f.width = O.width, f.top = p, f.left = k
+            E = G;
+            const _ = g.getBoundingClientRect();
+            var b = _.top + _.height,
+                T = _.left;
+            if (E) {
+                const Q = E.getBoundingClientRect();
+                b = b - Q.top, T = T - Q.left
+            } else b += window.scrollY, T += window.scrollX;
+            f.width = _.width, f.top = b, f.left = T
         }
         const R = {
                 cursor: "pointer",
                 padding: 10
             },
             ne = !d && n.length > 0 && n[0].value || "";
         return t.jsxs(t.Fragment, {
             children: [t.jsx("input", {
                 id: r,
                 name: e.data.name + "__autocomplete",
                 type: "text",
                 className: "form-control",
-                onFocus: T => {
-                    T.target.select(), q(T)
+                onFocus: E => {
+                    E.target.select(), j(E)
                 },
-                onChange: q,
-                onMouseLeave: I,
-                onBlur: I,
+                onChange: j,
+                onMouseLeave: B,
+                onBlur: B,
                 defaultValue: ne,
                 style: h,
-                "data-label": w(e.data.label)
+                "data-label": C(e.data.label)
             }), s && i && t.jsxs("ul", {
                 style: f,
-                onMouseLeave: M,
-                onMouseEnter: function(T) {
+                onMouseLeave: y,
+                onMouseEnter: function(E) {
                     u = !0
                 },
                 children: [s.length == 0 && t.jsx("li", {
                     style: R,
                     children: "Nenhuma opção encontrada."
-                }), s.map(T => t.jsx("li", {
+                }), s.map(E => t.jsx("li", {
                     onClick: () => {
-                        o(!1), e.onSelect ? e.onSelect(T) : S(T)
+                        o(!1), e.onSelect ? e.onSelect(E) : v(E)
                     },
                     style: R,
                     className: "autocomplete-item",
-                    "data-label": w(T.value),
-                    children: T.value
+                    "data-label": C(E.value),
+                    children: E.value
                 }, Math.random()))]
             })]
         })
     }
 
-    function I(h) {
+    function B(h) {
         u = !1, setTimeout(function() {
-            M(h)
+            y(h)
         }, 250)
     }
 
-    function M(h) {
+    function y(h) {
         const f = document.getElementById(a),
             g = document.getElementById(r);
         d || f.options.length > 0 && g.value != f.options[0].innerHTML && (f.innerHTML = "", g.value = "", o(!1)), h.target.tagName == "UL" ? o(!1) : u || o(!1)
     }
 
-    function q(h) {
+    function j(h) {
         clearTimeout(l), l = setTimeout(function() {
             const f = e.data.choices.indexOf("?") < 0 ? "?" : "&";
-            o(!0), E("GET", e.data.choices + f + "term=" + h.target.value, function(p) {
-                c(p)
+            o(!0), I("GET", e.data.choices + f + "term=" + h.target.value, function(b) {
+                c(b)
             })
         }, 1e3)
     }
 
-    function S(h) {
+    function v(h) {
         const f = document.getElementById(a),
             g = document.getElementById(r);
-        f.innerHTML == null && (f.innerHTML = ""), Array.isArray(h) ? f.innerHTML = h.map(p => `<option selected value="${p.id}">${p.value}</option>`).join("") : d ? (f.innerHTML += `<option selected value="${h.id}">${h.value}</option>`, g.value = "") : (f.innerHTML = `<option selected value="${h.id}">${h.value}</option>`, g.value = h.value), e.data.onchange && Se(g.closest("form"), e.data.onchange)
+        f.innerHTML == null && (f.innerHTML = ""), Array.isArray(h) ? f.innerHTML = h.map(b => `<option selected value="${b.id}">${b.value}</option>`).join("") : d ? (f.innerHTML += `<option selected value="${h.id}">${h.value}</option>`, g.value = "") : (f.innerHTML = `<option selected value="${h.id}">${h.value}</option>`, g.value = h.value), e.data.onchange && Se(g.closest("form"), e.data.onchange)
     }
 
-    function F(h) {
+    function L(h) {
         const f = document.getElementById(a);
         var g = Array.from(f.options);
-        f.innerHTML = g.slice(0, h).concat(g.slice(h + 1)).map(p => `<option selected value="${p.value}">${p.innerHTML}</option>`).join(""), c([])
+        f.innerHTML = g.slice(0, h).concat(g.slice(h + 1)).map(b => `<option selected value="${b.value}">${b.innerHTML}</option>`).join(""), c([])
     }
 
     function D() {
         return t.jsxs(t.Fragment, {
-            children: [m(), v(), j()]
+            children: [m(), w(), S()]
         })
     }
     return D()
 }
 
 function rt(e) {
     function n() {
         var a = {
             ...Y
         };
         return a.height = 100, t.jsx("textarea", {
             id: e.data.name,
             name: e.data.name,
-            "data-label": w(e.data.label),
+            "data-label": C(e.data.label),
             style: a,
             defaultValue: e.data.value || "",
             className: "form-control"
         })
     }
     return n()
 }
@@ -1698,15 +1698,15 @@
                 },
                 children: [t.jsx("input", {
                     id: a.name + n + c,
                     type: "radio",
                     name: a.name,
                     defaultValue: s.id,
                     defaultChecked: r(s),
-                    "data-label": w(s.value),
+                    "data-label": C(s.value),
                     onClick: function() {
                         d(a.name + n + c)
                     },
                     onMouseEnter: function() {
                         i(a.name + n + c)
                     }
                 }), t.jsx("label", {
@@ -1742,15 +1742,15 @@
                 },
                 children: [t.jsx("input", {
                     id: a.name + n + o,
                     type: "checkbox",
                     name: a.name,
                     defaultValue: i.id,
                     defaultChecked: r(i),
-                    "data-label": w(i.value)
+                    "data-label": C(i.value)
                 }), t.jsx("label", {
                     htmlFor: a.name + n + o,
                     children: i.value
                 })]
             }, n + o))
         })
     }
@@ -1760,15 +1760,15 @@
 function lt(e) {
     var n = e.data;
     return t.jsx(t.Fragment, {
         children: t.jsx("select", {
             className: "form-control",
             id: n.name,
             name: n.name,
-            "data-label": w(n.label),
+            "data-label": C(n.label),
             defaultValue: n.value,
             style: Y,
             children: n.choices.map(a => t.jsx("option", {
                 value: a.id,
                 children: a.value
             }, Math.random()))
         })
@@ -1783,21 +1783,21 @@
     function d() {
         return !e.data.required && t.jsx("div", {
             id: "info-" + n,
             children: t.jsxs(le, {
                 data: {
                     text: "Esta informação é opcional. Controle seu preenchimento com o botão ao lado."
                 },
-                children: [t.jsx(B, {
+                children: [t.jsx(A, {
                     primary: !0,
                     icon: "pen-clip",
                     onClick: () => i(!0),
                     id: "show-" + n,
                     display: r.value ? "none" : "inline"
-                }), t.jsx(B, {
+                }), t.jsx(A, {
                     primary: !0,
                     icon: "trash",
                     onClick: () => i(!1),
                     id: "hide-" + n,
                     display: r.value ? "inline" : "none"
                 })]
             })
@@ -1832,15 +1832,15 @@
         const c = {
             margin: 0
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
                 style: c,
-                "data-label": w(e.data.label),
+                "data-label": C(e.data.label),
                 children: e.data.label
             }), d(), o()]
         })
     }
     return s()
 }
 
@@ -1860,78 +1860,78 @@
                 data: l
             }), t.jsxs("div", {
                 style: {
                     textAlign: "center",
                     marginTop: 10,
                     marginBottom: 10
                 },
-                children: [t.jsx(B, {
+                children: [t.jsx(A, {
                     primary: !0,
                     icon: "plus",
                     onClick: () => i(),
                     id: "extra-add-" + x + "-",
                     display: m
-                }), t.jsx(B, {
+                }), t.jsx(A, {
                     primary: !0,
                     icon: "trash",
                     onClick: () => o(x),
                     display: "inline"
                 })]
             })]
         }, Math.random())
     }
 
     function d() {
         const l = s(),
             m = l.length > 0 ? "none" : "inline";
         document.getElementById("add-" + a).style.display = m;
         for (var x = 0; x < n; x++) {
-            var v = document.getElementById("extra-add-" + x + "-");
-            v.style.display = "none"
+            var w = document.getElementById("extra-add-" + x + "-");
+            w.style.display = "none"
         }
         if (l.length > 0) {
-            var v = document.getElementById("extra-add-" + l[l.length - 1] + "-");
-            v.style.display = "inline"
+            var w = document.getElementById("extra-add-" + l[l.length - 1] + "-");
+            w.style.display = "inline"
         }
     }
 
     function i() {
         d();
         var l = JSON.parse(JSON.stringify(e.data.template));
         l.fields ? (l.fields.map(function(m) {
             m.name = m.name.replace("__n__", "__" + n + "__")
         }), l.fields[0].value = 0) : l.fieldsets.map(function(m) {
             m.fields.map(function(x) {
-                x.map(function(v) {
-                    v.name = v.name.replace("__n__", "__" + n + "__")
+                x.map(function(w) {
+                    w.name = w.name.replace("__n__", "__" + n + "__")
                 }), x[0].value = 0
             })
-        }), W.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(l, "inline")), setTimeout(d, 100)
+        }), P.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(l, "inline")), setTimeout(d, 100)
     }
 
     function o(l) {
         const m = e.data.template,
-            v = (m.fields ? m.fields[0] : m.fieldsets[0].fields[0][0]).name.replace("__n__", "__" + l + "__"),
-            j = document.querySelector("input[name=" + v + "]");
-        parseInt(j.value) == 0 ? j.value = "" : j.value = -parseInt(j.value), document.getElementById("form-" + l + "-" + a).style.display = "none", d()
+            w = (m.fields ? m.fields[0] : m.fieldsets[0].fields[0][0]).name.replace("__n__", "__" + l + "__"),
+            S = document.querySelector("input[name=" + w + "]");
+        parseInt(S.value) == 0 ? S.value = "" : S.value = -parseInt(S.value), document.getElementById("form-" + l + "-" + a).style.display = "none", d()
     }
 
     function s() {
         for (var l = [], m = 0; m < n; m++) document.getElementById("form-" + m + "-" + a).style.display == "block" && l.push(m);
         return l
     }
 
     function c() {
         return t.jsx("div", {
             id: "info-" + a,
             children: t.jsx(le, {
                 data: {
                     text: 'Clique no botão com o ícone de "+" para adicionar e com o ícone da "lixeira" para remover.'
                 },
-                children: t.jsx(B, {
+                children: t.jsx(A, {
                     primary: !0,
                     icon: "add",
                     onClick: () => i(),
                     id: "add-" + a,
                     display: e.data.value.length > 0 ? "none" : "inline"
                 })
             })
@@ -1942,15 +1942,15 @@
         const l = {
             margin: 0
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
                 style: l,
-                "data-label": w(e.data.label),
+                "data-label": C(e.data.label),
                 children: e.data.label
             }), t.jsx("div", {
                 children: !1
             }), t.jsxs("div", {
                 id: a,
                 className: "fieldset-inline-forms",
                 children: [c(), e.data.value.map(function(m, x) {
@@ -1977,15 +1977,15 @@
         return e.data.fields ? t.jsx("div", {
             className: "form-fields",
             children: e.data.fields.map(r => n(r))
         }) : e.data.fieldsets.map(r => t.jsx("div", {
             className: "form-fieldset",
             children: r.type == "inline" ? n(r) : t.jsxs(t.Fragment, {
                 children: [t.jsx("h2", {
-                    "data-label": w(r.title),
+                    "data-label": C(r.title),
                     style: {
                         margin: 0
                     },
                     children: r.title
                 }), t.jsx("div", {
                     className: "fieldset-fields",
                     children: r.fields.map(d => t.jsx("div", {
@@ -2024,15 +2024,15 @@
                 text: e.data.info
             }
         })
     }
 
     function d() {
         if (e.data.display) return t.jsxs(t.Fragment, {
-            children: [e.data.display.map(l => t.jsx(y, {
+            children: [e.data.display.map(l => t.jsx(p, {
                 data: l
             }, Math.random())), t.jsx("div", {
                 style: {
                     marginTop: 30
                 }
             })]
         })
@@ -2046,20 +2046,20 @@
 
     function o() {
         return t.jsxs("div", {
             style: {
                 marginTop: 20,
                 textAlign: "right"
             },
-            children: [t.jsx(B, {
+            children: [t.jsx(A, {
                 onClick: c,
                 label: "Cancelar",
                 default: !0,
                 display: "inline"
-            }), t.jsx(B, {
+            }), t.jsx(A, {
                 onClick: u,
                 label: "Enviar",
                 primary: !0,
                 display: "inline",
                 icon: "chevron-right",
                 spin: !0
             })]
@@ -2090,24 +2090,24 @@
         V()
     }
 
     function u(l) {
         l.preventDefault();
         var m = document.getElementById(n),
             x = new FormData(m);
-        E("POST", e.data.url, function(j) {
-            if (l.target.dataset.spinning && (l.target.querySelector("i.fa-spin").style.display = "none", l.target.querySelector("i.fa-" + l.target.dataset.spinning).style.display = "inline-block"), j.type == "response") return V(), Ye(), ye(j);
-            var I = j.text;
-            console.log(j), Object.keys(j.errors).map(function(M) {
-                if (M == "__all__") I = j.errors[M];
+        I("POST", e.data.url, function(S) {
+            if (l.target.dataset.spinning && (l.target.querySelector("i.fa-spin").style.display = "none", l.target.querySelector("i.fa-" + l.target.dataset.spinning).style.display = "inline-block"), S.type == "response") return V(), Ye(), ye(S);
+            var B = S.text;
+            console.log(S), Object.keys(S.errors).map(function(y) {
+                if (y == "__all__") B = S.errors[y];
                 else {
-                    const q = m.querySelector("#" + M + "_error");
-                    q.querySelector("span").innerHTML = j.errors[M], q.style.display = "block"
+                    const j = m.querySelector("#" + y + "_error");
+                    j.querySelector("span").innerHTML = S.errors[y], j.style.display = "block"
                 }
-            }), ee(I, !0)
+            }), ee(B, !0)
         }, x)
     }
     return s()
 }
 
 function ct(e) {
     function n() {
@@ -2130,27 +2130,27 @@
         })
     }
     return n()
 }
 
 function ut(e) {
     e.data.id == null && (e.data.id = Math.random());
-    const [n, a] = C.useState(e.data);
+    const [n, a] = M.useState(e.data);
 
     function r() {
         const h = {
             margin: 0
         };
         return n.attrname ? t.jsx("h2", {
             style: h,
-            "data-label": w(n.title),
+            "data-label": C(n.title),
             children: n.title
         }) : t.jsx("h1", {
             style: h,
-            "data-label": w(n.title),
+            "data-label": C(n.title),
             children: n.title
         })
     }
 
     function d() {
         const h = {
             display: "flex",
@@ -2180,59 +2180,59 @@
                 width: "100%",
                 margin: "auto",
                 paddingBottom: 20,
                 lineHeight: "2.5rem"
             },
             children: n.subsets.map(function(h, f) {
                 var g = n.subset === h.name || !n.subset && f == 0;
-                return t.jsxs(P, {
+                return t.jsxs(W, {
                     href: "#",
                     style: {
                         paddingBottom: 5,
                         paddingLeft: 15,
                         paddingRight: 15,
                         fontWeight: g ? "bold" : "normal",
                         borderBottom: g ? "solid 3px #2670e8" : 0,
                         textDecoration: "none",
                         color: "#0c326f"
                     },
-                    onClick: function(p) {
-                        p.preventDefault(), s(h.name)
+                    onClick: function(b) {
+                        b.preventDefault(), s(h.name)
                     },
-                    dataLabel: w(h.label),
+                    dataLabel: C(h.label),
                     children: [h.label, " ", t.jsx(ct, {
                         total: h.count
                     })]
                 }, Math.random())
             })
         })
     }
 
     function s(h) {
         const f = document.getElementById("subset-" + e.data.id);
-        f.value = h || "", S()
+        f.value = h || "", v()
     }
 
     function c(h, f, g) {
-        const p = document.getElementById("form-" + e.data.id);
-        p.querySelector("input[name=" + n.calendar.field + "__day]").value = h || "", p.querySelector("input[name=" + n.calendar.field + "__month]").value = f || "", p.querySelector("input[name=" + n.calendar.field + "__year]").value = g || "", S()
+        const b = document.getElementById("form-" + e.data.id);
+        b.querySelector("input[name=" + n.calendar.field + "__day]").value = h || "", b.querySelector("input[name=" + n.calendar.field + "__month]").value = f || "", b.querySelector("input[name=" + n.calendar.field + "__year]").value = g || "", v()
     }
 
     function u() {
         if (n.calendar) {
-            const k = ["SEG", "TER", "QUA", "QUI", "SEX", "SAB", "DOM"],
+            const T = ["SEG", "TER", "QUA", "QUI", "SEX", "SAB", "DOM"],
                 R = ["JANEIRO", "FEVEVEIRO", "MARÇO", "ABRIL", "MAIO", "JUNHO", "JULHO", "AGOSTO", "SETEMRO", "OUTUBRO", "NOVEMBRO", "DEZEMBRO"],
                 ne = {
                     width: "100%",
                     borderSpacing: 0,
                     borderCollapse: "collapse",
                     marginTop: 15,
                     marginBottom: 15
                 },
-                T = {
+                E = {
                     marginLeft: "17",
                     textAlign: "right",
                     paddingRight: 2,
                     paddingTop: 2,
                     float: "right",
                     fontSize: "0.8rem"
                 },
@@ -2249,15 +2249,15 @@
                     display: "block",
                     width: 30,
                     height: 30,
                     margin: "auto",
                     cursor: "pointer",
                     lineHeight: "2rem"
                 },
-                O = {
+                _ = {
                     padding: 10,
                     textAlign: "center"
                 },
                 Q = {
                     display: "flex",
                     justifyContent: "space-between",
                     alignItems: "baseline"
@@ -2268,16 +2268,16 @@
                     [],
                     [],
                     [],
                     [],
                     [],
                     []
                 ], f = n.calendar.month - 1, g = new Date(n.calendar.year, n.calendar.month - 1, 1); g.getDay() > 1;) g.setDate(g.getDate() - 1);
-            for (var p = 0;
-                (g.getMonth() <= f || h[p].length < 7) && (h[p].length == 7 && (p += 1), p != 5);) h[p].push({
+            for (var b = 0;
+                (g.getMonth() <= f || h[b].length < 7) && (h[b].length == 7 && (b += 1), b != 5);) h[b].push({
                 date: g.getDate(),
                 total: n.calendar.total[g.toLocaleDateString("pt-BR")],
                 today: g.getDate() === Ee.getDate(),
                 selected: ce ? g.getDate() == ce.getDate() : !1
             }), g.setDate(g.getDate() + 1);
             return t.jsxs("div", {
                 className: "calendar",
@@ -2294,16 +2294,16 @@
                             align: "center",
                             style: {
                                 margin: 0
                             },
                             children: [R[n.calendar.month - 1], " ", n.calendar.year]
                         }), n.calendar.day && t.jsxs("div", {
                             align: "center",
-                            className: T,
-                            children: [new Date(n.calendar.year, n.calendar.month - 1, n.calendar.day).toLocaleDateString("pt-BR"), t.jsx(b, {
+                            className: E,
+                            children: [new Date(n.calendar.year, n.calendar.month - 1, n.calendar.day).toLocaleDateString("pt-BR"), t.jsx(k, {
                                 default: !0,
                                 icon: "x",
                                 onClick: () => c(null, n.calendar.month, n.calendar.year),
                                 style: {
                                     marginLeft: 10,
                                     cursor: "pointer"
                                 }
@@ -2316,44 +2316,44 @@
                             onClick: () => c(null, n.calendar.next.month, n.calendar.next.year)
                         })
                     })]
                 }), t.jsxs("table", {
                     style: ne,
                     children: [t.jsx("thead", {
                         children: t.jsx("tr", {
-                            children: k.map(ae => t.jsx("th", {
+                            children: T.map(ae => t.jsx("th", {
                                 children: ae
                             }, Math.random()))
                         })
                     }), t.jsx("tbody", {
                         children: h.map(ae => t.jsx("tr", {
-                            children: ae.map(L => t.jsxs("td", {
+                            children: ae.map(O => t.jsxs("td", {
                                 style: z,
                                 children: [t.jsx("div", {
-                                    style: T,
-                                    children: L.today ? t.jsx("span", {
+                                    style: E,
+                                    children: O.today ? t.jsx("span", {
                                         style: {
                                             textDecoration: "underline"
                                         },
-                                        children: L.date
-                                    }) : L.date + L.today
-                                }), L.total && t.jsx("div", {
-                                    style: O,
-                                    onClick: () => c(L.date, n.calendar.month, n.calendar.year),
+                                        children: O.date
+                                    }) : O.date + O.today
+                                }), O.total && t.jsx("div", {
+                                    style: _,
+                                    onClick: () => c(O.date, n.calendar.month, n.calendar.year),
                                     children: t.jsx("div", {
                                         style: G,
                                         children: t.jsx("span", {
                                             style: {
-                                                textDecoration: L.selected ? "underline" : "normal"
+                                                textDecoration: O.selected ? "underline" : "normal"
                                             },
-                                            children: L.total
+                                            children: O.total
                                         })
                                     })
-                                }), !L.total && t.jsx("div", {
-                                    style: O,
+                                }), !O.total && t.jsx("div", {
+                                    style: _,
                                     children: " "
                                 })]
                             }, Math.random()))
                         }, Math.random()))
                     })]
                 })]
             })
@@ -2397,38 +2397,38 @@
                 children: h.title
             }, Math.random()), t.jsx("td", {
                 style: g,
                 children: t.jsx("div", {
                     style: {
                         verticalAlign: "center"
                     },
-                    children: h.actions.map(function(p) {
+                    children: h.actions.map(function(b) {
                         return t.jsx(N, {
-                            data: p,
+                            data: b,
                             default: !0,
                             compact: !0
                         }, Math.random())
                     })
                 })
             })]
         }, Math.random()) : t.jsxs("tr", {
-            children: [h.data.map(function(p) {
-                return p.label != "ID" && t.jsx("td", {
+            children: [h.data.map(function(b) {
+                return b.label != "ID" && t.jsx("td", {
                     style: f,
-                    children: U(p.value)
+                    children: U(b.value)
                 }, Math.random())
             }), t.jsx("td", {
                 style: g,
                 children: t.jsx("div", {
                     style: {
                         verticalAlign: "center"
                     },
-                    children: h.actions.map(function(p) {
+                    children: h.actions.map(function(b) {
                         return t.jsx(N, {
-                            data: p,
+                            data: b,
                             default: !0,
                             compact: !0
                         }, Math.random())
                     })
                 })
             })]
         }, Math.random())
@@ -2436,26 +2436,26 @@
 
     function x() {
         return n.data.length > 0 ? n.renderer ? t.jsx("div", {
             style: {
                 marginBottom: 15
             },
             children: n.data.map(function(h) {
-                return h.type = n.renderer, t.jsx(y, {
+                return h.type = n.renderer, t.jsx(p, {
                     data: h
                 }, Math.random())
             })
-        }) : v() : t.jsx(le, {
+        }) : w() : t.jsx(le, {
             data: {
                 text: "Nenhum registro encontrado."
             }
         })
     }
 
-    function v() {
+    function w() {
         const h = {
                 width: "100%",
                 overflowX: "auto"
             },
             f = {
                 width: "100%",
                 lineHeight: "2rem",
@@ -2472,56 +2472,56 @@
                         return m(g)
                     })
                 })]
             })
         })
     }
 
-    function j(h) {
+    function S(h) {
         const g = document.getElementById("form-" + e.data.id).querySelector("input[name=page]");
-        g.value = h, S()
+        g.value = h, v()
     }
 
-    function I() {
+    function B() {
         const h = document.getElementById("form-" + e.data.id);
         if (h) {
-            const k = h.querySelector("input[name=page]");
-            k && (k.value = n.pagination.page.current)
+            const T = h.querySelector("input[name=page]");
+            T && (T.value = n.pagination.page.current)
         }
         const f = {
                 display: "flex",
                 justifyContent: "space-between",
                 lineHeight: "4rem",
                 alignItems: "baseline"
             },
             g = {
                 display: "inline",
                 paddingRight: 10
             },
-            p = {
+            b = {
                 marginLeft: 10,
                 marginRight: 10,
                 height: "2.5rem",
                 paddingLeft: 5,
                 paddingRight: 5,
                 textAlign: "center"
             };
         return n.pagination.page.total > 1 && t.jsxs("div", {
             style: f,
             children: [t.jsxs("div", {
                 children: [t.jsxs("div", {
                     style: g,
                     children: ["Exibir", t.jsx("select", {
-                        style: p,
+                        style: b,
                         name: "page_size",
-                        onChange: () => j(1),
+                        onChange: () => S(1),
                         value: n.pagination.page.size,
-                        children: n.pagination.page.sizes.map(function(k) {
+                        children: n.pagination.page.sizes.map(function(T) {
                             return t.jsx("option", {
-                                children: k
+                                children: T
                             }, Math.random())
                         })
                     })]
                 }), t.jsx("div", {
                     style: g,
                     children: "|"
                 }), t.jsxs("div", {
@@ -2540,37 +2540,37 @@
                         style: {
                             width: 30,
                             marginLeft: 10,
                             marginRight: 10,
                             height: "2rem",
                             textAlign: "center"
                         },
-                        onKeyDown: function(k) {
-                            k.key == "Enter" && (k.preventDefault(), j(k.target.value < 0 ? 1 : Math.min(k.target.value, n.pagination.page.total)))
+                        onKeyDown: function(T) {
+                            T.key == "Enter" && (T.preventDefault(), S(T.target.value < 0 ? 1 : Math.min(T.target.value, n.pagination.page.total)))
                         }
                     }), t.jsx("div", {
                         style: g,
                         children: "|"
-                    }), n.pagination.page.previous && t.jsx(B, {
+                    }), n.pagination.page.previous && t.jsx(A, {
                         icon: "chevron-left",
                         default: !0,
                         display: "inline",
-                        onClick: () => j(n.pagination.page.previous)
-                    }), n.pagination.page.next && t.jsx(B, {
+                        onClick: () => S(n.pagination.page.previous)
+                    }), n.pagination.page.next && t.jsx(A, {
                         icon: "chevron-right",
                         default: !0,
                         display: "inline",
-                        onClick: () => j(n.pagination.page.next)
+                        onClick: () => S(n.pagination.page.next)
                     })]
                 })
             })]
         })
     }
 
-    function M() {
+    function y() {
         return t.jsx("div", {
             align: "right",
             style: {
                 marginTop: 20,
                 marginBottom: 20
             },
             children: n.actions.map(function(h) {
@@ -2578,95 +2578,95 @@
                     data: h,
                     primary: !0
                 }, Math.random())
             })
         })
     }
 
-    function q() {
+    function j() {
         const h = {
                 backgroundColor: "#f8f8f8",
                 borderBottom: "solid 1px #DDD",
                 marginBottom: 10,
                 padding: 10
             },
             f = n.search.length > 0,
             g = n.filters.length > 0;
         if ((n.bi || n.data.length > 0) && (f || g)) {
-            const p = {
+            const b = {
                 name: "q",
                 value: "",
                 mask: null,
                 type: "text",
                 label: "Palavras-chaves"
             };
             return t.jsxs("div", {
                 style: h,
                 children: [t.jsxs($, {
                     width: 250,
                     children: [f && t.jsx("div", {
                         children: t.jsx(K, {
-                            data: p
+                            data: b
                         })
-                    }), g && n.filters.map(function(k) {
-                        return k.type != "hidden" && t.jsx("div", {
+                    }), g && n.filters.map(function(T) {
+                        return T.type != "hidden" && t.jsx("div", {
                             children: t.jsx(K, {
-                                data: k
+                                data: T
                             })
                         }, Math.random())
                     }), t.jsx("div", {
-                        children: t.jsx(B, {
-                            onClick: S,
+                        children: t.jsx(A, {
+                            onClick: v,
                             label: "Filtrar",
                             icon: "filter",
                             primary: !0
                         })
                     })]
-                }), g && n.filters.map(function(k) {
-                    return k.type == "hidden" && t.jsx("div", {
+                }), g && n.filters.map(function(T) {
+                    return T.type == "hidden" && t.jsx("div", {
                         children: t.jsx(K, {
-                            data: k
+                            data: T
                         })
                     }, Math.random())
                 })]
             })
         }
     }
 
-    function S() {
+    function v() {
         i(!0);
         var h;
         const f = new URLSearchParams(new FormData(document.getElementById("form-" + e.data.id))).toString();
-        e.data.url.indexOf("?") > 0 ? h = e.data.url + "&" + f : h = e.data.url + "?" + f, E("GET", h, function(g) {
+        e.data.url.indexOf("?") > 0 ? h = e.data.url + "&" + f : h = e.data.url + "?" + f, I("GET", h, function(g) {
             a(g), i(!1)
         })
     }
 
-    function F() {
+    function L() {
         return n.bi ? t.jsxs(t.Fragment, {
-            children: [q(), n.bi.map(function(h) {
+            children: [j(), n.bi.map(function(h) {
                 return t.jsx($, {
                     width: 300,
                     alignItems: "start",
                     children: h.map(function(f) {
                         return t.jsx("div", {
-                            children: t.jsx(y, {
+                            children: t.jsx(p, {
                                 data: f
                             })
                         }, Math.random())
                     })
                 }, Math.random())
             })]
         }) : t.jsxs(t.Fragment, {
-            children: [M(), o(), q(), u(), x(), I()]
+            children: [y(), o(), j(), u(), x(), B()]
         })
     }
 
     function D() {
-        window[e.data.id] = () => S();
+        window[e.data.id] = () => v();
         const h = {
             backgroundColor: "white",
             padding: 20
         };
         return t.jsx("div", {
             className: "reloadable",
             id: e.data.id,
@@ -2675,15 +2675,15 @@
                 id: "form-" + e.data.id,
                 children: [t.jsx("div", {
                     children: !1
                 }), t.jsx("input", {
                     type: "hidden",
                     name: "subset",
                     id: "subset-" + e.data.id
-                }), d(), F()]
+                }), d(), L()]
             })
         })
     }
     return D()
 }
 
 function te(e) {
@@ -2798,15 +2798,15 @@
     return t.jsx(de, {
         area: !0,
         headers: e.headers,
         rows: e.rows
     })
 }
 
-function _(e) {
+function F(e) {
     var n = e.invert || !1,
         a = e.type || "bar",
         r = e.stack,
         d = {
             type: "value"
         },
         i = {
@@ -2881,55 +2881,55 @@
             option: l
         })
     }
     return u()
 }
 
 function ft(e) {
-    return t.jsx(_, {
+    return t.jsx(F, {
         headers: e.headers,
         rows: e.rows
     })
 }
 
 function gt(e) {
-    return t.jsx(_, {
+    return t.jsx(F, {
         type: "line",
         headers: e.headers,
         rows: e.rows
     })
 }
 
 function xt(e) {
-    return t.jsx(_, {
+    return t.jsx(F, {
         area: !0,
         type: "line",
         headers: e.headers,
         rows: e.rows
     })
 }
 
 function yt(e) {
-    return t.jsx(_, {
+    return t.jsx(F, {
         stack: "1",
         headers: e.headers,
         rows: e.rows
     })
 }
 
 function pt(e) {
-    return t.jsx(_, {
+    return t.jsx(F, {
         invert: !0,
         headers: e.headers,
         rows: e.rows
     })
 }
 
 function vt(e) {
-    return t.jsx(_, {
+    return t.jsx(F, {
         invert: !0,
         stack: "1",
         headers: e.headers,
         rows: e.rows
     })
 }
 
@@ -3089,15 +3089,15 @@
                 });
             case "progress":
                 return t.jsx(wt, {
                     headers: e.headers,
                     rows: e.rows
                 });
             default:
-                return t.jsx(_, {
+                return t.jsx(F, {
                     headers: e.headers,
                     rows: e.rows
                 })
         }
     }
 
     function a() {
@@ -3121,15 +3121,15 @@
         return e.data.chart ? t.jsx(fe, {
             type: e.data.chart,
             title: e.data.title,
             rows: r
         }) : t.jsxs("div", {
             className: "statistics",
             children: [e.data.title && t.jsx("h2", {
-                "data-label": w(e.data.title),
+                "data-label": C(e.data.title),
                 children: e.data.title
             }), t.jsx("table", {
                 style: {
                     width: "100%"
                 },
                 children: t.jsx("tbody", {
                     children: r.map(i => t.jsx("tr", {
@@ -3161,36 +3161,36 @@
             type: e.data.chart,
             title: e.data.title,
             headers: r,
             rows: d
         }) : t.jsxs("div", {
             className: "statistics",
             children: [e.data.title && t.jsx("h2", {
-                "data-label": w(e.data.title),
+                "data-label": C(e.data.title),
                 children: e.data.title
             }), t.jsxs("table", {
                 style: {
                     width: "100%"
                 },
                 children: [r && t.jsx("thead", {
                     children: t.jsx("tr", {
                         children: r.map(x => t.jsx("th", {
                             children: x
                         }, Math.random()))
                     })
                 }), t.jsxs("tbody", {
                     children: [d.map(x => t.jsx("tr", {
-                        children: x.map((v, j) => j == 0 ? t.jsx("th", {
-                            children: v
+                        children: x.map((w, S) => S == 0 ? t.jsx("th", {
+                            children: w
                         }, Math.random()) : t.jsx("td", {
                             align: "center",
                             style: {
-                                backgroundColor: j == x.length - 1 && r && r[r.length - 1] == "TOTAL" ? "var(--info-color)" : "inherite"
+                                backgroundColor: S == x.length - 1 && r && r[r.length - 1] == "TOTAL" ? "var(--info-color)" : "inherite"
                             },
-                            children: U(v)
+                            children: U(w)
                         }, Math.random()))
                     }, Math.random())), o.length > 0 && t.jsxs("tr", {
                         children: [t.jsx("th", {
                             children: "TOTAL"
                         }), o.map(x => t.jsxs("td", {
                             align: "center",
                             style: {
@@ -3201,15 +3201,15 @@
                     }, Math.random())]
                 })]
             })]
         })
     }
     return Array.isArray(e.data.series) ? n() : a()
 }
-const Me = {
+const Te = {
     primary: "#1351b4",
     success: "green",
     warning: "orange",
     info: "blue",
     danger: "red"
 };
 
@@ -3240,15 +3240,15 @@
             align: "center",
             children: [window.application.menu.image && t.jsx("div", {
                 children: t.jsx("img", {
                     src: window.application.menu.image,
                     style: i
                 })
             }), t.jsx("div", {
-                children: t.jsx(P, {
+                children: t.jsx(W, {
                     dataLabel: "Editar Perfil",
                     href: "/api/editprofile/",
                     style: {
                         textDecoration: "none"
                     },
                     children: window.application.menu.user
                 })
@@ -3287,33 +3287,33 @@
             c = {
                 padding: 5,
                 fontSize: "1.2rem"
             };
         return i.url ? t.jsx("li", {
             style: s,
             onClick: n,
-            children: t.jsxs(P, {
+            children: t.jsxs(W, {
                 href: i.url,
-                dataLabel: w(i.label),
+                dataLabel: C(i.label),
                 style: {
                     textDecoration: "none"
                 },
-                children: [o == 0 && t.jsx(b, {
+                children: [o == 0 && t.jsx(k, {
                     icon: i.icon || "dot-circle",
                     style: c
                 }), i.label]
             })
         }, Math.random()) : i.items.length > 0 && t.jsxs("li", {
             onClick: n,
             style: s,
-            "data-label": w(i.label),
-            children: [o == 0 && t.jsx(b, {
+            "data-label": C(i.label),
+            children: [o == 0 && t.jsx(k, {
                 icon: i.icon || "dot-circle",
                 style: c
-            }), i.label, t.jsx(b, {
+            }), i.label, t.jsx(k, {
                 icon: "chevron-right",
                 style: {
                     float: "right",
                     paddingTop: 8
                 }
             }), t.jsx("ul", {
                 style: {
@@ -3372,15 +3372,15 @@
                 i.pushManager.subscribe({
                     userVisibleOnly: !0,
                     applicationServerKey: o
                 }).then(function(s) {
                     if (console.log(s), n = JSON.stringify(s), console.log(n), s) {
                         alert("Notificação ativada com sucesso.");
                         var c = new FormData;
-                        c.append("subscription", n), E("POST", "/api/pushsubscribe/", function(u) {
+                        c.append("subscription", n), I("POST", "/api/pushsubscribe/", function(u) {
                             console.log(u)
                         }, c)
                     } else {
                         alert("Problema ao ativar notificações.");
                         return
                     }
                 }).catch(function(s) {
@@ -3389,26 +3389,26 @@
             } else console.log("No registered service worker.")
         }).catch(function(i) {
             alert("Erro"), console.error("Service Worker Error", i)
         }) : alert("Push messaging is not supported")
     }
 
     function d() {
-        return t.jsx(b, {
+        return t.jsx(k, {
             onClick: r,
             icon: "bell",
             style: {
                 cursor: "pointer"
             }
         })
     }
     return d()
 }
 
-function Mt(e) {
+function Tt(e) {
     function n() {
         if (window.innerWidth > 800) return;
         const a = {
                 position: "fixed",
                 display: "flex",
                 width: 50,
                 height: 50,
@@ -3426,56 +3426,56 @@
         return t.jsxs(t.Fragment, {
             children: [t.jsx("div", {
                 style: {
                     ...a,
                     bottom: 80
                 },
                 onClick: () => history.back(),
-                children: t.jsx(b, {
+                children: t.jsx(k, {
                     icon: "arrow-left",
                     style: r
                 })
             }), t.jsx("div", {
                 style: {
                     ...a,
                     bottom: 20
                 },
                 onClick: () => window.scrollTo(0, 0),
-                children: t.jsx(b, {
+                children: t.jsx(k, {
                     icon: "arrow-up",
                     style: r
                 })
             })]
         })
     }
     return n()
 }
 
-function Tt(e) {
-    const [n, a] = C.useState(e.data);
+function Mt(e) {
+    const [n, a] = M.useState(e.data);
     window.loaddata = d => a(d);
 
     function r() {
         const d = {
             minHeight: 400,
             margin: 20
         };
         return t.jsx("div", {
             style: d,
             id: "container",
-            children: t.jsx(y, {
+            children: t.jsx(p, {
                 data: n
             }, Math.random())
         })
     }
     return r()
 }
 
 function Et(e) {
-    C.useEffect(() => {
+    M.useEffect(() => {
         const l = localStorage.getItem("message");
         l && (localStorage.removeItem("message"), ee(l)), window.addEventListener("resize", () => {
             const m = document.querySelector("aside");
             m.style.display = window.innerWidth < 800 ? "none" : "block"
         })
     }, []);
 
@@ -3507,15 +3507,15 @@
             };
         return e.data.navbar ? t.jsxs("div", {
             style: l,
             children: [t.jsxs("div", {
                 style: {
                     padding: 20
                 },
-                children: [t.jsx(b, {
+                children: [t.jsx(k, {
                     icon: "navicon",
                     style: {
                         fontSize: "1.5rem",
                         marginRight: 10,
                         cursor: "pointer"
                     },
                     onClick: a
@@ -3540,15 +3540,15 @@
                     style: {
                         padding: 10
                     },
                     children: t.jsx(X, {
                         actions: e.data.navbar.adder,
                         position: {},
                         dataLabel: "plus",
-                        children: t.jsx(b, {
+                        children: t.jsx(k, {
                             icon: "plus"
                         })
                     })
                 }), t.jsx("div", {
                     style: {
                         padding: 10
                     },
@@ -3557,27 +3557,27 @@
                     style: {
                         padding: 10
                     },
                     children: t.jsx(X, {
                         actions: e.data.navbar.tools,
                         position: {},
                         dataLabel: "tools",
-                        children: t.jsx(b, {
+                        children: t.jsx(k, {
                             icon: "tools"
                         })
                     })
                 }), e.data.navbar.settings.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
                     children: t.jsx(X, {
                         actions: e.data.navbar.settings,
                         position: {},
                         dataLabel: "gear",
-                        children: t.jsx(b, {
+                        children: t.jsx(k, {
                             icon: "gear"
                         })
                     })
                 }), window.innerWidth > 800 && t.jsx(Ce, {
                     data: m,
                     style: {
                         padding: 10
@@ -3586,15 +3586,15 @@
                 }), e.data.navbar.usermenu.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
                     children: t.jsx(X, {
                         actions: e.data.navbar.usermenu,
                         position: {},
-                        dataLabel: w(e.data.navbar.user),
+                        dataLabel: C(e.data.navbar.user),
                         children: e.data.navbar.user
                     })
                 })]
             })]
         }) : null
     }
 
@@ -3615,32 +3615,32 @@
                 margin: 15
             },
             m = {
                 color: "#1351b4"
             };
         return e.data.navbar && t.jsxs("div", {
             style: l,
-            children: [t.jsx(b, {
+            children: [t.jsx(k, {
                 icon: "home",
                 style: m
             }), " Área Administrativa"]
         })
     }
 
     function s() {
         return t.jsxs("main", {
             style: {
                 flexGrow: 6,
                 minWidth: "400px"
             },
-            children: [o(), t.jsx(Tt, {
+            children: [o(), t.jsx(Mt, {
                 data: e.data.content
             }), t.jsx("footer", {
                 children: c()
-            }), t.jsx(Mt, {})]
+            }), t.jsx(Tt, {})]
         })
     }
 
     function c() {
         return e.data.footer ? t.jsxs("div", {
             align: "center",
             children: [t.jsx("div", {
@@ -3667,14 +3667,209 @@
             })]
         })
     }
     return u()
 }
 
 function It(e) {
+    var n = null,
+        a = null,
+        r = null,
+        d = navigator.getUserMedia || navigator.webkitGetUserMedia || navigator.mozGetUserMedia,
+        i = {
+            constraints: {
+                mandatory: {
+                    OfferToReceiveAudio: !0,
+                    OfferToReceiveVideo: !0
+                },
+                offerToReceiveAudio: 1,
+                offerToReceiveVideo: 1
+            },
+            sdpTransform: y => y.replace("a=fmtp:111 minptime=10;useinbandfec=1", "a=fmtp:111 ptime=5;useinbandfec=1;stereo=1;maxplaybackrate=48000;maxaveragebitrat=128000;sprop-stereo=1")
+        };
+    M.useEffect(() => {
+        n = new Peer("123456" + e.data.caller.replaceAll(".", "")), n.on("open", function(y) {
+            document.getElementById("callerid").innerHTML = e.data.caller
+        }), n.on("call", function(y) {
+            d({
+                video: {
+                    width: {
+                        exact: 320
+                    },
+                    height: {
+                        exact: 240
+                    }
+                },
+                audio: !0
+            }, function(j) {
+                a = j;
+                var v = document.getElementById("video2");
+                v.addEventListener("loadedmetadata", function(L) {
+                    v.style.width = this.videoWidth / 4 + "px", v.style.height = this.videoHeight / 4 + "px", v.style.marginLeft = -this.videoWidth / 4 + "px", v.style.visibility = "visible"
+                }, !1), v.srcObject = a, y.answer(j), y.on("stream", function(L) {
+                    r = L, document.getElementById("video1").srcObject = r
+                }), y.on("close", function() {
+                    c()
+                }), n.on("error", function(L) {
+                    c()
+                })
+            }, function(j) {
+                console.log("Failed to get local stream", j)
+            })
+        }), n.on("error", function(y) {
+            y.type == "browser-incompatible" ? alert("Navegador incompatível.") : y.type == "invalid-id" ? alert("Usuário inexistente.") : y.type == "network" ? alert("Problema na conexão do usuário.") : y.type == "peer-unavailable" && alert("Usuário indisponível.")
+        })
+    }, []);
+
+    function o() {
+        l(a, "audio"), l(a, "video"), l(r, "audio"), l(r, "video")
+    }
+
+    function s() {
+        m(a, "audio"), m(a, "video"), m(r, "audio"), m(r, "video")
+    }
+
+    function c() {
+        u(a, "audio"), u(a, "video"), u(r, "audio"), u(r, "video"), a = null, r = null, document.getElementById("video1").srcObject = null, document.getElementById("video2").srcObject = null, console.log("Stopped!")
+    }
+
+    function u(y, j) {
+        y != null && y.getTracks().forEach(v => {
+            v.readyState == "live" && v.kind === j && v.stop()
+        })
+    }
+
+    function l(y, j) {
+        y != null && y.getTracks().forEach(v => {
+            v.readyState == "live" && v.kind === j && (v.enabled = !1)
+        })
+    }
+
+    function m(y, j) {
+        y != null && y.getTracks().forEach(v => {
+            v.readyState == "live" && v.kind === j && (v.enabled = !0)
+        })
+    }
+
+    function x() {
+        var y = document.getElementById("video1");
+        y.style.width == "" ? y.style.width = "400px" : y.style.width = ""
+    }
+
+    function w() {
+        var y = n.call("123456" + e.data.receiver.replaceAll(".", ""), a, i);
+        y.on("stream", function(j) {
+            r = j, document.getElementById("video1").srcObject = r
+        }), y.on("close", function() {
+            c()
+        }), n.on("error", function(j) {
+            c()
+        })
+    }
+
+    function S() {
+        if (a != null && r == null) return w();
+        if (a != null && r != null) return s();
+        d({
+            video: {
+                width: {
+                    exact: 320
+                },
+                height: {
+                    exact: 240
+                }
+            },
+            audio: {
+                autoGainControl: !1,
+                channelCount: 2,
+                echoCancellation: !1,
+                latency: 0,
+                noiseSuppression: !1,
+                sampleRate: 48e3,
+                sampleSize: 16,
+                volume: 1
+            }
+        }, function(y) {
+            a = y;
+            var j = document.getElementById("video2");
+            j.addEventListener("loadedmetadata", function(v) {
+                j.style.width = this.videoWidth / 4 + "px", j.style.height = this.videoHeight / 4 + "px", j.style.marginLeft = -this.videoWidth / 4 + "px", j.style.visibility = "visible"
+            }, !1), j.srcObject = a, w()
+        }, function(y) {
+            alert("Failed to get local stream.")
+        })
+    }
+
+    function B() {
+        var y = {
+                width: "fit-content",
+                margin: "auto"
+            },
+            j = {
+                position: "absolute",
+                color: "white",
+                padding: "5px"
+            },
+            v = {
+                color: "white",
+                backgroundColor: "black",
+                padding: 2
+            },
+            L = {
+                position: "absolute",
+                marginTop: "-30px"
+            },
+            D = {
+                backgroundColor: "black"
+            },
+            h = {
+                visibility: "hidden",
+                width: "0px"
+            };
+        return t.jsxs("div", {
+            style: y,
+            children: [t.jsx("div", {
+                id: "callerid",
+                style: j
+            }), t.jsx("video", {
+                id: "video1",
+                style: D,
+                playsInline: !0,
+                autoPlay: !0
+            }), t.jsx("video", {
+                id: "video2",
+                style: h,
+                playsInline: !0,
+                autoPlay: !0
+            }), t.jsxs("div", {
+                style: L,
+                children: [t.jsx(k, {
+                    style: v,
+                    onClick: S,
+                    icon: "play"
+                }), t.jsx(k, {
+                    style: v,
+                    onClick: o,
+                    icon: "pause"
+                }), t.jsx(k, {
+                    style: v,
+                    onClick: c,
+                    icon: "stop"
+                }), t.jsx(k, {
+                    style: v,
+                    onClick: x,
+                    icon: "maximize"
+                })]
+            })]
+        })
+    }
+    return B()
+}
+
+function Bt(e) {
     return t.jsx("img", {
         src: e.data.src,
         style: {
             width: "100%"
         }
     })
 }
@@ -3693,30 +3888,30 @@
                 height: e.data.height,
                 borderRadius: e.data.round ? "50%" : 0
             }
         })
     })
 }
 
-function Bt(e) {
+function Lt(e) {
     return t.jsx("iframe", {
         width: e.data.width || "100%",
         height: e.data.height || "400px",
         id: "gmap_canvas",
         src: "https://maps.google.com/maps?q=" + e.data.latitude + "," + e.data.longitude + "&t=&z=13&ie=UTF8&iwloc=&output=embed",
         frameBorder: "0",
         scrolling: "no",
         marginHeight: "0",
         marginWidth: "0"
     })
 }
 
-function qt(e) {
+function At(e) {
     function n(i) {
-        return e.data.icon ? i.done ? t.jsx(b, {
+        return e.data.icon ? i.done ? t.jsx(k, {
             style: {
                 marginTop: 6
             },
             icon: e.data.icon
         }) : t.jsx("span", {
             children: " "
         }) : t.jsx("div", {
@@ -3790,15 +3985,15 @@
                 })
             })
         })
     }
     return d()
 }
 
-function At(e) {
+function qt(e) {
     function n() {
         const a = {
                 display: "inline-block",
                 width: "100%",
                 backgroundColor: "#DDD",
                 borderRadius: 5,
                 marginTop: 5
@@ -3809,15 +4004,15 @@
             d = {
                 display: "block",
                 paddingTop: 2,
                 paddingBottom: 2,
                 color: "white",
                 borderRadius: 5,
                 width: e.data.value + "%",
-                backgroundColor: Me[e.data.style]
+                backgroundColor: Te[e.data.style]
             };
         return t.jsx("span", {
             style: a,
             children: t.jsx("span", {
                 style: d,
                 children: t.jsxs("span", {
                     style: r,
@@ -3825,24 +4020,24 @@
                 })
             })
         })
     }
     return n()
 }
 
-function Lt(e) {
+function Ot(e) {
     function n() {
-        return e.data.color = Me[e.data.style], t.jsx(Te, {
+        return e.data.color = Te[e.data.style], t.jsx(Me, {
             data: e.data
         })
     }
     return n()
 }
 
-function Te(e) {
+function Me(e) {
     function n() {
         const a = {
             color: "white",
             width: "fit-content",
             borderRadius: 5,
             textWrap: "nowrap",
             padding: 10,
@@ -3889,23 +4084,23 @@
                 textTransform: "uppercase",
                 height: 70,
                 color: "#0c326f"
             };
         return e.data.items.length ? t.jsxs("div", {
             style: a,
             children: [t.jsx("h2", {
-                "data-label": w(e.data.title),
+                "data-label": C(e.data.title),
                 children: e.data.title
             }), t.jsx("div", {
-                children: e.data.items.map(o => t.jsxs(P, {
+                children: e.data.items.map(o => t.jsxs(W, {
                     href: o.url,
                     style: r,
                     dataLabel: o.label,
                     children: [t.jsx("div", {
-                        children: t.jsx(b, {
+                        children: t.jsx(k, {
                             style: d,
                             icon: o.icon
                         })
                     }), t.jsx("div", {
                         style: i,
                         children: o.label
                     })]
@@ -3932,46 +4127,46 @@
                 children: a
             }, Math.random()))
         })
     }
     return n()
 }
 
-function Ot(e) {
+function _t(e) {
     function n() {
-        return e.data.url ? t.jsx(P, {
+        return e.data.url ? t.jsx(W, {
             href: e.data.url,
             imodal: !!e.data.modal,
-            children: e.data.icon ? t.jsx(b, {
+            children: e.data.icon ? t.jsx(k, {
                 icon: e.data.icon
             }) : e.data.url
         }) : t.jsx("span", {
             children: "-"
         })
     }
     return n()
 }
 
-function _t(e) {
+function Ft(e) {
     function n() {
         return t.jsx("iframe", {
             src: e.data.url,
             width: "100%",
             height: 500,
             style: {
                 border: 0
             }
         })
     }
     return n()
 }
 
-function Ft(e) {
+function zt(e) {
     const n = Math.random();
-    C.useEffect(() => {
+    M.useEffect(() => {
         new QRCode(document.getElementById(n), {
             text: e.data.text,
             width: 128,
             height: 128,
             colorDark: "#333333",
             colorLight: "#ffffff",
             correctLevel: QRCode.CorrectLevel.H
@@ -3982,29 +4177,29 @@
         return t.jsx("div", {
             id: n
         })
     }
     return a()
 }
 
-function zt(e) {
+function Ht(e) {
     function n() {
         return t.jsx($, {
             width: 400,
             children: e.data.items.map((a, r) => t.jsx("div", {
-                children: t.jsx(y, {
+                children: t.jsx(p, {
                     data: a
                 })
             }, Math.random()))
         })
     }
     return n()
 }
 
-function Ht(e) {
+function Wt(e) {
     function n() {
         return t.jsxs("div", {
             children: [t.jsx("h2", {
                 children: e.data.title
             }), t.jsx("div", {
                 style: {
                     fontSize: "12rem",
@@ -4017,83 +4212,84 @@
     }
     return n()
 }
 var Z, se = {};
 const Pt = "/api/application/",
     ge = localStorage.getItem("application");
 
-function y(e) {
+function p(e) {
     const n = se[e.data.type];
     return n ? Ie.createElement(n, {
         data: e.data
     }) : t.jsx("div", {
         children: JSON.stringify(e.data)
     })
 }
-y.register = function(e, n) {
+p.register = function(e, n) {
     se[n.toLowerCase()] = e
 };
-y.render = function(e) {
+p.render = function(e) {
     Z = e, document.location.pathname == "/" ? localStorage.getItem("token") ? window.reload("/app/dashboard/") : window.reload("/app/login/") : document.location.pathname == "/app/login/" && (localStorage.getItem("token") || localStorage.getItem("application")) ? (localStorage.removeItem("token"), localStorage.removeItem("application"), document.location.reload()) : window.reload(document.location.href)
 };
-y.register(Ht, "Counter");
-y.register(st, "Form");
-y.register(ut, "QuerySet");
-y.register(Pe, "Fieldset");
-y.register(J, "Field");
-y.register(Ue, "Object");
-y.register(Ve, "Section");
-y.register(Je, "Group");
-y.register(jt, "Statistics");
-y.register(Dt, "Image");
-y.register(It, "Banner");
-y.register(Bt, "Map");
-y.register(qt, "Steps");
-y.register(Ft, "QrCode");
-y.register(Te, "Badge");
-y.register(Lt, "Status");
-y.register(At, "Progress");
-y.register(kt, "Color");
-y.register(Rt, "Boxes");
-y.register(Nt, "Shell");
-y.register(Ot, "FileLink");
-y.register(_t, "FilePreview");
-y.register(Le, "Response");
-y.register(Et, "Application");
-y.register(De, "IconSet");
-y.register(zt, "Grid");
-y.register(ze, "Rows");
-y.register(He, "Timeline");
+p.register(Wt, "Counter");
+p.register(st, "Form");
+p.register(ut, "QuerySet");
+p.register(We, "Fieldset");
+p.register(J, "Field");
+p.register(Ue, "Object");
+p.register(Ve, "Section");
+p.register(Je, "Group");
+p.register(jt, "Statistics");
+p.register(Dt, "Image");
+p.register(Bt, "Banner");
+p.register(Lt, "Map");
+p.register(At, "Steps");
+p.register(zt, "QrCode");
+p.register(Me, "Badge");
+p.register(Ot, "Status");
+p.register(qt, "Progress");
+p.register(kt, "Color");
+p.register(Rt, "Boxes");
+p.register(Nt, "Shell");
+p.register(_t, "FileLink");
+p.register(Ft, "FilePreview");
+p.register(qe, "Response");
+p.register(Et, "Application");
+p.register(Be, "IconSet");
+p.register(Ht, "Grid");
+p.register(ze, "Rows");
+p.register(He, "Timeline");
+p.register(It, "WebConf");
 window.addEventListener("popstate", e => {
     window.reload(e.currentTarget.location.href)
 });
 window.reload = function(e) {
     const n = e.split("/app/")[1].split("/")[0];
-    se[n] ? E("GET", A(e), function(a) {
-        Z.render(t.jsx(y, {
+    se[n] ? I("GET", q(e), function(a) {
+        Z.render(t.jsx(p, {
             data: {
                 type: n,
                 data: a
             }
         }))
     }) : (e != document.location.href && window.history.pushState({
         url: e
-    }, "", e), ge ? (window.application = JSON.parse(ge), E("GET", A(e), function(a) {
-        window.application.content = a, Z.render(t.jsx(y, {
+    }, "", e), ge ? (window.application = JSON.parse(ge), I("GET", q(e), function(a) {
+        window.application.content = a, Z.render(t.jsx(p, {
             data: window.application
         }, Math.random()))
-    })) : E("GET", Pt, function(r) {
-        window.application = r, localStorage.setItem("application", JSON.stringify(window.application)), E("GET", A(e), function(d) {
-            window.application.content = d, Z.render(t.jsx(y, {
+    })) : I("GET", Pt, function(r) {
+        window.application = r, localStorage.setItem("application", JSON.stringify(window.application)), I("GET", q(e), function(d) {
+            window.application.content = d, Z.render(t.jsx(p, {
                 data: window.application
             }, Math.random()))
         })
     }))
 };
 window.load = function(e) {
     e.indexOf(window.origin) >= 0 || e.startsWith("/") ? (e != document.location.href && e != document.location.pathname && window.history.pushState({
         url: e
-    }, "", e), E("GET", A(e), function(n) {
+    }, "", e), I("GET", q(e), function(n) {
         window.loaddata(n)
     })) : document.location.href = e
 };
-y.render(W.createRoot(document.getElementById("root")));
+p.render(P.createRoot(document.getElementById("root")));
```

### Comparing `pyslth-0.2.5/slth/static/js/peerjs.min.js` & `pyslth-0.2.6/slth/static/js/peerjs.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/static/js/qrcode.min.js` & `pyslth-0.2.6/slth/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/static/js/react-trigger-change.js` & `pyslth-0.2.6/slth/static/js/react-trigger-change.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/static/js/react.min.js` & `pyslth-0.2.6/slth/static/js/react.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/static/js/vanilla-masker.js` & `pyslth-0.2.6/slth/static/js/vanilla-masker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/static/js/vanilla-masker.min.js` & `pyslth-0.2.6/slth/static/js/vanilla-masker.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/statistics.py` & `pyslth-0.2.6/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/templates/index.html` & `pyslth-0.2.6/slth/templates/index.html`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/templates/service-worker.js` & `pyslth-0.2.6/slth/templates/service-worker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/tests.py` & `pyslth-0.2.6/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/urls.py` & `pyslth-0.2.6/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/utils.py` & `pyslth-0.2.6/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.2.5/slth/views.py` & `pyslth-0.2.6/slth/views.py`

 * *Files identical despite different names*


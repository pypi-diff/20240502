# Comparing `tmp/pretix-venueless-1.3.0.tar.gz` & `tmp/pretix_venueless-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-venueless-1.3.0.tar", last modified: Tue Apr  4 17:23:03 2023, max compression
+gzip compressed data, was "pretix_venueless-1.3.1.tar", last modified: Thu May  2 14:20:35 2024, max compression
```

## Comparing `pretix-venueless-1.3.0.tar` & `pretix_venueless-1.3.1.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/
--rw-r--r--   0 raphael   (1000) raphael   (1000)      557 2022-02-19 19:28:00.000000 pretix-venueless-1.3.0/LICENSE
--rw-r--r--   0 raphael   (1000) raphael   (1000)      135 2022-02-19 19:28:00.000000 pretix-venueless-1.3.0/MANIFEST.in
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1152 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/PKG-INFO
--rw-r--r--   0 raphael   (1000) raphael   (1000)      901 2022-02-19 19:28:00.000000 pretix-venueless-1.3.0/README.rst
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/
--rw-r--r--   0 raphael   (1000) raphael   (1000)       22 2023-03-28 08:19:49.000000 pretix-venueless-1.3.0/pretix_venueless/__init__.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)      797 2023-03-28 08:19:49.000000 pretix-venueless-1.3.0/pretix_venueless/apps.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/locale/
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/locale/ar/
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/locale/ar/LC_MESSAGES/
--rw-r--r--   0 raphael   (1000) raphael   (1000)      321 2022-09-29 11:35:17.000000 pretix-venueless-1.3.0/pretix_venueless/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2299 2022-03-31 20:05:34.000000 pretix-venueless-1.3.0/pretix_venueless/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/locale/de/
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/locale/de/LC_MESSAGES/
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2053 2022-09-29 11:35:17.000000 pretix-venueless-1.3.0/pretix_venueless/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 raphael   (1000) raphael   (1000)     3071 2022-03-31 20:05:34.000000 pretix-venueless-1.3.0/pretix_venueless/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/locale/de_Informal/
--rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-02-19 19:28:00.000000 pretix-venueless-1.3.0/pretix_venueless/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/locale/de_Informal/LC_MESSAGES/
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2054 2022-09-29 11:35:17.000000 pretix-venueless-1.3.0/pretix_venueless/locale/de_Informal/LC_MESSAGES/django.mo
--rw-r--r--   0 raphael   (1000) raphael   (1000)     3065 2022-03-31 20:05:34.000000 pretix-venueless-1.3.0/pretix_venueless/locale/de_Informal/LC_MESSAGES/django.po
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2302 2022-03-31 20:05:34.000000 pretix-venueless-1.3.0/pretix_venueless/locale/django.pot
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/locale/fi/
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/locale/fi/LC_MESSAGES/
--rw-r--r--   0 raphael   (1000) raphael   (1000)      677 2022-09-29 11:35:17.000000 pretix-venueless-1.3.0/pretix_venueless/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2528 2022-09-29 09:20:55.000000 pretix-venueless-1.3.0/pretix_venueless/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/locale/hr/
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/locale/hr/LC_MESSAGES/
--rw-r--r--   0 raphael   (1000) raphael   (1000)      321 2023-01-30 14:36:13.000000 pretix-venueless-1.3.0/pretix_venueless/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2277 2023-01-30 14:35:40.000000 pretix-venueless-1.3.0/pretix_venueless/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/locale/ja/
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/locale/ja/LC_MESSAGES/
--rw-r--r--   0 raphael   (1000) raphael   (1000)      321 2022-09-29 11:35:17.000000 pretix-venueless-1.3.0/pretix_venueless/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2299 2022-03-31 20:05:34.000000 pretix-venueless-1.3.0/pretix_venueless/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/locale/nl/
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/locale/nl/LC_MESSAGES/
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2004 2022-09-29 11:35:17.000000 pretix-venueless-1.3.0/pretix_venueless/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 raphael   (1000) raphael   (1000)     3039 2022-03-31 20:05:34.000000 pretix-venueless-1.3.0/pretix_venueless/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/locale/nl_Informal/
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/locale/nl_Informal/LC_MESSAGES/
--rw-r--r--   0 raphael   (1000) raphael   (1000)      330 2022-09-29 11:35:17.000000 pretix-venueless-1.3.0/pretix_venueless/locale/nl_Informal/LC_MESSAGES/django.mo
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2308 2022-03-31 20:05:34.000000 pretix-venueless-1.3.0/pretix_venueless/locale/nl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/locale/pt_PT/
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 raphael   (1000) raphael   (1000)      324 2022-09-29 11:35:17.000000 pretix-venueless-1.3.0/pretix_venueless/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2302 2022-03-31 20:05:34.000000 pretix-venueless-1.3.0/pretix_venueless/locale/pt_PT/LC_MESSAGES/django.po
--rw-r--r--   0 raphael   (1000) raphael   (1000)     4596 2023-02-09 10:43:54.000000 pretix-venueless-1.3.0/pretix_venueless/signals.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/static/
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/static/pretix_venueless/
--rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-02-19 19:28:00.000000 pretix-venueless-1.3.0/pretix_venueless/static/pretix_venueless/.gitkeep
--rw-r--r--   0 raphael   (1000) raphael   (1000)    14395 2022-03-21 15:29:57.000000 pretix-venueless-1.3.0/pretix_venueless/static/pretix_venueless/logo.svg
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/templates/
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless/templates/pretix_venueless/
--rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-02-19 19:28:00.000000 pretix-venueless-1.3.0/pretix_venueless/templates/pretix_venueless/.gitkeep
--rw-r--r--   0 raphael   (1000) raphael   (1000)     2122 2022-02-19 19:28:00.000000 pretix-venueless-1.3.0/pretix_venueless/templates/pretix_venueless/order_info.html
--rw-r--r--   0 raphael   (1000) raphael   (1000)      571 2022-02-19 19:28:00.000000 pretix-venueless-1.3.0/pretix_venueless/templates/pretix_venueless/settings.html
--rw-r--r--   0 raphael   (1000) raphael   (1000)      426 2022-12-17 17:28:51.000000 pretix-venueless-1.3.0/pretix_venueless/urls.py
--rw-r--r--   0 raphael   (1000) raphael   (1000)     7250 2023-02-09 10:43:31.000000 pretix-venueless-1.3.0/pretix_venueless/views.py
-drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/pretix_venueless.egg-info/
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1152 2023-04-04 17:23:03.000000 pretix-venueless-1.3.0/pretix_venueless.egg-info/PKG-INFO
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1699 2023-04-04 17:23:03.000000 pretix-venueless-1.3.0/pretix_venueless.egg-info/SOURCES.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)        1 2023-04-04 17:23:03.000000 pretix-venueless-1.3.0/pretix_venueless.egg-info/dependency_links.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)       69 2023-04-04 17:23:03.000000 pretix-venueless-1.3.0/pretix_venueless.egg-info/entry_points.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)        6 2023-04-04 17:23:03.000000 pretix-venueless-1.3.0/pretix_venueless.egg-info/requires.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)       17 2023-04-04 17:23:03.000000 pretix-venueless-1.3.0/pretix_venueless.egg-info/top_level.txt
--rw-r--r--   0 raphael   (1000) raphael   (1000)      363 2023-04-04 17:23:03.566604 pretix-venueless-1.3.0/setup.cfg
--rw-r--r--   0 raphael   (1000) raphael   (1000)     1059 2022-12-17 17:29:03.000000 pretix-venueless-1.3.0/setup.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.429160 pretix_venueless-1.3.1/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      557 2022-02-19 19:28:00.000000 pretix_venueless-1.3.1/LICENSE
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      135 2022-02-19 19:28:00.000000 pretix_venueless-1.3.1/MANIFEST.in
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1970 2024-05-02 14:20:35.429160 pretix_venueless-1.3.1/PKG-INFO
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      894 2023-05-19 14:15:33.000000 pretix_venueless-1.3.1/README.rst
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.429160 pretix_venueless-1.3.1/pretix_venueless/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       22 2024-04-26 11:44:47.000000 pretix_venueless-1.3.1/pretix_venueless/__init__.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      804 2024-04-26 11:44:47.000000 pretix_venueless-1.3.1/pretix_venueless/apps.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.429160 pretix_venueless-1.3.1/pretix_venueless/locale/
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.425827 pretix_venueless-1.3.1/pretix_venueless/locale/ar/
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.429160 pretix_venueless-1.3.1/pretix_venueless/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      321 2022-09-29 11:35:17.000000 pretix_venueless-1.3.1/pretix_venueless/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2299 2022-03-31 20:05:34.000000 pretix_venueless-1.3.1/pretix_venueless/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.425827 pretix_venueless-1.3.1/pretix_venueless/locale/de/
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.429160 pretix_venueless-1.3.1/pretix_venueless/locale/de/LC_MESSAGES/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2053 2022-09-29 11:35:17.000000 pretix_venueless-1.3.1/pretix_venueless/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     3071 2022-03-31 20:05:34.000000 pretix_venueless-1.3.1/pretix_venueless/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.429160 pretix_venueless-1.3.1/pretix_venueless/locale/de_Informal/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-02-19 19:28:00.000000 pretix_venueless-1.3.1/pretix_venueless/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.429160 pretix_venueless-1.3.1/pretix_venueless/locale/de_Informal/LC_MESSAGES/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2054 2022-09-29 11:35:17.000000 pretix_venueless-1.3.1/pretix_venueless/locale/de_Informal/LC_MESSAGES/django.mo
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     3065 2022-03-31 20:05:34.000000 pretix_venueless-1.3.1/pretix_venueless/locale/de_Informal/LC_MESSAGES/django.po
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2302 2022-03-31 20:05:34.000000 pretix_venueless-1.3.1/pretix_venueless/locale/django.pot
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.425827 pretix_venueless-1.3.1/pretix_venueless/locale/fi/
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.429160 pretix_venueless-1.3.1/pretix_venueless/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      677 2022-09-29 11:35:17.000000 pretix_venueless-1.3.1/pretix_venueless/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2528 2022-09-29 09:20:55.000000 pretix_venueless-1.3.1/pretix_venueless/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.425827 pretix_venueless-1.3.1/pretix_venueless/locale/hr/
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.429160 pretix_venueless-1.3.1/pretix_venueless/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      321 2023-01-30 14:36:13.000000 pretix_venueless-1.3.1/pretix_venueless/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2277 2023-01-30 14:35:40.000000 pretix_venueless-1.3.1/pretix_venueless/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.425827 pretix_venueless-1.3.1/pretix_venueless/locale/ja/
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.429160 pretix_venueless-1.3.1/pretix_venueless/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      321 2022-09-29 11:35:17.000000 pretix_venueless-1.3.1/pretix_venueless/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2299 2022-03-31 20:05:34.000000 pretix_venueless-1.3.1/pretix_venueless/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.425827 pretix_venueless-1.3.1/pretix_venueless/locale/nl/
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.429160 pretix_venueless-1.3.1/pretix_venueless/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2004 2022-09-29 11:35:17.000000 pretix_venueless-1.3.1/pretix_venueless/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     3039 2022-03-31 20:05:34.000000 pretix_venueless-1.3.1/pretix_venueless/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.425827 pretix_venueless-1.3.1/pretix_venueless/locale/nl_Informal/
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.429160 pretix_venueless-1.3.1/pretix_venueless/locale/nl_Informal/LC_MESSAGES/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      330 2022-09-29 11:35:17.000000 pretix_venueless-1.3.1/pretix_venueless/locale/nl_Informal/LC_MESSAGES/django.mo
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2308 2022-03-31 20:05:34.000000 pretix_venueless-1.3.1/pretix_venueless/locale/nl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.425827 pretix_venueless-1.3.1/pretix_venueless/locale/pt_PT/
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.429160 pretix_venueless-1.3.1/pretix_venueless/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      324 2022-09-29 11:35:17.000000 pretix_venueless-1.3.1/pretix_venueless/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2302 2022-03-31 20:05:34.000000 pretix_venueless-1.3.1/pretix_venueless/locale/pt_PT/LC_MESSAGES/django.po
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     4595 2024-04-23 12:46:37.000000 pretix_venueless-1.3.1/pretix_venueless/signals.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.425827 pretix_venueless-1.3.1/pretix_venueless/static/
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.429160 pretix_venueless-1.3.1/pretix_venueless/static/pretix_venueless/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-02-19 19:28:00.000000 pretix_venueless-1.3.1/pretix_venueless/static/pretix_venueless/.gitkeep
+-rw-r--r--   0 raphael   (1000) raphael   (1000)    14395 2022-03-21 15:29:57.000000 pretix_venueless-1.3.1/pretix_venueless/static/pretix_venueless/logo.svg
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.425827 pretix_venueless-1.3.1/pretix_venueless/templates/
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.429160 pretix_venueless-1.3.1/pretix_venueless/templates/pretix_venueless/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        0 2022-02-19 19:28:00.000000 pretix_venueless-1.3.1/pretix_venueless/templates/pretix_venueless/.gitkeep
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     2122 2022-02-19 19:28:00.000000 pretix_venueless-1.3.1/pretix_venueless/templates/pretix_venueless/order_info.html
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      571 2022-02-19 19:28:00.000000 pretix_venueless-1.3.1/pretix_venueless/templates/pretix_venueless/settings.html
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      418 2024-04-23 12:46:37.000000 pretix_venueless-1.3.1/pretix_venueless/urls.py
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     7282 2024-04-23 12:46:37.000000 pretix_venueless-1.3.1/pretix_venueless/views.py
+drwxr-xr-x   0 raphael   (1000) raphael   (1000)        0 2024-05-02 14:20:35.429160 pretix_venueless-1.3.1/pretix_venueless.egg-info/
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1970 2024-05-02 14:20:35.000000 pretix_venueless-1.3.1/pretix_venueless.egg-info/PKG-INFO
+-rw-r--r--   0 raphael   (1000) raphael   (1000)     1714 2024-05-02 14:20:35.000000 pretix_venueless-1.3.1/pretix_venueless.egg-info/SOURCES.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        1 2024-05-02 14:20:35.000000 pretix_venueless-1.3.1/pretix_venueless.egg-info/dependency_links.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      137 2024-05-02 14:20:35.000000 pretix_venueless-1.3.1/pretix_venueless.egg-info/entry_points.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)        6 2024-05-02 14:20:35.000000 pretix_venueless-1.3.1/pretix_venueless.egg-info/requires.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       17 2024-05-02 14:20:35.000000 pretix_venueless-1.3.1/pretix_venueless.egg-info/top_level.txt
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      923 2023-05-19 14:15:33.000000 pretix_venueless-1.3.1/pyproject.toml
+-rw-r--r--   0 raphael   (1000) raphael   (1000)      363 2024-05-02 14:20:35.429160 pretix_venueless-1.3.1/setup.cfg
+-rw-r--r--   0 raphael   (1000) raphael   (1000)       38 2023-05-19 14:15:33.000000 pretix_venueless-1.3.1/setup.py
```

### Comparing `pretix-venueless-1.3.0/LICENSE` & `pretix_venueless-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-venueless-1.3.0/PKG-INFO` & `pretix_venueless-1.3.1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,22 @@
-Metadata-Version: 2.1
-Name: pretix-venueless
-Version: 1.3.0
-Summary: Integrates pretix with venueless.org
-Home-page: https://github.com/pretix/pretix-venueless
-Author: Raphael Michel
-Author-email: michel@rami.io
-License: Apache
-License-File: LICENSE
-
 Venueless integration
 ==========================
 
 This is a plugin for `pretix`_. 
 
 Development setup
 -----------------
 
 1. Make sure that you have a working `pretix development setup`_.
 
 2. Clone this repository, eg to ``local/pretix-venueless``.
 
 3. Activate the virtual environment you use for pretix development.
 
-4. Execute ``python setup.py develop`` within this directory to register this application with pretix's plugin registry.
+4. Execute ``pip install -e .`` within this directory to register this application with pretix's plugin registry.
 
 5. Execute ``make`` within this directory to compile translations.
 
 6. Restart your local pretix server. You can now use the plugin from this repository for your events by enabling it in
    the 'plugins' tab in the settings.
```

### Comparing `pretix-venueless-1.3.0/pretix_venueless/apps.py` & `pretix_venueless-1.3.1/pretix_venueless/apps.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,11 +18,11 @@
         author = 'Raphael Michel'
         description = gettext_lazy('Grant access to your venueless event to your customers.')
         visible = True
         picture = "pretix_venueless/logo.svg"
         featured = True
         version = __version__
         category = 'INTEGRATION'
-        compatibility = "pretix>=4.17.0"
+        compatibility = "pretix>=2024.4.0.dev0"
 
     def ready(self):
         from . import signals  # NOQA
```

### Comparing `pretix-venueless-1.3.0/pretix_venueless/locale/ar/LC_MESSAGES/django.po` & `pretix_venueless-1.3.1/pretix_venueless/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-venueless-1.3.0/pretix_venueless/locale/de/LC_MESSAGES/django.mo` & `pretix_venueless-1.3.1/pretix_venueless/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `pretix-venueless-1.3.0/pretix_venueless/locale/de/LC_MESSAGES/django.po` & `pretix_venueless-1.3.1/pretix_venueless/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-venueless-1.3.0/pretix_venueless/locale/de_Informal/LC_MESSAGES/django.mo` & `pretix_venueless-1.3.1/pretix_venueless/locale/de_Informal/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `pretix-venueless-1.3.0/pretix_venueless/locale/de_Informal/LC_MESSAGES/django.po` & `pretix_venueless-1.3.1/pretix_venueless/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-venueless-1.3.0/pretix_venueless/locale/django.pot` & `pretix_venueless-1.3.1/pretix_venueless/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-venueless-1.3.0/pretix_venueless/locale/fi/LC_MESSAGES/django.mo` & `pretix_venueless-1.3.1/pretix_venueless/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `pretix-venueless-1.3.0/pretix_venueless/locale/fi/LC_MESSAGES/django.po` & `pretix_venueless-1.3.1/pretix_venueless/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-venueless-1.3.0/pretix_venueless/locale/hr/LC_MESSAGES/django.po` & `pretix_venueless-1.3.1/pretix_venueless/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-venueless-1.3.0/pretix_venueless/locale/ja/LC_MESSAGES/django.po` & `pretix_venueless-1.3.1/pretix_venueless/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-venueless-1.3.0/pretix_venueless/locale/nl/LC_MESSAGES/django.mo` & `pretix_venueless-1.3.1/pretix_venueless/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `pretix-venueless-1.3.0/pretix_venueless/locale/nl/LC_MESSAGES/django.po` & `pretix_venueless-1.3.1/pretix_venueless/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-venueless-1.3.0/pretix_venueless/locale/nl_Informal/LC_MESSAGES/django.po` & `pretix_venueless-1.3.1/pretix_venueless/locale/nl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-venueless-1.3.0/pretix_venueless/locale/pt_PT/LC_MESSAGES/django.po` & `pretix_venueless-1.3.1/pretix_venueless/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-venueless-1.3.0/pretix_venueless/signals.py` & `pretix_venueless-1.3.1/pretix_venueless/signals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from django.dispatch import receiver
 from django.template.loader import get_template
 from django.urls import resolve, reverse
 from django.utils.timezone import now
 from i18nfield.strings import LazyI18nString
-
-from pretix.base.models import Order, Event
+from pretix.base.models import Event, Order
 from pretix.base.reldate import RelativeDateWrapper
 from pretix.base.settings import settings_hierarkey
 from pretix.base.signals import event_copy_data, item_copy_data
 from pretix.control.signals import nav_event_settings
 from pretix.presale.signals import order_info_top, position_info_top
```

### Comparing `pretix-venueless-1.3.0/pretix_venueless/static/pretix_venueless/logo.svg` & `pretix_venueless-1.3.1/pretix_venueless/static/pretix_venueless/logo.svg`

 * *Files identical despite different names*

### Comparing `pretix-venueless-1.3.0/pretix_venueless/templates/pretix_venueless/order_info.html` & `pretix_venueless-1.3.1/pretix_venueless/templates/pretix_venueless/order_info.html`

 * *Files identical despite different names*

### Comparing `pretix-venueless-1.3.0/pretix_venueless/templates/pretix_venueless/settings.html` & `pretix_venueless-1.3.1/pretix_venueless/templates/pretix_venueless/settings.html`

 * *Files identical despite different names*

### Comparing `pretix-venueless-1.3.0/pretix_venueless/views.py` & `pretix_venueless-1.3.1/pretix_venueless/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import datetime
-
 import jwt
 from django import forms
 from django.core.exceptions import PermissionDenied
 from django.http import Http404
 from django.shortcuts import redirect
 from django.urls import reverse
 from django.utils.decorators import method_decorator
 from django.utils.timezone import now
-from django.utils.translation import gettext_lazy as _, gettext
+from django.utils.translation import gettext, gettext_lazy as _
 from django.views import View
 from django.views.decorators.clickjacking import xframe_options_exempt
-from i18nfield.forms import I18nFormField, I18nTextarea
-
-from pretix.base.forms import SettingsForm, SecretKeySettingsField
-from pretix.base.models import Event, Order, Item, Question, CheckinList
+from i18nfield.forms import I18nFormField
+from pretix.base.forms import (
+    I18nMarkdownTextarea, SecretKeySettingsField, SettingsForm,
+)
+from pretix.base.models import CheckinList, Event, Item, Order, Question
 from pretix.base.reldate import RelativeDateTimeField
 from pretix.base.services.checkin import perform_checkin
-from pretix.control.views.event import EventSettingsFormView, EventSettingsViewMixin
+from pretix.control.views.event import (
+    EventSettingsFormView, EventSettingsViewMixin,
+)
 from pretix.presale.views import EventViewMixin
 from pretix.presale.views.order import OrderPositionDetailMixin
 
 
 class VenuelessSettingsForm(SettingsForm):
     venueless_url = forms.URLField(
         label=_("Venueless URL"),
@@ -73,15 +75,15 @@
         required=False,
         queryset=Question.objects.none(),
         initial=None
     )
     venueless_text = I18nFormField(
         label=_('Introductory text'),
         required=False,
-        widget=I18nTextarea,
+        widget=I18nMarkdownTextarea,
     )
 
     def __init__(self, *args, **kwargs):
         event = kwargs['obj']
         super().__init__(*args, **kwargs)
         self.fields['venueless_items'].queryset = event.items.all()
         self.fields['venueless_questions'].queryset = event.questions.all()
```

### Comparing `pretix-venueless-1.3.0/pretix_venueless.egg-info/SOURCES.txt` & `pretix_venueless-1.3.1/pretix_venueless.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 pretix_venueless/__init__.py
 pretix_venueless/apps.py
 pretix_venueless/signals.py
 pretix_venueless/urls.py
 pretix_venueless/views.py
```


# Comparing `tmp/ckanext_admin_panel-1.0.11.tar.gz` & `tmp/ckanext_admin_panel-1.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext_admin_panel-1.0.11.tar", last modified: Mon Apr 29 10:45:02 2024, max compression
+gzip compressed data, was "ckanext_admin_panel-1.0.12.tar", last modified: Thu May  2 11:41:54 2024, max compression
```

## Comparing `ckanext_admin_panel-1.0.11.tar` & `ckanext_admin_panel-1.0.12.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/
--rw-r--r--   0 berry     (1000) berry     (1000)    34500 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/LICENSE
--rw-r--r--   0 berry     (1000) berry     (1000)      207 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/MANIFEST.in
--rw-r--r--   0 berry     (1000) berry     (1000)     8109 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/PKG-INFO
--rw-r--r--   0 berry     (1000) berry     (1000)     6970 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/README.md
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/
--rw-r--r--   0 berry     (1000) berry     (1000)      221 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/__init__.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_cron/
--rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/__init__.py
--rw-r--r--   0 berry     (1000) berry     (1000)     1324 2024-04-29 09:11:07.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/cli.py
--rw-r--r--   0 berry     (1000) berry     (1000)     1252 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/col_renderers.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_cron/collection/
--rw-r--r--   0 berry     (1000) berry     (1000)       70 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/collection/__init__.py
--rw-r--r--   0 berry     (1000) berry     (1000)     4444 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/collection/cron.py
--rw-r--r--   0 berry     (1000) berry     (1000)      251 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/config.py
--rw-r--r--   0 berry     (1000) berry     (1000)      248 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/const.py
--rw-r--r--   0 berry     (1000) berry     (1000)     1384 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/helpers.py
--rw-r--r--   0 berry     (1000) berry     (1000)      417 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/interfaces.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_cron/logic/
--rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/logic/__init__.py
--rw-r--r--   0 berry     (1000) berry     (1000)     2654 2024-04-29 09:18:55.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/logic/action.py
--rw-r--r--   0 berry     (1000) berry     (1000)      784 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/logic/auth.py
--rw-r--r--   0 berry     (1000) berry     (1000)     3094 2024-04-29 08:59:14.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/logic/schema.py
--rw-r--r--   0 berry     (1000) berry     (1000)     2219 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/logic/validators.py
--rw-r--r--   0 berry     (1000) berry     (1000)     3406 2024-04-29 07:22:40.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/model.py
--rw-r--r--   0 berry     (1000) berry     (1000)     2637 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/plugin.py
--rw-r--r--   0 berry     (1000) berry     (1000)      418 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/types.py
--rw-r--r--   0 berry     (1000) berry     (1000)     3701 2024-04-29 09:54:16.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/utils.py
--rw-r--r--   0 berry     (1000) berry     (1000)     7768 2024-04-29 08:21:06.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/views.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_doi/
--rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-22 08:08:05.000000 ckanext_admin_panel-1.0.11/ckanext/ap_doi/__init__.py
--rw-r--r--   0 berry     (1000) berry     (1000)     4375 2024-04-23 09:06:42.000000 ckanext_admin_panel-1.0.11/ckanext/ap_doi/collection.py
--rw-r--r--   0 berry     (1000) berry     (1000)      216 2024-04-23 12:04:03.000000 ckanext_admin_panel-1.0.11/ckanext/ap_doi/config.py
--rw-r--r--   0 berry     (1000) berry     (1000)       39 2024-04-22 08:20:24.000000 ckanext_admin_panel-1.0.11/ckanext/ap_doi/const.py
--rw-r--r--   0 berry     (1000) berry     (1000)     4042 2024-04-24 10:10:27.000000 ckanext_admin_panel-1.0.11/ckanext/ap_doi/plugin.py
--rw-r--r--   0 berry     (1000) berry     (1000)     4160 2024-04-23 10:19:36.000000 ckanext_admin_panel-1.0.11/ckanext/ap_doi/utils.py
--rw-r--r--   0 berry     (1000) berry     (1000)     3662 2024-04-24 10:08:37.000000 ckanext_admin_panel-1.0.11/ckanext/ap_doi/views.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_example/
--rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_example/__init__.py
--rw-r--r--   0 berry     (1000) berry     (1000)     2257 2024-04-24 10:11:27.000000 ckanext_admin_panel-1.0.11/ckanext/ap_example/plugin.py
--rw-r--r--   0 berry     (1000) berry     (1000)     1553 2024-04-24 10:08:30.000000 ckanext_admin_panel-1.0.11/ckanext/ap_example/views.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_log/
--rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_log/__init__.py
--rw-r--r--   0 berry     (1000) berry     (1000)      529 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_log/col_renderers.py
--rw-r--r--   0 berry     (1000) berry     (1000)     4146 2024-04-23 14:19:12.000000 ckanext_admin_panel-1.0.11/ckanext/ap_log/collection.py
--rw-r--r--   0 berry     (1000) berry     (1000)      823 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_log/log_handlers.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_log/logic/
--rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_log/logic/__init__.py
--rw-r--r--   0 berry     (1000) berry     (1000)     2207 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_log/model.py
--rw-r--r--   0 berry     (1000) berry     (1000)     1693 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_log/plugin.py
--rw-r--r--   0 berry     (1000) berry     (1000)     1195 2024-04-29 07:56:45.000000 ckanext_admin_panel-1.0.11/ckanext/ap_log/views.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_main/
--rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/__init__.py
--rw-r--r--   0 berry     (1000) berry     (1000)     2482 2024-04-29 10:43:14.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/col_renderers.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_main/collection/
--rw-r--r--   0 berry     (1000) berry     (1000)      134 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/collection/__init__.py
--rw-r--r--   0 berry     (1000) berry     (1000)     3332 2024-04-22 18:25:05.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/collection/base.py
--rw-r--r--   0 berry     (1000) berry     (1000)     6406 2024-04-29 10:41:23.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/collection/content.py
--rw-r--r--   0 berry     (1000) berry     (1000)     4713 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/collection/user.py
--rw-r--r--   0 berry     (1000) berry     (1000)      350 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/config.py
--rw-r--r--   0 berry     (1000) berry     (1000)     5267 2024-04-24 10:08:44.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/helpers.py
--rw-r--r--   0 berry     (1000) berry     (1000)      716 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/interfaces.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_main/logic/
--rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/logic/__init__.py
--rw-r--r--   0 berry     (1000) berry     (1000)     4799 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/logic/action.py
--rw-r--r--   0 berry     (1000) berry     (1000)      285 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/logic/auth.py
--rw-r--r--   0 berry     (1000) berry     (1000)      689 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/logic/schema.py
--rw-r--r--   0 berry     (1000) berry     (1000)     2196 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/plugin.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_main/tests/
--rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/tests/__init__.py
--rw-r--r--   0 berry     (1000) berry     (1000)      212 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/tests/test_plugin.py
--rw-r--r--   0 berry     (1000) berry     (1000)      706 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/types.py
--rw-r--r--   0 berry     (1000) berry     (1000)     1108 2024-04-24 09:55:12.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/utils.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_main/views/
--rw-r--r--   0 berry     (1000) berry     (1000)      291 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/views/__init__.py
--rw-r--r--   0 berry     (1000) berry     (1000)     5750 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/views/basic.py
--rw-r--r--   0 berry     (1000) berry     (1000)      467 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/views/config.py
--rw-r--r--   0 berry     (1000) berry     (1000)     4530 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/views/content.py
--rw-r--r--   0 berry     (1000) berry     (1000)     4750 2024-04-25 10:25:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/views/generics.py
--rw-r--r--   0 berry     (1000) berry     (1000)     5767 2024-04-23 08:23:29.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/views/user.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_support/
--rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/__init__.py
--rw-r--r--   0 berry     (1000) berry     (1000)      497 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/col_renderers.py
--rw-r--r--   0 berry     (1000) berry     (1000)     4648 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/collection.py
--rw-r--r--   0 berry     (1000) berry     (1000)      353 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/config.py
--rw-r--r--   0 berry     (1000) berry     (1000)      309 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/helpers.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_support/logic/
--rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/logic/__init__.py
--rw-r--r--   0 berry     (1000) berry     (1000)     2268 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/logic/action.py
--rw-r--r--   0 berry     (1000) berry     (1000)      545 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/logic/auth.py
--rw-r--r--   0 berry     (1000) berry     (1000)     1527 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/logic/schema.py
--rw-r--r--   0 berry     (1000) berry     (1000)      773 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/logic/validators.py
--rw-r--r--   0 berry     (1000) berry     (1000)     2692 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/model.py
--rw-r--r--   0 berry     (1000) berry     (1000)     1995 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/plugin.py
--rw-r--r--   0 berry     (1000) berry     (1000)      330 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/types.py
--rw-r--r--   0 berry     (1000) berry     (1000)     4646 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/views.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext_admin_panel.egg-info/
--rw-r--r--   0 berry     (1000) berry     (1000)     8109 2024-04-29 10:45:02.000000 ckanext_admin_panel-1.0.11/ckanext_admin_panel.egg-info/PKG-INFO
--rw-r--r--   0 berry     (1000) berry     (1000)     2670 2024-04-29 10:45:02.000000 ckanext_admin_panel-1.0.11/ckanext_admin_panel.egg-info/SOURCES.txt
--rw-r--r--   0 berry     (1000) berry     (1000)        1 2024-04-29 10:45:02.000000 ckanext_admin_panel-1.0.11/ckanext_admin_panel.egg-info/dependency_links.txt
--rw-r--r--   0 berry     (1000) berry     (1000)      560 2024-04-29 10:45:02.000000 ckanext_admin_panel-1.0.11/ckanext_admin_panel.egg-info/entry_points.txt
--rw-r--r--   0 berry     (1000) berry     (1000)        8 2024-04-29 10:45:02.000000 ckanext_admin_panel-1.0.11/ckanext_admin_panel.egg-info/namespace_packages.txt
--rw-r--r--   0 berry     (1000) berry     (1000)      265 2024-04-29 10:45:02.000000 ckanext_admin_panel-1.0.11/ckanext_admin_panel.egg-info/requires.txt
--rw-r--r--   0 berry     (1000) berry     (1000)        8 2024-04-29 10:45:02.000000 ckanext_admin_panel-1.0.11/ckanext_admin_panel.egg-info/top_level.txt
--rw-r--r--   0 berry     (1000) berry     (1000)     2974 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/pyproject.toml
--rw-r--r--   0 berry     (1000) berry     (1000)       16 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/requirements.txt
--rw-r--r--   0 berry     (1000) berry     (1000)     2240 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/setup.cfg
--rw-r--r--   0 berry     (1000) berry     (1000)      528 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/setup.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-05-02 11:41:54.286460 ckanext_admin_panel-1.0.12/
+-rw-r--r--   0 berry     (1000) berry     (1000)    34500 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/LICENSE
+-rw-r--r--   0 berry     (1000) berry     (1000)      207 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/MANIFEST.in
+-rw-r--r--   0 berry     (1000) berry     (1000)     9712 2024-05-02 11:41:54.286460 ckanext_admin_panel-1.0.12/PKG-INFO
+-rw-r--r--   0 berry     (1000) berry     (1000)     8573 2024-04-29 12:18:54.000000 ckanext_admin_panel-1.0.12/README.md
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-05-02 11:41:54.276460 ckanext_admin_panel-1.0.12/ckanext/
+-rw-r--r--   0 berry     (1000) berry     (1000)      221 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/__init__.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-05-02 11:41:54.276460 ckanext_admin_panel-1.0.12/ckanext/ap_cron/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_cron/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1324 2024-04-29 09:11:07.000000 ckanext_admin_panel-1.0.12/ckanext/ap_cron/cli.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1252 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_cron/col_renderers.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-05-02 11:41:54.276460 ckanext_admin_panel-1.0.12/ckanext/ap_cron/collection/
+-rw-r--r--   0 berry     (1000) berry     (1000)       70 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_cron/collection/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4477 2024-04-29 12:40:55.000000 ckanext_admin_panel-1.0.12/ckanext/ap_cron/collection/cron.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      251 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_cron/config.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      268 2024-04-29 12:35:40.000000 ckanext_admin_panel-1.0.12/ckanext/ap_cron/const.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1384 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_cron/helpers.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      417 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_cron/interfaces.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-05-02 11:41:54.276460 ckanext_admin_panel-1.0.12/ckanext/ap_cron/logic/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_cron/logic/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     2654 2024-04-29 09:18:55.000000 ckanext_admin_panel-1.0.12/ckanext/ap_cron/logic/action.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      784 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_cron/logic/auth.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     3094 2024-04-29 08:59:14.000000 ckanext_admin_panel-1.0.12/ckanext/ap_cron/logic/schema.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     2219 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_cron/logic/validators.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     3406 2024-04-29 07:22:40.000000 ckanext_admin_panel-1.0.12/ckanext/ap_cron/model.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     2637 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_cron/plugin.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      418 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_cron/types.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     3761 2024-04-29 12:36:10.000000 ckanext_admin_panel-1.0.12/ckanext/ap_cron/utils.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     7768 2024-04-29 08:21:06.000000 ckanext_admin_panel-1.0.12/ckanext/ap_cron/views.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-05-02 11:41:54.276460 ckanext_admin_panel-1.0.12/ckanext/ap_doi/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-22 08:08:05.000000 ckanext_admin_panel-1.0.12/ckanext/ap_doi/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4361 2024-04-29 12:41:51.000000 ckanext_admin_panel-1.0.12/ckanext/ap_doi/collection.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      216 2024-04-23 12:04:03.000000 ckanext_admin_panel-1.0.12/ckanext/ap_doi/config.py
+-rw-r--r--   0 berry     (1000) berry     (1000)       39 2024-04-22 08:20:24.000000 ckanext_admin_panel-1.0.12/ckanext/ap_doi/const.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4238 2024-05-02 11:39:18.000000 ckanext_admin_panel-1.0.12/ckanext/ap_doi/plugin.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4160 2024-04-23 10:19:36.000000 ckanext_admin_panel-1.0.12/ckanext/ap_doi/utils.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     3662 2024-04-24 10:08:37.000000 ckanext_admin_panel-1.0.12/ckanext/ap_doi/views.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-05-02 11:41:54.276460 ckanext_admin_panel-1.0.12/ckanext/ap_example/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_example/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     2257 2024-04-24 10:11:27.000000 ckanext_admin_panel-1.0.12/ckanext/ap_example/plugin.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1553 2024-04-24 10:08:30.000000 ckanext_admin_panel-1.0.12/ckanext/ap_example/views.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-05-02 11:41:54.276460 ckanext_admin_panel-1.0.12/ckanext/ap_log/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_log/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      529 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_log/col_renderers.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4146 2024-04-23 14:19:12.000000 ckanext_admin_panel-1.0.12/ckanext/ap_log/collection.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      823 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_log/log_handlers.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-05-02 11:41:54.276460 ckanext_admin_panel-1.0.12/ckanext/ap_log/logic/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_log/logic/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     2207 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_log/model.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1693 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_log/plugin.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1195 2024-04-29 07:56:45.000000 ckanext_admin_panel-1.0.12/ckanext/ap_log/views.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-05-02 11:41:54.286460 ckanext_admin_panel-1.0.12/ckanext/ap_main/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     2482 2024-04-29 10:43:14.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/col_renderers.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-05-02 11:41:54.286460 ckanext_admin_panel-1.0.12/ckanext/ap_main/collection/
+-rw-r--r--   0 berry     (1000) berry     (1000)      134 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/collection/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     3332 2024-04-22 18:25:05.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/collection/base.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     6427 2024-04-29 12:39:12.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/collection/content.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4750 2024-04-29 12:40:46.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/collection/user.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      350 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/config.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     5267 2024-05-02 07:32:17.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/helpers.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1078 2024-05-02 07:45:21.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/interfaces.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-05-02 11:41:54.286460 ckanext_admin_panel-1.0.12/ckanext/ap_main/logic/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/logic/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4799 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/logic/action.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      285 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/logic/auth.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      689 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/logic/schema.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     2196 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/plugin.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-05-02 11:41:54.286460 ckanext_admin_panel-1.0.12/ckanext/ap_main/tests/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/tests/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      212 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/tests/test_plugin.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      706 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/types.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1108 2024-05-02 07:32:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/utils.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-05-02 11:41:54.286460 ckanext_admin_panel-1.0.12/ckanext/ap_main/views/
+-rw-r--r--   0 berry     (1000) berry     (1000)      291 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/views/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     5750 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/views/basic.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      467 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/views/config.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4530 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/views/content.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     5345 2024-05-02 08:02:06.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/views/generics.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     5767 2024-04-23 08:23:29.000000 ckanext_admin_panel-1.0.12/ckanext/ap_main/views/user.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-05-02 11:41:54.286460 ckanext_admin_panel-1.0.12/ckanext/ap_support/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_support/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      497 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_support/col_renderers.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4648 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_support/collection.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      353 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_support/config.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      309 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_support/helpers.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-05-02 11:41:54.286460 ckanext_admin_panel-1.0.12/ckanext/ap_support/logic/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_support/logic/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     2268 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_support/logic/action.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      545 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_support/logic/auth.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1527 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_support/logic/schema.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      773 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_support/logic/validators.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     2692 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_support/model.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1995 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_support/plugin.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      330 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_support/types.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4646 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/ckanext/ap_support/views.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-05-02 11:41:54.286460 ckanext_admin_panel-1.0.12/ckanext_admin_panel.egg-info/
+-rw-r--r--   0 berry     (1000) berry     (1000)     9712 2024-05-02 11:41:54.000000 ckanext_admin_panel-1.0.12/ckanext_admin_panel.egg-info/PKG-INFO
+-rw-r--r--   0 berry     (1000) berry     (1000)     2670 2024-05-02 11:41:54.000000 ckanext_admin_panel-1.0.12/ckanext_admin_panel.egg-info/SOURCES.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)        1 2024-05-02 11:41:54.000000 ckanext_admin_panel-1.0.12/ckanext_admin_panel.egg-info/dependency_links.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)      560 2024-05-02 11:41:54.000000 ckanext_admin_panel-1.0.12/ckanext_admin_panel.egg-info/entry_points.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)        8 2024-05-02 11:41:54.000000 ckanext_admin_panel-1.0.12/ckanext_admin_panel.egg-info/namespace_packages.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)      265 2024-05-02 11:41:54.000000 ckanext_admin_panel-1.0.12/ckanext_admin_panel.egg-info/requires.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)        8 2024-05-02 11:41:54.000000 ckanext_admin_panel-1.0.12/ckanext_admin_panel.egg-info/top_level.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)     2974 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/pyproject.toml
+-rw-r--r--   0 berry     (1000) berry     (1000)       16 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/requirements.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)     2240 2024-05-02 11:41:54.286460 ckanext_admin_panel-1.0.12/setup.cfg
+-rw-r--r--   0 berry     (1000) berry     (1000)      528 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.12/setup.py
```

### Comparing `ckanext_admin_panel-1.0.11/LICENSE` & `ckanext_admin_panel-1.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/PKG-INFO` & `ckanext_admin_panel-1.0.12/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-admin-panel
-Version: 1.0.11
+Version: 1.0.12
 Summary: Custom admin panel for CKAN to expand default functionality
 Home-page: https://github.com/mutantsan/ckanext-admin-panel
 Author: Oleksandr Cherniavskyi
 Author-email: mutantsan@gmail.com
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
@@ -42,14 +42,17 @@
   - [TODO](#todo)
   - [Registering config sections](#registering-config-sections)
   - [Requirements](#requirements)
   - [Installation](#installation)
   - [Config settings](#config-settings)
   - [Enabling logging](#enabling-logging)
   - [Enable CRON logging](#enable-cron-logging)
+  - [User CRON manager](#user-cron-manager)
+    - [Scheduling](#scheduling)
+    - [Create cron job](#create-cron-job)
   - [Developer installation](#developer-installation)
   - [Tests](#tests)
   - [License](#license)
 
 ## TODO
 This extension is under development, so there are many things to do:
 
@@ -218,14 +221,36 @@
 	```
 2. Use the newly created logger by specifiyng it in `loggers` section.
 	```
     [loggers]
 	keys = root, ckan, ckanext, werkzeug, flask_app, ap_cron
 	```
 
+## User CRON manager
+
+### Scheduling
+Each cron job can be manually triggered from the cron manager page. However, it's essential to schedule a single command with crontab to automatically trigger all jobs created within CKAN. For example:
+
+    */10 * * * * /usr/lib/ckan/default/bin/ckan -c /etc/ckan/default/production.ini ap-cron trigger-jobs
+
+This command checks all the jobs every 10 minutes to determine if they should be run again. Without scheduling this command, you can manually initiate a specific job through the user interface by clicking the `Run` button. Alternatively, you can execute all scheduled jobs by clicking the `Run active jobs` button.
+
+### Create cron job
+To create a cron job, navigate to the cron manager page and click the `Add cron job` button. 
+
+Each job must include the following components:
+
+- Name: A label used primarily in the UI for identification.
+- Actions: One or more CKAN actions that will be executed.
+- Data: JSON-formatted data that provides arguments to the initial action.
+- Job Timeout: The maximum duration allowed for a job to run before it is deemed to have failed.
+- Schedule: A cron expression that specifies the frequency and timing of the job execution.
+
+It is important to note that console commands are not permitted within cron jobs for security reasons. Instead, only CKAN actions can be executed. You can chain multiple actions together; each subsequent action will receive the result of the previous one as its arguments.
+
 ## Developer installation
 
 To install ckanext-admin-panel for development, activate your CKAN virtualenv and
 do:
 
     git clone https://github.com/mutantsan/ckanext-admin-panel.git
     cd ckanext-admin-panel
```

### Comparing `ckanext_admin_panel-1.0.11/README.md` & `ckanext_admin_panel-1.0.12/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -12,14 +12,17 @@
   - [TODO](#todo)
   - [Registering config sections](#registering-config-sections)
   - [Requirements](#requirements)
   - [Installation](#installation)
   - [Config settings](#config-settings)
   - [Enabling logging](#enabling-logging)
   - [Enable CRON logging](#enable-cron-logging)
+  - [User CRON manager](#user-cron-manager)
+    - [Scheduling](#scheduling)
+    - [Create cron job](#create-cron-job)
   - [Developer installation](#developer-installation)
   - [Tests](#tests)
   - [License](#license)
 
 ## TODO
 This extension is under development, so there are many things to do:
 
@@ -188,14 +191,36 @@
 	```
 2. Use the newly created logger by specifiyng it in `loggers` section.
 	```
     [loggers]
 	keys = root, ckan, ckanext, werkzeug, flask_app, ap_cron
 	```
 
+## User CRON manager
+
+### Scheduling
+Each cron job can be manually triggered from the cron manager page. However, it's essential to schedule a single command with crontab to automatically trigger all jobs created within CKAN. For example:
+
+    */10 * * * * /usr/lib/ckan/default/bin/ckan -c /etc/ckan/default/production.ini ap-cron trigger-jobs
+
+This command checks all the jobs every 10 minutes to determine if they should be run again. Without scheduling this command, you can manually initiate a specific job through the user interface by clicking the `Run` button. Alternatively, you can execute all scheduled jobs by clicking the `Run active jobs` button.
+
+### Create cron job
+To create a cron job, navigate to the cron manager page and click the `Add cron job` button. 
+
+Each job must include the following components:
+
+- Name: A label used primarily in the UI for identification.
+- Actions: One or more CKAN actions that will be executed.
+- Data: JSON-formatted data that provides arguments to the initial action.
+- Job Timeout: The maximum duration allowed for a job to run before it is deemed to have failed.
+- Schedule: A cron expression that specifies the frequency and timing of the job execution.
+
+It is important to note that console commands are not permitted within cron jobs for security reasons. Instead, only CKAN actions can be executed. You can chain multiple actions together; each subsequent action will receive the result of the previous one as its arguments.
+
 ## Developer installation
 
 To install ckanext-admin-panel for development, activate your CKAN virtualenv and
 do:
 
     git clone https://github.com/mutantsan/ckanext-admin-panel.git
     cd ckanext-admin-panel
```

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_cron/cli.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_cron/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_cron/col_renderers.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_cron/col_renderers.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_cron/collection/cron.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_cron/collection/cron.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             "schedule": "schedule",
             "updated_at": "Updated At",
             "last_run": "Last run",
             "state": "State",
             "row_actions": "Actions",
         },
         width={
+            "bulk-action": "3%",
             "data": "30%",
             "row_actions": "15%",
         },
         serializers={
             "data": [("json_display", {})],
             "schedule": [("schedule", {})],
             "updated_at": [("date", {})],
```

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_cron/helpers.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_cron/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_cron/logic/action.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_cron/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_cron/logic/auth.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_cron/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_cron/logic/schema.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_cron/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_cron/logic/validators.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_cron/logic/validators.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_cron/model.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_cron/model.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_cron/plugin.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_cron/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_cron/utils.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_cron/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 from typing import Any
 
 from croniter import croniter
 
 import ckan.plugins.toolkit as tk
 
-from ckanext.ap_cron.const import ERRORS, KWARGS, LOG_NAME
+from ckanext.ap_cron.const import ERRORS, KWARGS, RESULTS, LOG_NAME
 from ckanext.ap_cron.model import CronJob
 from ckanext.ap_cron.types import DictizedCronJob
 
 log = logging.getLogger(LOG_NAME)
 
 
 def get_next_run_datetime(date: datetime.datetime, schedule: str) -> datetime.datetime:
@@ -89,25 +89,27 @@
         log.info("[id:%s] Starting to run an action %s", job.id, action)
 
         try:
             result = tk.get_action(action)({"ignore_auth": True}, payload)
             payload = result if result else {}
         except tk.ValidationError as e:
             e.error_dict["action_name"] = action
-            e.error_dict["kwargs"] = payload # type: ignore
+            e.error_dict[KWARGS] = payload # type: ignore
             job.data[ERRORS] = e.error_dict
 
             log.exception(
                 "[id:%s] An action %s has failed. Terminating...", job.id, action
             )
             log.exception("[id:%s] Error dict %s", job.id, e.error_dict)
 
             return _update_job_state(
                 {"id": job.id, "state": CronJob.State.failed, "data": job.data}
             )
+        else:
+            job.data[RESULTS] = result
 
         log.info("[id:%s] The action %s was executed successfully...", job.id, action)
 
     log.info("[id:%s] The cron job has successfuly finished", job.id)
 
     return _update_job_state(
         {"id": job.id, "state": CronJob.State.finished, "data": job.data}
```

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_cron/views.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_cron/views.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_doi/collection.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_doi/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,14 @@
 
     return row
 
 
 class ApDOICollection(collection_base.ApCollection):
     SerializerFactory = collection_base.ApHtmxTableSerializer.with_attributes(
         row_dictizer=row_dictizer,
-        # record_template="ap_doi/record.html",
-        # pager_template="ap_doi/pager.html",
     )
 
     ColumnsFactory = collection_base.ApColumns.with_attributes(
         names=[
             "bulk-action",
             "title",
             "doi_status",
@@ -52,15 +50,20 @@
             "title": "Title",
             "doi_status": "Status",
             "identifier": "DOI",
             "timestamp": "Timestamp",
             "published": "Publish Date",
             "row_actions": "Actions",
         },
-        width={"title": "15%", "doi_status": "10%", "row_actions": "20%"},
+        width={
+            "bulk-action": "3%",
+            "title": "15%",
+            "doi_status": "10%",
+            "row_actions": "20%",
+        },
         serializers={
             "timestamp": [("date", {})],
             "published": [("date", {})],
         },
     )
 
     DataFactory = ApiData.with_attributes(
```

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_doi/plugin.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_doi/plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import logging
 from typing import Any
 from os import path
 
 from yaml import safe_load
 
 import ckan.plugins as p
 import ckan.logic as logic
@@ -18,14 +19,16 @@
 from ckanext.collection.interfaces import CollectionFactory, ICollection
 from ckanext.ap_doi.collection import ApDOICollection
 
 import ckanext.ap_doi.const as const
 import ckanext.ap_doi.utils as utils
 import ckanext.ap_doi.config as config
 
+log = logging.getLogger(__name__)
+
 
 @tk.blanket.blueprints
 @tk.blanket.actions
 @tk.blanket.auth_functions
 class AdminPanelDoiPlugin(p.SingletonPlugin):
     p.implements(p.IConfigurer)
     p.implements(p.IPackageController, inherit=True)
@@ -116,15 +119,21 @@
 
 
 class ApDOIPlugin(DOIPlugin):
     def after_dataset_create(self, context, pkg_dict):
         if config.is_mock_api_calls():
             return
 
-        super(ApDOIPlugin, self).after_dataset_create(context, pkg_dict)
+        try:
+            super(ApDOIPlugin, self).after_dataset_create(context, pkg_dict)
+        except Exception as e:
+            log.error(e)
 
     ## IPackageController
     def after_dataset_update(self, context, pkg_dict):
         if config.is_mock_api_calls():
             return
 
-        super(ApDOIPlugin, self).after_dataset_update(context, pkg_dict)
+        try:
+            super(ApDOIPlugin, self).after_dataset_update(context, pkg_dict)
+        except Exception as e:
+            log.error(e)
```

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_doi/utils.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_doi/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_doi/views.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_doi/views.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_example/plugin.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_example/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_example/views.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_example/views.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_log/col_renderers.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_log/col_renderers.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_log/collection.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_log/collection.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_log/log_handlers.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_log/log_handlers.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_log/model.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_log/model.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_log/plugin.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_log/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_log/views.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_log/views.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_main/col_renderers.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_main/col_renderers.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_main/collection/base.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_main/collection/base.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_main/collection/content.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_main/collection/content.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         sortable={
             "title",
             "type",
             "state",
             "metadata_created",
             "metadata_modified",
         },
-        width={"title": "15%", "notes": "20%", "row_actions": "15%"},
+        width={"bulk-action": "3%", "title": "15%", "notes": "20%", "row_actions": "15%"},
         searchable={"title", "notes"},
         labels={
             "bulk-action": tk.literal(
                 tags.input_(
                     type="checkbox",
                     name="bulk_check",
                     id="bulk_check",
```

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_main/collection/user.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_main/collection/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         sortable={
             "name",
             "fullname",
             "email",
             "state",
             "sysadmin",
         },
+        width={"bulk-action": "3%"},
         searchable={"name", "fullname"},
         labels={
             "bulk-action": tk.literal(
                 tags.input_(
                     type="checkbox",
                     name="bulk_check",
                     id="bulk_check",
```

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_main/helpers.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_main/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_main/interfaces.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_main/interfaces.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from typing import Any
+
 from ckan.plugins.interfaces import Interface
 
 import ckanext.ap_main.types as ap_types
 
 
 class IAdminPanel(Interface):
     def register_toolbar_button(
@@ -18,7 +20,17 @@
         Return a dictionary mapping renderes names (strings) to renderer
         fucntions. For example::
 
             {'col_counter': col_counter}
 
         """
         return {}
+
+    def before_config_update(self, schema_id: str, data: dict[str, Any]) -> None:
+        """Called before configuration update"""
+        pass
+
+    def after_config_update(
+        self, schema_id: str, data_before_update: dict[str, Any], data: dict[str, Any]
+    ) -> None:
+        """Called after configuration update"""
+        pass
```

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_main/logic/action.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_main/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_main/logic/schema.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_main/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_main/plugin.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_main/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_main/types.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_main/types.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_main/utils.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_main/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_main/views/basic.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_main/views/basic.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_main/views/content.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_main/views/content.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_main/views/generics.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_main/views/generics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from __future__ import annotations
 
 from typing import Any
 
 from flask.views import MethodView
 
 import ckan.plugins.toolkit as tk
+import ckan.plugins as p
 from ckan.logic import parse_params
 
+from ckanext.ap_main.interfaces import IAdminPanel
+
 
 class ApConfigurationPageView(MethodView):
     def __init__(
         self,
         schema_id: str,
         render_template: str = "admin_panel/config/autogenerated_config.html",
         breadcrum_label: str = "Configuration",
@@ -101,36 +104,52 @@
 
     def post(self):
         self.schema = self.get_config_schema()
         self.data = parse_params(tk.request.form)
         self.disable_non_editable_fields()
         self.throw_away_undeclared_fields()
 
+        conf_before_update = {key: tk.config[key] for key in self.data.keys()}
+
+        for plugin in reversed(list(p.PluginImplementations(IAdminPanel))):
+            plugin.before_config_update(self.schema_id, self.data)
+
         try:
             if tk.request.form.get("reset"):
                 tk.get_action("editable_config_reset")(
                     {},
                     {"keys": list(self.data)},
                 )
             else:
                 tk.get_action("editable_config_change")(
                     {},
                     {"options": self.data},
                 )
         except tk.ObjectNotFound as e:
-            tk.h.flash_error(tk._("No default value found for option {}".format(e.message)))
+            tk.h.flash_error(
+                tk._("No default value found for option {}".format(e.message))
+            )
             return tk.render(
                 self.render_template,
-                self.prepare_extra_vars(self.schema, self.data, {"test": "No default value"}),
+                self.prepare_extra_vars(
+                    self.schema, self.data, {"test": "No default value"}
+                ),
             )
         except tk.ValidationError as e:
             return tk.render(
                 self.render_template,
                 self.prepare_extra_vars(self.schema, self.data, e.error_dict),
             )
 
+        for plugin in reversed(list(p.PluginImplementations(IAdminPanel))):
+            plugin.after_config_update(
+                self.schema_id,
+                conf_before_update,
+                self.data,
+            )
+
         tk.h.flash_success(self.success_update_message)
 
         return tk.redirect_to(tk.request.endpoint)
 
     def throw_away_undeclared_fields(self) -> None:
         self.data = {k: v for k, v in self.data.items() if k in tk.config}
```

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_main/views/user.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_main/views/user.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_support/collection.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_support/collection.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_support/logic/action.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_support/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_support/logic/auth.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_support/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_support/logic/schema.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_support/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_support/logic/validators.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_support/logic/validators.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_support/model.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_support/model.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_support/plugin.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_support/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext/ap_support/views.py` & `ckanext_admin_panel-1.0.12/ckanext/ap_support/views.py`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext_admin_panel.egg-info/PKG-INFO` & `ckanext_admin_panel-1.0.12/ckanext_admin_panel.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-admin-panel
-Version: 1.0.11
+Version: 1.0.12
 Summary: Custom admin panel for CKAN to expand default functionality
 Home-page: https://github.com/mutantsan/ckanext-admin-panel
 Author: Oleksandr Cherniavskyi
 Author-email: mutantsan@gmail.com
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
@@ -42,14 +42,17 @@
   - [TODO](#todo)
   - [Registering config sections](#registering-config-sections)
   - [Requirements](#requirements)
   - [Installation](#installation)
   - [Config settings](#config-settings)
   - [Enabling logging](#enabling-logging)
   - [Enable CRON logging](#enable-cron-logging)
+  - [User CRON manager](#user-cron-manager)
+    - [Scheduling](#scheduling)
+    - [Create cron job](#create-cron-job)
   - [Developer installation](#developer-installation)
   - [Tests](#tests)
   - [License](#license)
 
 ## TODO
 This extension is under development, so there are many things to do:
 
@@ -218,14 +221,36 @@
 	```
 2. Use the newly created logger by specifiyng it in `loggers` section.
 	```
     [loggers]
 	keys = root, ckan, ckanext, werkzeug, flask_app, ap_cron
 	```
 
+## User CRON manager
+
+### Scheduling
+Each cron job can be manually triggered from the cron manager page. However, it's essential to schedule a single command with crontab to automatically trigger all jobs created within CKAN. For example:
+
+    */10 * * * * /usr/lib/ckan/default/bin/ckan -c /etc/ckan/default/production.ini ap-cron trigger-jobs
+
+This command checks all the jobs every 10 minutes to determine if they should be run again. Without scheduling this command, you can manually initiate a specific job through the user interface by clicking the `Run` button. Alternatively, you can execute all scheduled jobs by clicking the `Run active jobs` button.
+
+### Create cron job
+To create a cron job, navigate to the cron manager page and click the `Add cron job` button. 
+
+Each job must include the following components:
+
+- Name: A label used primarily in the UI for identification.
+- Actions: One or more CKAN actions that will be executed.
+- Data: JSON-formatted data that provides arguments to the initial action.
+- Job Timeout: The maximum duration allowed for a job to run before it is deemed to have failed.
+- Schedule: A cron expression that specifies the frequency and timing of the job execution.
+
+It is important to note that console commands are not permitted within cron jobs for security reasons. Instead, only CKAN actions can be executed. You can chain multiple actions together; each subsequent action will receive the result of the previous one as its arguments.
+
 ## Developer installation
 
 To install ckanext-admin-panel for development, activate your CKAN virtualenv and
 do:
 
     git clone https://github.com/mutantsan/ckanext-admin-panel.git
     cd ckanext-admin-panel
```

### Comparing `ckanext_admin_panel-1.0.11/ckanext_admin_panel.egg-info/SOURCES.txt` & `ckanext_admin_panel-1.0.12/ckanext_admin_panel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/ckanext_admin_panel.egg-info/entry_points.txt` & `ckanext_admin_panel-1.0.12/ckanext_admin_panel.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/pyproject.toml` & `ckanext_admin_panel-1.0.12/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext_admin_panel-1.0.11/setup.cfg` & `ckanext_admin_panel-1.0.12/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-admin-panel
-version = 1.0.11
+version = 1.0.12
 description = Custom admin panel for CKAN to expand default functionality
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mutantsan/ckanext-admin-panel
 author = Oleksandr Cherniavskyi
 author_email = mutantsan@gmail.com
 license = AGPL
```

### Comparing `ckanext_admin_panel-1.0.11/setup.py` & `ckanext_admin_panel-1.0.12/setup.py`

 * *Files identical despite different names*


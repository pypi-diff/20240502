# Comparing `tmp/pigeonpost-0.4.3.tar.gz` & `tmp/pigeonpost-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigeonpost-0.4.3.tar", last modified: Wed May  1 16:23:57 2024, max compression
+gzip compressed data, was "pigeonpost-0.4.4.tar", last modified: Thu May  2 21:57:37 2024, max compression
```

## Comparing `pigeonpost-0.4.3.tar` & `pigeonpost-0.4.4.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.546938 pigeonpost-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-01 16:23:57.546938 pigeonpost-0.4.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.538938 pigeonpost-0.4.3/pigeon/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.538938 pigeonpost-0.4.3/pigeon/conf/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/conf/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/conf/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/conf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.542938 pigeonpost-0.4.3/pigeon/core/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/core/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/core/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/core/secure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/core/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.542938 pigeonpost-0.4.3/pigeon/default/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/default/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.542938 pigeonpost-0.4.3/pigeon/files/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/files/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/files/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.542938 pigeonpost-0.4.3/pigeon/http/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/http/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/http/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/http/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/http/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.542938 pigeonpost-0.4.3/pigeon/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.546938 pigeonpost-0.4.3/pigeon/middleware/components/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/cache_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/component.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/content_negotiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/cors.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/date.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/host.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/mediafiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/method.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/components/staticfiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.546938 pigeonpost-0.4.3/pigeon/middleware/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/conversion/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.546938 pigeonpost-0.4.3/pigeon/middleware/conversion/mime/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/conversion/mime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/conversion/mime/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/conversion/mime/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/middleware/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.546938 pigeonpost-0.4.3/pigeon/templating/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/templating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/templating/templater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.546938 pigeonpost-0.4.3/pigeon/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/utils/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3227 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/pigeon/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:57.546938 pigeonpost-0.4.3/pigeonpost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-01 16:23:57.000000 pigeonpost-0.4.3/pigeonpost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-01 16:23:57.000000 pigeonpost-0.4.3/pigeonpost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:23:57.000000 pigeonpost-0.4.3/pigeonpost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-01 16:23:57.000000 pigeonpost-0.4.3/pigeonpost.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 16:23:57.000000 pigeonpost-0.4.3/pigeonpost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 16:23:57.000000 pigeonpost-0.4.3/pigeonpost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-01 16:23:57.550938 pigeonpost-0.4.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-05-01 16:23:52.000000 pigeonpost-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.136956 pigeonpost-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-02 21:57:37.136956 pigeonpost-0.4.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.128956 pigeonpost-0.4.4/pigeon/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.128956 pigeonpost-0.4.4/pigeon/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/conf/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/conf/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/conf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.128956 pigeonpost-0.4.4/pigeon/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/core/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/core/secure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/core/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.128956 pigeonpost-0.4.4/pigeon/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/default/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.128956 pigeonpost-0.4.4/pigeon/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/files/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/files/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.128956 pigeonpost-0.4.4/pigeon/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/http/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/http/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/http/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/http/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.132956 pigeonpost-0.4.4/pigeon/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.132956 pigeonpost-0.4.4/pigeon/middleware/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/cache_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/content_negotiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/mediafiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/components/staticfiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.132956 pigeonpost-0.4.4/pigeon/middleware/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/conversion/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.132956 pigeonpost-0.4.4/pigeon/middleware/conversion/mime/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/conversion/mime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/conversion/mime/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/conversion/mime/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/middleware/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.132956 pigeonpost-0.4.4/pigeon/templating/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/templating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/templating/templater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.136956 pigeonpost-0.4.4/pigeon/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/utils/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3260 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/pigeon/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:57:37.136956 pigeonpost-0.4.4/pigeonpost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-02 21:57:37.000000 pigeonpost-0.4.4/pigeonpost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-02 21:57:37.000000 pigeonpost-0.4.4/pigeonpost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 21:57:37.000000 pigeonpost-0.4.4/pigeonpost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-02 21:57:37.000000 pigeonpost-0.4.4/pigeonpost.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-02 21:57:37.000000 pigeonpost-0.4.4/pigeonpost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 21:57:37.000000 pigeonpost-0.4.4/pigeonpost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-02 21:57:37.136956 pigeonpost-0.4.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-05-02 21:57:28.000000 pigeonpost-0.4.4/setup.py
```

### Comparing `pigeonpost-0.4.3/pigeon/conf/manager.py` & `pigeonpost-0.4.4/pigeon/conf/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import importlib
 from pathlib import Path
 from typing import Any
 import pigeon.conf.settings as settings
-import pigeon.utils.logger as logger
 
 
 class ManagerMeta(type):
     def __getattr__(self, key: str) -> Any:
         # get attribute from settings
         key = key.upper()
         if(hasattr(settings, key)): return getattr(settings, key)
```

### Comparing `pigeonpost-0.4.3/pigeon/conf/settings.py` & `pigeonpost-0.4.4/pigeon/conf/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 
 # HTTPS
 USE_HTTPS = False
 CERTIFICATE_PATH = None
 PRIVATE_KEY_PATH = None
 PRIVATE_KEY_PASSWD = None
 
+# EXCEPTION HANDLING & DEBUG MODE
+CRASH_ON_FAILURE = False
+DEBUG_MODE = True
+
 # MIME PARSERS
 MIME_PARSERS = {
     'application/json': 'pigeon.middleware.conversion.mime.parsers.JSONParser',
     'application/x-www-form-urlencoded': 'pigeon.middleware.conversion.mime.parsers.UrlencodedFormParser',
     'multipart/form-data': 'pigeon.middleware.conversion.mime.parsers.MultiPartFormParser',
 }
```

### Comparing `pigeonpost-0.4.3/pigeon/core/handler.py` & `pigeonpost-0.4.4/pigeon/core/handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import socket
+import sys
 import pigeon.middleware as middleware
 import pigeon.utils.logger as logger
 from pigeon.http import HTTPRequest, HTTPResponse
-import traceback
 
 log = logger.Log('HANDLER', 'cyan')
 
 
 def receive_data(client_sock: socket.socket, size: int = 4096) -> bytes:
     while True:
         try:
@@ -51,15 +51,15 @@
 
             # send response to client
             log.verbose(f'SENDING RESPONSE TO {client_address[0]}:{client_address[1]}')
             client_sock.sendall(response.__bytes__('ascii'))
             log.verbose(f'RESPONSE SENT')
 
         except Exception as e:
-            log.error(f'EXCEPTION OCCURED WHILE HANDLING REQUEST FROM {client_address[0]}:{client_address[1]}: \n{"".join(traceback.format_tb(e.__traceback__))}\t{e}\n')
+            sys.excepthook(None, e, None, custom_log=log, description=f'EXCEPTION OCCURED WHILE HANDLING REQUEST FROM {client_address[0]}:{client_address[1]}')
 
         # do not keep connection open on error
         if response.is_error:
             break
 
         # client asks to terminate connection
         if not request.tags.keep_alive:
```

### Comparing `pigeonpost-0.4.3/pigeon/core/secure.py` & `pigeonpost-0.4.4/pigeon/core/secure.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.3/pigeon/core/server.py` & `pigeonpost-0.4.4/pigeon/core/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import socket
+import sys
 from pigeon.conf import Manager
 import pigeon.utils.logger as logger
 import pigeon.core.secure as secure
 import pigeon.core.handler as handler
 import pigeon.files.static as static
 import pigeon.templating.templater as templater
 import threading
@@ -36,15 +37,15 @@
     # configure https if specified in settings
     if Manager.use_https:
         log.verbose('USING HTTPS')
         secure_sock = secure.make_secure(sock, Manager.certificate_path, Manager.private_key_path, Manager.private_key_passwd)
         # securing socket failed
         if not secure_sock:
             log.critical('HTTPS FAILED')
-            exit(-1)
+            sys.exit(-1, force=True)
 
         sock = secure_sock
 
     # listen for incoming connections and then forward them to the handler
     sock.listen()
 
     try:
@@ -61,11 +62,12 @@
 
             log.verbose(f'CONNECTION FROM {client_address[0]}:{client_address[1]}')
             threading.Thread(target=handler.handle_connection, args=(client_sock, client_address)).start()
 
     # user exit - close socket
     except KeyboardInterrupt:
         print('\n')
-        log.info('EXITING')
+        log.info('EXITING (USER INTERRUPT)')
         log.warning('APPLICATION WILL EXIT ONCE THREADS HAVE BEEN TERMINATED')
         sock.shutdown(socket.SHUT_RDWR)
         sock.close()
+        sys.exit(0, force=True)
```

### Comparing `pigeonpost-0.4.3/pigeon/files/media.py` & `pigeonpost-0.4.4/pigeon/files/media.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.3/pigeon/files/static.py` & `pigeonpost-0.4.4/pigeon/files/static.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.3/pigeon/http/message.py` & `pigeonpost-0.4.4/pigeon/http/message.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.3/pigeon/http/request.py` & `pigeonpost-0.4.4/pigeon/http/request.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.3/pigeon/http/response.py` & `pigeonpost-0.4.4/pigeon/http/response.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.3/pigeon/middleware/auth.py` & `pigeonpost-0.4.4/pigeon/middleware/auth.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.3/pigeon/middleware/components/__init__.py` & `pigeonpost-0.4.4/pigeon/middleware/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.3/pigeon/middleware/components/cache_control.py` & `pigeonpost-0.4.4/pigeon/middleware/components/cache_control.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.3/pigeon/middleware/components/component.py` & `pigeonpost-0.4.4/pigeon/middleware/components/component.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.3/pigeon/middleware/components/connection.py` & `pigeonpost-0.4.4/pigeon/middleware/components/connection.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.3/pigeon/middleware/components/content_negotiation.py` & `pigeonpost-0.4.4/pigeon/middleware/components/content_negotiation.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.3/pigeon/middleware/components/cors.py` & `pigeonpost-0.4.4/pigeon/middleware/components/cors.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.3/pigeon/middleware/components/host.py` & `pigeonpost-0.4.4/pigeon/middleware/components/host.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.3/pigeon/middleware/components/mediafiles.py` & `pigeonpost-0.4.4/pigeon/middleware/components/mediafiles.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.3/pigeon/middleware/components/method.py` & `pigeonpost-0.4.4/pigeon/middleware/components/method.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.3/pigeon/middleware/components/staticfiles.py` & `pigeonpost-0.4.4/pigeon/middleware/components/staticfiles.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.3/pigeon/middleware/conversion/converter.py` & `pigeonpost-0.4.4/pigeon/middleware/conversion/converter.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.3/pigeon/middleware/conversion/mime/parsers.py` & `pigeonpost-0.4.4/pigeon/middleware/conversion/mime/parsers.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.3/pigeon/middleware/pipe.py` & `pigeonpost-0.4.4/pigeon/middleware/pipe.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+import sys
 import pigeon.utils.logger as logger
 from pigeon.http.message import HTTPMessage
 from pigeon.http import HTTPRequest, HTTPResponse, error
 import pigeon.conf.middleware as middleware
 import pigeon.middleware.conversion.converter as converter
 from pigeon.middleware.tags import MiddlewareTags
-import traceback
 
 log = logger.Log('MIDDLEWARE', 'green')
 
 
 def preprocess(raw: bytes) -> HTTPResponse | HTTPRequest:
     """
     Tries to parse the raw request and checks whether the request is valid.
@@ -16,30 +16,28 @@
     """
     log.debug(f'PREPROCESSING REQUEST...')
     
     # try parsing the request
     try:
         request: HTTPRequest = converter.parse(raw)
     except Exception as e:
-        log.warning(f'COULD NOT PARSE REQUEST - SKIPPING')
-        log.debug(f'TRACEBACK: \n{"".join(traceback.format_tb(e.__traceback__))}\t{e}\n')
+        sys.excepthook(None, e, None, custom_log=log, description='COULD NOT PARSE REQUEST - SKIPPING')
         return error(400)
     
     if request.protocol not in middleware.HTTP_VERSIONS:
         # server doesn't understand protocol
         log.warning(f'RECEIVED REQUEST OF UNKNOWN PROTOCOL VERSION - SKIPPING')
         return error(505)
     
     # try processing the request
     try:
         request.tags = MiddlewareTags()
         return middleware.PROCESSORS[request.protocol].preprocess(request=request)
     except Exception as e:
-        log.warning(f'MIDDLEWARE FAILED WHEN PREPROCESSING REQUEST - SKIPPING')
-        log.debug(f'TRACEBACK: \n{"".join(traceback.format_tb(e.__traceback__))}\t{e}\n')
+        sys.excepthook(None, e, None, custom_log=log, description='MIDDLEWARE FAILED WHEN PREPROCESSING REQUEST - SKIPPING')
         return error(500)
 
 
 def process(message: HTTPMessage) -> HTTPResponse:
     """
     Gathers the response from the application logic.
     """
@@ -49,15 +47,19 @@
     if message.is_error:
         log.info(f'PREPROCESSOR RETURNED ERROR {message.status}')
         # request failed preprocessing - return error to client
         # do not further process request
         return message
 
     # process request
-    response = middleware.PROCESSORS[message.protocol].process(request=message)
+    try:
+        response = middleware.PROCESSORS[message.protocol].process(request=message)
+    except Exception as e:
+        sys.excepthook(None, e, None, custom_log=log, description='VIEW RAISED EXCEPTION')
+        response = error(500)
 
     # if processor returned an error log it
     if response.is_error:
         log.warning(f'PROCESSOR RETURNED ERROR {response.status}')
 
     return response
 
@@ -76,10 +78,9 @@
     
     # try processing the request
     try:
         response = middleware.PROCESSORS[request.protocol].postprocess(response=response, request=request)
         # request failed postprocessing - return error to client
         return response
     except Exception as e:
-        log.warning(f'MIDDLEWARE FAILED WHEN POSTPROCESSING REQUEST - SKIPPING')
-        log.debug(f'TRACEBACK: \n{"".join(traceback.format_tb(e.__traceback__))}\t{e}\n')
+        sys.excepthook(None, e, None, custom_log=log, description='MIDDLEWARE FAILED WHEN POSTPROCESSING REQUEST - SKIPPING')
         return error(code=500, request=request)
```

### Comparing `pigeonpost-0.4.3/pigeon/middleware/processing.py` & `pigeonpost-0.4.4/pigeon/middleware/processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from pigeon.http import HTTPRequest, HTTPResponse, error
 from typing import Callable
 import pigeon.middleware.components as comp
 import pigeon.utils.logger as logger
-import traceback
-
 
 class Processor:
     @classmethod
     def preprocess(cls,  request: HTTPRequest) -> HTTPRequest | HTTPResponse:
         raise NotImplementedError
 
     @classmethod
```

### Comparing `pigeonpost-0.4.3/pigeon/middleware/tags.py` & `pigeonpost-0.4.4/pigeon/middleware/tags.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.3/pigeon/middleware/views.py` & `pigeonpost-0.4.4/pigeon/middleware/views.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.3/pigeon/templating/templater.py` & `pigeonpost-0.4.4/pigeon/templating/templater.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.3/pigeon/utils/common.py` & `pigeonpost-0.4.4/pigeon/utils/common.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.3/pigeon/utils/logger.py` & `pigeonpost-0.4.4/pigeon/utils/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,19 +69,19 @@
     def debug(self, *args, prefix='', end='\n', subname=''):
         self.message_blocked = Manager.verbosity < 4
         if not self.message_blocked:
             with lock:
                 print('[#ffaaff]DEBUG    [/]', end='')
                 self._print_msg(*args, end=end, subname=subname)
 
-    def sublog(self, *args, color='white', end='\n'):
+    def sublog(self, *args, color='white][/', end='\n'):
         """
         For log messages that give extra context and details on the previous logmessage.
         They will only be logged if the previous log message was logged as well.
         """
         if not self.message_blocked:
             with lock:
                 msg = ''
                 for arg in args: msg += arg
                 msg = msg.replace('\n', self.off_color+'\n│   [/]['+color+']')
-                print('├─  ', style=self.off_color[1:-1], end='')
-                print(msg, style=color)
+                print(f'{self.off_color}├─  [/]', end='')
+                print('['+color+']'+msg+('[/]' if color!='white][/' else ''))
```

### Comparing `pigeonpost-0.4.3/pigeonpost.egg-info/SOURCES.txt` & `pigeonpost-0.4.4/pigeonpost.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/bento_lib-9.1.0.tar.gz` & `tmp/bento_lib-9.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bento_lib-9.1.0.tar", last modified: Fri Nov 10 21:47:37 2023, max compression
+gzip compressed data, was "bento_lib-9.2.0.tar", last modified: Mon Nov 13 20:42:02 2023, max compression
```

## Comparing `bento_lib-9.1.0.tar` & `bento_lib-9.2.0.tar`

### file list

```diff
@@ -1,63 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 21:47:37.393429 bento_lib-9.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2023-11-10 21:47:24.000000 bento_lib-9.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-10 21:47:24.000000 bento_lib-9.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2023-11-10 21:47:37.393429 bento_lib-9.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2023-11-10 21:47:24.000000 bento_lib-9.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 21:47:37.385429 bento_lib-9.1.0/bento_lib/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 21:47:37.385429 bento_lib-9.1.0/bento_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/auth/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 21:47:37.385429 bento_lib-9.1.0/bento_lib/auth/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/auth/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9816 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/auth/middleware/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/auth/middleware/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/auth/middleware/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/auth/middleware/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/auth/middleware/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/auth/middleware/mark_authz_done_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6432 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/auth/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/auth/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/auth/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 21:47:37.385429 bento_lib-9.1.0/bento_lib/drs/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/drs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 21:47:37.389429 bento_lib-9.1.0/bento_lib/events/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8687 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/events/_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/events/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/events/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/package.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 21:47:37.389429 bento_lib-9.1.0/bento_lib/responses/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/responses/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/responses/fastapi_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/responses/flask_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 21:47:37.389429 bento_lib-9.1.0/bento_lib/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/schemas/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/schemas/bento.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/schemas/bento_data_use.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/schemas/ga4gh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/schemas/ga4gh_service_info.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 21:47:37.389429 bento_lib-9.1.0/bento_lib/search/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/search/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    26842 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/search/data_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/search/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    22589 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/search/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     9376 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/search/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 21:47:37.389429 bento_lib-9.1.0/bento_lib/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/workflows/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/workflows/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2023-11-10 21:47:24.000000 bento_lib-9.1.0/bento_lib/workflows/workflow_set.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 21:47:37.385429 bento_lib-9.1.0/bento_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2023-11-10 21:47:37.000000 bento_lib-9.1.0/bento_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2023-11-10 21:47:37.000000 bento_lib-9.1.0/bento_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-10 21:47:37.000000 bento_lib-9.1.0/bento_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      263 2023-11-10 21:47:37.000000 bento_lib-9.1.0/bento_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-10 21:47:37.000000 bento_lib-9.1.0/bento_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-10 21:47:37.393429 bento_lib-9.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2023-11-10 21:47:24.000000 bento_lib-9.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:42:02.143327 bento_lib-9.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2023-11-13 20:41:48.000000 bento_lib-9.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-13 20:41:48.000000 bento_lib-9.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2023-11-13 20:42:02.143327 bento_lib-9.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2023-11-13 20:41:48.000000 bento_lib-9.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:42:02.131327 bento_lib-9.2.0/bento_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:42:02.135327 bento_lib-9.2.0/bento_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/auth/django_remote_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/auth/headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:42:02.135327 bento_lib-9.2.0/bento_lib/auth/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/auth/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9816 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/auth/middleware/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/auth/middleware/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/auth/middleware/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/auth/middleware/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/auth/middleware/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/auth/middleware/mark_authz_done_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6432 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/auth/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/auth/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/auth/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/auth/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:42:02.135327 bento_lib-9.2.0/bento_lib/drs/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/drs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:42:02.135327 bento_lib-9.2.0/bento_lib/events/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8687 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/events/_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/events/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/package.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:42:02.135327 bento_lib-9.2.0/bento_lib/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/responses/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/responses/fastapi_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/responses/flask_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:42:02.139327 bento_lib-9.2.0/bento_lib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/schemas/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/schemas/bento.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/schemas/bento_data_use.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/schemas/ga4gh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/schemas/ga4gh_service_info.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:42:02.139327 bento_lib-9.2.0/bento_lib/search/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/search/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26842 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/search/data_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/search/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22589 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/search/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9376 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/search/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:42:02.139327 bento_lib-9.2.0/bento_lib/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/workflows/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/workflows/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2023-11-13 20:41:48.000000 bento_lib-9.2.0/bento_lib/workflows/workflow_set.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:42:02.131327 bento_lib-9.2.0/bento_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2023-11-13 20:42:02.000000 bento_lib-9.2.0/bento_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2023-11-13 20:42:02.000000 bento_lib-9.2.0/bento_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-13 20:42:02.000000 bento_lib-9.2.0/bento_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2023-11-13 20:42:02.000000 bento_lib-9.2.0/bento_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-13 20:42:02.000000 bento_lib-9.2.0/bento_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-13 20:42:02.143327 bento_lib-9.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2023-11-13 20:41:48.000000 bento_lib-9.2.0/setup.py
```

### Comparing `bento_lib-9.1.0/LICENSE` & `bento_lib-9.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bento_lib-9.1.0/PKG-INFO` & `bento_lib-9.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bento_lib
-Version: 9.1.0
+Version: 9.2.0
 Summary: A set of common utilities and helpers for Bento platform services.
 Home-page: https://github.com/bento-platform/bento_lib
 Author: David Lougheed, Paul Pillot
 Author-email: david.lougheed@mail.mcgill.ca, paul.pillot@computationalgenomics.ca
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `bento_lib-9.1.0/README.md` & `bento_lib-9.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bento_lib-9.1.0/bento_lib/auth/middleware/base.py` & `bento_lib-9.2.0/bento_lib/auth/middleware/base.py`

 * *Files identical despite different names*

### Comparing `bento_lib-9.1.0/bento_lib/auth/middleware/django.py` & `bento_lib-9.2.0/bento_lib/auth/middleware/django.py`

 * *Files identical despite different names*

### Comparing `bento_lib-9.1.0/bento_lib/auth/middleware/fastapi.py` & `bento_lib-9.2.0/bento_lib/auth/middleware/fastapi.py`

 * *Files identical despite different names*

### Comparing `bento_lib-9.1.0/bento_lib/auth/middleware/flask.py` & `bento_lib-9.2.0/bento_lib/auth/middleware/flask.py`

 * *Files identical despite different names*

### Comparing `bento_lib-9.1.0/bento_lib/auth/permissions.py` & `bento_lib-9.2.0/bento_lib/auth/permissions.py`

 * *Files identical despite different names*

### Comparing `bento_lib-9.1.0/bento_lib/drs/utils.py` & `bento_lib-9.2.0/bento_lib/drs/utils.py`

 * *Files identical despite different names*

### Comparing `bento_lib-9.1.0/bento_lib/events/_event_bus.py` & `bento_lib-9.2.0/bento_lib/events/_event_bus.py`

 * *Files identical despite different names*

### Comparing `bento_lib-9.1.0/bento_lib/events/notifications.py` & `bento_lib-9.2.0/bento_lib/events/notifications.py`

 * *Files identical despite different names*

### Comparing `bento_lib-9.1.0/bento_lib/events/types.py` & `bento_lib-9.2.0/bento_lib/events/types.py`

 * *Files identical despite different names*

### Comparing `bento_lib-9.1.0/bento_lib/responses/errors.py` & `bento_lib-9.2.0/bento_lib/responses/errors.py`

 * *Files identical despite different names*

### Comparing `bento_lib-9.1.0/bento_lib/responses/fastapi_errors.py` & `bento_lib-9.2.0/bento_lib/responses/fastapi_errors.py`

 * *Files identical despite different names*

### Comparing `bento_lib-9.1.0/bento_lib/responses/flask_errors.py` & `bento_lib-9.2.0/bento_lib/responses/flask_errors.py`

 * *Files identical despite different names*

### Comparing `bento_lib-9.1.0/bento_lib/schemas/bento_data_use.schema.json` & `bento_lib-9.2.0/bento_lib/schemas/bento_data_use.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-9.1.0/bento_lib/schemas/ga4gh_service_info.schema.json` & `bento_lib-9.2.0/bento_lib/schemas/ga4gh_service_info.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-9.1.0/bento_lib/search/data_structure.py` & `bento_lib-9.2.0/bento_lib/search/data_structure.py`

 * *Files identical despite different names*

### Comparing `bento_lib-9.1.0/bento_lib/search/operations.py` & `bento_lib-9.2.0/bento_lib/search/operations.py`

 * *Files identical despite different names*

### Comparing `bento_lib-9.1.0/bento_lib/search/postgres.py` & `bento_lib-9.2.0/bento_lib/search/postgres.py`

 * *Files identical despite different names*

### Comparing `bento_lib-9.1.0/bento_lib/search/queries.py` & `bento_lib-9.2.0/bento_lib/search/queries.py`

 * *Files identical despite different names*

### Comparing `bento_lib-9.1.0/bento_lib/types.py` & `bento_lib-9.2.0/bento_lib/types.py`

 * *Files identical despite different names*

### Comparing `bento_lib-9.1.0/bento_lib/workflows/models.py` & `bento_lib-9.2.0/bento_lib/workflows/models.py`

 * *Files identical despite different names*

### Comparing `bento_lib-9.1.0/bento_lib/workflows/workflow_set.py` & `bento_lib-9.2.0/bento_lib/workflows/workflow_set.py`

 * *Files identical despite different names*

### Comparing `bento_lib-9.1.0/bento_lib.egg-info/PKG-INFO` & `bento_lib-9.2.0/bento_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bento-lib
-Version: 9.1.0
+Version: 9.2.0
 Summary: A set of common utilities and helpers for Bento platform services.
 Home-page: https://github.com/bento-platform/bento_lib
 Author: David Lougheed, Paul Pillot
 Author-email: david.lougheed@mail.mcgill.ca, paul.pillot@computationalgenomics.ca
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `bento_lib-9.1.0/bento_lib.egg-info/SOURCES.txt` & `bento_lib-9.2.0/bento_lib.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 bento_lib/types.py
 bento_lib.egg-info/PKG-INFO
 bento_lib.egg-info/SOURCES.txt
 bento_lib.egg-info/dependency_links.txt
 bento_lib.egg-info/requires.txt
 bento_lib.egg-info/top_level.txt
 bento_lib/auth/__init__.py
+bento_lib/auth/django_remote_user.py
 bento_lib/auth/exceptions.py
+bento_lib/auth/headers.py
 bento_lib/auth/permissions.py
 bento_lib/auth/resources.py
+bento_lib/auth/roles.py
 bento_lib/auth/types.py
 bento_lib/auth/middleware/__init__.py
 bento_lib/auth/middleware/base.py
 bento_lib/auth/middleware/constants.py
 bento_lib/auth/middleware/django.py
 bento_lib/auth/middleware/fastapi.py
 bento_lib/auth/middleware/flask.py
```

### Comparing `bento_lib-9.1.0/setup.py` & `bento_lib-9.2.0/setup.py`

 * *Files identical despite different names*


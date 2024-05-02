# Comparing `tmp/onboardapis-2.0.0rc1.tar.gz` & `tmp/onboardapis-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboardapis-2.0.0rc1.tar", last modified: Wed Apr 17 22:39:26 2024, max compression
+gzip compressed data, was "onboardapis-2.0.0rc2.tar", last modified: Thu May  2 19:59:52 2024, max compression
```

## Comparing `onboardapis-2.0.0rc1.tar` & `onboardapis-2.0.0rc2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.278626 onboardapis-2.0.0rc1/onboardapis/
--rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/bus/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/bus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12305 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/other/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/other/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/plane/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/plane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/ship/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/ship/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/train/
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/train/at/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/at/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/train/at/obb/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/at/obb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/at/obb/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/at/obb/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/train/de/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/train/de/bth/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/bth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/train/de/db/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/db/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/db/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/db/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/train/de/flix/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/flix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/flix/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/flix/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.282626 onboardapis-2.0.0rc1/onboardapis/train/de/me/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/me/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/me/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/me/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/onboardapis/train/de/tdh/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/tdh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/de/tdh/apis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/onboardapis/train/fr/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/fr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/onboardapis/train/fr/sncf/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/fr/sncf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/fr/sncf/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/fr/sncf/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/onboardapis/train/it/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/it/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/onboardapis/train/it/ti/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/it/ti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/it/ti/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/it/ti/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/onboardapis/train/third_party/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/third_party/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/onboardapis/train/third_party/icomera/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/third_party/icomera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/third_party/icomera/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/third_party/icomera/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/onboardapis/train/third_party/unwired/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/third_party/unwired/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/third_party/unwired/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/third_party/unwired/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/train/third_party/unwired/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/onboardapis/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/onboardapis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-04-17 22:39:26.000000 onboardapis-2.0.0rc1/onboardapis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-17 22:39:26.000000 onboardapis-2.0.0rc1/onboardapis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 22:39:26.000000 onboardapis-2.0.0rc1/onboardapis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-17 22:39:26.000000 onboardapis-2.0.0rc1/onboardapis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 22:39:26.000000 onboardapis-2.0.0rc1/onboardapis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-17 22:39:21.000000 onboardapis-2.0.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 22:39:26.286626 onboardapis-2.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.266661 onboardapis-2.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-05-02 19:59:52.266661 onboardapis-2.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.258661 onboardapis-2.0.0rc2/onboardapis/
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.258661 onboardapis-2.0.0rc2/onboardapis/bus/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/bus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.258661 onboardapis-2.0.0rc2/onboardapis/other/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/other/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.258661 onboardapis-2.0.0rc2/onboardapis/plane/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/plane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.258661 onboardapis-2.0.0rc2/onboardapis/ship/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/ship/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.258661 onboardapis-2.0.0rc2/onboardapis/train/
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.258661 onboardapis-2.0.0rc2/onboardapis/train/at/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/at/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.258661 onboardapis-2.0.0rc2/onboardapis/train/at/obb/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/at/obb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/at/obb/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/at/obb/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.258661 onboardapis-2.0.0rc2/onboardapis/train/de/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.258661 onboardapis-2.0.0rc2/onboardapis/train/de/bth/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/bth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.262661 onboardapis-2.0.0rc2/onboardapis/train/de/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/db/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8062 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/db/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/db/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.262661 onboardapis-2.0.0rc2/onboardapis/train/de/flix/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/flix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/flix/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/flix/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.262661 onboardapis-2.0.0rc2/onboardapis/train/de/me/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/me/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/me/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/me/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.262661 onboardapis-2.0.0rc2/onboardapis/train/de/tdh/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/tdh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/de/tdh/apis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.262661 onboardapis-2.0.0rc2/onboardapis/train/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/fr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.262661 onboardapis-2.0.0rc2/onboardapis/train/fr/sncf/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/fr/sncf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/fr/sncf/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/fr/sncf/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.262661 onboardapis-2.0.0rc2/onboardapis/train/it/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/it/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.262661 onboardapis-2.0.0rc2/onboardapis/train/it/ti/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/it/ti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/it/ti/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/it/ti/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.262661 onboardapis-2.0.0rc2/onboardapis/train/third_party/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/third_party/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.262661 onboardapis-2.0.0rc2/onboardapis/train/third_party/icomera/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/third_party/icomera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/third_party/icomera/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/third_party/icomera/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.266661 onboardapis-2.0.0rc2/onboardapis/train/third_party/unwired/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/third_party/unwired/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/third_party/unwired/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/third_party/unwired/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/train/third_party/unwired/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/onboardapis/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:59:52.266661 onboardapis-2.0.0rc2/onboardapis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-05-02 19:59:52.000000 onboardapis-2.0.0rc2/onboardapis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-02 19:59:52.000000 onboardapis-2.0.0rc2/onboardapis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:59:52.000000 onboardapis-2.0.0rc2/onboardapis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-02 19:59:52.000000 onboardapis-2.0.0rc2/onboardapis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-02 19:59:52.000000 onboardapis-2.0.0rc2/onboardapis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-02 19:59:45.000000 onboardapis-2.0.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 19:59:52.266661 onboardapis-2.0.0rc2/setup.cfg
```

### Comparing `onboardapis-2.0.0rc1/LICENSE` & `onboardapis-2.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc1/PKG-INFO` & `onboardapis-2.0.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: onboardapis
-Version: 2.0.0rc1
-Summary: A pure Python wrapper for the on-board APIs of many different transportation providers
+Version: 2.0.0rc2
+Summary: A pure Python wrapper for the on-board APIs of many different transportation providers.
 Author-email: Felix Zenk <felix.zenk@web.de>
 License: MIT
 Project-URL: Homepage, https://felix-zenk.github.io/onboardapis
-Project-URL: Source, https://github.com/felix-zenk/onboardapis
-Project-URL: Documentation, https://felix-zenk.github.io/onboardapis/docs/
+Project-URL: Documentation, https://felix-zenk.github.io/onboardapis/
+Project-URL: Repository, https://github.com/felix-zenk/onboardapis
 Project-URL: Issues, https://github.com/felix-zenk/onboardapis/issues
 Keywords: api,train,public-transport
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -29,14 +29,15 @@
 Requires-Dist: restfly>=1.4.7
 Requires-Dist: requests>=2.31.0
 Requires-Dist: beautifulsoup4>=4.12.2
 Requires-Dist: typing-extensions>=4.9.0
 Provides-Extra: dev
 Requires-Dist: flake8>=7.0.0; extra == "dev"
 Requires-Dist: pdoc>=14.4.0; extra == "dev"
+Requires-Dist: build>=1.2.1; extra == "dev"
 
 onboardapis
 ===
 
 [![Python versions](https://img.shields.io/pypi/pyversions/onboardapis)](https://pypi.org/project/onboardapis)
 [![PyPI version](https://badge.fury.io/py/onboardapis.svg)](https://pypi.org/project/onboardapis)
 [![Build package](https://github.com/felix-zenk/onboardapis/actions/workflows/build.yml/badge.svg)](https://github.com/felix-zenk/onboardapis/actions/workflows/build.yml)
@@ -153,17 +154,17 @@
 > The name of a conversion function is the unit which will be the result of the conversion.
 > Different units can be passed to a conversion function as keywords.
 > Keywords can be combined to return the sum of the input units.
 
 ---
 
 ## Documentation
-[![Documentation status](https://img.shields.io/github/actions/workflow/status/felix-zenk/onboardapis/docs.yml?label=docs)](https://felix-zenk.github.io/onboardapis/docs/)
+[![GitHub-Pages](https://github.com/felix-zenk/onboardapis/actions/workflows/docs.yml/badge.svg)](https://felix-zenk.github.io/onboardapis/)
 
-#### Access the documentation on [GitHub-Pages](https://felix-zenk.github.io/onboardapis/docs/).
+#### Access the documentation on [GitHub-Pages](https://felix-zenk.github.io/onboardapis/).
 
 
 ## Supported APIs
 
 | API                   | [API scope](#api-scope) | Type  | Country      | Operator                                                                           |
 |-----------------------|-------------------------|-------|--------------|------------------------------------------------------------------------------------|
 | RailnetRegio          | geo                     | train | at (Austria) | obb (Österreichische Bundesbahnen)                                                 |
```

### Comparing `onboardapis-2.0.0rc1/README.md` & `onboardapis-2.0.0rc2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -117,17 +117,17 @@
 > The name of a conversion function is the unit which will be the result of the conversion.
 > Different units can be passed to a conversion function as keywords.
 > Keywords can be combined to return the sum of the input units.
 
 ---
 
 ## Documentation
-[![Documentation status](https://img.shields.io/github/actions/workflow/status/felix-zenk/onboardapis/docs.yml?label=docs)](https://felix-zenk.github.io/onboardapis/docs/)
+[![GitHub-Pages](https://github.com/felix-zenk/onboardapis/actions/workflows/docs.yml/badge.svg)](https://felix-zenk.github.io/onboardapis/)
 
-#### Access the documentation on [GitHub-Pages](https://felix-zenk.github.io/onboardapis/docs/).
+#### Access the documentation on [GitHub-Pages](https://felix-zenk.github.io/onboardapis/).
 
 
 ## Supported APIs
 
 | API                   | [API scope](#api-scope) | Type  | Country      | Operator                                                                           |
 |-----------------------|-------------------------|-------|--------------|------------------------------------------------------------------------------------|
 | RailnetRegio          | geo                     | train | at (Austria) | obb (Österreichische Bundesbahnen)                                                 |
```

### Comparing `onboardapis-2.0.0rc1/onboardapis/__init__.py` & `onboardapis-2.0.0rc2/onboardapis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,29 +58,30 @@
           InitialConnectionError: If the connection to the API could not be established.
         """
         if not hasattr(self, '_api'):
             return  # Abstract class without API implementation
 
         if isinstance(self._api, ThreadedAPI):
             self._api.start()
-            while not self._api.connected:
+            while not self._api.is_connected:
                 sleep(.1)
             return
 
         return
 
     def shutdown(self) -> None:
         """
         This method will be called when exiting the context manager and can be overwritten by subclasses.
 
         :return: Nothing
         :rtype: None
         """
         pass
 
+    @property
     def now(self) -> datetime:
         """
         Get the current time as seen by the vehicle
 
         :return: The current time
         :rtype: datetime.datetime
         """
```

### Comparing `onboardapis-2.0.0rc1/onboardapis/data.py` & `onboardapis-2.0.0rc2/onboardapis/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 import importlib.metadata
 import logging
 import time
 
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass
 from functools import wraps
+from json import JSONDecodeError
 from typing import TypeVar, Generic, ClassVar, Any
 from threading import Thread
 
 from geopy.point import Point
 from geopy.distance import geodesic
 from gql import Client
 from gql.transport.requests import RequestsHTTPTransport
 from restfly import APISession
 
 from .units import coordinates_decimal_to_dms
-from .exceptions import APIConnectionError
+from .exceptions import APIConnectionError, InitialConnectionError
 
 __all__ = [
     "ID",
     "StationType",
     "get_package_version",
     "default",
     "ScheduledEvent",
@@ -35,28 +36,29 @@
     "API",
     "store",
     "ThreadedAPI",
     "BlockingRestAPI",
     "ThreadedRestAPI",
     "BlockingGraphQlAPI",
     "ThreadedGraphQlAPI",
-    "InternetAccessInterface",
-    "InternetMetricsInterface",
 ]
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 """A type variable for generics."""
 
 ID = TypeVar("ID", str, int)
 """A TypeVar indicating the return type of Vehicle.id"""
 
 StationType = TypeVar("StationType", bound="Station")
-"""A TypeVar indicating the return type of the StationsMixin properties"""
+"""A TypeVar indicating the Station type"""
+
+ApiType = TypeVar("ApiType", bound="API")
+"""A TypeVar indicating the API type"""
 
 
 def get_package_version() -> str:
     """Return the version of the ``onboardapis`` package."""
     try:
         return importlib.metadata.version('onboardapis')
     except importlib.metadata.PackageNotFoundError:
@@ -134,22 +136,24 @@
             + (f" {self.heading:.2f}°" if self.heading is not None else "")
         )
         return coordinates
 
     def __getitem__(self, item):
         return (self.latitude, self.longitude)[item]
 
-    def calculate_distance(self, other):
+    def calculate_distance(self, other: Position | Point) -> float:
         """
         Calculate the distance (in meters) between this position and another position.
 
         :param other: The other position
         :return: The distance in meters
         """
-        return geodesic(self.to_point(), other.to_point()).meters
+        if not isinstance(other, (Position, Point)):
+            raise ValueError
+        return geodesic(self.to_point(), other.to_point() if isinstance(other, Position) else other).meters
 
     def to_point(self, with_altitude: bool = False) -> Point:
         """Convert to a ``geopy.point.Point``."""
         return Point(self.latitude, self.longitude, altitude=self.altitude if with_altitude else None)
 
 
 class API(metaclass=ABCMeta):
@@ -158,25 +162,25 @@
     API_URL: ClassVar[str]
     """The base URL for the API."""
 
     def __init__(self):
         """Initialize a new ``API``."""
         self._data = dict()
 
-    def load(self, key: str, __default: Any = None) -> Any:
+    def load(self, key: str, default: Any = None) -> Any:  # noqa: F402
         """Load data from the cache.
 
         Args:
             key: The key to load.
-            __default: The default value to return if the key is not present.
+            default: The default value to return if the key is not present.
 
         Returns:
             The data if present, else the default.
         """
-        return self._data.get(key, __default)
+        return self._data.get(key, default)
 
     def store(self, key: str, value: Any) -> None:
         """Store data in the cache.
 
         Args:
             key: The key the data should be stored under.
             value: The data to store.
@@ -217,71 +221,73 @@
     raise ValueError('You need to apply this decorator to a method of an API!')
     # Really any callable works just fine, but in this case the decorator will do nothing
 
 
 class ThreadedAPI(API, Thread):
     """An ``API`` that refreshes the data in a new thread."""
 
-    _running: bool
-    _connected: bool
+    _is_running: bool
+    _is_connected: bool
 
     def __init__(self) -> None:
         """Initialize a new ``ThreadedAPI``."""
         API.__init__(self)
         Thread.__init__(
             self,
             target=self._run,
             name=f"API-Thread for '{self.API_URL}'",
             daemon=True,
         )
-        self._running = False
-        self._connected = False
+        self._is_running = False
+        self._is_connected = False
 
     @property
-    def connected(self) -> bool:
+    def is_connected(self) -> bool:
         """Check whether the connector is connected to the server"""
-        return self._connected and self._running
+        return self._is_connected and self._is_running
 
     def _run(self) -> None:
         """The main loop that will run in a separate thread."""
         # thread join checks per second
         tps = 20
         counter = 0
-        self._running = True
-        while self._running:
+        self._is_running = True
+        while self._is_running:
             # If the counter is not 0, just wait and check for a thread join
             if counter != 0:
                 time.sleep(1 / tps)
                 counter = (counter + 1) % tps
                 continue
 
             # The target time for when to perform the next refresh after this one
             target = time.time_ns() + int(1e9)
 
             try:
                 self.refresh()
-                self._connected = True
-            except APIConnectionError as e:
+                self._is_connected = True
+            except (APIConnectionError, JSONDecodeError) as e:
+                if not self._is_connected:
+                    raise InitialConnectionError from e
                 logger.error(f"{e}")
                 continue
 
             counter = (tps - int(max(0.0, (target - time.time_ns()) / 1e9) * tps)) % tps
 
     def stop(self) -> None:
         """Stop requesting data and shut down the separate thread."""
-        self._running = False
+        self._is_running = False
         if self.is_alive():
             self.join()
 
     def reset(self) -> None:
         """Reset the thread and the cache so that they can be reused with ``start()``."""
         self.stop()
         Thread.__init__(self)
         API.__init__(self)
-        self._connected = False
+        self._is_connected = False
 
     @abstractmethod
     def refresh(self) -> None:
         """Method that collects data from the server and stores it in the cache."""
         raise NotImplementedError
 
 
@@ -302,95 +308,48 @@
         APISession._build_session(self, **kwargs)
         self._session.headers.update({"User-Agent": "Python/onboardapis (%s)" % get_package_version()})
 
 
 class ThreadedRestAPI(ThreadedAPI, BlockingRestAPI, metaclass=ABCMeta):
     """A threaded version of the ``BlockingRestAPI``."""
 
-    def __init__(self, **kwargs) -> None:
+    def __init__(self, **kwargs: Any) -> None:
         """Initialize a new ``ThreadedRestAPI``."""
         kwargs['url'] = kwargs.pop('url', self.API_URL)
         APISession.__init__(self, **kwargs)
         ThreadedAPI.__init__(self)
 
 
 class BlockingGraphQlAPI(Client, API):
     """A GraphQL ``API`` that uses a ``gql.client.Client`` to fetch data."""
 
-    def __init__(self, **kwargs) -> None:
+    def __init__(self, **kwargs: Any) -> None:
         """Initialize a new ``BlockingGraphQlAPI``.
 
         Args:
             kwargs: The kwargs to pass to the underlying ``gql.client.Client``.
         """
-        kwargs |= dict(
-            transport=RequestsHTTPTransport(
+        kwargs.update({
+            'transport': kwargs.pop('transport', RequestsHTTPTransport(
                 url=self.API_URL,
                 headers={
                     'Content-Type': 'application/json',
                     'User-Agent': 'Python/onboardapis (%s)' % get_package_version(),
                 },
-            ),
-            fetch_schema_from_transport=True,
-        )
+            )),
+            'fetch_schema_from_transport': kwargs.pop('fetch_schema_from_transport', True),
+        })
         Client.__init__(self, **kwargs)
         API.__init__(self)
 
 
 class ThreadedGraphQlAPI(BlockingGraphQlAPI, ThreadedAPI, metaclass=ABCMeta):
     """A threaded version of the ``BlockingGraphQlAPI``."""
 
-    def __init__(self, kwargs: Any = None) -> None:
+    def __init__(self, **kwargs: Any) -> None:
         """Initialize a new ``ThreadedGraphQlAPI``.
 
         Args:
             kwargs: The kwargs to pass to the underlying ``gql.client.Client``.
         """
         BlockingGraphQlAPI.__init__(self, **kwargs)
         ThreadedAPI.__init__(self)
-
-
-class InternetAccessInterface(metaclass=ABCMeta):
-    """Interface adding functions for connecting and disconnecting to the internet
-    as well as viewing the current status."""
-
-    _is_enabled: bool = False
-    """Cached information on connection status"""
-
-    @abstractmethod
-    def enable(self) -> None:
-        """Enable the internet access for this device.
-
-        Request internet access for this device by automatically accepting the terms of service
-        and signing in to the captive portal.
-
-        Raises:
-            ConnectionError: If the internet access is temporarily not available.
-        """
-        self._is_enabled = True
-
-    @abstractmethod
-    def disable(self) -> None:
-        """Disable the internet access for this device.
-
-        Disable the internet access for this device by signing out of the captive portal.
-
-        Raises:
-            ConnectionError: If the internet access is temporarily not available.
-        """
-        if not self.is_enabled:
-            return
-
-        self._is_enabled = False
-
-    @property
-    def is_enabled(self) -> bool:
-        """Return whether the internet access is enabled for this device."""
-        return self._is_enabled
-
-
-class InternetMetricsInterface(metaclass=ABCMeta):
-    """Interface for information on limited internet access."""
-
-    @abstractmethod
-    def limit(self) -> int | None:
-        """Return the total internet access quota in MB or `None` if there is none."""
```

### Comparing `onboardapis-2.0.0rc1/onboardapis/exceptions.py` & `onboardapis-2.0.0rc2/onboardapis/exceptions.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc1/onboardapis/mixins.py` & `onboardapis-2.0.0rc2/onboardapis/mixins.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
 from datetime import timedelta
 from typing import Generic
 
 from .exceptions import DataInvalidError
-from .data import Position, InternetAccessInterface, ID, StationType
-from . import Station
+from .data import Position, ID, StationType, API
 
 
 class PositionMixin(metaclass=ABCMeta):
     @property
     @abstractmethod
     def position(self) -> Position:
         """
@@ -44,15 +43,15 @@
 
 
 class StationsMixin(Generic[StationType], metaclass=ABCMeta):
     """
     Functionality for a vehicle that provides information on the journey.
     """
 
-    def calculate_distance(self, station: Station) -> float:
+    def calculate_distance(self, station: StationType) -> float:
         """Calculate the distance in meters between the train and a station.
 
         Use the trains ``position`` or ``distance`` to calculate the distance to ``station``.
 
         Args:
             station: The station to calculate the distance to
 
@@ -146,13 +145,67 @@
         :return: The distance
         :rtype: float
         """
         return self.calculate_distance(self.origin)
 
 
 class InternetAccessMixin(metaclass=ABCMeta):
+    """Adds the internet_access property to a class
+    that defines an :class:`InternetAccessInterface` as ``_internet_access``."""
     _internet_access: InternetAccessInterface
 
     @property
     def internet_access(self) -> InternetAccessInterface:
-        """An interface to enable or disable the internet access for this device."""
+        """An interface to manage the internet access for this device."""
         return self._internet_access
+
+
+class InternetAccessInterface(metaclass=ABCMeta):
+    """Interface adding functions for connecting and disconnecting to the internet
+    as well as viewing the current status."""
+
+    _is_enabled: bool = False
+    """Cached information on connection status"""
+    _api: API
+
+    def __init__(self, api: API) -> None:
+        self._api = api
+
+    @abstractmethod
+    def enable(self) -> None:
+        """Enable the internet access for this device.
+
+        Request internet access for this device by automatically accepting the terms of service
+        and signing in to the captive portal.
+
+        Raises:
+            ConnectionError: If the internet access is temporarily not available.
+        """
+        self._is_enabled = True
+
+    @abstractmethod
+    def disable(self) -> None:
+        """Disable the internet access for this device.
+
+        Disable the internet access for this device by signing out of the captive portal.
+
+        Raises:
+            ConnectionError: If the internet access is temporarily not available.
+        """
+        if not self.is_enabled:
+            return
+
+        self._is_enabled = False
+
+    @property
+    def is_enabled(self) -> bool:
+        """Return whether the internet access is enabled for this device."""
+        return self._is_enabled
+
+
+class InternetMetricsInterface(metaclass=ABCMeta):
+    """Interface for information on limited internet access."""
+
+    @abstractmethod
+    def limit(self) -> int | None:
+        """Return the total internet access quota in MB or `None` if there is none."""
+
```

### Comparing `onboardapis-2.0.0rc1/onboardapis/protocols.py` & `onboardapis-2.0.0rc2/onboardapis/protocols.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 The protocols defined here match the properties of the classes in `onboardapis.mixins`.
 """
 from __future__ import annotations
 
 from typing import Protocol
 
-from .data import ID, StationType, Position, InternetAccessInterface
+from .data import ID, StationType, Position
+from .mixins import InternetAccessInterface
 
 
 class SupportsPosition(Protocol):
     # noinspection PyPropertyDefinition
     @property
     def position(self) -> Position: ...
```

### Comparing `onboardapis-2.0.0rc1/onboardapis/train/__init__.py` & `onboardapis-2.0.0rc2/onboardapis/train/__init__.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc1/onboardapis/train/at/obb/apis.py` & `onboardapis-2.0.0rc2/onboardapis/train/at/obb/apis.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc1/onboardapis/train/at/obb/interfaces.py` & `onboardapis-2.0.0rc2/onboardapis/train/at/obb/interfaces.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc1/onboardapis/train/de/db/apis.py` & `onboardapis-2.0.0rc2/onboardapis/train/de/db/apis.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,36 +2,38 @@
 
 import logging
 import re
 
 from typing import Literal
 from datetime import datetime, timedelta
 
+from typing_extensions import deprecated
+
 from ....exceptions import DataInvalidError
 from ....data import ID, default, ScheduledEvent, Position
 from ....mixins import SpeedMixin, PositionMixin, StationsMixin, InternetAccessMixin
 from ....units import ms
 from ... import Train, TrainStation
 from .mappings import id_name_map
-from .interfaces import ICEPortalAPI, ZugPortalAPI
+from .interfaces import ICEPortalAPI, RegioGuideAPI, ICEPortalInternetInterface
 
 logger = logging.getLogger(__name__)
 
 InternetStatus = Literal["NO_INFO", "NO_INTERNET", "UNSTABLE", "WEAK", "MIDDLE", "HIGH"]
 
 
 class ICEPortal(Train, SpeedMixin, PositionMixin, StationsMixin[TrainStation], InternetAccessMixin):
-    """
-    Wrapper for interacting with the DB ICE Portal API
-    """
+    """Wrapper for interacting with the DB ICE Portal API."""
 
     _api: ICEPortalAPI
+    _internet_access: ICEPortalInternetInterface
 
     def __init__(self):
         self._api = ICEPortalAPI()
+        self._internet_access = ICEPortalInternetInterface(self._api)
         Train.__init__(self)
 
     def now(self) -> datetime:
         return datetime.fromtimestamp(int(default(
             self._api["status"].get("serverTime", None), 0,
         )) / 1000)
 
@@ -100,15 +102,15 @@
         stop_info = (
             self._api["trip"].get("trip", {}).get("stopInfo", {})
         )
         station_id = default(stop_info.get("actualNext"))
         # Get the station from the stations dict
         try:
             return self.stations_dict[station_id]
-        except AttributeError as e:
+        except KeyError as e:
             raise DataInvalidError("No current station found") from e
 
     @property
     def speed(self) -> float:
         return ms(kmh=self._api["status"].get("speed", 0))
 
     @property
@@ -224,23 +226,21 @@
             self._api["status"]
             .get("connectivity", {})
             .get("remainingTimeSeconds", "")
         )
         return None if default(remaining_seconds) is None else timedelta(seconds=int(remaining_seconds))
 
 
-class ZugPortal(Train, StationsMixin[TrainStation]):
-    """
-    Wrapper for interacting with the DB Zug Portal API
-    """
+class RegioGuide(Train, StationsMixin[TrainStation]):
+    """Wrapper for interacting with the DB Regio-Guide API, formerly Zug Portal."""
 
-    _api: ZugPortalAPI
+    _api: RegioGuideAPI
 
     def __init__(self):
-        self._api = ZugPortalAPI()
+        self._api = RegioGuideAPI()
         Train.__init__(self)
 
     @property
     def id(self) -> ID:
         return self._api['journey'].get('no')
 
     @property
@@ -278,11 +278,15 @@
             )
             for index, stop in enumerate(self._api['journey'].get('stops', []))
         }
 
     @property
     def current_station(self) -> TrainStation:
         station, *_ = (*filter(
-            lambda s: self.now() < default(s.arrival.actual, s.departure.actual),
+            lambda s: self.now < default(s.arrival.actual, s.departure.actual),
             self.stations
         ), None)
         return self.destination if station is None else station
+
+
+ZugPortal = deprecated('Renamed by DB. Use RegioGuide instead.')(RegioGuide)
+"""Renamed by DB. Use RegioGuide instead."""
```

### Comparing `onboardapis-2.0.0rc1/onboardapis/train/de/db/interfaces.py` & `onboardapis-2.0.0rc2/onboardapis/train/de/db/interfaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 
 from bs4 import BeautifulSoup
 from geopy import Point
 from geopy.distance import distance
 
 from ....data import (
     ID,
-    BlockingRestAPI,
+    ThreadedRestAPI,
     ScheduledEvent,
     default,
     store,
-    InternetAccessInterface,
-    InternetMetricsInterface,
+    BlockingRestAPI,
 )
+from ....mixins import InternetAccessInterface, InternetMetricsInterface
 from ... import ConnectingTrain
 
 logger = logging.getLogger(__name__)
 
 
-class ICEPortalAPI(BlockingRestAPI):
+class ICEPortalAPI(ThreadedRestAPI):
     API_URL = "https://iceportal.de"
 
     @store('bap')
     @lru_cache
     def bap_service_status(self):
         return self.get("bap/api/bap-service-status").json()
 
@@ -95,64 +95,66 @@
             return
 
         self[f"connections_{station_id}"] = connections
         yield from connections
         return
 
 
-class ICEInternetAccessInterface(BlockingRestAPI, InternetAccessInterface, InternetMetricsInterface):
-    API_URL = 'https://login.wifionice.de'
+class ICEPortalInternetInterface(InternetAccessInterface, InternetMetricsInterface):
+    _api: ICEPortalAPI
 
     def enable(self):
         """WIP: DOES NOT WORK YET!"""
-        soup = BeautifulSoup(self.get('de').text, 'html.parser')
+        response = self._api.get('de')
+        soup = BeautifulSoup(response.text, 'html.parser')
 
         # Check if the user is already online
         if soup.find(id='accept') is None:
             return
 
         # User is offline
-        logger.info('Cookie: %s', self._session.cookies['csrf'])
-        response = self.post('de', json={
-            'CSRFToken': self._session.cookies['csrf'],
+        logger.info('Cookie: %s', response.cookies['csrf'])
+        response = self._api.post('de', json={
+            'CSRFToken': response.cookies['csrf'],
             'login': True,
         })
         response.raise_for_status()
 
         # Check if login was successful
         if not (response.is_redirect and response.url.startswith(ICEPortalAPI.API_URL)):
             raise ConnectionError('Login failed!')
 
     def disable(self):
         """WIP: DOES NOT WORK YET!"""
-        soup = BeautifulSoup(self.get('de').text, 'html.parser')
+        response = self._api.get('de')
+        soup = BeautifulSoup(response.text, 'html.parser')
 
         # Check if user is already offline
         if soup.find(id='accept') is not None:
             return
 
         # User is online
-        response = self.post('de', json={
-            'CSRFToken': self._session.cookies['csrf'],
+        response = self._api.post('de', json={
+            'CSRFToken': response.cookies['csrf'],
             'logout': True,
         })
         response.raise_for_status()
 
         # Check if logout was successful
         if BeautifulSoup(response.text, 'html.parser').find(id='accept', recursive=True) is None:
             raise ConnectionError('Logout failed!')
 
     @property
     def is_enabled(self) -> bool:
         return BeautifulSoup(
-            self.get('de').text, 'html.parser'
+            self._api.get('de').text, 'html.parser'
         ).find(id='accept') is None
 
     def limit(self) -> float | None:
-        usage_info = self.get('usage_info')
+        usage_info = self._api.get('usage_info')
         if usage_info.status_code == HTTPStatus.NOT_IMPLEMENTED:
             return None
         return usage_info.json()['limit']  # TODO min api version = 14?
 
 
 class ModeOfTransport(Enum):
     UNKNOWN = 'UNKNOWN'
@@ -173,16 +175,16 @@
         return self.HIGH_SPEED_TRAIN, self.REGIONAL_TRAIN, self.INTER_REGIONAL_TRAIN
 
     @property
     def trains(self) -> tuple[ModeOfTransport, ...]:
         return self.local_trains + self.long_distance_trains
 
 
-class ZugPortalAPI(BlockingRestAPI):
-    API_URL = "https://zugportal.de"
+class RegioGuideAPI(BlockingRestAPI):
+    API_URL = "https://regio-guide.de"
 
     @store('journey')
     def journey(self):
         return self.get("@prd/zupo-travel-information/api/public/ri/journey").json()
 
     def refresh(self) -> None:
         self.journey()
@@ -225,7 +227,11 @@
                     actual=item['platform'],
                 ),
                 vehicle_type=item['train']['category'],
             )
             for item
             in departure_board.get('items', [])
         )
+
+
+ZugPortalAPI = RegioGuideAPI
+"""Renamed by DB. Use RegioGuideAPI instead."""
```

### Comparing `onboardapis-2.0.0rc1/onboardapis/train/de/db/mappings.py` & `onboardapis-2.0.0rc2/onboardapis/train/de/db/mappings.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc1/onboardapis/train/de/flix/apis.py` & `onboardapis-2.0.0rc2/onboardapis/train/de/flix/apis.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc1/onboardapis/train/de/me/apis.py` & `onboardapis-2.0.0rc2/onboardapis/train/de/me/apis.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc1/onboardapis/train/de/me/interfaces.py` & `onboardapis-2.0.0rc2/onboardapis/train/de/me/interfaces.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 import logging
 
 from bs4 import BeautifulSoup
 
 from ....exceptions import APIConnectionError
-from ....data import BlockingRestAPI, InternetAccessInterface
+from ....data import BlockingRestAPI
+from ....mixins import InternetAccessInterface
 
 logger = logging.getLogger(__name__)
 
 
 class MetronomAPI(BlockingRestAPI):
     # noinspection HttpUrlsUsage
     API_URL = 'http://wifi.metronom.de'
```

### Comparing `onboardapis-2.0.0rc1/onboardapis/train/fr/sncf/apis.py` & `onboardapis-2.0.0rc2/onboardapis/train/fr/sncf/apis.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc1/onboardapis/train/fr/sncf/interfaces.py` & `onboardapis-2.0.0rc2/onboardapis/train/fr/sncf/interfaces.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc1/onboardapis/train/it/ti/apis.py` & `onboardapis-2.0.0rc2/onboardapis/train/it/ti/apis.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc1/onboardapis/train/it/ti/interfaces.py` & `onboardapis-2.0.0rc2/onboardapis/train/it/ti/interfaces.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc1/onboardapis/train/third_party/unwired/apis.py` & `onboardapis-2.0.0rc2/onboardapis/train/third_party/unwired/apis.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from __future__ import annotations
 
 import logging
 import re
 
-from abc import ABCMeta
-from datetime import datetime, timedelta
-
 from ....mixins import InternetAccessMixin
 from ....data import ID
 from ... import Train
-from .interfaces import GenericUnwiredAPI
+from .interfaces import GenericUnwiredAPI, GenericUnwiredInternetAccessInterface
 
 logger = logging.getLogger(__name__)
 
 
 class GenericUnwiredTrain(Train, InternetAccessMixin):
     _api: GenericUnwiredAPI
+    _internet_access: GenericUnwiredInternetAccessInterface
 
     def __init__(self):
+        if not hasattr(self, '_api'):
+            self._api = GenericUnwiredAPI()
+        if not hasattr(self, '_internet_access'):
+            self._internet_access = GenericUnwiredInternetAccessInterface(self._api)
         Train.__init__(self)
         InternetAccessMixin.__init__(self)
 
     @property
     def id(self) -> ID:
         return self._api['journey']['id']
```

### Comparing `onboardapis-2.0.0rc1/onboardapis/train/third_party/unwired/interfaces.py` & `onboardapis-2.0.0rc2/onboardapis/train/third_party/unwired/interfaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import ClassVar
 from urllib.parse import parse_qs, urlparse
 
 from gql import gql
 
 from ....exceptions import InitialConnectionError
 from ....data import ThreadedGraphQlAPI, get_package_version
+from ....mixins import InternetAccessInterface
 
 logger = logging.getLogger(__name__)
 
 
 class GenericUnwiredAPI(ThreadedGraphQlAPI):
     API_URL = 'https://wasabi-splashpage.wifi.unwired.at/api/graphql'
     UNWIRED_GRAPHQL_QUERY: ClassVar[str] = '''
@@ -183,23 +184,33 @@
         ThreadedGraphQlAPI.__init__(self)
         try:
             response = requests.get(
                 'https://unwired.info/?source=wasabi',
                 headers={'User-Agent': 'Python/onboardapis (%s)' % get_package_version()}
             )
             self._user_session_id, *_ = parse_qs(urlparse(response.url).query)['user_session_id']
-            self.refresh()
         except (ConnectionError, KeyError) as e:
             raise InitialConnectionError from e
 
     def refresh(self) -> None:
         response = self.execute(
             document=gql(self.UNWIRED_GRAPHQL_QUERY),
             variable_values={
                 "widget_id": "363a8707-5e3e-4a5b-b565-9d22470dfd25",
                 "language": "de",
                 "user_session_id": self._user_session_id,
             }
         )
 
         journey = json.loads(response['feed_widget']['widget']['json'])
-        self._data['journey'] = journey['course']
+        self._data['journey'] = (
+            {} if 'content' in journey.keys()  # No journey info found for your location!
+            else journey['course']
+        )
+
+
+class GenericUnwiredInternetAccessInterface(InternetAccessInterface):
+    def enable(self) -> None:  # TODO: implement
+        pass
+
+    def disable(self) -> None:  # TODO: implement
+        pass
```

### Comparing `onboardapis-2.0.0rc1/onboardapis/train/third_party/unwired/mixins.py` & `onboardapis-2.0.0rc2/onboardapis/train/third_party/unwired/mixins.py`

 * *Files 13% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             )
             for station in self._api['journey']['stops']
         }
 
     @property
     def current_station(self) -> TrainStation:
         station, *_ = filter(
-            lambda s: self.now() < s.arrival.actual,
+            lambda s: self.now < s.arrival.actual,
             filter(
                 lambda s: s.arrival.actual is not None,
                 self.stations
             )
         )
         return station
```

### Comparing `onboardapis-2.0.0rc1/onboardapis/units.py` & `onboardapis-2.0.0rc2/onboardapis/units.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc1/onboardapis.egg-info/PKG-INFO` & `onboardapis-2.0.0rc2/onboardapis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: onboardapis
-Version: 2.0.0rc1
-Summary: A pure Python wrapper for the on-board APIs of many different transportation providers
+Version: 2.0.0rc2
+Summary: A pure Python wrapper for the on-board APIs of many different transportation providers.
 Author-email: Felix Zenk <felix.zenk@web.de>
 License: MIT
 Project-URL: Homepage, https://felix-zenk.github.io/onboardapis
-Project-URL: Source, https://github.com/felix-zenk/onboardapis
-Project-URL: Documentation, https://felix-zenk.github.io/onboardapis/docs/
+Project-URL: Documentation, https://felix-zenk.github.io/onboardapis/
+Project-URL: Repository, https://github.com/felix-zenk/onboardapis
 Project-URL: Issues, https://github.com/felix-zenk/onboardapis/issues
 Keywords: api,train,public-transport
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -29,14 +29,15 @@
 Requires-Dist: restfly>=1.4.7
 Requires-Dist: requests>=2.31.0
 Requires-Dist: beautifulsoup4>=4.12.2
 Requires-Dist: typing-extensions>=4.9.0
 Provides-Extra: dev
 Requires-Dist: flake8>=7.0.0; extra == "dev"
 Requires-Dist: pdoc>=14.4.0; extra == "dev"
+Requires-Dist: build>=1.2.1; extra == "dev"
 
 onboardapis
 ===
 
 [![Python versions](https://img.shields.io/pypi/pyversions/onboardapis)](https://pypi.org/project/onboardapis)
 [![PyPI version](https://badge.fury.io/py/onboardapis.svg)](https://pypi.org/project/onboardapis)
 [![Build package](https://github.com/felix-zenk/onboardapis/actions/workflows/build.yml/badge.svg)](https://github.com/felix-zenk/onboardapis/actions/workflows/build.yml)
@@ -153,17 +154,17 @@
 > The name of a conversion function is the unit which will be the result of the conversion.
 > Different units can be passed to a conversion function as keywords.
 > Keywords can be combined to return the sum of the input units.
 
 ---
 
 ## Documentation
-[![Documentation status](https://img.shields.io/github/actions/workflow/status/felix-zenk/onboardapis/docs.yml?label=docs)](https://felix-zenk.github.io/onboardapis/docs/)
+[![GitHub-Pages](https://github.com/felix-zenk/onboardapis/actions/workflows/docs.yml/badge.svg)](https://felix-zenk.github.io/onboardapis/)
 
-#### Access the documentation on [GitHub-Pages](https://felix-zenk.github.io/onboardapis/docs/).
+#### Access the documentation on [GitHub-Pages](https://felix-zenk.github.io/onboardapis/).
 
 
 ## Supported APIs
 
 | API                   | [API scope](#api-scope) | Type  | Country      | Operator                                                                           |
 |-----------------------|-------------------------|-------|--------------|------------------------------------------------------------------------------------|
 | RailnetRegio          | geo                     | train | at (Austria) | obb (Österreichische Bundesbahnen)                                                 |
```

### Comparing `onboardapis-2.0.0rc1/onboardapis.egg-info/SOURCES.txt` & `onboardapis-2.0.0rc2/onboardapis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc1/pyproject.toml` & `onboardapis-2.0.0rc2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "onboardapis"
-description = "A pure Python wrapper for the on-board APIs of many different transportation providers"
-version = "2.0.0rc1"
+description = "A pure Python wrapper for the on-board APIs of many different transportation providers."
+version = "2.0.0rc2"
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.8"
 keywords = ["api", "train", "public-transport"]
 license = { text = "MIT" }
 authors = [
     { name = "Felix Zenk", email = "felix.zenk@web.de" },
 ]
@@ -36,20 +36,21 @@
     "Typing :: Typed",
 ]
 
 [project.optional-dependencies]
 dev = [
     "flake8>=7.0.0",
     "pdoc>=14.4.0",
+    "build>=1.2.1",
 ]
 
 [project.urls]
 Homepage = "https://felix-zenk.github.io/onboardapis"
-Source = "https://github.com/felix-zenk/onboardapis"
-Documentation = "https://felix-zenk.github.io/onboardapis/docs/"
+Documentation = "https://felix-zenk.github.io/onboardapis/"
+Repository = "https://github.com/felix-zenk/onboardapis"
 Issues = "https://github.com/felix-zenk/onboardapis/issues"
 
 [tool.setuptools.packages.find]
 include = ["onboardapis*"]
 
 [tool.setuptools.package-data]
 onboardapis = ["py.typed"]
```


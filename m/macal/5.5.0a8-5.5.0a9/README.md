# Comparing `tmp/macal-5.5.0a8.tar.gz` & `tmp/macal-5.5.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macal-5.5.0a8.tar", last modified: Fri Apr 26 14:56:30 2024, max compression
+gzip compressed data, was "macal-5.5.0a9.tar", last modified: Mon Apr 29 10:52:32 2024, max compression
```

## Comparing `macal-5.5.0a8.tar` & `macal-5.5.0a9.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-26 14:56:30.670874 macal-5.5.0a8/
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-26 14:56:30.660874 macal-5.5.0a8/.vscode/
--rw-r--r--   0 marco     (1000) marco     (1000)      540 2024-04-15 15:12:14.000000 macal-5.5.0a8/.vscode/launch.json
--rw-r--r--   0 marco     (1000) marco     (1000)       51 2024-04-15 15:12:14.000000 macal-5.5.0a8/.vscode/settings.json
--rw-r--r--   0 marco     (1000) marco     (1000)     1184 2024-03-22 12:04:18.000000 macal-5.5.0a8/LICENSE.txt
--rw-r--r--   0 marco     (1000) marco     (1000)      179 2024-04-16 17:31:53.000000 macal-5.5.0a8/MANIFEST.in
--rw-r--r--   0 marco     (1000) marco     (1000)    57180 2024-04-26 14:56:30.670874 macal-5.5.0a8/PKG-INFO
--rw-r--r--   0 marco     (1000) marco     (1000)    56335 2024-04-26 14:55:01.000000 macal-5.5.0a8/README.md
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-26 14:56:30.660874 macal-5.5.0a8/documentation/
--rw-r--r--   0 marco     (1000) marco     (1000)     7076 2024-04-15 15:03:44.000000 macal-5.5.0a8/documentation/history.txt
--rw-r--r--   0 marco     (1000) marco     (1000)     1037 2024-04-25 07:29:24.000000 macal-5.5.0a8/pyproject.toml
--rw-r--r--   0 marco     (1000) marco     (1000)       38 2024-04-26 14:56:30.670874 macal-5.5.0a8/setup.cfg
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-26 14:56:30.660874 macal-5.5.0a8/src/
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-26 14:56:30.660874 macal-5.5.0a8/src/macal/
--rw-r--r--   0 marco     (1000) marco     (1000)     1474 2024-04-26 14:56:03.000000 macal-5.5.0a8/src/macal/__about__.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:11:34.000000 macal-5.5.0a8/src/macal/__init__.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-26 14:56:30.670874 macal-5.5.0a8/src/macal/frontend/
--rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:10:27.000000 macal-5.5.0a8/src/macal/frontend/__init__.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-26 14:56:30.670874 macal-5.5.0a8/src/macal/frontend/ast/
--rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:13:42.000000 macal-5.5.0a8/src/macal/frontend/ast/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2568 2024-04-08 13:40:36.000000 macal-5.5.0a8/src/macal/frontend/ast/kind.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1892 2024-04-08 20:08:54.000000 macal-5.5.0a8/src/macal/frontend/ast/metadata.py
--rw-r--r--   0 marco     (1000) marco     (1000)    32164 2024-04-09 13:34:29.000000 macal-5.5.0a8/src/macal/frontend/ast/node.py
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 23:39:28.000000 macal-5.5.0a8/src/macal/frontend/ast/py.typed
--rw-r--r--   0 marco     (1000) marco     (1000)    20787 2024-04-15 14:41:47.000000 macal-5.5.0a8/src/macal/frontend/mlexer.py
--rw-r--r--   0 marco     (1000) marco     (1000)    49026 2024-04-16 21:09:39.000000 macal-5.5.0a8/src/macal/frontend/mparser.py
--rw-r--r--   0 marco     (1000) marco     (1000)     5053 2024-04-16 15:52:59.000000 macal-5.5.0a8/src/macal/frontend/mparserstate.py
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 16:29:45.000000 macal-5.5.0a8/src/macal/frontend/py.typed
--rw-r--r--   0 marco     (1000) marco     (1000)     5623 2024-04-18 13:45:52.000000 macal-5.5.0a8/src/macal/macal.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2172 2024-04-08 15:16:25.000000 macal-5.5.0a8/src/macal/mexceptions.py
--rw-r--r--   0 marco     (1000) marco     (1000)    16383 2024-04-26 09:49:29.000000 macal-5.5.0a8/src/macal/mrepl.py
--rw-r--r--   0 marco     (1000) marco     (1000)     7436 2024-04-15 17:26:42.000000 macal-5.5.0a8/src/macal/mrun.py
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 16:29:34.000000 macal-5.5.0a8/src/macal/py.typed
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-26 14:56:30.670874 macal-5.5.0a8/src/macal/runtime/
--rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:10:21.000000 macal-5.5.0a8/src/macal/runtime/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)     9289 2024-04-16 15:54:17.000000 macal-5.5.0a8/src/macal/runtime/menvironment.py
--rw-r--r--   0 marco     (1000) marco     (1000)     4011 2024-04-10 20:55:22.000000 macal-5.5.0a8/src/macal/runtime/mimporter.py
--rw-r--r--   0 marco     (1000) marco     (1000)    72797 2024-04-18 13:35:19.000000 macal-5.5.0a8/src/macal/runtime/minterpreter.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-26 14:56:30.670874 macal-5.5.0a8/src/macal/runtime/native/
--rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-23 23:21:40.000000 macal-5.5.0a8/src/macal/runtime/native/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-24 20:22:17.000000 macal-5.5.0a8/src/macal/runtime/native/py.typed
--rw-r--r--   0 marco     (1000) marco     (1000)     2129 2024-04-15 14:35:04.000000 macal-5.5.0a8/src/macal/runtime/native/system.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1618 2024-03-24 06:01:49.000000 macal-5.5.0a8/src/macal/runtime/native/time.py
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-23 18:22:52.000000 macal-5.5.0a8/src/macal/runtime/py.typed
--rw-r--r--   0 marco     (1000) marco     (1000)     1705 2024-04-08 15:40:52.000000 macal-5.5.0a8/src/macal/runtime/value_type.py
--rw-r--r--   0 marco     (1000) marco     (1000)    17433 2024-04-11 16:42:19.000000 macal-5.5.0a8/src/macal/runtime/values.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-26 14:56:30.670874 macal-5.5.0a8/src/macal.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)    57180 2024-04-26 14:56:30.000000 macal-5.5.0a8/src/macal.egg-info/PKG-INFO
--rw-r--r--   0 marco     (1000) marco     (1000)     1563 2024-04-26 14:56:30.000000 macal-5.5.0a8/src/macal.egg-info/SOURCES.txt
--rw-r--r--   0 marco     (1000) marco     (1000)        1 2024-04-26 14:56:30.000000 macal-5.5.0a8/src/macal.egg-info/dependency_links.txt
--rw-r--r--   0 marco     (1000) marco     (1000)       66 2024-04-26 14:56:30.000000 macal-5.5.0a8/src/macal.egg-info/entry_points.txt
--rw-r--r--   0 marco     (1000) marco     (1000)       87 2024-04-26 14:56:30.000000 macal-5.5.0a8/src/macal.egg-info/requires.txt
--rw-r--r--   0 marco     (1000) marco     (1000)        6 2024-04-26 14:56:30.000000 macal-5.5.0a8/src/macal.egg-info/top_level.txt
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-26 14:56:30.670874 macal-5.5.0a8/tests/
--rw-r--r--   0 marco     (1000) marco     (1000)     1030 2024-04-18 12:40:10.000000 macal-5.5.0a8/tests/agent.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-26 14:56:30.670874 macal-5.5.0a8/tests/lib/
--rw-r--r--   0 marco     (1000) marco     (1000)      639 2023-11-17 02:10:51.000000 macal-5.5.0a8/tests/lib/csv.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      996 2023-11-17 14:12:28.000000 macal-5.5.0a8/tests/lib/ext_csv.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2135 2024-04-04 21:12:11.000000 macal-5.5.0a8/tests/lib/ext_io.py
--rw-r--r--   0 marco     (1000) marco     (1000)      873 2023-11-17 14:12:28.000000 macal-5.5.0a8/tests/lib/ext_keyring.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2265 2023-11-17 14:12:28.000000 macal-5.5.0a8/tests/lib/ext_math.py
--rw-r--r--   0 marco     (1000) marco     (1000)     3810 2024-04-09 08:23:31.000000 macal-5.5.0a8/tests/lib/ext_strings.py
--rw-r--r--   0 marco     (1000) marco     (1000)     4601 2023-11-17 14:12:28.000000 macal-5.5.0a8/tests/lib/ext_syslog.py
--rw-r--r--   0 marco     (1000) marco     (1000)     4082 2024-04-10 19:30:13.000000 macal-5.5.0a8/tests/lib/ext_system.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1910 2023-11-17 14:12:28.000000 macal-5.5.0a8/tests/lib/ext_time.py
--rw-r--r--   0 marco     (1000) marco     (1000)      942 2024-04-04 21:00:01.000000 macal-5.5.0a8/tests/lib/io.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      808 2023-11-17 02:12:56.000000 macal-5.5.0a8/tests/lib/keyring.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     1329 2024-04-05 15:54:51.000000 macal-5.5.0a8/tests/lib/math.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)    34808 2024-04-10 20:24:42.000000 macal-5.5.0a8/tests/lib/meraki_api_library_v1.py
--rw-r--r--   0 marco     (1000) marco     (1000)     5577 2024-04-10 20:38:33.000000 macal-5.5.0a8/tests/lib/meraki_v1.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     2047 2023-11-27 14:53:48.000000 macal-5.5.0a8/tests/lib/strings.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      661 2023-11-17 02:14:43.000000 macal-5.5.0a8/tests/lib/syslog.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     2923 2024-04-18 14:01:00.000000 macal-5.5.0a8/tests/lib/system.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      991 2023-11-17 02:16:00.000000 macal-5.5.0a8/tests/lib/time.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     5867 2024-04-09 23:07:14.000000 macal-5.5.0a8/tests/test.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-29 10:52:32.805925 macal-5.5.0a9/
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-29 10:52:32.795925 macal-5.5.0a9/.vscode/
+-rw-r--r--   0 marco     (1000) marco     (1000)      540 2024-04-15 15:12:14.000000 macal-5.5.0a9/.vscode/launch.json
+-rw-r--r--   0 marco     (1000) marco     (1000)       51 2024-04-15 15:12:14.000000 macal-5.5.0a9/.vscode/settings.json
+-rw-r--r--   0 marco     (1000) marco     (1000)     1184 2024-03-22 12:04:18.000000 macal-5.5.0a9/LICENSE.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)      179 2024-04-16 17:31:53.000000 macal-5.5.0a9/MANIFEST.in
+-rw-r--r--   0 marco     (1000) marco     (1000)    57180 2024-04-29 10:52:32.805925 macal-5.5.0a9/PKG-INFO
+-rw-r--r--   0 marco     (1000) marco     (1000)    56335 2024-04-26 14:55:01.000000 macal-5.5.0a9/README.md
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-29 10:52:32.795925 macal-5.5.0a9/documentation/
+-rw-r--r--   0 marco     (1000) marco     (1000)     7076 2024-04-15 15:03:44.000000 macal-5.5.0a9/documentation/history.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)     1037 2024-04-25 07:29:24.000000 macal-5.5.0a9/pyproject.toml
+-rw-r--r--   0 marco     (1000) marco     (1000)       38 2024-04-29 10:52:32.805925 macal-5.5.0a9/setup.cfg
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-29 10:52:32.795925 macal-5.5.0a9/src/
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-29 10:52:32.795925 macal-5.5.0a9/src/macal/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1474 2024-04-29 10:48:54.000000 macal-5.5.0a9/src/macal/__about__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:11:34.000000 macal-5.5.0a9/src/macal/__init__.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-29 10:52:32.795925 macal-5.5.0a9/src/macal/frontend/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:10:27.000000 macal-5.5.0a9/src/macal/frontend/__init__.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-29 10:52:32.795925 macal-5.5.0a9/src/macal/frontend/ast/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:13:42.000000 macal-5.5.0a9/src/macal/frontend/ast/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2568 2024-04-08 13:40:36.000000 macal-5.5.0a9/src/macal/frontend/ast/kind.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1892 2024-04-08 20:08:54.000000 macal-5.5.0a9/src/macal/frontend/ast/metadata.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    32164 2024-04-09 13:34:29.000000 macal-5.5.0a9/src/macal/frontend/ast/node.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 23:39:28.000000 macal-5.5.0a9/src/macal/frontend/ast/py.typed
+-rw-r--r--   0 marco     (1000) marco     (1000)    20787 2024-04-15 14:41:47.000000 macal-5.5.0a9/src/macal/frontend/mlexer.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    49026 2024-04-16 21:09:39.000000 macal-5.5.0a9/src/macal/frontend/mparser.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     5053 2024-04-16 15:52:59.000000 macal-5.5.0a9/src/macal/frontend/mparserstate.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 16:29:45.000000 macal-5.5.0a9/src/macal/frontend/py.typed
+-rw-r--r--   0 marco     (1000) marco     (1000)     5589 2024-04-29 10:51:42.000000 macal-5.5.0a9/src/macal/macal.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2172 2024-04-08 15:16:25.000000 macal-5.5.0a9/src/macal/mexceptions.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    16383 2024-04-26 09:49:29.000000 macal-5.5.0a9/src/macal/mrepl.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     7436 2024-04-15 17:26:42.000000 macal-5.5.0a9/src/macal/mrun.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 16:29:34.000000 macal-5.5.0a9/src/macal/py.typed
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-29 10:52:32.795925 macal-5.5.0a9/src/macal/runtime/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:10:21.000000 macal-5.5.0a9/src/macal/runtime/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     9289 2024-04-16 15:54:17.000000 macal-5.5.0a9/src/macal/runtime/menvironment.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     4011 2024-04-10 20:55:22.000000 macal-5.5.0a9/src/macal/runtime/mimporter.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    72797 2024-04-18 13:35:19.000000 macal-5.5.0a9/src/macal/runtime/minterpreter.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-29 10:52:32.795925 macal-5.5.0a9/src/macal/runtime/native/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-23 23:21:40.000000 macal-5.5.0a9/src/macal/runtime/native/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-24 20:22:17.000000 macal-5.5.0a9/src/macal/runtime/native/py.typed
+-rw-r--r--   0 marco     (1000) marco     (1000)     2129 2024-04-15 14:35:04.000000 macal-5.5.0a9/src/macal/runtime/native/system.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1618 2024-03-24 06:01:49.000000 macal-5.5.0a9/src/macal/runtime/native/time.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-23 18:22:52.000000 macal-5.5.0a9/src/macal/runtime/py.typed
+-rw-r--r--   0 marco     (1000) marco     (1000)     1705 2024-04-08 15:40:52.000000 macal-5.5.0a9/src/macal/runtime/value_type.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    17433 2024-04-11 16:42:19.000000 macal-5.5.0a9/src/macal/runtime/values.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-29 10:52:32.805925 macal-5.5.0a9/src/macal.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)    57180 2024-04-29 10:52:32.000000 macal-5.5.0a9/src/macal.egg-info/PKG-INFO
+-rw-r--r--   0 marco     (1000) marco     (1000)     1563 2024-04-29 10:52:32.000000 macal-5.5.0a9/src/macal.egg-info/SOURCES.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)        1 2024-04-29 10:52:32.000000 macal-5.5.0a9/src/macal.egg-info/dependency_links.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)       66 2024-04-29 10:52:32.000000 macal-5.5.0a9/src/macal.egg-info/entry_points.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)       87 2024-04-29 10:52:32.000000 macal-5.5.0a9/src/macal.egg-info/requires.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)        6 2024-04-29 10:52:32.000000 macal-5.5.0a9/src/macal.egg-info/top_level.txt
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-29 10:52:32.795925 macal-5.5.0a9/tests/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1030 2024-04-18 12:40:10.000000 macal-5.5.0a9/tests/agent.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-29 10:52:32.805925 macal-5.5.0a9/tests/lib/
+-rw-r--r--   0 marco     (1000) marco     (1000)      639 2023-11-17 02:10:51.000000 macal-5.5.0a9/tests/lib/csv.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      996 2023-11-17 14:12:28.000000 macal-5.5.0a9/tests/lib/ext_csv.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2135 2024-04-04 21:12:11.000000 macal-5.5.0a9/tests/lib/ext_io.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      873 2023-11-17 14:12:28.000000 macal-5.5.0a9/tests/lib/ext_keyring.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2265 2023-11-17 14:12:28.000000 macal-5.5.0a9/tests/lib/ext_math.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     3810 2024-04-09 08:23:31.000000 macal-5.5.0a9/tests/lib/ext_strings.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     4601 2023-11-17 14:12:28.000000 macal-5.5.0a9/tests/lib/ext_syslog.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     4082 2024-04-10 19:30:13.000000 macal-5.5.0a9/tests/lib/ext_system.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1910 2023-11-17 14:12:28.000000 macal-5.5.0a9/tests/lib/ext_time.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      942 2024-04-04 21:00:01.000000 macal-5.5.0a9/tests/lib/io.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      808 2023-11-17 02:12:56.000000 macal-5.5.0a9/tests/lib/keyring.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     1329 2024-04-05 15:54:51.000000 macal-5.5.0a9/tests/lib/math.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)    34808 2024-04-10 20:24:42.000000 macal-5.5.0a9/tests/lib/meraki_api_library_v1.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     5577 2024-04-10 20:38:33.000000 macal-5.5.0a9/tests/lib/meraki_v1.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     2047 2023-11-27 14:53:48.000000 macal-5.5.0a9/tests/lib/strings.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      661 2023-11-17 02:14:43.000000 macal-5.5.0a9/tests/lib/syslog.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     2923 2024-04-18 14:01:00.000000 macal-5.5.0a9/tests/lib/system.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      991 2023-11-17 02:16:00.000000 macal-5.5.0a9/tests/lib/time.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     5867 2024-04-09 23:07:14.000000 macal-5.5.0a9/tests/test.py
```

### Comparing `macal-5.5.0a8/.vscode/launch.json` & `macal-5.5.0a9/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/LICENSE.txt` & `macal-5.5.0a9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/PKG-INFO` & `macal-5.5.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macal
-Version: 5.5.0a8
+Version: 5.5.0a9
 Summary: Macal DSL is used for collecting and transforming data from various sources.
 Author-email: Marco Caspers <SamaDevTeam@westcon.com>
 Project-URL: Homepage, https://github.com/Sama-Developer/macal
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `macal-5.5.0a8/README.md` & `macal-5.5.0a9/README.md`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/documentation/history.txt` & `macal-5.5.0a9/documentation/history.txt`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/pyproject.toml` & `macal-5.5.0a9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/src/macal/__about__.py` & `macal-5.5.0a9/src/macal/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,12 +25,12 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
 #
 # SPDX-License-Identifier: MIT
 #
 
-__version__ = "5.5.0.alpha.8"
+__version__ = "5.5.0.alpha.9"
 __author__ = "Marco Caspers"
 __email__ = "samadevteam@westcon.com"
 __copyright__ = "Copyright 2024 Westcon Sama Development Team"
 __license__ = "MIT License"
```

### Comparing `macal-5.5.0a8/src/macal/__init__.py` & `macal-5.5.0a9/src/macal/__init__.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/src/macal/frontend/__init__.py` & `macal-5.5.0a9/src/macal/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/src/macal/frontend/ast/__init__.py` & `macal-5.5.0a9/src/macal/frontend/ast/__init__.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/src/macal/frontend/ast/kind.py` & `macal-5.5.0a9/src/macal/frontend/ast/kind.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/src/macal/frontend/ast/metadata.py` & `macal-5.5.0a9/src/macal/frontend/ast/metadata.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/src/macal/frontend/ast/node.py` & `macal-5.5.0a9/src/macal/frontend/ast/node.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/src/macal/frontend/mlexer.py` & `macal-5.5.0a9/src/macal/frontend/mlexer.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/src/macal/frontend/mparser.py` & `macal-5.5.0a9/src/macal/frontend/mparser.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/src/macal/frontend/mparserstate.py` & `macal-5.5.0a9/src/macal/frontend/mparserstate.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/src/macal/macal.py` & `macal-5.5.0a9/src/macal/macal.py`

 * *Files 9% similar despite different names*

```diff
@@ -119,34 +119,32 @@
     def AssignVariable(self, name: str, value: Any) -> None:
         """Assign a value to a variable in the global environment."""
 
         self.__environment.AssignVar(
             name=name, value=self._convert(value, env=self.__environment), meta=None
         )
 
-    def Run(self, filename: str) -> None:
+    def Run(self, filename: str) -> IRuntimeValue:
         """Run a Macal file."""
         try:
-            self.RunUnsafe(filename=filename, debug=False)
+            return self.RunUnsafe(filename=filename, debug=False)
         except RuntimeErrorLC as e:
             print(f"{e}")
-            sys.exit(1)
         except SyntaxError as e:
             print(f"{e}")
-            sys.exit(1)
         except RuntimeError as e:
             print(f"{e}")
-            sys.exit(1)
+        # to keep the linter happy
+        return None  # type: ignore
 
-    def RunUnsafe(self, filename: str, debug: bool = False) -> None:
+    def RunUnsafe(self, filename: str, debug: bool = False) -> IRuntimeValue:
         """Run a Macal file in debug mode, without any crash protections."""
         with open(filename, "r") as f:
             source = f.read()
         self.__parser_state.filename = filename
         parser = Parser(filename)
         program = parser.ProduceAST(source, state=self.__parser_state, debug=debug)
         interpreter = Interpreter()
         for path in self._search_paths:
             interpreter.add_path(str(pathlib.Path(path).absolute()))
         ret = interpreter.evaluate(program, self.__environment)
-        if isinstance(ret, HaltValue):
-            sys.exit(ret.value.value)
+        return ret
```

### Comparing `macal-5.5.0a8/src/macal/mexceptions.py` & `macal-5.5.0a9/src/macal/mexceptions.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/src/macal/mrepl.py` & `macal-5.5.0a9/src/macal/mrepl.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/src/macal/mrun.py` & `macal-5.5.0a9/src/macal/mrun.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/src/macal/runtime/__init__.py` & `macal-5.5.0a9/src/macal/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/src/macal/runtime/menvironment.py` & `macal-5.5.0a9/src/macal/runtime/menvironment.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/src/macal/runtime/mimporter.py` & `macal-5.5.0a9/src/macal/runtime/mimporter.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/src/macal/runtime/minterpreter.py` & `macal-5.5.0a9/src/macal/runtime/minterpreter.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/src/macal/runtime/native/__init__.py` & `macal-5.5.0a9/src/macal/runtime/native/__init__.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/src/macal/runtime/native/system.py` & `macal-5.5.0a9/src/macal/runtime/native/system.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/src/macal/runtime/native/time.py` & `macal-5.5.0a9/src/macal/runtime/native/time.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/src/macal/runtime/value_type.py` & `macal-5.5.0a9/src/macal/runtime/value_type.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/src/macal/runtime/values.py` & `macal-5.5.0a9/src/macal/runtime/values.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/src/macal.egg-info/PKG-INFO` & `macal-5.5.0a9/src/macal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macal
-Version: 5.5.0a8
+Version: 5.5.0a9
 Summary: Macal DSL is used for collecting and transforming data from various sources.
 Author-email: Marco Caspers <SamaDevTeam@westcon.com>
 Project-URL: Homepage, https://github.com/Sama-Developer/macal
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `macal-5.5.0a8/src/macal.egg-info/SOURCES.txt` & `macal-5.5.0a9/src/macal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/tests/agent.py` & `macal-5.5.0a9/tests/agent.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/tests/lib/csv.mcl` & `macal-5.5.0a9/tests/lib/csv.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/tests/lib/ext_csv.py` & `macal-5.5.0a9/tests/lib/ext_csv.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/tests/lib/ext_io.py` & `macal-5.5.0a9/tests/lib/ext_io.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/tests/lib/ext_keyring.py` & `macal-5.5.0a9/tests/lib/ext_keyring.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/tests/lib/ext_math.py` & `macal-5.5.0a9/tests/lib/ext_math.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/tests/lib/ext_strings.py` & `macal-5.5.0a9/tests/lib/ext_strings.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/tests/lib/ext_syslog.py` & `macal-5.5.0a9/tests/lib/ext_syslog.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/tests/lib/ext_system.py` & `macal-5.5.0a9/tests/lib/ext_system.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/tests/lib/ext_time.py` & `macal-5.5.0a9/tests/lib/ext_time.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/tests/lib/io.mcl` & `macal-5.5.0a9/tests/lib/io.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/tests/lib/keyring.mcl` & `macal-5.5.0a9/tests/lib/keyring.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/tests/lib/math.mcl` & `macal-5.5.0a9/tests/lib/math.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/tests/lib/meraki_api_library_v1.py` & `macal-5.5.0a9/tests/lib/meraki_api_library_v1.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/tests/lib/meraki_v1.mcl` & `macal-5.5.0a9/tests/lib/meraki_v1.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/tests/lib/strings.mcl` & `macal-5.5.0a9/tests/lib/strings.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/tests/lib/syslog.mcl` & `macal-5.5.0a9/tests/lib/syslog.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/tests/lib/system.mcl` & `macal-5.5.0a9/tests/lib/system.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/tests/lib/time.mcl` & `macal-5.5.0a9/tests/lib/time.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a8/tests/test.py` & `macal-5.5.0a9/tests/test.py`

 * *Files identical despite different names*


# Comparing `tmp/aurora_cli-2.5.1.0.tar.gz` & `tmp/aurora_cli-2.6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aurora_cli-2.5.1.0.tar", last modified: Sun Apr 28 14:28:31 2024, max compression
+gzip compressed data, was "aurora_cli-2.6.0.0.tar", last modified: Thu May  2 18:27:35 2024, max compression
```

## Comparing `aurora_cli-2.5.1.0.tar` & `aurora_cli-2.6.0.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 14:28:31.636833 aurora_cli-2.5.1.0/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)    11358 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/LICENSE
--rw-r--r--   0 keygenqt  (1000) keygenqt  (1000)     1474 2024-04-28 14:28:31.635833 aurora_cli-2.5.1.0/PKG-INFO
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1260 2024-04-27 18:28:50.000000 aurora_cli-2.5.1.0/README.md
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 14:28:31.630833 aurora_cli-2.5.1.0/aurora_cli/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2177 2024-04-28 08:53:15.000000 aurora_cli-2.5.1.0/aurora_cli/__main__.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 14:28:31.631833 aurora_cli-2.5.1.0/aurora_cli/src/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/__init__.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 14:28:31.631833 aurora_cli-2.5.1.0/aurora_cli/src/features/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/__init__.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 14:28:31.631833 aurora_cli-2.5.1.0/aurora_cli/src/features/devices/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/devices/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3695 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/devices/group_device.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3206 2024-04-27 18:28:50.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/devices/group_emulator.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     6158 2024-04-28 08:53:15.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/devices/group_emulator_vm.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 14:28:31.631833 aurora_cli-2.5.1.0/aurora_cli/src/features/devices/impl/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/devices/impl/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3478 2024-04-27 18:28:50.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/devices/impl/common.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2900 2024-04-27 18:28:50.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/devices/impl/utils.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 14:28:31.632833 aurora_cli-2.5.1.0/aurora_cli/src/features/flutter/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/flutter/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4015 2024-04-27 18:28:50.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/flutter/group_flutter.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4846 2024-04-28 08:53:15.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/flutter/group_flutter_build.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1013 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/flutter/group_flutter_debug.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     7772 2024-04-28 14:23:20.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/flutter/group_flutter_debug_dart.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4115 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/flutter/group_flutter_debug_gdb.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2039 2024-04-27 18:28:50.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/flutter/group_flutter_icon.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     5129 2024-04-27 18:28:50.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/flutter/group_flutter_plugins.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 14:28:31.632833 aurora_cli-2.5.1.0/aurora_cli/src/features/flutter/impl/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/flutter/impl/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)    24329 2024-04-28 13:49:56.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/flutter/impl/utils.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 14:28:31.633833 aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1958 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/group_psdk.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1078 2024-04-27 18:28:50.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/group_psdk_available.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1945 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/group_psdk_clear.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     5457 2024-04-27 18:28:50.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/group_psdk_install.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1165 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/group_psdk_installed.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4767 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/group_psdk_package.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1542 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/group_psdk_remove.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2994 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/group_psdk_sign.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1977 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/group_psdk_sudoers.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1351 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/group_psdk_targets.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2248 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/group_psdk_validate.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 14:28:31.633833 aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/impl/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/impl/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     8046 2024-04-28 08:53:15.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/impl/utils.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 14:28:31.634833 aurora_cli-2.5.1.0/aurora_cli/src/features/sdk/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/sdk/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4011 2024-04-27 18:28:50.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/sdk/group_sdk.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 14:28:31.634833 aurora_cli-2.5.1.0/aurora_cli/src/features/sdk/impl/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/sdk/impl/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2597 2024-04-27 18:28:50.000000 aurora_cli-2.5.1.0/aurora_cli/src/features/sdk/impl/utils.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 14:28:31.635833 aurora_cli-2.5.1.0/aurora_cli/src/support/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/support/__init__.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 14:28:31.635833 aurora_cli-2.5.1.0/aurora_cli/src/support/alive_bar/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/support/alive_bar/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2413 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/support/alive_bar/git_progress_alive_bar.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1499 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/support/alive_bar/progress_alive_bar.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     7080 2024-04-28 14:26:56.000000 aurora_cli-2.5.1.0/aurora_cli/src/support/conf.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1291 2024-04-28 14:22:58.000000 aurora_cli-2.5.1.0/aurora_cli/src/support/dependency.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1979 2024-04-27 18:28:50.000000 aurora_cli-2.5.1.0/aurora_cli/src/support/dependency_required.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3096 2024-04-27 18:28:50.000000 aurora_cli-2.5.1.0/aurora_cli/src/support/download.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     7232 2024-04-27 18:28:50.000000 aurora_cli-2.5.1.0/aurora_cli/src/support/helper.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1965 2024-03-16 15:04:33.000000 aurora_cli-2.5.1.0/aurora_cli/src/support/output.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1531 2024-04-27 18:28:50.000000 aurora_cli-2.5.1.0/aurora_cli/src/support/sdk.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     5097 2024-04-27 18:28:50.000000 aurora_cli-2.5.1.0/aurora_cli/src/support/ssh.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)    17907 2024-04-28 14:20:11.000000 aurora_cli-2.5.1.0/aurora_cli/src/support/texts.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2119 2024-04-27 18:28:50.000000 aurora_cli-2.5.1.0/aurora_cli/src/support/vbox.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2098 2024-04-27 18:28:50.000000 aurora_cli-2.5.1.0/aurora_cli/src/support/versions.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-04-28 14:28:31.635833 aurora_cli-2.5.1.0/aurora_cli.egg-info/
--rw-r--r--   0 keygenqt  (1000) keygenqt  (1000)     1474 2024-04-28 14:28:31.000000 aurora_cli-2.5.1.0/aurora_cli.egg-info/PKG-INFO
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2623 2024-04-28 14:28:31.000000 aurora_cli-2.5.1.0/aurora_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        1 2024-04-28 14:28:31.000000 aurora_cli-2.5.1.0/aurora_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       56 2024-04-28 14:28:31.000000 aurora_cli-2.5.1.0/aurora_cli.egg-info/entry_points.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)      168 2024-04-28 14:28:31.000000 aurora_cli-2.5.1.0/aurora_cli.egg-info/requires.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       18 2024-04-28 14:28:31.000000 aurora_cli-2.5.1.0/aurora_cli.egg-info/top_level.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       38 2024-04-28 14:28:31.636833 aurora_cli-2.5.1.0/setup.cfg
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1823 2024-04-28 14:26:51.000000 aurora_cli-2.5.1.0/setup.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.517164 aurora_cli-2.6.0.0/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)    11358 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/LICENSE
+-rw-r--r--   0 keygenqt  (1000) keygenqt  (1000)     1474 2024-05-02 18:27:35.517164 aurora_cli-2.6.0.0/PKG-INFO
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1260 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/README.md
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.509164 aurora_cli-2.6.0.0/aurora_cli/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2177 2024-04-28 08:53:15.000000 aurora_cli-2.6.0.0/aurora_cli/__main__.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.509164 aurora_cli-2.6.0.0/aurora_cli/src/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/__init__.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.509164 aurora_cli-2.6.0.0/aurora_cli/src/features/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/__init__.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.509164 aurora_cli-2.6.0.0/aurora_cli/src/features/devices/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/devices/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3695 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/devices/group_device.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3206 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/devices/group_emulator.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     6158 2024-04-28 08:53:15.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/devices/group_emulator_vm.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.513164 aurora_cli-2.6.0.0/aurora_cli/src/features/devices/impl/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/devices/impl/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3478 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/devices/impl/common.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2900 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/devices/impl/utils.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.513164 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4015 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4846 2024-04-28 08:53:15.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_build.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1013 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_debug.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     7772 2024-04-28 14:23:20.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_debug_dart.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4481 2024-05-02 18:22:53.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_debug_gdb.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2039 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_icon.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     5129 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_plugins.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.513164 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/impl/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/impl/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)    24329 2024-04-28 13:49:56.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/impl/utils.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.513164 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1958 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1078 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_available.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1945 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_clear.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     5457 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_install.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1165 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_installed.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4767 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_package.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1542 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_remove.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2994 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_sign.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1977 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_sudoers.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1351 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_targets.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2248 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_validate.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.513164 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/impl/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/impl/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     8046 2024-04-28 08:53:15.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/impl/utils.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.513164 aurora_cli-2.6.0.0/aurora_cli/src/features/sdk/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/sdk/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4011 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/sdk/group_sdk.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.513164 aurora_cli-2.6.0.0/aurora_cli/src/features/sdk/impl/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/sdk/impl/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2597 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/sdk/impl/utils.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.517164 aurora_cli-2.6.0.0/aurora_cli/src/support/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/__init__.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.517164 aurora_cli-2.6.0.0/aurora_cli/src/support/alive_bar/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/alive_bar/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2413 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/alive_bar/git_progress_alive_bar.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1499 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/alive_bar/progress_alive_bar.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     7080 2024-05-02 18:23:24.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/conf.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1291 2024-04-28 14:22:58.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/dependency.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1979 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/dependency_required.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3096 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/download.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     7232 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/helper.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1965 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/output.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1531 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/sdk.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     5097 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/ssh.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)    17907 2024-04-28 14:20:11.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/texts.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2119 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/vbox.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2098 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/versions.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.517164 aurora_cli-2.6.0.0/aurora_cli.egg-info/
+-rw-r--r--   0 keygenqt  (1000) keygenqt  (1000)     1474 2024-05-02 18:27:35.000000 aurora_cli-2.6.0.0/aurora_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2623 2024-05-02 18:27:35.000000 aurora_cli-2.6.0.0/aurora_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        1 2024-05-02 18:27:35.000000 aurora_cli-2.6.0.0/aurora_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       56 2024-05-02 18:27:35.000000 aurora_cli-2.6.0.0/aurora_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)      168 2024-05-02 18:27:35.000000 aurora_cli-2.6.0.0/aurora_cli.egg-info/requires.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       18 2024-05-02 18:27:35.000000 aurora_cli-2.6.0.0/aurora_cli.egg-info/top_level.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       38 2024-05-02 18:27:35.517164 aurora_cli-2.6.0.0/setup.cfg
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1823 2024-05-02 18:23:17.000000 aurora_cli-2.6.0.0/setup.py
```

### Comparing `aurora_cli-2.5.1.0/LICENSE` & `aurora_cli-2.6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/PKG-INFO` & `aurora_cli-2.6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aurora-cli
-Version: 2.5.1.0
+Version: 2.6.0.0
 Summary: An application that simplifies the life of an application developer for the Aurora OS.
 Home-page: https://github.com/keygenqt/aurora-cli
 Author: Vitaliy Zarubin
 Author-email: keygenqt@gmail.com
 Requires-Python: >=3.8.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aurora_cli-2.5.1.0/README.md` & `aurora_cli-2.6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/__main__.py` & `aurora_cli-2.6.0.0/aurora_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/devices/group_device.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/devices/group_device.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/devices/group_emulator.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/devices/group_emulator.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/devices/group_emulator_vm.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/devices/group_emulator_vm.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/devices/impl/common.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/devices/impl/common.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/devices/impl/utils.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/devices/impl/utils.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/flutter/group_flutter.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/flutter/group_flutter_build.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_build.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/flutter/group_flutter_debug.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_debug.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/flutter/group_flutter_debug_dart.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_debug_dart.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/flutter/group_flutter_debug_gdb.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_debug_gdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,38 +14,45 @@
 limitations under the License.
 """
 import os
 from pathlib import Path
 
 import click
 
-from aurora_cli.src.features.devices.impl.utils import device_ssh_select
+from aurora_cli.src.features.devices.impl.utils import device_ssh_select, emulator_ssh_select
 from aurora_cli.src.features.flutter.impl.utils import get_spec_keys, GDB_INIT_DATA, GDB_VSCODE_DATA
 from aurora_cli.src.support.conf import Conf
 from aurora_cli.src.support.dependency import check_dependency_vscode_plugin
 from aurora_cli.src.support.dependency_required import check_dependency_vscode, check_dependency_gdb_multiarch
 from aurora_cli.src.support.helper import pc_command, find_path_file
 from aurora_cli.src.support.output import VerboseType, echo_stdout, echo_stderr
 from aurora_cli.src.support.ssh import download_file_sftp, ssh_client_exec_command
 from aurora_cli.src.support.texts import AppTexts
 
 
 @click.group(name='gdb', invoke_without_command=True)
 @click.pass_context
 @click.option('-i', '--index', type=click.INT, help='Specify index device')
+@click.option('-p', '--port', type=click.INT, default=20000, help='Specify port for gdb server')
+@click.option('-e', '--emulator', is_flag=True, default=False, help="Run on emulator")
 @click.option('-v', '--verbose', is_flag=True, help='Detailed output')
-def group_flutter_debug_gdb(ctx: {}, index: int, verbose: bool):
+def group_flutter_debug_gdb(ctx: {}, index: int, port: int, emulator: bool, verbose: bool):
     """Project configure and run on device for gdb debug."""
 
-    port_gdb_server = 2345
+    workdir = ctx.obj.get_workdir()
 
     echo_stdout(AppTexts.preparing())
 
     # Get device client
-    client, data = device_ssh_select(ctx, index)
+    if emulator:
+        client = emulator_ssh_select(workdir=workdir)
+        device_ip = '127.0.0.1'
+    else:
+        client, data = device_ssh_select(ctx, index)
+        device_ip = data['ip']
 
     # Required dependency
     check_dependency_vscode()
     check_dependency_gdb_multiarch()
 
     # Install vscode extensions
     for extension in [
@@ -99,17 +106,17 @@
         print(GDB_INIT_DATA.format(package=package_name), file=file)
 
     # Create launch.json app flutter
     launch.unlink(missing_ok=True)
     with open(launch, 'w') as file:
         print(GDB_VSCODE_DATA.format(
             rmp_path=file_path,
-            ip=data['ip'],
-            port=port_gdb_server,
+            ip=device_ip,
+            port=port,
         ), file=file)
 
     # Run server
     ssh_client_exec_command(
         client,
-        'gdbserver --multi :{}'.format(port_gdb_server),
+        'gdbserver --multi :{}'.format(port),
         ctx.obj.get_type_output(verbose)
     )
```

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/flutter/group_flutter_icon.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_icon.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/flutter/group_flutter_plugins.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_plugins.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/flutter/impl/utils.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/impl/utils.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/group_psdk.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/group_psdk_available.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_available.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/group_psdk_clear.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_clear.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/group_psdk_install.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_install.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/group_psdk_installed.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_installed.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/group_psdk_package.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_package.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/group_psdk_remove.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_remove.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/group_psdk_sign.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_sign.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/group_psdk_sudoers.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_sudoers.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/group_psdk_targets.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_targets.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/group_psdk_validate.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_validate.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/psdk/impl/utils.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/impl/utils.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/sdk/group_sdk.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/sdk/group_sdk.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/features/sdk/impl/utils.py` & `aurora_cli-2.6.0.0/aurora_cli/src/features/sdk/impl/utils.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/support/alive_bar/git_progress_alive_bar.py` & `aurora_cli-2.6.0.0/aurora_cli/src/support/alive_bar/git_progress_alive_bar.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/support/alive_bar/progress_alive_bar.py` & `aurora_cli-2.6.0.0/aurora_cli/src/support/alive_bar/progress_alive_bar.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/support/conf.py` & `aurora_cli-2.6.0.0/aurora_cli/src/support/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 from aurora_cli.src.support.helper import get_path_file, get_request
 from aurora_cli.src.support.output import echo_stdout, VerboseType, echo_stderr
 from aurora_cli.src.support.texts import AppTexts
 
 # Data versions
 APP_NAME = 'aurora-cli'
-APP_VERSION = '2.5.1'
+APP_VERSION = '2.6.0'
 
 # Default path config
 PATH_CONF = '~/.aurora-cli/configuration.yaml'
 
 # Temp folder
 PATH_TEMP = '~/.aurora-cli/temp'
```

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/support/dependency.py` & `aurora_cli-2.6.0.0/aurora_cli/src/support/dependency.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/support/dependency_required.py` & `aurora_cli-2.6.0.0/aurora_cli/src/support/dependency_required.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/support/download.py` & `aurora_cli-2.6.0.0/aurora_cli/src/support/download.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/support/helper.py` & `aurora_cli-2.6.0.0/aurora_cli/src/support/helper.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/support/output.py` & `aurora_cli-2.6.0.0/aurora_cli/src/support/output.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/support/sdk.py` & `aurora_cli-2.6.0.0/aurora_cli/src/support/sdk.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/support/ssh.py` & `aurora_cli-2.6.0.0/aurora_cli/src/support/ssh.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/support/texts.py` & `aurora_cli-2.6.0.0/aurora_cli/src/support/texts.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/support/vbox.py` & `aurora_cli-2.6.0.0/aurora_cli/src/support/vbox.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli/src/support/versions.py` & `aurora_cli-2.6.0.0/aurora_cli/src/support/versions.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/aurora_cli.egg-info/PKG-INFO` & `aurora_cli-2.6.0.0/aurora_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aurora-cli
-Version: 2.5.1.0
+Version: 2.6.0.0
 Summary: An application that simplifies the life of an application developer for the Aurora OS.
 Home-page: https://github.com/keygenqt/aurora-cli
 Author: Vitaliy Zarubin
 Author-email: keygenqt@gmail.com
 Requires-Python: >=3.8.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aurora_cli-2.5.1.0/aurora_cli.egg-info/SOURCES.txt` & `aurora_cli-2.6.0.0/aurora_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.5.1.0/setup.py` & `aurora_cli-2.6.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 ```
 """
 
 setuptools.setup(
     name='aurora-cli',
-    version='2.5.1.0',
+    version='2.6.0.0',
     author='Vitaliy Zarubin',
     author_email='keygenqt@gmail.com',
     description='An application that simplifies the life of an application developer for the Aurora OS.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/keygenqt/aurora-cli",
     packages=setuptools.find_packages(exclude=['*tests.*', '*tests']),
```


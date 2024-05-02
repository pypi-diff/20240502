# Comparing `tmp/mozdevice-4.1.1.tar.gz` & `tmp/mozdevice-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mozdevice-4.1.1.tar", last modified: Fri Jul  7 16:56:55 2023, max compression
+gzip compressed data, was "mozdevice-4.1.2.tar", last modified: Thu May  2 09:06:03 2024, max compression
```

## Comparing `mozdevice-4.1.1.tar` & `mozdevice-4.1.2.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-07-07 16:56:55.000000 mozdevice-4.1.1/
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      439 2023-07-07 16:56:55.000000 mozdevice-4.1.1/PKG-INFO
-drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-07-07 16:56:55.000000 mozdevice-4.1.1/mozdevice/
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     6920 2023-03-10 23:28:57.000000 mozdevice-4.1.1/mozdevice/__init__.py
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)   182366 2023-03-10 23:28:57.000000 mozdevice-4.1.1/mozdevice/adb.py
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      376 2023-03-10 23:28:57.000000 mozdevice-4.1.1/mozdevice/adb_android.py
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)    10343 2023-03-10 23:28:57.000000 mozdevice-4.1.1/mozdevice/remote_process_monitor.py
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     1541 2023-03-10 23:28:57.000000 mozdevice-4.1.1/mozdevice/version_codes.py
-drwxrwxr-x   0 gbrown    (1000) gbrown    (1000)        0 2023-07-07 16:56:55.000000 mozdevice-4.1.1/mozdevice.egg-info/
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      439 2023-07-07 16:56:55.000000 mozdevice-4.1.1/mozdevice.egg-info/PKG-INFO
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)      377 2023-07-07 16:56:55.000000 mozdevice-4.1.1/mozdevice.egg-info/SOURCES.txt
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        1 2023-07-07 16:56:55.000000 mozdevice-4.1.1/mozdevice.egg-info/dependency_links.txt
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       37 2023-07-07 16:56:55.000000 mozdevice-4.1.1/mozdevice.egg-info/entry_points.txt
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)        1 2023-07-07 16:56:55.000000 mozdevice-4.1.1/mozdevice.egg-info/not-zip-safe
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       12 2023-07-07 16:56:55.000000 mozdevice-4.1.1/mozdevice.egg-info/requires.txt
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       10 2023-07-07 16:56:55.000000 mozdevice-4.1.1/mozdevice.egg-info/top_level.txt
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)       67 2023-07-07 16:56:55.000000 mozdevice-4.1.1/setup.cfg
--rw-rw-r--   0 gbrown    (1000) gbrown    (1000)     1075 2023-07-07 16:25:07.000000 mozdevice-4.1.1/setup.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2024-05-02 09:06:03.617632 mozdevice-4.1.2/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      420 2024-05-02 09:06:03.617632 mozdevice-4.1.2/PKG-INFO
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2024-05-02 09:06:03.616633 mozdevice-4.1.2/mozdevice/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     6920 2024-02-27 12:31:33.000000 mozdevice-4.1.2/mozdevice/__init__.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)   182234 2024-03-11 15:02:53.000000 mozdevice-4.1.2/mozdevice/adb.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      376 2024-02-27 12:31:33.000000 mozdevice-4.1.2/mozdevice/adb_android.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    10344 2024-02-27 12:31:33.000000 mozdevice-4.1.2/mozdevice/remote_process_monitor.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1541 2024-02-27 12:31:33.000000 mozdevice-4.1.2/mozdevice/version_codes.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2024-05-02 09:06:03.617632 mozdevice-4.1.2/mozdevice.egg-info/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      420 2024-05-02 09:06:03.000000 mozdevice-4.1.2/mozdevice.egg-info/PKG-INFO
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      458 2024-05-02 09:06:03.000000 mozdevice-4.1.2/mozdevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        1 2024-05-02 09:06:03.000000 mozdevice-4.1.2/mozdevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        1 2024-05-02 09:06:03.000000 mozdevice-4.1.2/mozdevice.egg-info/not-zip-safe
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       12 2024-05-02 09:06:03.000000 mozdevice-4.1.2/mozdevice.egg-info/requires.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       10 2024-05-02 09:06:03.000000 mozdevice-4.1.2/mozdevice.egg-info/top_level.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       67 2024-05-02 09:06:03.617632 mozdevice-4.1.2/setup.cfg
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1075 2024-05-01 13:08:14.000000 mozdevice-4.1.2/setup.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2024-05-02 09:06:03.617632 mozdevice-4.1.2/tests/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     2224 2024-02-27 12:31:33.000000 mozdevice-4.1.2/tests/test_chown.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      676 2024-02-27 12:31:33.000000 mozdevice-4.1.2/tests/test_escape_command_line.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1226 2024-02-27 12:31:33.000000 mozdevice-4.1.2/tests/test_is_app_installed.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     3868 2024-02-27 12:31:33.000000 mozdevice-4.1.2/tests/test_socket_connection.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mozdevice-4.1.1/mozdevice/__init__.py` & `mozdevice-4.1.2/mozdevice/__init__.py`

 * *Files identical despite different names*

### Comparing `mozdevice-4.1.1/mozdevice/adb.py` & `mozdevice-4.1.2/mozdevice/adb.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import shutil
 import signal
 import subprocess
 import sys
 import tempfile
 import time
 import traceback
-from distutils import dir_util
+from shutil import copytree
 from threading import Thread
 
 import six
 from six.moves import range
 
 from . import version_codes
 
@@ -1085,17 +1085,15 @@
                     if self.shell_output("su -c id", timeout=timeout).find(uid) != -1:
                         self._have_su = True
                         self._logger.info("su -c supported")
                 except ADBError as e:
                     self._logger.debug("Check for su -c failed: {}".format(e))
 
                 # Check if Android's su 0 command works.
-                # su 0 id will hang on Pixel 2 8.1.0/OPM2.171019.029.B1/4720900
-                # rooted via magisk. If we already have detected su -c support,
-                # we can skip this check.
+                # If we already have detected su -c support, we can skip this check.
                 try:
                     if (
                         not self._have_su
                         and self.shell_output("su 0 id", timeout=timeout).find(uid)
                         != -1
                     ):
                         self._have_android_su = True
@@ -2979,15 +2977,15 @@
             # force push to use the correct filename in the remote directory
             remote = posixpath.join(remote, os.path.basename(local))
         elif os.path.isdir(local):
             copy_required = True
             temp_parent = tempfile.mkdtemp()
             remote_name = os.path.basename(remote)
             new_local = os.path.join(temp_parent, remote_name)
-            dir_util.copy_tree(local, new_local)
+            copytree(local, new_local)
             local = new_local
             # See do_sync_push in
             # https://android.googlesource.com/platform/system/core/+/master/adb/file_sync_client.cpp
             # Work around change in behavior in adb 1.0.36 where if
             # the remote destination directory exists, adb push will
             # copy the source directory *into* the destination
             # directory otherwise it will copy the source directory
@@ -3132,15 +3130,15 @@
                     self.command_output(["pull", intermediate, local], timeout=timeout)
                 except ADBError as e:
                     self._logger.error("pull %s %s: %s" % (intermediate, local, str(e)))
                 finally:
                     self.rm(intermediate, recursive=True, force=True, timeout=timeout)
         finally:
             if copy_required:
-                dir_util.copy_tree(local, original_local)
+                copytree(local, original_local, dirs_exist_ok=True)
                 shutil.rmtree(temp_parent)
 
     def get_file(self, remote, offset=None, length=None, timeout=None):
         """Pull file from device and return the file's content
 
         :param str remote: The path of the remote file.
         :param offset: If specified, return only content beyond this offset.
@@ -4131,15 +4129,15 @@
             acmd.extend(["-a", intent])
 
         # Note that isinstance(True, int) and isinstance(False, int)
         # is True. This means we must test the type of the value
         # against bool prior to testing it against int in order to
         # prevent falsely identifying a bool value as an int.
         if extras:
-            for (key, val) in extras.items():
+            for key, val in extras.items():
                 if isinstance(val, bool):
                     extra_type_param = "--ez"
                 elif isinstance(val, int):
                     extra_type_param = "--ei"
                 else:
                     extra_type_param = "--es"
                 acmd.extend([extra_type_param, str(key), str(val)])
@@ -4192,15 +4190,15 @@
                  :exc:`ADBError`
         """
         extras = {}
 
         if moz_env:
             # moz_env is expected to be a dictionary of environment variables:
             # Fennec itself will set them when launched
-            for (env_count, (env_key, env_val)) in enumerate(moz_env.items()):
+            for env_count, (env_key, env_val) in enumerate(moz_env.items()):
                 extras["env" + str(env_count)] = env_key + "=" + env_val
 
         # Additional command line arguments that fennec will read and use (e.g.
         # with a custom profile)
         if extra_args:
             extras["args"] = " ".join(extra_args)
 
@@ -4257,21 +4255,21 @@
                  :exc:`ADBError`
         """
         extras = {}
 
         if moz_env:
             # moz_env is expected to be a dictionary of environment variables:
             # geckoview_example itself will set them when launched
-            for (env_count, (env_key, env_val)) in enumerate(moz_env.items()):
+            for env_count, (env_key, env_val) in enumerate(moz_env.items()):
                 extras["env" + str(env_count)] = env_key + "=" + env_val
 
         # Additional command line arguments that the app will read and use (e.g.
         # with a custom profile)
         if extra_args:
-            for (arg_count, arg) in enumerate(extra_args):
+            for arg_count, arg in enumerate(extra_args):
                 extras["arg" + str(arg_count)] = arg
 
         extras["use_multiprocess"] = e10s
         extras["out_file"] = out_file
         self.launch_application(
             app_name,
             "%s.%s" % (app_name, activity_name),
@@ -4325,21 +4323,21 @@
                  :exc:`ADBError`
         """
         extras = {}
 
         if moz_env:
             # moz_env is expected to be a dictionary of environment variables:
             # geckoview_example itself will set them when launched
-            for (env_count, (env_key, env_val)) in enumerate(moz_env.items()):
+            for env_count, (env_key, env_val) in enumerate(moz_env.items()):
                 extras["env" + str(env_count)] = env_key + "=" + env_val
 
         # Additional command line arguments that the app will read and use (e.g.
         # with a custom profile)
         if extra_args:
-            for (arg_count, arg) in enumerate(extra_args):
+            for arg_count, arg in enumerate(extra_args):
                 extras["arg" + str(arg_count)] = arg
 
         extras["use_multiprocess"] = e10s
         self.launch_application(
             app_name,
             "%s.%s" % (app_name, activity_name),
             intent,
```

### Comparing `mozdevice-4.1.1/mozdevice/remote_process_monitor.py` & `mozdevice-4.1.2/mozdevice/remote_process_monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                         self.last_test_seen = message["test"]
                     elif message.get("action") == "test_end":
                         self.last_test_seen = "{} (finished)".format(message["test"])
                     elif message.get("action") == "suite_end":
                         self.last_test_seen = "Last test finished"
                     elif message.get("action") == "log":
                         line = message["message"].strip()
-                        m = re.match(".*:\s*(\d*)", line)
+                        m = re.match(r".*:\s*(\d*)", line)
                         if m:
                             try:
                                 val = int(m.group(1))
                                 if "Passed:" in line:
                                     self.counts["pass"] += val
                                     self.last_test_seen = "Last test finished"
                                 elif "Failed:" in line:
```

### Comparing `mozdevice-4.1.1/mozdevice/version_codes.py` & `mozdevice-4.1.2/mozdevice/version_codes.py`

 * *Files identical despite different names*

### Comparing `mozdevice-4.1.1/setup.py` & `mozdevice-4.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
 from setuptools import setup
 
 PACKAGE_NAME = "mozdevice"
-PACKAGE_VERSION = "4.1.1"
+PACKAGE_VERSION = "4.1.2"
 
 deps = ["mozlog >= 6.0"]
 
 setup(
     name=PACKAGE_NAME,
     version=PACKAGE_VERSION,
     description="Mozilla-authored device management",
```


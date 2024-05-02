# Comparing `tmp/easyland-0.7.0.tar.gz` & `tmp/easyland-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyland-0.7.0.tar", last modified: Tue Apr 30 21:30:25 2024, max compression
+gzip compressed data, was "easyland-0.7.1.tar", last modified: Thu May  2 09:46:05 2024, max compression
```

## Comparing `easyland-0.7.0.tar` & `easyland-0.7.1.tar`

### file list

```diff
@@ -1,25 +1,21 @@
-drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-04-30 21:30:25.072284 easyland-0.7.0/
--rw-r--r--   0 ju        (1000) ju        (1000)     1066 2024-04-25 19:16:43.000000 easyland-0.7.0/LICENSE.txt
--rw-r--r--   0 ju        (1000) ju        (1000)     8934 2024-04-30 21:30:25.072284 easyland-0.7.0/PKG-INFO
--rw-r--r--   0 ju        (1000) ju        (1000)     8072 2024-04-26 21:14:52.000000 easyland-0.7.0/README.md
--rw-r--r--   0 ju        (1000) ju        (1000)      959 2024-04-30 15:54:01.000000 easyland-0.7.0/pyproject.toml
--rw-r--r--   0 ju        (1000) ju        (1000)       38 2024-04-30 21:30:25.072284 easyland-0.7.0/setup.cfg
-drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-04-30 21:30:25.068951 easyland-0.7.0/src/
-drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-04-30 21:30:25.068951 easyland-0.7.0/src/easyland/
--rw-r--r--   0 ju        (1000) ju        (1000)       68 2024-04-30 21:22:48.000000 easyland-0.7.0/src/easyland/__init__.py
--rw-r--r--   0 ju        (1000) ju        (1000)     1896 2024-04-30 21:25:33.000000 easyland-0.7.0/src/easyland/command.py
--rw-r--r--   0 ju        (1000) ju        (1000)      718 2024-04-30 21:25:58.000000 easyland-0.7.0/src/easyland/config.py
-drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-04-30 21:30:25.068951 easyland-0.7.0/src/easyland/configs/
--rw-r--r--   0 ju        (1000) ju        (1000)      501 2024-04-26 12:14:22.000000 easyland-0.7.0/src/easyland/configs/listener.py
--rw-r--r--   0 ju        (1000) ju        (1000)     1356 2024-04-30 10:22:55.000000 easyland-0.7.0/src/easyland/configs/myConfig.py
--rw-r--r--   0 ju        (1000) ju        (1000)     2561 2024-04-30 21:26:10.000000 easyland-0.7.0/src/easyland/daemon.py
--rw-r--r--   0 ju        (1000) ju        (1000)     2021 2024-04-30 21:26:24.000000 easyland-0.7.0/src/easyland/idle.py
--rw-r--r--   0 ju        (1000) ju        (1000)      234 2024-04-25 15:23:43.000000 easyland-0.7.0/src/easyland/log.py
--rwxr-xr-x   0 ju        (1000) ju        (1000)     1267 2024-04-30 21:25:17.000000 easyland-0.7.0/src/easyland/main.py
-drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-04-30 21:30:25.072284 easyland-0.7.0/src/easyland.egg-info/
--rw-r--r--   0 ju        (1000) ju        (1000)     8934 2024-04-30 21:30:25.000000 easyland-0.7.0/src/easyland.egg-info/PKG-INFO
--rw-r--r--   0 ju        (1000) ju        (1000)      477 2024-04-30 21:30:25.000000 easyland-0.7.0/src/easyland.egg-info/SOURCES.txt
--rw-r--r--   0 ju        (1000) ju        (1000)        1 2024-04-30 21:30:25.000000 easyland-0.7.0/src/easyland.egg-info/dependency_links.txt
--rw-r--r--   0 ju        (1000) ju        (1000)       48 2024-04-30 21:30:25.000000 easyland-0.7.0/src/easyland.egg-info/entry_points.txt
--rw-r--r--   0 ju        (1000) ju        (1000)       18 2024-04-30 21:30:25.000000 easyland-0.7.0/src/easyland.egg-info/requires.txt
--rw-r--r--   0 ju        (1000) ju        (1000)        9 2024-04-30 21:30:25.000000 easyland-0.7.0/src/easyland.egg-info/top_level.txt
+drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-02 09:46:05.306784 easyland-0.7.1/
+-rw-r--r--   0 ju        (1000) ju        (1000)     1066 2024-04-25 19:16:43.000000 easyland-0.7.1/LICENSE.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)    13317 2024-05-02 09:46:05.306784 easyland-0.7.1/PKG-INFO
+-rw-r--r--   0 ju        (1000) ju        (1000)    12446 2024-05-01 21:56:58.000000 easyland-0.7.1/README.md
+-rw-r--r--   0 ju        (1000) ju        (1000)      968 2024-05-01 21:54:38.000000 easyland-0.7.1/pyproject.toml
+-rw-r--r--   0 ju        (1000) ju        (1000)       38 2024-05-02 09:46:05.306784 easyland-0.7.1/setup.cfg
+drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-02 09:46:05.303451 easyland-0.7.1/src/
+drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-02 09:46:05.306784 easyland-0.7.1/src/easyland/
+-rw-r--r--   0 ju        (1000) ju        (1000)      142 2024-05-01 07:14:10.000000 easyland-0.7.1/src/easyland/__init__.py
+-rw-r--r--   0 ju        (1000) ju        (1000)     2405 2024-05-01 17:31:04.000000 easyland-0.7.1/src/easyland/command.py
+-rw-r--r--   0 ju        (1000) ju        (1000)     4656 2024-05-01 20:22:29.000000 easyland-0.7.1/src/easyland/daemon.py
+-rw-r--r--   0 ju        (1000) ju        (1000)     2229 2024-05-01 20:26:14.000000 easyland-0.7.1/src/easyland/idle.py
+-rw-r--r--   0 ju        (1000) ju        (1000)      236 2024-05-01 11:08:03.000000 easyland-0.7.1/src/easyland/log.py
+-rwxr-xr-x   0 ju        (1000) ju        (1000)     1245 2024-05-01 21:54:48.000000 easyland-0.7.1/src/easyland/main.py
+drwxr-xr-x   0 ju        (1000) ju        (1000)        0 2024-05-02 09:46:05.306784 easyland-0.7.1/src/easyland.egg-info/
+-rw-r--r--   0 ju        (1000) ju        (1000)    13317 2024-05-02 09:46:05.000000 easyland-0.7.1/src/easyland.egg-info/PKG-INFO
+-rw-r--r--   0 ju        (1000) ju        (1000)      388 2024-05-02 09:46:05.000000 easyland-0.7.1/src/easyland.egg-info/SOURCES.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)        1 2024-05-02 09:46:05.000000 easyland-0.7.1/src/easyland.egg-info/dependency_links.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)       48 2024-05-02 09:46:05.000000 easyland-0.7.1/src/easyland.egg-info/entry_points.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)       18 2024-05-02 09:46:05.000000 easyland-0.7.1/src/easyland.egg-info/requires.txt
+-rw-r--r--   0 ju        (1000) ju        (1000)        9 2024-05-02 09:46:05.000000 easyland-0.7.1/src/easyland.egg-info/top_level.txt
```

### Comparing `easyland-0.7.0/LICENSE.txt` & `easyland-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easyland-0.7.0/pyproject.toml` & `easyland-0.7.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "easyland"
-version = "0.7.0"
+version = "0.7.1"
 authors = [
     { name="Julien Pro", email="contact@julienpro.com"}
 ]
-description = "A python swiss-knife to manage wayand compositors like Hyprland"
+description = "A python swiss-knife to manage wayand compositors like Hyprland and Sway"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
     "pywayland>=0.4.17"
 ]
 classifiers = [
     "Intended Audience :: Developers",
```

### Comparing `easyland-0.7.0/src/easyland/command.py` & `easyland-0.7.1/src/easyland/command.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,20 +6,40 @@
 from easyland.log import logger
 
 class Command():
 
     def __init__(self):
         pass
 
-    def get_all_monitors(self):
-        monitors = self.hyprctl_command("monitors")
+    def sway_get_all_monitors(self):
+        monitors = self.exec("swaymsg -t get_outputs", decode_json = True)
         return monitors
     
-    def get_monitor(self, name = None, description = None, make = None, model = None):
-        monitors = self.get_all_monitors()
+    def sway_get_monitor(self, name = None, make = None, model = None):
+        monitors = self.sway_get_all_monitors()
+        for monitor in monitors:
+            if name is not None:
+                if name in monitor['name']:
+                    return monitor
+
+            if make is not None:
+                if make in monitor['make']:
+                    return monitor
+
+            if model is not None:
+                if model in monitor['model']:
+                    return monitor
+        return None
+
+    def hyprland_get_all_monitors(self):
+        monitors = self.exec("hyprctl -j monitors", decode_json = True)
+        return monitors
+    
+    def hyprland_get_monitor(self, name = None, description = None, make = None, model = None):
+        monitors = self.hyprland_get_all_monitors()
 
         for monitor in monitors:
             if name is not None:
                 if name in monitor['name']:
                     return monitor
 
             if description is not None:
@@ -31,33 +51,28 @@
                     return monitor
 
             if model is not None:
                 if model in monitor['model']:
                     return monitor
         return None
 
-    def hyprctl_command(self, command):
-        cmd = "hyprctl -j " + command
-        logger.info("Executing command: "+cmd) 
-        output = subprocess.check_output(cmd, shell=True)
-        decoded_output = output.decode("utf-8")
-        
-        try:
-            json_output = json.loads(decoded_output)
-        except json.decoder.JSONDecodeError as e:
-            return decoded_output
-        return json_output
-    
-    def shell_command(self, command):
-        command = command.strip()
-        if command.endswith('&'):
-            command = command[:-1]
+    def exec(self, command, background = False, decode_json = False):
+        if background:
             logger.info("Executing background command: "+command)
             with open(os.devnull, 'w') as fp:
                 subprocess.Popen(command, shell=True, stdout=fp)
+            return True
         else:
             logger.info("Executing command: "+command) 
             output = subprocess.check_output(command, shell=True)
             decoded_output = output.decode("utf-8")
-            return decoded_output
+            if decode_json:
+                try:
+                    json_output = json.loads(decoded_output)
+                except json.decoder.JSONDecodeError:
+                    return None
+                return json_output
+            else:
+                return decoded_output
+
```

### Comparing `easyland-0.7.0/src/easyland/idle.py` & `easyland-0.7.1/src/easyland/idle.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-import easyland.command as Command 
+# import .command as Command 
+from . import command
+from . import logger
 import subprocess
 import threading
 import os
 from pywayland.client import Display
 from pywayland.protocol.wayland.wl_seat import WlSeat
 from pywayland.protocol.ext_idle_notify_v1 import (
     ExtIdleNotificationV1,
     ExtIdleNotifierV1
 )
 
 class Idle():
     def __init__(self, config):
-        self.command = Command.Command()
+        # self.command = Command.Command()
+        self.command = command
         self._config = config
         self._display =  Display()
         self._display.connect()
         self._idle_notifier = None
         self._seat = None
         self._notifications = []
 
@@ -31,20 +34,22 @@
                 self._notifications[idx] = self._idle_notifier.get_idle_notification(c[0] * 1000, self._seat)
                 self._notifications[idx]._index = idx
                 self._notifications[idx].dispatcher['idled'] = self._idle_notifier_handler
                 self._notifications[idx].dispatcher['resumed'] = self._idle_notifier_resume_handler
 
     def _idle_notifier_handler(self, notification): 
         for command in self._config[notification._index][1]:
+            logger.info('Idle - Running command: ' + command)
             with open(os.devnull, 'w') as fp:
                 subprocess.Popen(command, shell=True, stdout=fp)
 
     def _idle_notifier_resume_handler(self, notification):
         if len(self._config[notification._index]) > 2:
             for command in self._config[notification._index][2]:
+                logger.info('Idle - Resuming: Running command: ' + command)
                 with open(os.devnull, 'w') as fp:
                     subprocess.Popen(command, shell=True, stdout=fp)
 
     def setup(self):
         reg = self._display.get_registry()
         reg.dispatcher['global'] = self._global_handler
         while True:
```

### Comparing `easyland-0.7.0/src/easyland/main.py` & `easyland-0.7.1/src/easyland/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 #!/usr/bin/env python3
 import argparse
 import importlib
 import importlib.util
 import importlib.machinery
 import sys
+import time
 import os
 from easyland.daemon import Daemon
 
-version = '0.7.0'
+version = '0.7.1'
 
 def import_from_path(path):
     module_name = os.path.basename(path).replace('-', '_').replace('.py', '')
     spec = importlib.util.spec_from_loader(module_name, importlib.machinery.SourceFileLoader(module_name, path))
     module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(module)
     sys.modules[module_name] = module
     return module
 
 def main():
 
-    parser = argparse.ArgumentParser(description="Easyland - A python swiss-knife to manage Wayland compositors like Hyprland")
-# parser.add_argument("-l", "--listen", action="store_true", help="Listen only")
+    parser = argparse.ArgumentParser(description="Easyland - A python swiss-knife to manage Wayland compositors like Hyprland and Sway")
     parser.add_argument("-c", "--config", help="Path to your config file")
     parser.add_argument("-v", "--version", action="store_true", help="Show the version")
     args = parser.parse_args()
 
     if args.version:
         print('Pyland version: ' + version)
         sys.exit()
 
     if not args.config:
         print('Please provide a config file with the option -c')
         sys.exit(1)
 
     config = import_from_path(args.config)
     daemon = Daemon(config)
+    while True:
+        time.sleep(1)
 
 if __name__ == '__main__':
     main()
```


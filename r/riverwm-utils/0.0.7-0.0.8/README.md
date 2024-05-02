# Comparing `tmp/riverwm-utils-0.0.7.tar.gz` & `tmp/riverwm-utils-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riverwm-utils-0.0.7.tar", last modified: Mon Jan 16 23:59:19 2023, max compression
+gzip compressed data, was "riverwm-utils-0.0.8.tar", last modified: Thu May  2 06:12:38 2024, max compression
```

## Comparing `riverwm-utils-0.0.7.tar` & `riverwm-utils-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 hastings  (1000) hastings  (1000)        0 2023-01-16 23:59:19.688981 riverwm-utils-0.0.7/
--rw-r--r--   0 hastings  (1000) hastings  (1000)     2984 2022-01-14 02:14:35.000000 riverwm-utils-0.0.7/.gitignore
--rw-r--r--   0 hastings  (1000) hastings  (1000)    35149 2022-01-14 02:36:29.000000 riverwm-utils-0.0.7/LICENSE
--rw-r--r--   0 hastings  (1000) hastings  (1000)     3058 2023-01-16 23:59:19.688981 riverwm-utils-0.0.7/PKG-INFO
--rw-r--r--   0 hastings  (1000) hastings  (1000)     2032 2022-12-22 00:52:44.000000 riverwm-utils-0.0.7/README.md
--rw-r--r--   0 hastings  (1000) hastings  (1000)       91 2022-01-14 01:30:15.000000 riverwm-utils-0.0.7/pyproject.toml
--rw-r--r--   0 hastings  (1000) hastings  (1000)       17 2022-01-14 02:50:48.000000 riverwm-utils-0.0.7/requirements.txt
-drwxr-xr-x   0 hastings  (1000) hastings  (1000)        0 2023-01-16 23:59:19.688981 riverwm-utils-0.0.7/riverwm_utils/
--rw-r--r--   0 hastings  (1000) hastings  (1000)        0 2022-01-14 01:28:58.000000 riverwm-utils-0.0.7/riverwm_utils/__init__.py
--rw-r--r--   0 hastings  (1000) hastings  (1000)     3679 2022-12-22 00:52:44.000000 riverwm-utils-0.0.7/riverwm_utils/river-control-unstable-v1.xml
--rw-r--r--   0 hastings  (1000) hastings  (1000)     6147 2022-12-22 00:52:44.000000 riverwm-utils-0.0.7/riverwm_utils/river-status-unstable-v1.xml
--rw-r--r--   0 hastings  (1000) hastings  (1000)     6366 2023-01-16 23:55:12.000000 riverwm-utils-0.0.7/riverwm_utils/riverwm_utils.py
--rw-r--r--   0 hastings  (1000) hastings  (1000)   140883 2022-12-22 00:52:44.000000 riverwm-utils-0.0.7/riverwm_utils/wayland.xml
-drwxr-xr-x   0 hastings  (1000) hastings  (1000)        0 2023-01-16 23:59:19.688981 riverwm-utils-0.0.7/riverwm_utils.egg-info/
--rw-r--r--   0 hastings  (1000) hastings  (1000)     3058 2023-01-16 23:59:19.000000 riverwm-utils-0.0.7/riverwm_utils.egg-info/PKG-INFO
--rw-r--r--   0 hastings  (1000) hastings  (1000)      473 2023-01-16 23:59:19.000000 riverwm-utils-0.0.7/riverwm_utils.egg-info/SOURCES.txt
--rw-r--r--   0 hastings  (1000) hastings  (1000)        1 2023-01-16 23:59:19.000000 riverwm-utils-0.0.7/riverwm_utils.egg-info/dependency_links.txt
--rw-r--r--   0 hastings  (1000) hastings  (1000)       87 2023-01-16 23:59:19.000000 riverwm-utils-0.0.7/riverwm_utils.egg-info/entry_points.txt
--rw-r--r--   0 hastings  (1000) hastings  (1000)       17 2023-01-16 23:59:19.000000 riverwm-utils-0.0.7/riverwm_utils.egg-info/requires.txt
--rw-r--r--   0 hastings  (1000) hastings  (1000)       14 2023-01-16 23:59:19.000000 riverwm-utils-0.0.7/riverwm_utils.egg-info/top_level.txt
--rw-r--r--   0 hastings  (1000) hastings  (1000)      789 2023-01-16 23:59:19.688981 riverwm-utils-0.0.7/setup.cfg
--rw-r--r--   0 hastings  (1000) hastings  (1000)       37 2022-06-15 03:24:33.000000 riverwm-utils-0.0.7/setup.py
+drwxr-xr-x   0 hastings  (1000) hastings  (1000)        0 2024-05-02 06:12:38.853416 riverwm-utils-0.0.8/
+-rw-r--r--   0 hastings  (1000) hastings  (1000)    35149 2023-07-03 09:14:06.000000 riverwm-utils-0.0.8/LICENSE
+-rw-r--r--   0 hastings  (1000) hastings  (1000)     2530 2024-05-02 06:12:38.853416 riverwm-utils-0.0.8/PKG-INFO
+-rw-r--r--   0 hastings  (1000) hastings  (1000)     2025 2023-07-03 09:14:06.000000 riverwm-utils-0.0.8/README.md
+-rw-r--r--   0 hastings  (1000) hastings  (1000)       91 2023-07-03 09:14:06.000000 riverwm-utils-0.0.8/pyproject.toml
+drwxr-xr-x   0 hastings  (1000) hastings  (1000)        0 2024-05-02 06:12:38.849416 riverwm-utils-0.0.8/riverwm_utils/
+-rw-r--r--   0 hastings  (1000) hastings  (1000)        0 2023-07-03 09:14:06.000000 riverwm-utils-0.0.8/riverwm_utils/__init__.py
+-rw-r--r--   0 hastings  (1000) hastings  (1000)     3679 2023-07-03 09:14:06.000000 riverwm-utils-0.0.8/riverwm_utils/river-control-unstable-v1.xml
+-rw-r--r--   0 hastings  (1000) hastings  (1000)     6147 2023-07-03 09:14:06.000000 riverwm-utils-0.0.8/riverwm_utils/river-status-unstable-v1.xml
+-rw-r--r--   0 hastings  (1000) hastings  (1000)     7737 2024-05-02 05:19:51.000000 riverwm-utils-0.0.8/riverwm_utils/riverwm_utils.py
+-rw-r--r--   0 hastings  (1000) hastings  (1000)   140883 2023-07-03 09:14:06.000000 riverwm-utils-0.0.8/riverwm_utils/wayland.xml
+drwxr-xr-x   0 hastings  (1000) hastings  (1000)        0 2024-05-02 06:12:38.853416 riverwm-utils-0.0.8/riverwm_utils.egg-info/
+-rw-r--r--   0 hastings  (1000) hastings  (1000)     2530 2024-05-02 06:12:38.000000 riverwm-utils-0.0.8/riverwm_utils.egg-info/PKG-INFO
+-rw-r--r--   0 hastings  (1000) hastings  (1000)      445 2024-05-02 06:12:38.000000 riverwm-utils-0.0.8/riverwm_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 hastings  (1000) hastings  (1000)        1 2024-05-02 06:12:38.000000 riverwm-utils-0.0.8/riverwm_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 hastings  (1000) hastings  (1000)       86 2024-05-02 06:12:38.000000 riverwm-utils-0.0.8/riverwm_utils.egg-info/entry_points.txt
+-rw-r--r--   0 hastings  (1000) hastings  (1000)       17 2024-05-02 06:12:38.000000 riverwm-utils-0.0.8/riverwm_utils.egg-info/requires.txt
+-rw-r--r--   0 hastings  (1000) hastings  (1000)       14 2024-05-02 06:12:38.000000 riverwm-utils-0.0.8/riverwm_utils.egg-info/top_level.txt
+-rw-r--r--   0 hastings  (1000) hastings  (1000)      789 2024-05-02 06:12:38.853416 riverwm-utils-0.0.8/setup.cfg
+-rw-r--r--   0 hastings  (1000) hastings  (1000)       65 2023-07-03 09:14:06.000000 riverwm-utils-0.0.8/setup.py
```

### Comparing `riverwm-utils-0.0.7/LICENSE` & `riverwm-utils-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `riverwm-utils-0.0.7/PKG-INFO` & `riverwm-utils-0.0.8/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 Metadata-Version: 2.1
 Name: riverwm-utils
-Version: 0.0.7
+Version: 0.0.8
 Summary: Utilities for the River Wayland compositor
 Home-page: https://github.com/NickHastings/riverwm-utils
 Author: Nick Hastings
 Author-email: nicholaschastings@gmail.com
 License: GPLv3
-Description: # riverwm-utils
-        Utilities for the River Wayland compositor. Currently just one utility is included.
-        
-        ## Usage
-        
-        ### cycle-focused-tags
-        
-        Change to either the next or previous focused tags.
-        
-        As can be seen in a [pull
-        request](https://github.com/riverwm/river/pull/506), this
-        functionality can easily be built directly into river. However, [as
-        explained by Leon
-        Plickat](https://github.com/riverwm/river/pull/506#issuecomment-1008021752)
-        there is a plan to separate the window management to a separate
-        client, and as such new additions are not being accepted. The
-        approach implemented here was suggested and sample code was
-        provided. That sample code forms the basis of this script.
-        
-        The script takes two arguments: the first is being the direction
-        next|previous, the second being the maximum number of tags at which
-        the cycling should wrap back to the first tag (or to the last tag from
-        the first tag). 
-        
-        If the second argument is omitted the maximum number of tags is
-        assumed to be 32.  If both arguments are ommited the direction,
-        next, will be used.
-        
-        The script can be called using spawn in the users init file. For example:
-        ```
-        riverctl map normal Mod4 Up spawn "cycle-focused-tags previous 9"
-        riverctl map normal Mod4 Down spawn "cycle-focused-tags next 9"
-        ```
-        
-        
-        ## Install
-        
-        ### Development version
-        Clone the repository:
-        ```
-        git clone https://github.com/NickHastings/riverwm-utils.git
-        ```
-        Install locally with pip
-        ```
-        python3 -m pip install ./riverwm-utils
-        ```
-        ### Stable realeases
-        ```
-        python3 -m pip install riverwm-utils
-        ```
-        
-        ### Wayland protocols and pywayland
-        
-        For `cycle-focused-tags` to work the relevant wayland protocol xml
-        files will need to be scanned by pywayland. If this has not already
-        been done `cycle-focused-tags` will attempt to do so.
-        
-        ## Licensing
-        
-        riverwm-utils is released under the GNU General Public License v3.0 only.
-        
-        The protocols in the `protocol` directory are released under various licenses by
-        various parties. You should refer to the copyright block of each protocol for
-        the licensing information.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# riverwm-utils
+Utilities for the River Wayland compositor. Currently just one utility is included.
+
+## Usage
+
+### cycle-focused-tags
+
+Change to either the next or previous focused tags.
+
+As can be seen in a [pull
+request](https://github.com/riverwm/river/pull/506), this
+functionality can easily be built directly into river. However, [as
+explained by Leon
+Plickat](https://github.com/riverwm/river/pull/506#issuecomment-1008021752)
+there is a plan to separate the window management to a separate
+client, and as such new additions are not being accepted. The
+approach implemented here was suggested and sample code was
+provided. That sample code forms the basis of this script.
+
+The script takes two arguments: the first is being the direction
+next|previous, the second being the maximum number of tags at which
+the cycling should wrap back to the first tag (or to the last tag from
+the first tag). 
+
+If the second argument is omitted the maximum number of tags is
+assumed to be 32.  If both arguments are ommited the direction,
+next, will be used.
+
+The script can be called using spawn in the users init file. For example:
+```
+riverctl map normal Mod4 Up spawn "cycle-focused-tags previous 9"
+riverctl map normal Mod4 Down spawn "cycle-focused-tags next 9"
+```
+
+
+## Install
+
+### Development version
+Clone the repository:
+```
+git clone https://github.com/NickHastings/riverwm-utils.git
+```
+Install locally with pip
+```
+python3 -m pip install ./riverwm-utils
+```
+### Stable realeases
+```
+python3 -m pip install riverwm-utils
+```
+
+### Wayland protocols and pywayland
+
+For `cycle-focused-tags` to work the relevant wayland protocol xml
+files will need to be scanned by pywayland. If this has not already
+been done `cycle-focused-tags` will attempt to do so.
+
+## Licensing
+
+riverwm-utils is released under the GNU General Public License v3.0 only.
+
+The protocols in the `*.xml` files are released under various licenses by
+various parties. You should refer to the copyright block of each protocol for
+the licensing information.
```

### Comparing `riverwm-utils-0.0.7/README.md` & `riverwm-utils-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,10 +55,10 @@
 files will need to be scanned by pywayland. If this has not already
 been done `cycle-focused-tags` will attempt to do so.
 
 ## Licensing
 
 riverwm-utils is released under the GNU General Public License v3.0 only.
 
-The protocols in the `protocol` directory are released under various licenses by
+The protocols in the `*.xml` files are released under various licenses by
 various parties. You should refer to the copyright block of each protocol for
 the licensing information.
```

### Comparing `riverwm-utils-0.0.7/riverwm_utils/river-control-unstable-v1.xml` & `riverwm-utils-0.0.8/riverwm_utils/river-control-unstable-v1.xml`

 * *Files identical despite different names*

### Comparing `riverwm-utils-0.0.7/riverwm_utils/river-status-unstable-v1.xml` & `riverwm-utils-0.0.8/riverwm_utils/river-status-unstable-v1.xml`

 * *Files identical despite different names*

### Comparing `riverwm-utils-0.0.7/riverwm_utils/riverwm_utils.py` & `riverwm-utils-0.0.8/riverwm_utils/riverwm_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,163 +1,191 @@
+'''Utilities for river wayland compositor'''
 import sys
 import os
-
-
-def scan():
-    this_dir = os.path.split(__file__)[0]
-    protocol_dir = os.path.join(this_dir)
-    input_files = ['wayland.xml',
-                   'river-control-unstable-v1.xml',
-                   'river-status-unstable-v1.xml']
-
-    protocols = [Protocol.parse_file(os.path.join(protocol_dir, input_file))
-                 for input_file in input_files]
-    protocol_imports = {
-        interface.name: protocol.name
-        for protocol in protocols
-        for interface in protocol.interface
-    }
-
-    pywayland_dir = os.path.split(pywayland.__file__)[0]
-    output_dir = os.path.join(pywayland_dir, 'protocol')
-    for protocol in protocols:
-        protocol.output(output_dir, protocol_imports)
-
+import argparse
+# pylint: disable=global-statement
 try:
     from pywayland.protocol.wayland import WlOutput
     from pywayland.protocol.wayland import WlSeat
     from pywayland.protocol.river_control_unstable_v1 import ZriverControlV1
     from pywayland.protocol.river_status_unstable_v1 import ZriverStatusManagerV1  # noqa: E501
 except ModuleNotFoundError:
     try:
         from pywayland.scanner.protocol import Protocol
         import pywayland
-        scan()
+        this_dir = os.path.split(__file__)[0]
+        protocol_dir = os.path.join(this_dir)
+        input_files = ['wayland.xml',
+                       'river-control-unstable-v1.xml',
+                       'river-status-unstable-v1.xml']
+
+        protocols = [Protocol.parse_file(os.path.join(
+            protocol_dir, input_file)) for input_file in input_files]
+        protocol_imports = {
+            interface.name: protocol.name
+            for protocol in protocols
+            for interface in protocol.interface
+        }
+
+        pywayland_dir = os.path.split(pywayland.__file__)[0]
+        output_dir = os.path.join(pywayland_dir, 'protocol')
+        for protocol in protocols:
+            protocol.output(output_dir, protocol_imports)
         print('Generated river bindings.')
         print('Please try running cycle-focused-tags again.')
 
-    except Exception:
-        this_dir = os.path.split(__file__)[0]
-        protocol_dir = os.path.normpath(os.path.join(this_dir, '..', 'protocol'))
+    except ImportError:
+        THIS_DIR = os.path.split(__file__)[0]
+        PROTOCOL_DIR = os.path.normpath(
+            os.path.join(THIS_DIR, '..', 'protocol'))
         ERROR_TEXT = (f'''
-        Your pywayland package does not have bindings for river-control-unstable-v1
-        and/or river-status-unstable-v1.
+        Your pywayland package does not have bindings for
+        river-control-unstable-v1 and/or river-status-unstable-v1.
 
         An attempt was made to generate them but it failed. You may be able to
         generate the manually with the following command:
 
-        python3 -m pywayland.scanner -i {protocol_dir}/wayland.xml '''
-                  f'{protocol_dir}/river-control-unstable-v1.xml '
-                  f'{protocol_dir}/river-status-unstable-v1.xml')
+        python3 -m pywayland.scanner -i {PROTOCOL_DIR}/wayland.xml '''
+                      f'{PROTOCOL_DIR}/river-control-unstable-v1.xml '
+                      f'{PROTOCOL_DIR}/river-status-unstable-v1.xml')
 
         print(ERROR_TEXT)
 
     sys.exit()
 
-from pywayland.client import Display
+from pywayland.client import Display  # pylint: disable=import-error
+
 
 STATUS_MANAGER = None
 CONTROL = None
 
 OUTPUTS = []
 SEAT = None
 
 
-class Output(object):
+class Output:
+    '''Represents a wayland output a.k.a. a display'''
     def __init__(self):
         self.wl_output = None
         self.focused_tags = None
+        self.tags = None
         self.status = None
 
     def destroy(self):
+        '''Cleanup'''
         if self.wl_output is not None:
             self.wl_output.destroy()
         if self.status is not None:
             self.status.destroy()
 
     def configure(self):
+        '''Setup'''
         self.status = STATUS_MANAGER.get_river_output_status(self.wl_output)
         self.status.user_data = self
         self.status.dispatcher["focused_tags"] = self.handle_focused_tags
 
-    def handle_focused_tags(self, output_status, tags):
+    def handle_focused_tags(self, _, tags):
+        '''Handle Event'''
         self.focused_tags = tags
 
 
-class Seat(object):
+class Seat:
+    '''Represtents a wayland seat'''
     def __init__(self):
         self.wl_seat = None
         self.status = None
         self.focused_output = None
 
     def destroy(self):
+        '''Cleanup'''
         if self.wl_seat is not None:
             self.wl_seat.destroy()
 
         if self.status is not None:
             self.status.destroy()
 
     def configure(self):
+        '''Setup'''
         self.status = STATUS_MANAGER.get_river_seat_status(self.wl_seat)
         self.status.user_data = self
         self.status.dispatcher["focused_output"] = self.handle_focused_output
 
     def handle_focused_output(self, _, wl_output):
+        '''Handle Event'''
         for output in OUTPUTS:
             if output.wl_output == wl_output:
                 self.focused_output = output
 
 
-def registry_handle_global(registry, id, interface, version):
+def registry_handle_global(registry, wid, interface, version):
+    '''Main Event Handler'''
     global STATUS_MANAGER
     global CONTROL
     global SEAT
 
     if interface == 'zriver_status_manager_v1':
-        STATUS_MANAGER = registry.bind(id, ZriverStatusManagerV1, version)
+        STATUS_MANAGER = registry.bind(wid, ZriverStatusManagerV1, version)
     elif interface == 'zriver_control_v1':
-        CONTROL = registry.bind(id, ZriverControlV1, version)
+        CONTROL = registry.bind(wid, ZriverControlV1, version)
     elif interface == 'wl_output':
         output = Output()
-        output.wl_output = registry.bind(id, WlOutput, version)
+        output.wl_output = registry.bind(wid, WlOutput, version)
         OUTPUTS.append(output)
     elif interface == 'wl_seat':
         # We only care about the first seat
         if SEAT is None:
             SEAT = Seat()
-            SEAT.wl_seat = registry.bind(id, WlSeat, version)
-
-
-USAGE = '''usage: cycle-focused-tags [DIRECTION] [NTAGS]
+            SEAT.wl_seat = registry.bind(wid, WlSeat, version)
 
-Change to either the next or previous focused tags.
 
-The DIRECTION argument shold be either 'next' or 'previous'.  The
-NTAGS argument indicates at which tag number the cycling should loop
-back to the first tag or to the last tag from the first tag.
-
-If NTAGS is ommiteed, 32 is assumed if both arguments are ommitted
-'next' is used as the DIRECTION.
-'''
+def check_direction(direction):
+    '''Check validity of direction argument'''
+    dir_char = direction[0].lower()
+    if dir_char not in ('p', 'n'):
+        raise argparse.ArgumentTypeError(f'Invalid direction: {direction}')
+
+    return dir_char
+
+
+def check_n_tags(n_tags):
+    '''Check validity of direction argument'''
+    i_n_tags = int(n_tags)
+    if i_n_tags < 1 or 32 < i_n_tags:
+        raise argparse.ArgumentTypeError(
+            f'Invalid max number of tags: {n_tags}')
+
+    return i_n_tags
+
+
+def parse_command_line() -> argparse.Namespace:
+    '''Read commanline arguments'''
+    parser = argparse.ArgumentParser(
+        description='Change to either the next or previous tags.',
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter
+    )
+    parser.add_argument(
+        'direction', default='next', nargs='?', type=check_direction,
+        help=('Direction to cycle through tags. Either "next" or "previous".')
+    )
+    parser.add_argument(
+        'n_tags', default=32, nargs='?', type=check_n_tags,
+        help=('The tag number the cycling should loop back to the first tag '
+              'or to the last tag from the first tag. Should be and integer '
+              'between 1 and 32 inclusive.')
+    )
+    parser.add_argument(
+        '--debug', '-d', action='store_true',
+        help='Enable debugging output.'
+    )
+    return parser.parse_args()
 
 
 def cycle_focused_tags():
-    n_tags = 32
-    direction = 'next'
-
-    if len(sys.argv) > 1:
-        direction = sys.argv[1]
-
-    if len(sys.argv) > 2:
-        n_tags = int(sys.argv[2])
-
-    if direction in ('-h', '--help'):
-        print(USAGE)
-        sys.exit(0)
-
+    '''Shift to next or previous tags'''
+    args = parse_command_line()
     display = Display()
     display.connect()
 
     registry = display.get_registry()
     registry.dispatcher["global"] = registry_handle_global
 
     display.dispatch(block=True)
@@ -177,18 +205,20 @@
     for output in OUTPUTS:
         output.configure()
 
     SEAT.configure()
 
     display.dispatch(block=True)
     display.roundtrip()
-    tags = SEAT.focused_output.focused_tags
+    used_tags = (1 << args.n_tags) - 1
+    tags = SEAT.focused_output.focused_tags & used_tags
+
     new_tags = 0
-    last_tag = 1 << (n_tags-1)
-    if direction == 'next':
+    last_tag = 1 << (args.n_tags - 1)
+    if args.direction == 'n':
         # If last tag is set => unset it and set first bit on new_tags
         if (tags & last_tag) != 0:
             tags ^= last_tag
             new_tags = 1
 
         new_tags |= (tags << 1)
 
@@ -197,14 +227,17 @@
         # last_tag bit on new tags
         if (tags & 1) != 0:
             tags ^= 1
             new_tags = last_tag
 
         new_tags |= (tags >> 1)
 
+    if args.debug:
+        print(f'0b{new_tags:010b} {new_tags}')
+
     CONTROL.add_argument("set-focused-tags")
     CONTROL.add_argument(str(new_tags))
     CONTROL.run_command(SEAT.wl_seat)
 
     display.dispatch(block=True)
     display.roundtrip()
```

### Comparing `riverwm-utils-0.0.7/riverwm_utils/wayland.xml` & `riverwm-utils-0.0.8/riverwm_utils/wayland.xml`

 * *Files identical despite different names*

### Comparing `riverwm-utils-0.0.7/riverwm_utils.egg-info/PKG-INFO` & `riverwm-utils-0.0.8/riverwm_utils.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 Metadata-Version: 2.1
 Name: riverwm-utils
-Version: 0.0.7
+Version: 0.0.8
 Summary: Utilities for the River Wayland compositor
 Home-page: https://github.com/NickHastings/riverwm-utils
 Author: Nick Hastings
 Author-email: nicholaschastings@gmail.com
 License: GPLv3
-Description: # riverwm-utils
-        Utilities for the River Wayland compositor. Currently just one utility is included.
-        
-        ## Usage
-        
-        ### cycle-focused-tags
-        
-        Change to either the next or previous focused tags.
-        
-        As can be seen in a [pull
-        request](https://github.com/riverwm/river/pull/506), this
-        functionality can easily be built directly into river. However, [as
-        explained by Leon
-        Plickat](https://github.com/riverwm/river/pull/506#issuecomment-1008021752)
-        there is a plan to separate the window management to a separate
-        client, and as such new additions are not being accepted. The
-        approach implemented here was suggested and sample code was
-        provided. That sample code forms the basis of this script.
-        
-        The script takes two arguments: the first is being the direction
-        next|previous, the second being the maximum number of tags at which
-        the cycling should wrap back to the first tag (or to the last tag from
-        the first tag). 
-        
-        If the second argument is omitted the maximum number of tags is
-        assumed to be 32.  If both arguments are ommited the direction,
-        next, will be used.
-        
-        The script can be called using spawn in the users init file. For example:
-        ```
-        riverctl map normal Mod4 Up spawn "cycle-focused-tags previous 9"
-        riverctl map normal Mod4 Down spawn "cycle-focused-tags next 9"
-        ```
-        
-        
-        ## Install
-        
-        ### Development version
-        Clone the repository:
-        ```
-        git clone https://github.com/NickHastings/riverwm-utils.git
-        ```
-        Install locally with pip
-        ```
-        python3 -m pip install ./riverwm-utils
-        ```
-        ### Stable realeases
-        ```
-        python3 -m pip install riverwm-utils
-        ```
-        
-        ### Wayland protocols and pywayland
-        
-        For `cycle-focused-tags` to work the relevant wayland protocol xml
-        files will need to be scanned by pywayland. If this has not already
-        been done `cycle-focused-tags` will attempt to do so.
-        
-        ## Licensing
-        
-        riverwm-utils is released under the GNU General Public License v3.0 only.
-        
-        The protocols in the `protocol` directory are released under various licenses by
-        various parties. You should refer to the copyright block of each protocol for
-        the licensing information.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# riverwm-utils
+Utilities for the River Wayland compositor. Currently just one utility is included.
+
+## Usage
+
+### cycle-focused-tags
+
+Change to either the next or previous focused tags.
+
+As can be seen in a [pull
+request](https://github.com/riverwm/river/pull/506), this
+functionality can easily be built directly into river. However, [as
+explained by Leon
+Plickat](https://github.com/riverwm/river/pull/506#issuecomment-1008021752)
+there is a plan to separate the window management to a separate
+client, and as such new additions are not being accepted. The
+approach implemented here was suggested and sample code was
+provided. That sample code forms the basis of this script.
+
+The script takes two arguments: the first is being the direction
+next|previous, the second being the maximum number of tags at which
+the cycling should wrap back to the first tag (or to the last tag from
+the first tag). 
+
+If the second argument is omitted the maximum number of tags is
+assumed to be 32.  If both arguments are ommited the direction,
+next, will be used.
+
+The script can be called using spawn in the users init file. For example:
+```
+riverctl map normal Mod4 Up spawn "cycle-focused-tags previous 9"
+riverctl map normal Mod4 Down spawn "cycle-focused-tags next 9"
+```
+
+
+## Install
+
+### Development version
+Clone the repository:
+```
+git clone https://github.com/NickHastings/riverwm-utils.git
+```
+Install locally with pip
+```
+python3 -m pip install ./riverwm-utils
+```
+### Stable realeases
+```
+python3 -m pip install riverwm-utils
+```
+
+### Wayland protocols and pywayland
+
+For `cycle-focused-tags` to work the relevant wayland protocol xml
+files will need to be scanned by pywayland. If this has not already
+been done `cycle-focused-tags` will attempt to do so.
+
+## Licensing
+
+riverwm-utils is released under the GNU General Public License v3.0 only.
+
+The protocols in the `*.xml` files are released under various licenses by
+various parties. You should refer to the copyright block of each protocol for
+the licensing information.
```

### Comparing `riverwm-utils-0.0.7/setup.cfg` & `riverwm-utils-0.0.8/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = riverwm-utils
-version = 0.0.7
+version = 0.0.8
 author = Nick Hastings
 author_email = nicholaschastings@gmail.com
 description = Utilities for the River Wayland compositor
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GPLv3
 license_file = LICENSE
```


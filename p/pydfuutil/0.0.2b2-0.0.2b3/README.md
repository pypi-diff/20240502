# Comparing `tmp/pydfuutil-0.0.2b2.tar.gz` & `tmp/pydfuutil-0.0.2b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydfuutil-0.0.2b2.tar", last modified: Tue Apr 30 20:56:30 2024, max compression
+gzip compressed data, was "pydfuutil-0.0.2b3.tar", last modified: Thu May  2 20:44:37 2024, max compression
```

## Comparing `pydfuutil-0.0.2b2.tar` & `pydfuutil-0.0.2b3.tar`

### file list

```diff
@@ -1,37 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:30.886746 pydfuutil-0.0.2b2/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16904 2024-04-30 20:56:30.886746 pydfuutil-0.0.2b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:30.886746 pydfuutil-0.0.2b2/pydfuutil/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37429 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16530 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/dfu.py
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/dfu_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/dfu_load.py
--rw-r--r--   0 runner    (1001) docker     (127)    19545 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/dfuse.py
--rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/dfuse_mem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/lmdfu.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/portable.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/quirks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/suffix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pydfuutil/usb_dfu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:30.886746 pydfuutil-0.0.2b2/pydfuutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16904 2024-04-30 20:56:30.000000 pydfuutil-0.0.2b2/pydfuutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-30 20:56:30.000000 pydfuutil-0.0.2b2/pydfuutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:56:30.000000 pydfuutil-0.0.2b2/pydfuutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-30 20:56:30.000000 pydfuutil-0.0.2b2/pydfuutil.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-30 20:56:30.000000 pydfuutil-0.0.2b2/pydfuutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 20:56:30.000000 pydfuutil-0.0.2b2/pydfuutil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 20:56:30.886746 pydfuutil-0.0.2b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:56:30.886746 pydfuutil-0.0.2b2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/tests/test_dfu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/tests/test_dfu_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/tests/test_dfu_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/tests/test_dfuse_mem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/tests/test_lmdfu.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-30 20:56:21.000000 pydfuutil-0.0.2b2/tests/test_quirks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:44:37.822127 pydfuutil-0.0.2b3/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16942 2024-05-02 20:44:37.822127 pydfuutil-0.0.2b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:44:37.818127 pydfuutil-0.0.2b3/pydfuutil/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34913 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16654 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/dfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/dfu_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/dfu_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18913 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/dfuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/dfuse_mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/lmdfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/portable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/quirks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/suffix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pydfuutil/usb_dfu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:44:37.818127 pydfuutil-0.0.2b3/pydfuutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16942 2024-05-02 20:44:37.000000 pydfuutil-0.0.2b3/pydfuutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-02 20:44:37.000000 pydfuutil-0.0.2b3/pydfuutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:44:37.000000 pydfuutil-0.0.2b3/pydfuutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-02 20:44:37.000000 pydfuutil-0.0.2b3/pydfuutil.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 20:44:37.000000 pydfuutil-0.0.2b3/pydfuutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 20:44:37.000000 pydfuutil-0.0.2b3/pydfuutil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 20:44:37.822127 pydfuutil-0.0.2b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:44:37.818127 pydfuutil-0.0.2b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/tests/test_dfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/tests/test_dfu_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/tests/test_dfu_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14411 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/tests/test_dfuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/tests/test_dfuse_mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/tests/test_lmdfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/tests/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-02 20:44:25.000000 pydfuutil-0.0.2b3/tests/test_quirks.py
```

### Comparing `pydfuutil-0.0.2b2/LICENSE` & `pydfuutil-0.0.2b3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.2b2/PKG-INFO` & `pydfuutil-0.0.2b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydfuutil
-Version: 0.0.2b2
+Version: 0.0.2b3
 Summary: PyDfuUtil - Pure python fork of dfu-util wrappers to libusb
 Author-email: o-murphy <thehelixpg@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -185,18 +185,19 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyusb
 Requires-Dist: libusb-package
-Requires-Dist: rich
 Requires-Dist: construct
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
+Provides-Extra: rich
+Requires-Dist: rich; extra == "rich"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pylint; extra == "test"
 
 # PyDfuUtil - Pure python fork of **[dfu-util](https://github.com/Stefan-Schmidt/dfu-util)** wrappers to **[libusb](https://github.com/libusb/libusb)**
 
 [![PyPI Version](https://img.shields.io/pypi/v/pydfuutil?label=PyPI&logo=pypi)](https://pypi.org/project/pydfuutil/)
```

### Comparing `pydfuutil-0.0.2b2/README.md` & `pydfuutil-0.0.2b3/README.md`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.2b2/pydfuutil/__main__.py` & `pydfuutil-0.0.2b3/pydfuutil/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,67 +5,68 @@
 """
 import argparse
 import errno
 import logging
 import os
 import re
 import sys
-from enum import IntFlag
+from enum import Enum
 from typing import Any, Callable, Literal
+import importlib.metadata
 
-import usb.core
-
-from pydfuutil import __version__, __copyright__
 from pydfuutil import dfu
-# from pydfuutil import dfuse
+from pydfuutil import dfuse
 from pydfuutil import dfu_load
-from pydfuutil.dfu_file import DFUFile, parse_dfu_suffix
-from pydfuutil.logger import get_logger
+from pydfuutil import dfu_file
+from pydfuutil import quirks
+from pydfuutil import usb_dfu
 from pydfuutil.portable import milli_sleep
-from pydfuutil.quirks import set_quirks, QUIRK_POLLTIMEOUT, QUIRK_FORCE_DFU11
-from pydfuutil.usb_dfu import USB_DT_DFU, bmAttributes, USB_DFU_FUNC_DESCRIPTOR
+from pydfuutil.logger import logger
+
+import usb.core
 
 try:
     import libusb_package
     from usb.backend import libusb1
+
     libusb1.get_backend(libusb_package.find_library)
-except ImportError:
+finally:
     pass
 
-logger = get_logger("pydfuutil")
-logger.setLevel(logging.INFO)
-usb_logger = logging.getLogger('usb')
+try:
+    __version__ = importlib.metadata.version("pydfuutil")
+except importlib.metadata.PackageNotFoundError:
+    __version__ = 'UNKNOWN'
 
+usb_logger = logging.getLogger('usb')
 MAX_DESC_STR_LEN = 253
-HAVE_GETPAGESIZE = not (sys.platform == 'win32')
-VERBOSE = False
+HAVE_GET_PAGESIZE = sys.platform != 'win32'
 
 
 def atoi(s: str) -> int:
     """
     Regular expression to match the integer part of the string
     :param s: input
     :return: Return 0 if no integer is found
     """
     match = re.match(r'^\s*([-+]?\d+)', s)
 
     if match:
         result = int(match.group(1))
         return result
-    else:
-        return 0
+    return 0
 
 
 def usb_path2devnum(path: str) -> int:
+    """parse the dev bus/port"""
     # TODO: wrong implementation
     parts = path.split('.')
     if len(parts) == 2:
         return int(parts[0]), int(parts[1])
-    else:
-        return 0
+    return 0
 
 
 def find_dfu_if(dev: usb.core.Device,
                 handler: Callable[[dfu.DfuIf, Any], Any] = None,
                 v: Any = None) -> int:
     """
     Find DFU interface for a given USB device.
@@ -220,29 +221,28 @@
     :param dfu_if: The DFU interface struct.
     :param v: Unused (can be any value).
     :return: Always returns 0.
     """
 
     name: str = get_alt_name(dfu_if)
     if name is None:
-        name = b"UNDEFINED"
+        name = "UNDEFINED"
 
-    print(f"Found {'DFU' if dfu_if.flags & dfu.Mode.IFF_DFU else 'Runtime'}: "
-          f"[{dfu_if.vendor:04x}:{dfu_if.product:04x}] devnum={dfu_if.devnum}, "
-          f"cfg={dfu_if.configuration}, intf={dfu_if.interface}, "
-          f"alt={dfu_if.altsetting}, name=\"{name}\"")
+    logger.info(f"Found {'DFU' if dfu_if.flags & dfu.Mode.IFF_DFU else 'Runtime'}: "
+                f"[{dfu_if.vendor:04x}:{dfu_if.product:04x}] devnum={dfu_if.devnum}, "
+                f"cfg={dfu_if.configuration}, intf={dfu_if.interface}, "
+                f"alt={dfu_if.altsetting}, name=\"{name}\"")
 
     return 0
 
 
 def list_dfu_interfaces(ctx: list[usb.core.Device]) -> int:
     """
     Walk the device tree and print out DFU devices.
 
-    :param dif: dfu.DfuIf
     :param ctx: libusb context
     :return: 0 on success.
     """
 
     for dev in ctx:
         find_dfu_if(dev, print_dfu_if, None)
         usb.util.dispose_resources(dev)
@@ -258,18 +258,16 @@
     :return: The alternate setting number if found, 0 otherwise.
     """
     name = get_alt_name(dfu_if)
     if name is None:
         return 0
     if name != v:
         return 0
-    """
-    Return altsetting+1 so that we can use return value 0 to indicate
-    "not found".
-    """
+    # Return altsetting+1 so that we can
+    # use return value 0 to indicate not found
     return dfu_if.altsetting + 1
 
 
 def count_dfu_interfaces(dev: usb.core.Device) -> int:
     """
     Count DFU interfaces within a single device.
 
@@ -289,22 +287,21 @@
 
 def iterate_dfu_devices(ctx: list[usb.core.Device], dif: dfu.DfuIf) -> list[usb.core.Device]:
     """
     Iterate over all matching DFU capable devices within the system.
 
     :param ctx: The USB context.
     :param dif: The DFU interface.
-    :param action: The action to perform for each device.
-    :param user: Additional user-defined data.
     :return: 0 on success, or an error code.
     """
     retval = []
     for dev in ctx:
 
-        if dif and (dif.flags & dfu.Mode.IFF_DEVNUM) and (dev.bus != dif.bus or dev.address != dif.devnum):
+        if (dif and (dif.flags & dfu.Mode.IFF_DEVNUM)
+                and (dev.bus != dif.bus or dev.address != dif.devnum)):
             continue
         if dif and (dif.flags & dfu.Mode.IFF_VENDOR) and dev.idVendor != dif.vendor:
             continue
         if dif and (dif.flags & dfu.Mode.IFF_PRODUCT) and dev.idProduct != dif.product:
             continue
         if not count_dfu_interfaces(dev):
             continue
@@ -322,53 +319,15 @@
     :param dif: The DFU interface instance.
     :return: 1 always.
     """
     dif.dev = dev
     return 1
 
 
-# def get_first_dfu_device(ctx: 'usb.core.Context', dif: dfu.DfuIf) -> int:
-#     """
-#     Find the first DFU-capable device and save it in dif.dev.
-#
-#     :param ctx: The USB context.
-#     :param dif: The DFU interface struct.
-#     :return: 0 on success, or an error code.
-#     """
-#     return iterate_dfu_devices(ctx, dif, found_dfu_device, dif)
-
-
-def count_one_dfu_device(dev: usb.core.Device, user: list) -> int:
-    """
-    Count one DFU device.
-
-    :param dev: The USB device.
-    :param user: User-defined data (should be an integer pointer).
-    :return: 0 always.
-    """
-    num = user
-    num[0] += 1
-    return 0
-
-
-# def count_dfu_devices(ctx: list[usb.core.Device], dif: dfu.DfuIf) -> int:
-#     """
-#     Count the number of DFU devices connected to the USB context.
-#
-#     :param ctx: The libusb context.
-#     :param dif: The DFU interface struct.
-#     :return: The number of DFU devices found.
-#     """
-#     num_found = 0
-#
-#     iterate_dfu_devices(ctx, dif, count_one_dfu_device, num_found)
-#     return num_found
-
-
-def parse_vendprod(string: str) -> tuple[int, int]:
+def parse_vid_pid(string: str) -> tuple[int, int]:
     """
     Parse a string containing vendor and product IDs in hexadecimal format.
 
     :param string: The string containing vendor and product IDs separated by ':'.
     :return: A tuple containing the vendor and product IDs.
     """
     vendor = 0
@@ -398,127 +357,127 @@
 
         dif.bus = atoi(dif.path)
         dif.devnum = res
         dif.flags |= dfu.Mode.IFF_DEVNUM
         return res
     except Exception as err:
         logger.error("USB device paths are not supported by this dfu-util.\n")
+        logger.debug(err)
         sys.exit(1)
 
 
 def find_descriptor(desc_list: list, desc_type: int, desc_index: int,
-                    res_buf: bytearray) -> int:
+                    res_buf: bytes) -> int:
     """
     Look for a descriptor in a concatenated descriptor list
     Will return desc_index'th match of given descriptor type
 
     :param desc_list: The concatenated descriptor list.
     :param desc_type: The type of descriptor to search for.
     :param desc_index: The index of the descriptor to find.
     :param res_buf: The buffer to store the found descriptor.
-    :param res_size: The maximum size of the result buffer.
     :return: length of found descriptor, limited to res_size
     """
 
     p: int = 0
     hit: int = 0
+    res_buf = bytearray(res_buf)
 
     while p + 1 < len(desc_list):
-        desclen = int(desc_list[p])
+        desc_len = int(desc_list[p])
 
-        if desclen == 0:
+        if desc_len == 0:
             logger.error("Invalid descriptor list")
             return -1
 
         if desc_list[p + 1] == desc_type and hit == desc_index:
-            if desclen > len(res_buf):
-                desclen = len(res_buf)
-            if p + desclen > len(desc_list):
-                desclen = len(desc_list) - p
-            res_buf[:desclen] = desc_list[p:p + desclen]
-            return desclen
+            desc_len = min(desc_len, len(res_buf))
+            if p + desc_len > len(desc_list):
+                desc_len = len(desc_list) - p
+            res_buf[:desc_len] = desc_list[p:p + desc_len]
+            return desc_len
 
         if desc_list[p + 1] == desc_type:
             hit += 1
 
         p += int(desc_list[p])
 
     return 0
 
 
 def usb_get_any_descriptor(dev: usb.core.Device,
                            desc_type: int,
                            desc_index: int,
-                           resbuf: bytearray) -> int:
+                           res_buf: bytes) -> int:
     """
     Look for a descriptor in the active configuration.
-    Will also find extra descriptors which are normally not returned by the standard libusb_get_descriptor().
+    Will also find extra descriptors which
+    are normally not returned by the standard libusb_get_descriptor().
 
-    :param dev_handle: The device handle.
+    :param dev: The device handle.
     :param desc_type: The descriptor type.
     :param desc_index: The descriptor index.
-    :param resbuf: The buffer to store the descriptor.
-    :param res_len: The maximum length of the descriptor buffer.
+    :param res_buf: The buffer to store the descriptor.
     :return: The length of the found descriptor.
     """
 
+    res_buf = bytearray(res_buf)
     # Get the total length of the configuration descriptors
     config = dev.get_active_configuration()
-    conflen = config.wTotalLength
+    conf_len = config.wTotalLength
 
     # Suck in the configuration descriptor list from device
 
-    cbuf = usb.control.get_descriptor(dev, usb.DT_CONFIG_SIZE, usb.DT_CONFIG, 0).tobytes()
+    c_buf = usb.control.get_descriptor(dev, usb.DT_CONFIG_SIZE, usb.DT_CONFIG, 0).tobytes()
 
-    # cbuf = dev.ctrl_transfer(usb.util.ENDPOINT_IN, usb.util.GET_DESCRIPTOR,
+    # c_buf = dev.ctrl_transfer(usb.util.ENDPOINT_IN, usb.util.GET_DESCRIPTOR,
     #                          (usb.util.DESC_TYPE_CONFIG << 8) | 0, 0, conflen)
 
-    if len(cbuf) < conflen:
+    if len(c_buf) < conf_len:
         logger.warning(
-            f"failed to retrieve complete configuration descriptor, got {len(cbuf)}/{conflen}"
+            f"failed to retrieve complete configuration descriptor, got {len(c_buf)}/{conf_len}"
         )
-        conflen = len(cbuf)
+        conf_len = len(c_buf)
 
     # Search through the configuration descriptor list
-    ret = find_descriptor(cbuf, desc_type, desc_index, resbuf)
+    ret = find_descriptor(c_buf, desc_type, desc_index, res_buf)
     if ret > 1:
-        if VERBOSE:
-            logger.info("Found descriptor in complete configuration descriptor list")
+        logger.debug("Found descriptor in complete configuration descriptor list")
         return ret
 
     # Finally try to retrieve it requesting the device directly
     # This is not supported on all devices for non-standard types
     # return dev.ctrl_transfer(usb.util.ENDPOINT_IN, usb.util.GET_DESCRIPTOR,
     #                          (desc_type << 8) | desc_index, 0, resbuf)
     return usb.control.get_descriptor(dev, usb.DT_CONFIG_SIZE, desc_type, desc_index).tobytes()
 
 
+# pylint: disable=invalid-name
 def get_cached_extra_descriptor(dev: usb.core.Device,
                                 bConfValue: int,
                                 intf: int,
                                 desc_type: int,
                                 desc_index: int,
-                                resbuf: bytearray) -> int:
+                                resbuf: bytes) -> int:
     """
     Get cached extra descriptor from libusb for an interface.
 
     :param dev: The USB device.
     :param bConfValue: The configuration value.
     :param intf: The interface number.
     :param desc_type: The descriptor type.
     :param desc_index: The descriptor index.
     :param resbuf: The buffer to store the descriptor.
-    :param res_len: The maximum length of the descriptor buffer.
     :return: The length of the found descriptor.
     """
     cfg = dev.configurations()[bConfValue - 1]
     try:
         intf_desc = cfg.interfaces()[intf]
     except usb.core.USBError as e:
-        if e.errno == usb.core.ENOENT:
+        if e.errno == errno.ENOENT:
             logger.error("Device is unconfigured")
         else:
             logger.error("Failed to get configuration descriptor")
         return -1
 
     ret = -1
 
@@ -528,87 +487,60 @@
 
         if extra_len > 1:
             ret = find_descriptor(extra, desc_type, desc_index, resbuf)
 
         if ret > 1:
             break
 
-    if ret < 2 and VERBOSE:
-        logger.info("Did not find cached descriptor")
+    if ret < 2:
+        logger.debug("Did not find cached descriptor")
 
     return ret
 
 
 VERSION = (f"{__version__}\n\n"
-           f"('Copyright 2005-2008 Weston Schmidt, Harald Welte and OpenMoko Inc.')\n"
-           f"{__copyright__}\n"
-           f"This program is Free Software and has ABSOLUTELY NO WARRANTY')\n")
+           f"2023 Yaroshenko Dmytro (https://github.com/o-murphy)\n")
 
 
-class Mode(IntFlag):
+class Mode(Enum):
+    """dfu-util cli mode"""
     NONE = 0
     VERSION = 1
     LIST = 2
     DETACH = 3
     UPLOAD = 4
     DOWNLOAD = 5
 
 
-def cpu_to_le16(value):
+def cpu_to_le16(value: int) -> bytes:
+    """Convert int to uint16le"""
     return value.to_bytes(2, byteorder='little')
 
 
-def le16_to_cpu(data):
+def le16_to_cpu(data: bytes) -> int:
+    """Convert uint16le to int"""
     return int.from_bytes(data, byteorder='little')
 
 
-# class IntOrBytes:
-#     def __init__(self, value):
-#         if isinstance(value, int):
-#             self._value = value
-#         elif isinstance(value, bytes):
-#             self._value = int.from_bytes(value, byteorder='big', signed=True)
-#         else:
-#             raise TypeError("Value must be int or bytes")
-#
-#     def __lt__(self, other):
-#         if isinstance(other, IntOrBytes):
-#             return self._value < other._value
-#         if isinstance(other, int):
-#             return self._value < other
-#         raise TypeError("Comparison with unsupported type")
-#
-#     def __eq__(self, other):
-#         if isinstance(other, IntOrBytes):
-#             return self._value == other._value
-#         elif isinstance(other, int):
-#             return self._value == other
-#         else:
-#             raise TypeError("Comparison with unsupported type")
-#
-#     def __repr__(self):
-#         return f"IntOrBytes({self._value})"
-
-
-def int_(value: [int, (bytes, bytearray)], order: Literal["little", "big"] = 'little'):
+def int_(value: [int, bytes, bytearray],
+         order: Literal["little", "big"] = 'little') -> int:
+    """coerce value to int"""
     if isinstance(value, int):
         return value
     if isinstance(value, (bytes, bytearray)):
         return int.from_bytes(value, order)
     raise TypeError("Unsupported type")
 
 
-def main() -> None:
-    # Todo: implement
-
-    global VERBOSE
+def main(argv) -> None:
+    """Cli entry point"""
 
     # Create argument parser
     parser = argparse.ArgumentParser(
-        prog="pydfuutil",
+        prog=f"pydfuutil v{__version__}",
         description="Python implementation of DFU-Util tools"
     )
 
     # Add arguments
     parser.add_argument("-V", "--version", action="version", version=VERSION,
                         help="Print the version number")
     parser.add_argument("-v", "--verbose", action="store_true",
@@ -637,31 +569,35 @@
                         help="Issue USB Reset signalling once we're finished")
     parser.add_argument("-s", "--dfuse-address", metavar="<address>",
                         help="ST DfuSe mode, specify target address "
                              "for raw file download or upload. "
                              "Not applicable for DfuSe file (.dfu) downloads")
 
     # Parse arguments
-    args = parser.parse_args()
-
+    if argv[0] == __file__:
+        argv.pop(0)
+    args = parser.parse_args(argv)
+    verbose = False
     dif: dfu.DfuIf = dfu.DfuIf()
-    file = DFUFile(None)
+    file = dfu_file.DFUFile(None)
     mode = Mode.NONE
     device_id_filter = None
     alt_name = None
     transfer_size = 0
     dfuse_device = 0
     dfuse_options = None
     final_reset = 0
 
-    func_dfu_rt = USB_DFU_FUNC_DESCRIPTOR.parse(bytes(USB_DFU_FUNC_DESCRIPTOR.sizeof()))
-    func_dfu = USB_DFU_FUNC_DESCRIPTOR.parse(bytes(USB_DFU_FUNC_DESCRIPTOR.sizeof()))
+    # func_dfu_rt = USB_DFU_FUNC_DESCRIPTOR.parse(bytes(USB_DFU_FUNC_DESCRIPTOR.sizeof()))
+    # func_dfu = USB_DFU_FUNC_DESCRIPTOR.parse(bytes(USB_DFU_FUNC_DESCRIPTOR.sizeof()))
+    func_dfu_rt = usb_dfu.FuncDescriptor()
+    func_dfu = usb_dfu.FuncDescriptor()
 
     if args.verbose:
-        VERBOSE = True
+        verbose = True
         logger.setLevel(logging.DEBUG)
         usb_logger.setLevel(logging.DEBUG)
 
     if args.list:
         mode = Mode.LIST
 
     if args.detach:
@@ -709,23 +645,21 @@
 
     if args.reset:
         final_reset = 1
 
     if args.dfuse_address:
         dfuse_options = args.dfuse_address
 
-    print(VERSION)
-
     if mode == Mode.NONE:
         logger.error("You need to specify one of -D or -U\n\n")
         parser.print_help()
         sys.exit(2)
 
     if device_id_filter:
-        dif.vendor, dif.product = parse_vendprod(device_id_filter)
+        dif.vendor, dif.product = parse_vid_pid(device_id_filter)
         logger.info(f"Filter on VID = 0x{dif.vendor:04X} PID = 0x{dif.product:04X}\n")
         if dif.vendor:
             dif.flags |= dfu.Mode.IFF_VENDOR
         if dif.product:
             dif.flags |= dfu.Mode.IFF_PRODUCT
 
     # libusb init
@@ -770,23 +704,23 @@
             sys.exit(1)
 
     find_dfu_if(dev, get_first_dfu_if)
     logger.debug(_rt_dif)
 
     logger.info(f"ID 0x{_rt_dif.vendor:04X}:0x{_rt_dif.product:04X}")
 
-    quirks = set_quirks(_rt_dif.vendor, _rt_dif.product, _rt_dif.bcdDevice)
+    _quirks = quirks.set_quirks(_rt_dif.vendor, _rt_dif.product, _rt_dif.bcdDevice)
 
     # Obtain run-time DFU functional descriptor without asking device
     # E.g. Free runner does not like to be requested at this point
 
     ret = get_cached_extra_descriptor(
         _rt_dif.dev, _rt_dif.configuration, _rt_dif.interface,
-        # USB_DT_DFU, 0, le16_to_cpu(func_dfu_rt.bcdDFUVersion)
-        USB_DT_DFU, 0, USB_DFU_FUNC_DESCRIPTOR.bcdDFUVersion.build(func_dfu_rt.bcdDFUVersion)
+        usb_dfu.USB_DT_DFU, 0,
+        cpu_to_le16(func_dfu_rt.bcdDFUVersion)
     )
     ret = int_(ret)
     if ret == 7:
         logger.info("Deducing device DFU version from functional descriptor "
                     "length")
         func_dfu_rt.bcdDFUVersion = 0x0100
     elif ret < 9:
@@ -799,67 +733,63 @@
 
     # Transition from run-Time mode to DFU mode
 
     # status_again
     def check_status():
         logger.debug('Status again')
         _log_msg = "Determining device status: "
-        # ret = int(status_ := dfu.get_status(_rt_dif.dev, _rt_dif.interface))
-        # ret = int(status_ := dif.get_status())
-        # if ret < 0:
         if int(status_ := dif.get_status()) < 0:
             logger.error(f"{_log_msg}error get_status")
             sys.exit(1)
         logger.info(f"{_log_msg}state = {status_.bState.to_string()}, "
                     f"status = {status_.bStatus}")
 
-        if not quirks & QUIRK_POLLTIMEOUT:
+        if not _quirks & quirks.QUIRK_POLLTIMEOUT:
             milli_sleep(status_.bwPollTimeout)
         return status_
 
-    while not (_rt_dif.flags & dfu.Mode.IFF_DFU):
+    while not _rt_dif.flags & dfu.Mode.IFF_DFU:
         # In the 'first round' during runtime mode, there can only be one
         # DFU Interface descriptor according to the DFU Spec.
 
-        # FIXME: check if the selected device really has only one
+        # TODO: check if the selected device really has only one
 
         logger.info("Claiming USB DFU Runtime Interface...")
         try:
             usb.util.claim_interface(_rt_dif.dev, _rt_dif.interface)
         except usb.core.USBError:
             logger.error(f"Cannot claim interface {_rt_dif.interface}")
             sys.exit(1)
 
         try:
             _rt_dif.dev.set_interface_altsetting(_rt_dif.interface, 0)
         except usb.core.USBError:
-            logger.error(f"Cannot set alt interface zero")
+            logger.error("Cannot set alt interface zero")
             sys.exit(1)
 
         status = check_status()
 
         if status.bState in (dfu.State.APP_IDLE, dfu.State.APP_DETACH):
             logger.info("Device really in Runtime Mode, send DFU "
                         "detach request...")
 
-            # if IntOrBytes(dfu.detach(_rt_dif.dev, _rt_dif.interface, 1000)) < 0:
             if int_(_rt_dif.detach(1000)) < 0:
                 logger.error("error detaching")
                 sys.exit(1)
 
-            if func_dfu_rt.bmAttributes & bmAttributes.USB_DFU_WILL_DETACH:
+            if func_dfu_rt.bmAttributes & usb_dfu.BmAttributes.USB_DFU_WILL_DETACH:
                 logger.info("Device will detach and reattach...")
             else:
                 logger.info("Resetting USB...\n")
                 try:
                     _rt_dif.dev.reset()
                 except usb.core.USBError:
                     logger.error("error resetting after detach")
             milli_sleep(2000)
-            break
+            break  # TODO: wtf? break there?
         elif status.bState == dfu.State.DFU_ERROR:
             logger.error("dfuERROR, clearing status")
             if dfu.clear_status(_rt_dif.dev, _rt_dif.interface) < 0:
                 logger.error("error detaching")
                 sys.exit(1)
         else:
             logger.info("Runtime device already in DFU state ?!?")
@@ -975,68 +905,68 @@
                 logger.error("error clear_status")
                 sys.exit(1)
 
             status = check_status()
 
         elif status.bState == (dfu.State.DFU_DOWNLOAD_IDLE, dfu.State.DFU_UPLOAD_IDLE):
             logger.warning("aborting previous incomplete transfer")
-            # if dfu.abort(dif.dev, dif.interface) < 0:
             if dif.abort() < 0:
                 logger.error("can't send DFU_ABORT")
                 sys.exit(1)
 
             status = check_status()
 
         elif status.bState == dfu.State.DFU_IDLE:
             logger.info("dfuIDLE, continuing")
             break
 
     if status.bStatus != dfu.Status.OK:
         logger.warning(f"DFU Status: {status.bStatus.to_string()}")
+
         # Clear our status & try again.
         dfu.clear_status(dif.dev, dif.interface)
-        # _ = int(status := dfu.get_status(dif.dev, dif.interface))
         _ = int(status := dif.get_status())
         if status.bStatus != dfu.Status.OK:
             logger.error(f"{status.bStatus}")
             sys.exit(1)
-        if not quirks & QUIRK_POLLTIMEOUT:
+        if not _quirks & quirks.QUIRK_POLLTIMEOUT:
             milli_sleep(status.bwPollTimeout)
 
     logger.debug(f"State: {status.bState.to_string()}, "
                  f"Status: {status.bStatus.to_string()} Continue...")
 
     # Get the DFU mode DFU functional descriptor
     # If it is not found cached, we will request it from the device
 
     ret = get_cached_extra_descriptor(
         dif.dev, dif.configuration, dif.interface,
-        USB_DT_DFU, 0, USB_DFU_FUNC_DESCRIPTOR.bcdDFUVersion.build(func_dfu.bcdDFUVersion)
+        usb_dfu.USB_DT_DFU, 0, cpu_to_le16(func_dfu.bcdDFUVersion)
     )
     ret = int_(ret)
 
     if ret < 7:
         logger.error("obtaining cached DFU functional descriptor")
         ret = usb_get_any_descriptor(
-            dif.dev, USB_DT_DFU, 0,
-            USB_DFU_FUNC_DESCRIPTOR.bcdDFUVersion.build(func_dfu_rt.bcdDFUVersion))
+            dif.dev, usb_dfu.USB_DT_DFU, 0,
+            cpu_to_le16(func_dfu_rt.bcdDFUVersion)
+        )
         ret = int_(ret)
 
     if ret == 7:
         logger.info("Deducing device DFU version from functional descriptor length")
         func_dfu.bcdDFUVersion = 0x0100
     elif ret < 9:
         logger.error("Error obtaining DFU functional descriptor")
         logger.info("Please report this as a bug!")
         logger.warning("Assuming DFU version 1.0")
         func_dfu.bcdDFUVersion = 0x0100
         logger.warning("Warning: Transfer size can not be detected")
         func_dfu.wTransferSize = 0
 
-    if quirks & QUIRK_FORCE_DFU11:
+    if _quirks & quirks.QUIRK_FORCE_DFU11:
         func_dfu.bcdDFUVersion = 0x0110
 
     logger.info(f"DFU mode device DFU version  0x{func_dfu.bcdDFUVersion:04X}")
 
     if func_dfu.bcdDFUVersion == 0x11a:
         dfuse_device = 1
 
@@ -1044,61 +974,60 @@
     if transfer_size:
         logger.info(f"Device returned transfer size {transfer_size}")
     else:
         logger.error("Transfer size must be specified")
         sys.exit(1)
 
     # autotools lie when cross-compiling for Windows using mingw32/64
-    if HAVE_GETPAGESIZE:
+    if HAVE_GET_PAGESIZE:
         # limitation of Linux usbdevio
         page_size = os.sysconf(os.sysconf_names['SC_PAGE_SIZE'])
         if transfer_size > page_size:
             transfer_size = page_size
             logger.info(f"Limited transfer size to {transfer_size}")
 
     # DFU specification
     # if dif.dev:  # strange think, unreachable
     #     logger.error(f"Failed to get device descriptor")
     #     sys.exit(1)
 
+    # pylint: disable=no-member
     if transfer_size < dif.dev.bMaxPacketSize0:
         logger.info(f"Adjusted transfer size to {transfer_size}")
 
     if mode == Mode.UPLOAD:
         # open for "exclusive" writing in a portable way
         try:
-            with open(file.name, "ab") as file.filep:
+            with open(file.name, "ab") as file.file_p:
                 if os.path.getsize(file.name) != 0:
                     logger.info(f"{file.name}: File exists")
                     sys.exit(1)
 
-
                 if dfuse_device or dfuse_options:
-                    raise NotImplementedError("DfuSe devices aren't support yet")
-
                     if dfuse.do_upload(dif, transfer_size, file, dfuse_options) < 0:
                         sys.exit(1)
                 else:
                     if dfu_load.do_upload(dif, transfer_size, file) < 0:
                         sys.exit(1)
 
         except OSError as e:
             logger.error(e)
             sys.exit(1)
 
     elif mode == Mode.DOWNLOAD:
         try:
             # Open file for reading in binary mode
-            with open(file.name, "rb") as filep:
-                if not filep:
+            with open(file.name, "rb") as file_p:
+                if not file_p:
                     logger.error(f"Error: Failed to open {file.name}")
                     sys.exit(1)
 
                 # Parse DFU suffix
-                ret = parse_dfu_suffix(file)
+                # ret = dfu_file.parse_dfu_suffix(file)
+                ret = file.parse_dfu_suffix()
                 if ret < 0:
                     sys.exit(1)
                 elif ret == 0:
                     logger.warning("File has no DFU suffix")
                 elif file.bcdDFU not in (0x0100, 0x011a):
                     logger.error(f"Unsupported DFU file revision 0x{file.bcdDFU:04x}")
                     sys.exit(1)
@@ -1114,15 +1043,15 @@
                                    f"does not match device 0x{dif.product:04x}")
 
                 # Perform download based on conditions
                 if dfuse_device or dfuse_options or file.bcdDFU == 0x011a:
                     if dfuse.do_dnload(dif, transfer_size, file, dfuse_options) < 0:
                         sys.exit(1)
                 else:
-                    if dfu_load.do_dnload(dif, transfer_size, file, quirks, VERBOSE) < 0:
+                    if dfu_load.do_dnload(dif, transfer_size, file, _quirks, verbose) < 0:
                         sys.exit(1)
 
         except OSError as e:
             logger.error(e)
             sys.exit(1)
 
     else:
@@ -1134,15 +1063,16 @@
         if int_(dif.detach(1000)) < 0:
             logger.error("can't detach")
         logger.info("Resetting USB to switch back to runtime mode")
         try:
             dif.dev.reset()
         except usb.core.USBError as e:
             logger.error("error resetting after download")
+            logger.debug(e)
 
     usb.util.release_interface(dif.dev, dif.interface)
     usb.util.dispose_resources(dif.dev)
     sys.exit(0)
 
 
 if __name__ == '__main__':
-    main()
+    main(sys.argv)
```

### Comparing `pydfuutil-0.0.2b2/pydfuutil/dfu.py` & `pydfuutil-0.0.2b3/pydfuutil/dfu.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """
 low-level DFU message sending routines (part of dfu-programmer).
 (C) 2023 Yaroshenko Dmytro (https://github.com/o-murphy)
 """
 
 import inspect
+import logging
 from dataclasses import dataclass
 from enum import IntEnum, IntFlag
 
 import usb.util
 
-from pydfuutil.logger import get_logger
+from pydfuutil.logger import logger
 
-logger = get_logger(__name__)
+
+_logger = logger.getChild(__name__.rsplit('.', maxsplit=1)[-1])
+_logger.setLevel(logging.DEBUG)
 
 
 class State(IntEnum):
     """Dfu states"""
     APP_IDLE = 0x00
     APP_DETACH = 0x01
     DFU_IDLE = 0x02
@@ -24,14 +27,16 @@
     DFU_DOWNLOAD_IDLE = 0x05
     DFU_MANIFEST_SYNC = 0x06
     DFU_MANIFEST = 0x07
     DFU_MANIFEST_WAIT_RESET = 0x08
     DFU_UPLOAD_IDLE = 0x09
     DFU_ERROR = 0x0a
 
+    UNKNOWN_ERROR = -1
+
     def to_string(self):
         """
         :return: State.self name by State Enum
         """
         return state_to_string(self)
 
 
@@ -120,27 +125,27 @@
     IFF_IFACE = 0x0800
     IFF_ALT = 0x1000
     IFF_DEVNUM = 0x2000
     IFF_PATH = 0x4000
 
 
 @dataclass(frozen=True)
-class StatusData:
+class StatusRetVal:
     """
     Converts dfu_get_status result bytes to applicable dataclass
     """
     # pylint: disable=invalid-name
     bStatus: Status = Status.ERROR_UNKNOWN
     bwPollTimeout: int = 0
     bState: State = State.DFU_ERROR
     iString: int = 0
 
     @classmethod
     def from_bytes(cls, data: bytes):
-        """Creates StatusData instance from bytes sequence"""
+        """Creates StatusRetVal instance from bytes sequence"""
         if len(data) >= 6:
             bStatus = (Status(data[0])
                        if data[0] in Status.__members__.values()
                        else Status.ERROR_UNKNOWN)
             bwPollTimeout = int.from_bytes(data[1:4], 'little')
             bState = (State(data[4])
                       if data[0] in State.__members__.values()
@@ -210,15 +215,15 @@
         """Binds self to dfu.upload()"""
         return upload(self.dev, self.interface, transaction, data_or_length)
 
     def abort(self) -> int:
         """Binds self to dfu.abort()"""
         return abort(self.dev, self.interface)
 
-    def get_status(self) -> StatusData:
+    def get_status(self) -> StatusRetVal:
         """Binds self to dfu.get_status()"""
         return get_status(self.dev, self.interface)
 
     def get_state(self) -> State:
         """Binds self to dfu.get_state()"""
         return get_state(self.dev, self.interface)
 
@@ -238,15 +243,15 @@
     else:
         if 0 != DEBUG_LEVEL:
             raise ValueError(f"dfu_init: Invalid timeout value {timeout}")
 
 
 def verify_init() -> int:
     """
-    Verifies setted TIMEOUT and DEBUG_LEVEL
+    Verifies provided TIMEOUT and DEBUG_LEVEL
     NOTE: (function: typing.Callable) not needed cause python can get it from stack
     :raise ValueError with caller function name
     :return: 0
     """
     caller = inspect.stack()[0][3]
     if INVALID_DFU_TIMEOUT == TIMEOUT:
         if 0 != DEBUG_LEVEL:
@@ -259,15 +264,15 @@
     NOTE: Maybe not needed cause python can define globals after
     :param level: logging level (DEBUG, INFO, WARNING, ERROR)
     """
 
     # pylint: disable=global-statement
     global DEBUG_LEVEL
     DEBUG_LEVEL = level
-    logger.setLevel(level)
+    _logger.setLevel(level)
 
 
 def detach(device: usb.core.Device, interface: int, timeout: int) -> bytes:
     """
 
      *  DETACH Request (DFU Spec 1.0, Section 5.1)
      *
@@ -282,26 +287,26 @@
     u have to free device and handle it again
     :param device: usb.core.Device
     :param interface: usb.core.Interface.bInterfaceNumber
     :param timeout: timeout to dfu detach
     :return: returns error code
     """
     verify_init()
-    logger.debug('DETACH...')
+    _logger.debug('DETACH...')
     result = device.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_OUT
                       | usb.util.CTRL_TYPE_CLASS
                       | usb.util.CTRL_RECIPIENT_INTERFACE,
         bRequest=Command.DETACH,
         wValue=timeout,
         wIndex=interface,
         data_or_wLength=None,
         timeout=TIMEOUT,
     )
-    logger.debug(f'DETACH {result >= 0}')
+    _logger.debug(f'DETACH {result >= 0}')
     return result
 
 
 def download(device: usb.core.Device,
              interface: int,
              transaction: int,
              data_or_length: [bytes, int]) -> int:
@@ -320,28 +325,28 @@
     :param device: usb.core.Device
     :param interface: usb.core.interface.bInterfaceNumber
     :param transaction: start page int(total_data_size/xfer_size)
     :param data_or_length: page size bytes(xfer_size) or xfer_size
     :return: downloaded data or error code in bytes
     """
     verify_init()
-    logger.debug('DFU_DOWNLOAD...')
+    _logger.debug('DFU_DOWNLOAD...')
 
     result = device.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_OUT
                       | usb.util.CTRL_TYPE_CLASS
                       | usb.util.CTRL_RECIPIENT_INTERFACE,
         bRequest=Command.DNLOAD,
         wValue=transaction,
         wIndex=interface,
         data_or_wLength=data_or_length,
         timeout=TIMEOUT,
     )
 
-    logger.debug(f'DFU_DOWNLOAD {result >= 0}')
+    _logger.debug(f'DFU_DOWNLOAD {result >= 0}')
     return result
 
 
 def upload(device: usb.core.Device,
            interface: int,
            transaction: int,
            data_or_length: [bytes, int]) -> bytes:
@@ -360,33 +365,33 @@
     :param device: usb.core.Device
     :param interface: usb.core.Interface.bInterfaceNumber
     :param transaction: start page int(total_data_size/xfer_size)
     :param data_or_length: page size bytes(xfer_size) or xfer_size
     :return: uploaded data or error code in bytes
     """
     verify_init()
-    logger.debug('DFU_UPLOAD...')
+    _logger.debug('UPLOAD...')
 
     result = device.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_IN
                       | usb.util.CTRL_TYPE_CLASS
                       | usb.util.CTRL_RECIPIENT_INTERFACE,
         bRequest=Command.UPLOAD,
         wValue=transaction,
         wIndex=interface,
         data_or_wLength=data_or_length,
         timeout=TIMEOUT,
     )
 
-    logger.debug(f'DFU_UPLOAD {len(result) >= 0}')
+    _logger.debug(f'UPLOAD {len(result) >= 0}')
 
     return result.tobytes()
 
 
-def get_status(device: usb.core.Device, interface: int) -> StatusData:
+def get_status(device: usb.core.Device, interface: int) -> StatusRetVal:
     """
      *  GETSTATUS Request (DFU Spec 1.0, Section 6.1.2)
      *
      *  device    - the usb_dev_handle to communicate with
      *  interface - the interface to communicate with
      *  status    - the data structure to be populated with the results
      *
@@ -394,34 +399,34 @@
 
     Returns DFU interface status
     :param device: usb.core.Device
     :param interface: usb.core.Interface.bInterfaceNumber
     :return: error code and _STATUS [Container, dict] object
     """
     verify_init()
-    logger.debug('DFU_GET_STATUS...')
+    _logger.debug('DFU_GET_STATUS...')
 
     length = 6
     result = device.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_IN
                       | usb.util.CTRL_TYPE_CLASS
                       | usb.util.CTRL_RECIPIENT_INTERFACE,
         bRequest=Command.GETSTATUS,
         wValue=0,
         wIndex=interface,
         data_or_wLength=length,
         timeout=TIMEOUT,
     )
 
     if len(result) == length:
-        status = StatusData.from_bytes(result.tobytes())
-        logger.debug(f'DFU_GET_STATUS {len(result) == 6}')
-        logger.debug(f'CURRENT STATE {status.bState.to_string()}')
+        status = StatusRetVal.from_bytes(result.tobytes())
+        _logger.debug(f'GET_STATUS {len(result) == 6}')
+        _logger.debug(f'CURRENT STATE {status.bState.to_string()}')
         return status
-    return StatusData.from_bytes(result)
+    return StatusRetVal.from_bytes(result)
 
 
 def clear_status(device: usb.core.Device, interface: int) -> int:
     """
      *  CLRSTATUS Request (DFU Spec 1.0, Section 6.1.3)
      *
      *  device    - the usb_dev_handle to communicate with
@@ -431,32 +436,32 @@
 
     Clears DFU interface status
     :param device: usb.core.Device
     :param interface: usb.core.Interface.bInterfaceNumber
     :return: error code
     """
     verify_init()
-    logger.debug('DFU_CLEAR_STATUS...')
+    _logger.debug('CLEAR_STATUS...')
 
     result = device.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_OUT
                       | usb.util.CTRL_TYPE_CLASS
                       | usb.util.CTRL_RECIPIENT_INTERFACE,
         bRequest=Command.CLRSTATUS,
         wValue=0,
         wIndex=interface,
         data_or_wLength=None,
         timeout=TIMEOUT,
     )
-    logger.debug(f'DFU_CLEAR_STATUS {result >= 0}')
+    _logger.debug(f'CLEAR_STATUS {result >= 0}')
 
     return result
 
 
-def get_state(device: usb.core.Device, interface: int) -> State:
+def get_state(device: usb.core.Device, interface: int) -> [State, int]:
     """
      *  GETSTATE Request (DFU Spec 1.0, Section 6.1.5)
      *
      *  device    - the usb_dev_handle to communicate with
      *  interface - the interface to communicate with
      *  length    - the maximum number of bytes to receive from the USB
      *              device - must be less than wTransferSize
@@ -480,15 +485,15 @@
         wValue=0,
         wIndex=interface,
         data_or_wLength=length,
         timeout=TIMEOUT,
     )
     value = result.tobytes()[0] < 1
     if value < 1:
-        return -1
+        return State(-1)
     if value in State.__members__.values():
         value = State(value)
     return value
 
 
 def abort(device: usb.core.Device, interface: int) -> int:
     """
@@ -501,28 +506,28 @@
 
     Aborts DFU command
     :param device: usb.core.Device
     :param interface: usb.core.Interface.bInterfaceNumber
     :return: error code
     """
     verify_init()
-    logger.debug('ABORT...')
+    _logger.debug('ABORT...')
 
     result = device.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_OUT
                       | usb.util.CTRL_TYPE_CLASS
                       | usb.util.CTRL_RECIPIENT_INTERFACE,
         bRequest=Command.ABORT,
         wValue=0,
         wIndex=interface,
         data_or_wLength=None,
         timeout=TIMEOUT,
     )
 
-    logger.debug(f'ABORT {result >= 0}')
+    _logger.debug(f'ABORT {result >= 0}')
 
     return result
 
 
 def state_to_string(state: int) -> [str, None]:
     """
     :param state:
```

### Comparing `pydfuutil-0.0.2b2/pydfuutil/dfu_file.py` & `pydfuutil-0.0.2b3/pydfuutil/dfu_file.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 import os
 from dataclasses import dataclass, field
 
 from construct import (Struct, Const, ByteSwapped, Default,
                        Int32ub, Int16ub, Int8sb,
                        ConstError, StreamError)
 
-from pydfuutil.logger import get_logger
+from pydfuutil.logger import logger
 
 __all__ = ('DFUFile', 'parse_dfu_suffix', 'generate_dfu_suffix')
 
-logger = get_logger("dfu-file")
+_logger = logger.getChild(__name__.rsplit('.', maxsplit=1)[-1])
 
 DFU_SUFFIX_LENGTH = 16
 
 crc32_table = [
     0x00000000, 0x77073096, 0xee0e612c, 0x990951ba, 0x076dc419, 0x706af48f,
     0xe963a535, 0x9e6495a3, 0x0edb8832, 0x79dcb8a4, 0xe0d5e91e, 0x97d2d988,
     0x09b64c2b, 0x7eb17cbd, 0xe7b82d07, 0x90bf1d91, 0x1db71064, 0x6ab020f2,
@@ -82,135 +82,142 @@
     """
     return crc32_table[(accum ^ delta) & 0xff] ^ (accum >> 8)
 
 
 @dataclass
 class DFUFile:  # pylint: disable=too-many-instance-attributes, invalid-name
     """Class to store DFU file data"""
-
-    name: str
-    filep: io.FileIO = field(default=None)
+    name: [str, None]
+    file_p: io.FileIO = field(default=None)
     size: int = field(default=0)
     dwCRC: int = field(default=0)
-    suffixlen: int = field(default=0)
+    suffix_len: int = field(default=0)
     bcdDFU: int = field(default=0)
     idVendor: int = field(default=0xffff)  # wildcard value
     idProduct: int = field(default=0xffff)  # wildcard value
     bcdDevice: int = field(default=0xffff)  # wildcard value
 
+    def parse_dfu_suffix(self) -> int:
+        """Bind parse_dfu_suffix to DFUFile instance"""
+        return parse_dfu_suffix(self)
+
+    def generate_dfu_suffix(self) -> int:
+        """Bind generate_dfu_suffix to DFUFile instance"""
+        return generate_dfu_suffix(self)
+
 
 def parse_dfu_suffix(file: DFUFile) -> int:
     """
-    reads the filep and name member, fills in all others
+    reads the file_p and name member, fills in all others
     :param file:
     :return: 0 if no DFU suffix, positive if valid DFU suffix, negative on file read error
     """
 
     crc = 0xffffffff
-    dfusuffix = bytearray([0] * DFU_SUFFIX_LENGTH)
+    dfu_suffix = bytearray([0] * DFU_SUFFIX_LENGTH)
 
     try:
-        with io.FileIO(file.name, 'rb') as file.filep:
-            file.size = file.filep.seek(0, os.SEEK_END)
-            file.filep.seek(0)
+        with io.FileIO(file.name, 'rb') as file.file_p:
+            file.size = file.file_p.seek(0, os.SEEK_END)
+            file.file_p.seek(0)
 
             if file.size < DFU_SUFFIX_LENGTH:
-                logger.error("File too short for DFU suffix")
+                _logger.error("File too short for DFU suffix")
                 return 0
 
-            firmware = bytearray(file.filep.read(file.size))
+            firmware = bytearray(file.file_p.read(file.size))
 
             for i in range(file.size - 4):
                 crc = crc32_byte(crc, firmware[i])
 
             del firmware
 
-            file.filep.seek(-DFU_SUFFIX_LENGTH, os.SEEK_END)
-            ret = file.filep.readinto(dfusuffix)
+            file.file_p.seek(-DFU_SUFFIX_LENGTH, os.SEEK_END)
+            ret = file.file_p.readinto(dfu_suffix)
 
             if ret < 0:
-                logger.error("Could not read DFU suffix")
+                _logger.error("Could not read DFU suffix")
                 return ret
             if ret < DFU_SUFFIX_LENGTH:
-                logger.error("Could not read whole DFU suffix")
+                _logger.error("Could not read whole DFU suffix")
                 return -1
 
-            suffix = _suffix.parse(dfusuffix)
+            suffix = _suffix.parse(dfu_suffix)
             file.dwCRC = suffix.dwCRC
 
             if file.dwCRC != crc:
-                logger.error("DFU CRC does not match")
+                _logger.error("DFU CRC does not match")
                 return 0
 
             file.bcdDFU = suffix.bcdDFU
-            logger.info(f"Dfu suffix version {hex(file.bcdDFU)}")
+            _logger.info(f"Dfu suffix version {hex(file.bcdDFU)}")
 
-            file.suffixlen = dfusuffix[11]
-            if file.suffixlen < DFU_SUFFIX_LENGTH:
-                logger.error(f"Unsupported DFU suffix length {file.suffixlen}")
+            file.suffix_len = dfu_suffix[11]
+            if file.suffix_len < DFU_SUFFIX_LENGTH:
+                _logger.error(f"Unsupported DFU suffix length {file.suffix_len}")
                 return 0
 
             file.idVendor = suffix.idVendor
             file.idProduct = suffix.idProduct
             file.bcdDevice = suffix.bcdDevice
 
     except StreamError as e:
-        logger.error(f"Could not read whole DFU suffix, {e}")
+        _logger.error(f"Could not read whole DFU suffix, {e}")
         ret = -1
     except ConstError as e:
-        logger.error(f"No valid DFU suffix signature, {e}")
+        _logger.error(f"No valid DFU suffix signature, {e}")
         ret = 0
     except Exception as e:
-        logger.exception(e)
+        _logger.exception(e)
         ret = -1
     return ret
 
 
 def generate_dfu_suffix(file: DFUFile) -> int:
     """
     reads file, generates CRC and adds DFU suffix to file
     :param file:
     :return: positive on success, negative on errors
     """
 
     file.size = 0
     file.dwCRC = 0xffffffff
-    file.suffixlen = DFU_SUFFIX_LENGTH
+    file.suffix_len = DFU_SUFFIX_LENGTH
     file.bcdDFU = 0x0100  # Default to bcdDFU version 1.0
 
     suffix_data = {
         'bcdDevice': file.bcdDevice,
         'idProduct': file.idProduct,
         'idVendor': file.idVendor,
         'bcdDFU': file.bcdDFU,
-        'bLength': file.suffixlen
+        'bLength': file.suffix_len
     }
 
-    dfusuffix = bytearray(_suffix.build(suffix_data))
+    dfu_suffix = bytearray(_suffix.build(suffix_data))
 
     try:
-        with io.FileIO(file.name, 'rb+') as filep:
-            file.size = filep.seek(0, os.SEEK_END)
-            filep.seek(0)
+        with io.FileIO(file.name, 'rb+') as file_p:
+            file.size = file_p.seek(0, os.SEEK_END)
+            file_p.seek(0)
 
             # Make space for all but CRC
-            firmware = bytearray(filep.read(file.size))
-            firmware.extend(dfusuffix[:12])
+            firmware = bytearray(file_p.read(file.size))
+            firmware.extend(dfu_suffix[:12])
             # Calculate CRC. It is calculated over file and suffix excluding the CRC itself
-            for i in range(file.size + file.suffixlen - 4):
+            for i in range(file.size + file.suffix_len - 4):
                 file.dwCRC = crc32_byte(file.dwCRC, firmware[i])
 
             del firmware
 
-            dfusuffix[12:16] = ByteSwapped(_suffix.subcon.dwCRC).build(file.dwCRC)
+            dfu_suffix[12:16] = ByteSwapped(_suffix.subcon.dwCRC).build(file.dwCRC)
 
             # Move to the end of the file
-            filep.seek(0, os.SEEK_END)
+            file_p.seek(0, os.SEEK_END)
 
             # Add the suffix at the end of the file
-            ret = filep.write(dfusuffix)
+            ret = file_p.write(dfu_suffix)
 
     except Exception as e:
-        logger.exception(e)
+        _logger.exception(e)
         ret = -1
 
     return ret
```

### Comparing `pydfuutil-0.0.2b2/pydfuutil/dfu_load.py` & `pydfuutil-0.0.2b3/pydfuutil/dfu_load.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,20 @@
 """
 (C) 2023 Yaroshenko Dmytro (https://github.com/o-murphy)
 """
 import logging
 
-from rich import progress
-
 from pydfuutil import dfu
 from pydfuutil.dfu_file import DFUFile
-from pydfuutil.logger import get_logger
+from pydfuutil.logger import logger
 from pydfuutil.portable import milli_sleep
+from pydfuutil.progress import Progress
 from pydfuutil.quirks import QUIRK_POLLTIMEOUT, DEFAULT_POLLTIMEOUT
 
-logger = get_logger(__name__)
-
-# VERBOSE: bool = False  # useless?
-
-_progress_bar = progress.Progress(
-    progress.TextColumn("[progress.description]{task.description}"),
-    progress.BarColumn(20),
-    progress.TaskProgressColumn(),
-    progress.TimeRemainingColumn(),
-    progress.DownloadColumn(),
-    progress.TransferSpeedColumn(),
-)
-
-PROGRESS_BAR_WIDTH = 50
+_logger = logger.getChild(__name__.rsplit('.', maxsplit=1)[-1])
 
 
 def do_upload(dif: dfu.DfuIf,
               xfer_size: int,
               file: DFUFile = None,
               total_size: int = -1) -> [int, bytes]:
     """
@@ -36,163 +22,150 @@
     :param dif: dfu.dfu_if
     :param xfer_size: chunk size
     :param file: optional - DFUFile object
     :param total_size: optional - total bytes expected to be uploaded
     :return: uploaded bytes or error code
     """
 
-    logger.info(f"bytes_per_hash={xfer_size}")
-    logger.info("Copying data from DFU device to PC")
-
-    upload_task = _progress_bar.add_task(
-        '[magenta1]Starting upload',
-        total=total_size if total_size >= 0 else None
-    )
+    _logger.info(f"bytes_per_hash={xfer_size}")
+    _logger.info("Copying data from DFU device to PC")
 
     total_bytes = 0
     transaction = dfu.TRANSACTION  # start page
     buf = bytearray(xfer_size)
 
-    while True:
-        # rc = dfu.upload(
-        #     device=dif.dev,
-        #     interface=dif.interface,
-        #     transaction=transaction,
-        #     data_or_length=buf
-        # )
-
-        rc = dif.upload(transaction, buf)
-
-        if len(rc) < 0:
-            ret = rc
-            break
+    with Progress() as progress:
+        progress.start_task(
+            description="Starting upload",
+            total=total_size if total_size >= 0 else None
+        )
 
-        if file:
-            write_rc = file.filep.write(rc)
+        while True:
+            rc = dif.upload(transaction, buf)
 
-            if write_rc < len(rc):
-                logger.error(f'Short file write: {write_rc}')
-                ret = total_bytes
+            if len(rc) < 0:
+                ret = rc
                 break
 
-        total_bytes += len(rc)
+            if file:
+                write_rc = file.file_p.write(rc)
+
+                if write_rc < len(rc):
+                    _logger.error(f'Short file write: {write_rc}')
+                    ret = total_bytes
+                    break
+
+            total_bytes += len(rc)
+
+            transaction += 1
+            progress.update(advance=xfer_size, description="Uploading...")
 
-        # last block, return
-        if (len(rc) < xfer_size) or (total_bytes >= total_size >= 0):
-            ret = total_bytes
-            break
-
-        transaction += 1
-        # _progress_bar.update(upload_task, advance=xfer_size)
-        _progress_bar.update(upload_task, advance=xfer_size, description='[magenta1]Uploading...')
-
-    _progress_bar.update(upload_task, description='[yellow4]Upload finished!')
-    _progress_bar.stop()
-    _progress_bar.remove_task(upload_task)
+            # last block, return
+            if (len(rc) < xfer_size) or (total_bytes >= total_size >= 0):
+                ret = total_bytes
+                break
+
+        progress.update(description='Upload finished!')
 
-    logger.debug(f"Received a total of {total_bytes} bytes")
-    return ret
+        _logger.debug(f"Received a total of {total_bytes} bytes")
+        return ret
 
 
 # pylint: disable=too-many-branches
 def do_dnload(dif: dfu.DfuIf, xfer_size: int, file: DFUFile, quirks: int, verbose: bool) -> int:
     """
     :param dif: DfuIf instance
     :param xfer_size: transaction size
     :param file: DFUFile instance
     :param quirks: quirks
     :param verbose: is verbose
     :return:
     """
 
-    logger.setLevel(logging.DEBUG if verbose else logging.INFO)
+    _logger.setLevel(logging.DEBUG if verbose else logging.INFO)
 
     bytes_sent = 0
     buf = bytearray(xfer_size)
 
-    bytes_per_hash = (file.size - file.suffixlen) // PROGRESS_BAR_WIDTH
-    if bytes_per_hash == 0:
-        bytes_per_hash = 1
-    logger.info(f"bytes_per_hash={bytes_per_hash}")
-
-    logger.info("Copying data from PC to DFU device")
-    logger.info("Starting download: ")
-    print("[", end="")
-
+    _logger.info("Copying data from PC to DFU device")
+    _logger.info("Starting download: ")
     try:
-        while bytes_sent < file.size - file.suffixlen:
-            # FIXME: no idea what's there
-            # bytes_left = file.size - file.suffixlen - bytes_sent
-            # chunk_size = min(bytes_left, xfer_size)
-
-            if (ret := file.filep.readinto(buf)) < 0:  # Handle read error
-                raise IOError(f"Error reading file: {file.name}")
-
-            # ret = dfu.download(dif.dev, dif.interface, ret, buf[:ret] if ret else None)
-            ret = dif.download(ret, buf[:ret] if ret else None)
-
-            if ret < 0:
-                raise IOError("Error during download")
-            bytes_sent += ret
 
-            while True:
-                # if int(status := dfu.get_status(dif.dev, dif.interface)) < 0:
-                if int(status := dif.get_status()) < 0:
-                    raise IOError("Error during download get_status")
-                if status.bState in (dfu.State.DFU_DOWNLOAD_IDLE, dfu.State.DFU_ERROR):
-                    break
-                # Wait while the device executes flashing
-                milli_sleep(
-                    DEFAULT_POLLTIMEOUT
-                    if quirks & QUIRK_POLLTIMEOUT
-                    else status.bwPollTimeout
-                )
-
-            if status.bStatus != dfu.Status.OK:
-                print(" failed!")
-                print(f"state({status.bState}) = {status.bState.to_string()}, "
-                      f"status({status.bStatus}) = {status.bStatus.to_string()}")
-                raise IOError("Failed")
-
-            print("#" * (bytes_sent // bytes_per_hash), end="")
-
-        # Send one zero-sized download request to signalize end
-        # if dfu.download(dif.dev, dif.interface, dfu.TRANSACTION, bytes()) < 0:
-        if dif.download(dfu.TRANSACTION, bytes()) < 0:
-            raise IOError("Error sending completion packet")
-
-        print("]")
-        logger.info("finished!")
-        logger.debug(f"Sent a total of {bytes_sent} bytes")
-
-        # Transition to MANIFEST_SYNC state
-        # if int(status := dfu.get_status(dif.dev, dif.interface)) < 0:
-        if int(status := dif.get_status()) < 0:
-            raise IOError("Unable to read DFU status")
-        logger.info(f"state({status.bState}) = {status.bState.to_string()}, "
-                    f"status({status.bStatus}) = {status.bStatus.to_string()}")
-
-        if not quirks & QUIRK_POLLTIMEOUT:
-            milli_sleep(status.bwPollTimeout)
-
-        # Deal correctly with ManifestationTolerant=0 / WillDetach bits
-        while status.bState in (dfu.State.DFU_MANIFEST_SYNC, dfu.State.DFU_MANIFEST):
-            # Some devices need some time before we can obtain the status
-            milli_sleep(1000)
-            # if int(status := dfu.get_status(dif.dev, dif.interface)) < 0:
+        with Progress() as progress:
+            total_size = file.size - file.suffix_len
+            progress.start_task(
+                description="Starting download",
+                total=total_size if total_size >= 0 else None
+            )
+
+            while bytes_sent < file.size - file.suffix_len:
+                # Note: no idea what's there
+                # bytes_left = file.size - file.suffix_len - bytes_sent
+                # chunk_size = min(bytes_left, xfer_size)
+
+                if (ret := file.file_p.readinto(buf)) < 0:  # Handle read error
+                    raise IOError(f"Error reading file: {file.name}")
+
+                ret = dif.download(ret, buf[:ret] if ret else None)
+
+                if ret < 0:
+                    raise IOError("Error during download")
+                bytes_sent += ret
+
+                while True:
+                    if int(status := dif.get_status()) < 0:
+                        raise IOError("Error during download get_status")
+                    if status.bState in (dfu.State.DFU_DOWNLOAD_IDLE, dfu.State.DFU_ERROR):
+                        break
+                    # Wait while the device executes flashing
+                    milli_sleep(
+                        DEFAULT_POLLTIMEOUT
+                        if quirks & QUIRK_POLLTIMEOUT
+                        else status.bwPollTimeout
+                    )
+
+                if status.bStatus != dfu.Status.OK:
+                    logger.error("Transfer failed!")
+                    print(f"state({status.bState}) = {status.bState.to_string()}, "
+                          f"status({status.bStatus}) = {status.bStatus.to_string()}")
+                    raise IOError("Downloading failed!")
+
+                progress.update(description="Downloading...", advance=xfer_size)
+
+            # Send one zero-sized download request to signalize end
+            if dif.download(dfu.TRANSACTION, bytes()) < 0:
+                raise IOError("Error sending completion packet")
+
+            progress.update(description="Download finished!")
+            _logger.info("finished!")
+            _logger.debug(f"Sent a total of {bytes_sent} bytes")
+
+            # Transition to MANIFEST_SYNC state
             if int(status := dif.get_status()) < 0:
                 raise IOError("Unable to read DFU status")
-            print(f"state({status.bState}) = {status.bState.to_string()}, "
-                  f"status({status.bStatus}) = {status.bStatus.to_string()}")
+            _logger.info(f"state({status.bState}) = {status.bState.to_string()}, "
+                         f"status({status.bStatus}) = {status.bStatus.to_string()}")
+
+            if not quirks & QUIRK_POLLTIMEOUT:
+                milli_sleep(status.bwPollTimeout)
+
+            # Deal correctly with ManifestationTolerant=0 / WillDetach bits
+            while status.bState in (dfu.State.DFU_MANIFEST_SYNC, dfu.State.DFU_MANIFEST):
+                # Some devices need some time before we can obtain the status
+                milli_sleep(1000)
+                if int(status := dif.get_status()) < 0:
+                    raise IOError("Unable to read DFU status")
+                _logger.info(f"state({status.bState}) = {status.bState.to_string()}, "
+                             f"status({status.bStatus}) = {status.bStatus.to_string()}")
 
-        if status.bState == dfu.State.DFU_IDLE:
-            logger.info("Done!")
+            if status.bState == dfu.State.DFU_IDLE:
+                _logger.info("Done!")
 
     except IOError as err:
-        logger.error(err)
+        _logger.error(err)
         return -1
 
     return bytes_sent
 
 
 def init() -> None:
     """Init dfu_load props"""
```

### Comparing `pydfuutil-0.0.2b2/pydfuutil/dfuse.py` & `pydfuutil-0.0.2b3/pydfuutil/dfuse.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,28 +5,25 @@
 """
 import argparse
 import errno
 import sys
 from enum import Enum
 
 import usb.util
-from construct import Int32ul
 
 from pydfuutil import dfu
 from pydfuutil.dfu_file import DFUFile
-from pydfuutil.dfuse_mem import find_segment, DFUSE, parse_memory_layout, free_segment_list
-from pydfuutil.logger import get_logger
+from pydfuutil.dfuse_mem import find_segment, DFUSE, parse_memory_layout, MemSegment
+from pydfuutil.logger import logger
 from pydfuutil.portable import milli_sleep
 
-logger = get_logger(__name__)
-logger.warning("Module pydfuutil.dfuse aren't work as expected, "
-               "will reimplemented in future")
+_logger = logger.getChild(__name__.rsplit('.', maxsplit=1)[-1])
 
 VERBOSE = False
-MEM_LAYOUT: list = []
+MEM_LAYOUT: [MemSegment, None] = None
 
 TIMEOUT = 5000
 
 
 class Command(Enum):
     """DFUSE commands"""
     SET_ADDRESS = 0x1
@@ -37,15 +34,15 @@
 
 def quad2uint(p: bytes) -> int:
     """
     Convert a 4-byte sequence into an unsigned integer (little-endian).
     :param p: 4-byte sequence
     :return: Converted unsigned integer
     """
-    return Int32ul.parse(p)
+    return int.from_bytes(p, byteorder='little', signed=False)
 
 
 def parse_options(options: str) -> argparse.Namespace:
     """
     Parse DFU options string and set corresponding flags and values.
     :param options: DFU options string containing address, modifiers, and values.
     :return: None
@@ -69,35 +66,35 @@
     :param dif: DFU interface
     :param address: Address for the command
     :param command: DfuSe command to execute
     :return: None
     """
     buf = bytearray(5)
 
-    length: int
     ret: int
     dst: [dict, None]
 
     try:
 
         if command == Command.ERASE_PAGE:
             segment = find_segment(MEM_LAYOUT, address)
+
             if not segment or not segment.mem_type & DFUSE.ERASABLE:
                 raise IOError(f"Page at 0x{address:08x} cannot be erased")
 
             page_size = segment.pagesize
             if VERBOSE > 1:
-                logger.info(
+                _logger.info(
                     f"Erasing page size {page_size} at address 0x{address:08x}, "
                     f"page starting at 0x{address & ~(page_size - 1):08x}")
-            buf[0], length = 0x41, 5  # Erase command
-            # last_erased = address  # useless?
+            buf[0], length = 0x41, 5  # Note: Unused variable 'length'
+            # last_erased = address  # Note: useless?
         elif command == Command.SET_ADDRESS:
             if VERBOSE > 2:
-                logger.debug(f"Setting address pointer to 0x{address:08x}")
+                _logger.debug(f"Setting address pointer to 0x{address:08x}")
             buf[0], length = 0x21, 5  # Set Address Pointer command
         elif command == Command.MASS_ERASE:
             buf[0], length = 0x41, 1  # Mass erase command when length = 1
         elif command == Command.READ_UNPROTECT:
             buf[0], length = 0x92, 1
         else:
             raise ValueError(f"Non-supported special command {command}")
@@ -108,73 +105,68 @@
 
         # for i in range(1, 5):
         #     buf[i] = (address >> (8 * (i - 1))) & 0xFF
 
         for i in range(0, 4):
             buf[i + 1] = (address >> (8 * i)) & 0xFF
 
-        if download(dif, length, buf, 0) < 0:
+        if download(dif, buf, 0) < 0:
             raise IOError("Error during special command download")
 
-        # ret = int(dst := dfu.get_status(dif.dev, dif.interface))
         ret = int(dst := dif.get_status())
         if ret < 0:
             raise IOError("Error during special command get_status")
 
         if dst.bState != dfu.State.DFU_DOWNLOAD_BUSY:
             raise IOError("Wrong state after command download")
 
         # Wait while command is executed
         if VERBOSE:
-            logger.info(f"Poll timeout {dst.bwPollTimeout} ms")
+            _logger.info(f"Poll timeout {dst.bwPollTimeout} ms")
 
         milli_sleep(dst.bwPollTimeout)
 
         if command == Command.READ_UNPROTECT:
             return ret
 
-        # ret = int(dst := dfu.get_status(dif.dev, dif.interface))
         ret = int(dst := dif.get_status())
         if ret < 0:
-            logger.error(
+            _logger.error(
                 f"state({dst.bState}) = {dst.bState.to_string()}, "
                 f"status({dst.bStatus}) = {dst.bStatus.to_string()}")
             raise IOError("Error during second get_status")
 
         if dst.bStatus != dfu.Status.OK:
             raise IOError("Command not correctly executed")
 
         milli_sleep(dst.bwPollTimeout)
 
-        # if dfu.abort(dif.dev, dif.interface) < 0:
         if dif.abort() < 0:
             raise IOError("Error sending dfu abort request")
 
-        # ret = int(dst := dfu.get_status(dif.dev, dif.interface))
         ret = int(dst := dif.get_status())
         if ret < 0:
             raise IOError("Error during abort get_status")
 
         if dst.bState != dfu.State.DFU_IDLE:
             raise IOError("Failed to enter idle state on abort")
 
     except (ValueError, IOError) as err:
-        logger.error(err)
+        _logger.error(err)
         sys.exit(1)
 
     milli_sleep(dst.bwPollTimeout)
     return ret
 
 
-def upload(dif: dfu.DfuIf, length: int, data: bytes, transaction: int) -> int:
+def upload(dif: dfu.DfuIf, data: bytes, transaction: int) -> int:
     """
     UPLOAD request for DfuSe 1.1a
 
     :param dif: The USB device handle
-    :param length: The length of the data to upload
     :param data: The data buffer to store the uploaded data
     :param transaction: The transaction ID for the upload
     :return: The status of the control transfer
     """
     status = dif.dev.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_IN |
                       usb.util.CTRL_TYPE_CLASS |
@@ -183,25 +175,24 @@
         wValue=transaction,
         wIndex=dif.interface,
         data_or_wLength=data,
         timeout=TIMEOUT
     )
 
     if status < 0:
-        logger.error(f"{upload.__name__}: libusb_control_msg returned {status}")
+        _logger.error(f"{upload.__name__}: libusb_control_msg returned {status}")
 
     return status
 
 
-def download(dif: dfu.DfuIf, length: int, data: bytes, transaction: int) -> int:
+def download(dif: dfu.DfuIf, data: bytes, transaction: int) -> int:
     """
     DNLOAD request for DfuSe 1.1a
 
     :param dif: The DFU interface object.
-    :param length: The length of the data to download.
     :param data: The data buffer to download.
     :param transaction: The transaction ID for the download.
     :return: The status of the control transfer.
     """
     status = dif.dev.ctrl_transfer(
         bmRequestType=usb.util.ENDPOINT_OUT |
                       usb.util.CTRL_TYPE_CLASS |
@@ -210,15 +201,15 @@
         wValue=transaction,
         wIndex=dif.interface,
         data_or_wLength=data,
         timeout=TIMEOUT
     )
 
     if status < 0:
-        logger.error(f"{download.__name__}: "
+        _logger.error(f"{download.__name__}: "
                      f"libusb_control_transfer returned {status}")
 
     return status
 
 
 def do_upload(dif: dfu.DfuIf, xfer_size: int, file: DFUFile, dfuse_options: [str, bytes]) -> int:
     """
@@ -243,51 +234,49 @@
             parsed_args = parse_options(dfuse_options)
             if parsed_args.length:
                 upload_limit = parsed_args.length
         else:
             raise ValueError("No options provided")
 
         if parsed_args.address:
-            # MEM_LAYOUT = parse_memory_layout(dif.alt_name.decode())
             MEM_LAYOUT = parse_memory_layout(dif.alt_name)  # HOTFIX
             if not MEM_LAYOUT:
                 raise IOError("Failed to parse memory layout")
 
             segment = find_segment(MEM_LAYOUT, parsed_args.address)
             if not parsed_args.force and (not segment or not segment.mem_type & DFUSE.READABLE):
                 raise IOError(f"Page at 0x{parsed_args.address:08x} is not readable")
 
             if not upload_limit:
                 upload_limit = segment.end - parsed_args.address + 1
-                logger.info(f"Limiting upload to end of memory segment, {upload_limit} bytes")
+                _logger.info(f"Limiting upload to end of memory segment, {upload_limit} bytes")
             special_command(dif, parsed_args.address, Command.SET_ADDRESS)
         else:
             # Bootloader decides the start address, unknown to us
             # Use a short length to lower risk of running out of bounds
             if not upload_limit:
                 upload_limit = 0x4000
-            logger.info("Limiting default upload to %i bytes", upload_limit)
+            _logger.info("Limiting default upload to %i bytes", upload_limit)
 
-        logger.info(f"bytes_per_hash={xfer_size}")
-        print("Starting upload: [")
+        _logger.info(f"bytes_per_hash={xfer_size}")
+        print("Starting upload: [")  # TODO: Progress
     except (ValueError, IOError) as err:
-        logger.error(err)
+        _logger.error(err)
         return -1
 
     while True:
-        if upload_limit - total_bytes < xfer_size:
-            xfer_size = upload_limit - total_bytes
-        rc = upload(dif, xfer_size, buf, transaction)
+        xfer_size = min(xfer_size, upload_limit - total_bytes)
+        rc = upload(dif, buf, transaction)
         if rc < 0:
-            logger.error("Error during upload")
+            _logger.error("Error during upload")
             ret = rc
             break
-        write_rc = file.filep.write(buf[:rc])
+        write_rc = file.file_p.write(buf[:rc])
         if write_rc < rc:
-            logger.error(f"Short file write: {rc}")
+            _logger.error(f"Short file write: {rc}")
             ret = -1
             break
         total_bytes += rc
         if rc < xfer_size or total_bytes >= upload_limit:
             # Last block, return successfully
             ret = total_bytes
             break
@@ -305,109 +294,105 @@
     :param dif: DfuIf object representing the DFU interface
     :param data: Data to be downloaded
     :param size: Size of the data chunk
     :param transaction: Transaction number
     :return: Number of bytes sent or error code
     """
 
-    ret = download(dif, size, data if size else None, transaction)
+    ret = download(dif, data if size else None, transaction)
 
     if ret < 0:
-        logger.error("Error during download")
+        _logger.error("Error during download")
         return ret
 
     bytes_sent = ret
 
     while True:
-        # ret = int(status := dfu.get_status(dif.dev, dif.interface))
         ret = int(status := dif.get_status())
         if ret < 0:
-            logger.error("Error during download get_status")
+            _logger.error("Error during download get_status")
             return ret
 
         # dst = ret # useless?
         milli_sleep(status.bwPollTimeout)
 
         if status.bState in (dfu.State.DFU_DOWNLOAD_IDLE,
                              dfu.State.DFU_ERROR,
                              dfu.State.DFU_MANIFEST):
             break
 
     if status.bState == dfu.State.DFU_MANIFEST:
-        logger.info("Transitioning to dfuMANIFEST state")
+        _logger.info("Transitioning to dfuMANIFEST state")
 
     if status.bStatus != dfu.Status.OK:
-        logger.error("Download failed!")
-        logger.error("state(%u) = %s, status(%u) = %s", status.bState,
-                     status.bState.to_string(), status.bStatus,
-                     status.bStatus.to_string())
+        _logger.error("Download failed!")
+        _logger.error("state(%u) = %s, status(%u) = %s", status.bState,
+                      status.bState.to_string(), status.bStatus,
+                      status.bStatus.to_string())
         return -1
 
     return bytes_sent
 
 
 # Writes an element of any size to the device, taking care of page erases
 # returns 0 on success, otherwise -EINVAL
 # pylint: disable=invalid-name
 def dnload_element(dif: dfu.DfuIf,
-                   dwElementAddress: int,
-                   dwElementSize: int,
+                   dw_element_address: int,
+                   dw_element_size: int,
                    data: bytes,
                    xfer_size: int) -> int:
     """
     Download an element in DFU.
 
     :param dif: DfuIf object representing the DFU interface
-    :param dwElementAddress: Element address
-    :param dwElementSize: Size of the element
+    :param dw_element_address: Element address
+    :param dw_element_size: Size of the element
     :param data: Data to be downloaded
     :param xfer_size: Transfer size
     :return: 0 if successful, error code otherwise
     """
 
     ret = 0
-    segment = find_segment(MEM_LAYOUT, dwElementAddress + dwElementSize - 1)
+    segment = find_segment(MEM_LAYOUT, dw_element_address + dw_element_size - 1)
 
     if not segment or not segment.mem_type & DFUSE.WRITEABLE:
-        logger.error(
-            f"Error: Last page at 0x{dwElementAddress + dwElementSize - 1:08x} is not writeable"
+        _logger.error(
+            f"Error: Last page at 0x{dw_element_address + dw_element_size - 1:08x} is not writeable"
         )
         return -1
 
     p = 0
-    while p < dwElementSize:
-        # page_size = segment.pagesize  # useless?
-        address = dwElementAddress + p
-        chunk_size = min(xfer_size, dwElementSize - p)
+    while p < dw_element_size:
+        address = dw_element_address + p
+        chunk_size = min(xfer_size, dw_element_size - p)
 
         segment = find_segment(MEM_LAYOUT, address)
         if not segment or not segment.mem_type & DFUSE.WRITEABLE:
-            logger.error(f"Error: Page at 0x{address:08x} is not writeable")
+            _logger.error(f"Error: Page at 0x{address:08x} is not writeable")
             return -1
 
         if VERBOSE:
-            logger.info(f"Download from image offset {p:08x} "
+            _logger.info(f"Download from image offset {p:08x} "
                         f"to memory {address:08x}-{address + chunk_size - 1:08x}"
                         f", size {chunk_size}")
-        else:
-            logger.info(".")
 
         special_command(dif, address, Command.SET_ADDRESS)
 
         # transaction = 2 for no address offset
         ret = dnload_chunk(dif, data[p:p + chunk_size], chunk_size, 2)
         if ret != chunk_size:
-            logger.error(f"Failed to write whole chunk: {ret} of {chunk_size} bytes")
+            _logger.error(f"Failed to write whole chunk: {ret} of {chunk_size} bytes")
             return -1
 
         # Move to the next chunk
         p += xfer_size
 
     if not VERBOSE:
-        logger.info("")
+        _logger.info("")
 
     return ret
 
 
 # Download raw binary file to DfuSe device
 def do_bin_dnload(dif: dfu.DfuIf, xfer_size: int, file: DFUFile, start_address: int) -> int:
     """
@@ -418,97 +403,98 @@
     :param file: DFUFile object containing the binary file
     :param start_address: Start address for the download
     :return: Number of bytes read or error code
     """
     dwElementAddress = start_address
     dwElementSize = file.size
 
-    logger.info(f"Downloading to address = 0x{dwElementAddress:08x}, size = {dwElementSize}")
+    _logger.info(f"Downloading to address = 0x{dwElementAddress:08x}, size = {dwElementSize}")
 
-    data = file.filep.read()
+    data = file.file_p.read()
     read_bytes = len(data)
 
     ret = dnload_element(dif, dwElementAddress, dwElementSize, data, xfer_size)
     if ret != 0:
         return ret
 
     if read_bytes != file.size:
-        logger.warning(f"Read {read_bytes} bytes, file size {file.size}")
+        _logger.warning(f"Read {read_bytes} bytes, file size {file.size}")
 
-    logger.info("File downloaded successfully")
+    _logger.info("File downloaded successfully")
     return read_bytes
 
 
 # Parse a DfuSe file and download contents to device
 def do_dfuse_dnload(dif: dfu.DfuIf, xfer_size: int, file: DFUFile) -> int:
     """
     Download data from a DfuSe file to the DFU device.
 
     :param dif: DfuIf object representing the DFU interface
     :param xfer_size: Transfer size
     :param file: DFUFile object containing the DfuSe file
     :return: Number of bytes read or error code
     """
-    dfuprefix = file.filep.read(11)
-    read_bytes = len(dfuprefix)
+    dfu_prefix = file.file_p.read(11)
+    read_bytes = len(dfu_prefix)
 
-    if dfuprefix != b'DfuSe\x01':
-        logger.error("No valid DfuSe signature")
+    if b'DfuSe\x01' not in dfu_prefix:
+        _logger.error("No valid DfuSe signature")
         return -errno.EINVAL
 
-    bTargets = dfuprefix[10]
-    logger.info(f"File contains {bTargets} DFU images")
+    bTargets = dfu_prefix[10]
+    _logger.info(f"File contains {bTargets} DFU images")
 
     for image in range(1, bTargets + 1):
-        logger.info(f"Parsing DFU image {image}")
-        target_prefix = file.filep.read(274)
+        _logger.info(f"Parsing DFU image {image}")
+        target_prefix = file.file_p.read(274)
         read_bytes += len(target_prefix)
 
         if target_prefix[:6] != b'Target':
-            logger.error("No valid target signature")
+            _logger.error("No valid target signature")
             return -errno.EINVAL
 
         bAlternateSetting = target_prefix[6]
-        dwNbElements = Int32ul.parse(target_prefix[266:270])
-        logger.info(
+        dwNbElements = int.from_bytes(target_prefix[266:270], byteorder='little')
+        size = int.from_bytes(target_prefix[270:274], byteorder='little')
+        _logger.info(
             f"Image for alternate setting {bAlternateSetting}, "
-            f"({dwNbElements} elements, total size = {Int32ul.parse(target_prefix[270:274])})")
+            f"({dwNbElements} elements, total size = {size})")
 
         if bAlternateSetting != dif.altsetting:
-            logger.warning("Image does not match current alternate setting.")
-            logger.warning("Please rerun with the correct -a option setting"
+            _logger.warning("Image does not match current alternate setting.")
+            _logger.warning("Please rerun with the correct -a option setting"
                            " to download this image!")
 
         for element in range(1, dwNbElements + 1):
-            logger.info(f"Parsing element {element}")
-            elementheader = file.filep.read(8)
-            dwElementAddress, dwElementSize = Int32ul[2].parse(elementheader)
-            logger.info(f"Address = 0x{dwElementAddress:08x}, Size = {dwElementSize}")
+            _logger.info(f"Parsing element {element}")
+            element_header = file.file_p.read(8)
+            dwElementAddress, dwElementSize, *_ = element_header
+            _logger.info(f"Address = 0x{dwElementAddress:08x}, Size = {dwElementSize}")
 
             # Sanity check
-            if read_bytes + dwElementSize + file.suffixlen > file.size:
-                logger.error("File too small for element size")
+            if read_bytes + dwElementSize + file.suffix_len > file.size:
+                _logger.error("File too small for element size")
                 return -errno.EINVAL
 
-            data = file.filep.read(dwElementSize)
+            data = file.file_p.read(dwElementSize)
             read_bytes += len(data)
 
             if bAlternateSetting == dif.altsetting:
                 ret = dnload_element(dif, dwElementAddress, dwElementSize, data, xfer_size)
                 if ret != 0:
                     return ret
 
     # Read through the whole file for bookkeeping
-    file.filep.read(file.suffixlen)
-    read_bytes += file.suffixlen
+    file.file_p.read(file.suffix_len)
+    read_bytes += file.suffix_len
 
     if read_bytes != file.size:
-        logger.warning(f"Read {read_bytes} bytes, file size {file.size}")
+        _logger.warning(f"Read {read_bytes} bytes, file size {file.size}")
 
-    logger.info("Done parsing DfuSe file")
+    _logger.info("Done parsing DfuSe file")
     return read_bytes
 
 
 def do_dnload(dif: dfu.DfuIf, xfer_size: int, file: DFUFile, dfuse_options: [str, bytes]) -> int:
     """
     Perform DFU download operation.
 
@@ -525,56 +511,56 @@
 
     try:
         if not dfuse_options:
             raise ValueError("No DFUse options provided")
 
         opts = parse_options(dfuse_options)
 
-        # MEM_LAYOUT = parse_memory_layout(dif.alt_name.decode())
         MEM_LAYOUT = parse_memory_layout(dif.alt_name)  # HOTFIX
         if not MEM_LAYOUT:
             raise IOError("Failed to parse memory layout")
 
         if opts.unprotect:
             if not opts.force:
                 raise PermissionError(
                     "The read unprotect command will erase the flash memory"
                     " and can only be used with force"
                 )
             special_command(dif, 0, Command.READ_UNPROTECT)
-            logger.info("Device disconnects, erases flash and resets now")
+            _logger.info("Device disconnects, erases flash and resets now")
             sys.exit(0)
 
         if opts.mass_erase:
             if not opts.force:
                 raise PermissionError("The mass erase command can only be used with force")
-            logger.info("Performing mass erase, this can take a moment")
+            _logger.info("Performing mass erase, this can take a moment")
             special_command(dif, 0, Command.MASS_ERASE)
 
     except (ValueError, PermissionError, IOError) as err:
-        logger.error(err)
+        _logger.error(err)
         sys.exit(1)
 
     if opts.address:
         if file.bcdDFU == 0x11a:
-            logger.error("This is a DfuSe file, not meant for raw download")
+            _logger.error("This is a DfuSe file, not meant for raw download")
             return -1
         ret = do_bin_dnload(dif, xfer_size, file, opts.address)
     else:
         if file.bcdDFU != 0x11a:
-            logger.error("Only DfuSe file version 1.1a is supported"
+            _logger.error("Only DfuSe file version 1.1a is supported"
                          ", (for raw binary download, use the --dfuse-address option)")
             return -1
         ret = do_dfuse_dnload(dif, xfer_size, file)
 
-    free_segment_list(MEM_LAYOUT)
+    # free_segment_list(MEM_LAYOUT)
+    MEM_LAYOUT = None
 
     if opts.leave:
         dnload_chunk(dif, b'', 0, 2)  # Zero-size
         # ret2 = int(dst := dfu.get_status(dif.dev, dif.interface))
         ret2 = int(dst := dif.get_status())
         if ret2 < 0:
-            logger.error("Error during download get_status")
+            _logger.error("Error during download get_status")
         if VERBOSE:
-            logger.info(f"bState = {dst.bState} and bStatus = {dst.bStatus}")
+            _logger.info(f"bState = {dst.bState} and bStatus = {dst.bStatus}")
 
     return ret
```

### Comparing `pydfuutil-0.0.2b2/pydfuutil/dfuse_mem.py` & `pydfuutil-0.0.2b3/pydfuutil/dfuse_mem.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,36 @@
 """
 import logging
 import re
 from dataclasses import dataclass, field
 from enum import IntFlag
 from typing import Iterator
 
-from pydfuutil.logger import get_logger
+from pydfuutil.logger import logger
 
-logger = get_logger("dfuse_mem")
+_logger = logger.getChild(__name__.rsplit('.', maxsplit=1)[-1])
 
 
 class DFUSE(IntFlag):
     """DFUSE read/write flags"""
     READABLE = 0x1
     ERASABLE = 0x2
     WRITEABLE = 0x4
 
 
 @dataclass
 class MemSegment:
-    """Memory segment"""
+    """
+    Memory segment
+
+    We're using `segment_stack`
+    instead of `segment_list`
+    to prevent misunderstanding
+    with python's `list` type
+    """
 
     start: int = 0
     end: int = 0
     pagesize: int = 0
     mem_type: int = 0
     next: 'MemSegment' = field(default=None)
 
@@ -86,147 +93,146 @@
         if not self.next:
             self.next = new_segment
         else:
             self.next.append(new_segment)
 
     def find(self, address: int) -> ['MemSegment', None]:
         """
-        Find a memory segment in the list containing the given element.
+        Find a memory segment in the stack containing the given element.
         :param address: MemSegment address for in the stack.
         """
         if self.start <= address <= self.end:
             return self
         if self.next is not None:
             return self.next.find(address)
         return None
 
-    def free(self) -> None:
-        """Useless cause of garbage collector"""
-        raise NotImplementedError("Useless cause of garbage collector")
+    # def free(self) -> None:
+    #     """Useless cause of garbage collector"""
+    #     raise NotImplementedError("Useless cause of garbage collector")
 
 
-def add_segment(seqment_sequence: [MemSegment, None], segment: MemSegment) -> MemSegment:
+def add_segment(segment_stack: [MemSegment, None], segment: MemSegment) -> MemSegment:
     """
-    :param seqment_sequence:
+    :param segment_stack:
     :param segment:
     :return: 0 if ok
     """
     new_element = MemSegment(segment.start, segment.end, segment.pagesize, segment.mem_type)
 
-    if not seqment_sequence:
-        # list can be empty on the first call
+    if not segment_stack:
+        # stack can be empty on the first call
         return new_element
 
-    # find the last element in the list
-    seqment_sequence.append(new_element)
-    return seqment_sequence
+    # find the last element in the stack
+    segment_stack.append(new_element)
+    return segment_stack
 
 
-def find_segment(segment_stack: MemSegment, address: int) -> [MemSegment, None]:
+def find_segment(segment_stack: [MemSegment, None], address: int) -> [MemSegment, None]:
     """
-    Find a memory segment in the list containing the given element.
+    Find a memory segment in the stack containing the given element.
 
     :param segment_stack: List of MemSegment instances.
     :param address: MemSegment address for in the stack.
     :return: MemSegment instance if found, None otherwise.
     """
+    if not segment_stack:
+        return None
     return segment_stack.find(address)
 
 
-def free_segment_list(segment_stack: MemSegment) -> None:
-    """
-    Free the memory allocated for the list of memory segments.
-    :param segment_stack: List of MemSegment instances.
-    """
-    del segment_stack
+# def free_segment_list(segment_stack: MemSegment) -> None:
+#     """Useless cause of garbage collector"""
+#     raise NotImplementedError("Useless cause of garbage collector")
 
 
 # Parse memory map from interface descriptor string
 # encoded as per ST document UM0424 section 4.3.2.
 
 def parse_memory_layout(intf_desc: [str, bytes], verbose: bool = False) -> [MemSegment, None]:
     """
     Parse memory map from interface descriptor string
     encoded as per ST document UM0424 section 4.3.2.
     :param intf_desc:
     :param verbose:
     :return: MemSegment instance
     """
 
-    logger.setLevel(logging.DEBUG if verbose else logging.INFO)
+    _logger.setLevel(logging.DEBUG if verbose else logging.INFO)
 
     if isinstance(intf_desc, bytes):
         intf_desc = intf_desc.decode('ascii')
 
     count: int = 0
-    segment_list: [MemSegment, None] = None
+    segment_stack: [MemSegment, None] = None
     address: [int, None] = None
 
     match = re.match(r'@([^/]+)', intf_desc)
     if match is None:
-        logger.error(f"Could not read name, name={match}")
+        _logger.error(f"Could not read name, name={match}")
         return None
     name = match.group(1)
-    logger.info(f"DfuSe interface name: {name}")
+    _logger.info(f"DfuSe interface name: {name}")
 
     intf_desc = intf_desc[match.end():]
 
     # while per segment
     while (match := re.match(r'/0x(\d+)/', intf_desc)) is not None:
         address = int(match.group(1), 16)
 
         intf_desc = intf_desc[match.end():]
 
         # while per address
         while (match := re.match(r'(\d+)\*(\d+)(\w)(\w)[,/]?', intf_desc)) is not None:
             _sectors, _size, multiplier, type_string = match.groups()
             sectors, size = int(_sectors), int(_size)
 
-            logger.debug(f"{sectors=}, {size=}, {multiplier=}, {type_string=}")
+            _logger.debug(f"{sectors=}, {size=}, {multiplier=}, {type_string=}")
 
             intf_desc = intf_desc[match.end():]
             count += 1
             mem_type = ord(type_string)
 
             if multiplier == 'B':
                 pass
             elif multiplier == 'K':
                 size *= 1024
             elif multiplier == 'M':
                 size *= 1024 * 1024
             elif multiplier in ('a', 'b', 'c', 'd', 'e', 'f', 'g'):
                 if not mem_type:
-                    logger.warning(f"Non-valid multiplier {multiplier}, "
+                    _logger.warning(f"Non-valid multiplier {multiplier}, "
                                    "interpreted as type identifier instead")
                     mem_type = multiplier
 
-            # fallthrough if memtype was already set
+            # fallthrough if mem_type was already set
             else:
-                logger.warning(f"Non-valid multiplier {multiplier} assuming bytes")
+                _logger.warning(f"Non-valid multiplier {multiplier} assuming bytes")
 
             if not mem_type:
-                logger.warning(f"No valid type for segment {count}")
+                _logger.warning(f"No valid type for segment {count}")
 
-            segment_list = add_segment(
-                segment_list,
+            segment_stack = add_segment(
+                segment_stack,
                 MemSegment(
                     address,
                     address + sectors * size - 1,
                     size,
                     mem_type & 7
                 )
             )
 
-            logger.debug(f"Memory segment at "
+            _logger.debug(f"Memory segment at "
                          f"0x{address:08x} {sectors} x {size} = {sectors * size} "
                          f"({'r' if mem_type & DFUSE.READABLE else ''}"
                          f"{'e' if mem_type & DFUSE.ERASABLE else ''}"
                          f"{'w' if mem_type & DFUSE.WRITEABLE else ''})")
 
             address += sectors * size
 
-        logger.debug(f"Parsed details of {count} segments")
+        _logger.debug(f"Parsed details of {count} segments")
 
     if address is None:
-        logger.error(f"Could not read address, {address=}")
+        _logger.error(f"Could not read address, {address=}")
 
-    return segment_list
+    return segment_stack
```

### Comparing `pydfuutil-0.0.2b2/pydfuutil/lmdfu.py` & `pydfuutil-0.0.2b3/pydfuutil/lmdfu.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 as per the Application Update Using the USB Device Firmware Upgrade Class
 (Document AN012373)
 https://www.ti.com/general/docs/lit/getliterature.tsp?literatureNumber=spma003&fileType=pdf
 """
 
 from pydfuutil.dfu_file import DFUFile, parse_dfu_suffix, generate_dfu_suffix
-from pydfuutil.logger import get_logger
+from pydfuutil.logger import logger
 
 __all__ = ('dfu_prefix',
            'add_prefix',
            'remove_prefix',
            'check_prefix',
            'parse_dfu_suffix',
            'generate_dfu_suffix')
 
-logger = get_logger("lmdfu")
+_logger = logger.getChild(__name__.rsplit('.', maxsplit=1)[-1])
 
 # dfu_prefix payload length excludes prefix and suffix
 
 
 dfu_prefix = (
     0x01,  # STELLARIS_DFU_PROG
     0x00,  # Reserved
@@ -41,119 +41,119 @@
     :param file: DFUFile instance representing the file to be modified.
     :param address: Integer representing the starting address for the TI Stellaris DFU prefix.
     :return: 0 on success, -1 on error.
     """
 
     try:
         # Get file length
-        file.filep.seek(0, 2)
-        length = file.filep.tell()
-        file.filep.seek(0, 0)
+        file.file_p.seek(0, 2)
+        length = file.file_p.tell()
+        file.file_p.seek(0, 0)
 
         # Read file content
-        data = file.filep.read()
+        data = file.file_p.read()
 
         # Allocate buffer
         lmdfu_dfu_prefix_buf = bytearray([0] * 16)
 
         # Fill Stellaris dfu_prefix with correct data
         addr = address // 1024
         lmdfu_dfu_prefix_buf[2] = addr & 0xff
         lmdfu_dfu_prefix_buf[3] = (addr >> 8) & 0xff
         lmdfu_dfu_prefix_buf[4] = length & 0xff
         lmdfu_dfu_prefix_buf[5] = (length >> 8) & 0xff
         lmdfu_dfu_prefix_buf[6] = (length >> 16) & 0xff
         lmdfu_dfu_prefix_buf[7] = (length >> 24) & 0xff
 
         # Write TI Stellaris DFU prefix to the file
-        file.filep.seek(0)
-        file.filep.write(lmdfu_dfu_prefix_buf)
+        file.file_p.seek(0)
+        file.file_p.write(lmdfu_dfu_prefix_buf)
 
         # Write file content after the TI Stellaris DFU prefix
-        file.filep.write(data)
+        file.file_p.write(data)
 
-        logger.info("TI Stellaris DFU prefix added.")
+        _logger.info("TI Stellaris DFU prefix added.")
 
         return 0
     except Exception as e:
-        logger.error(f"Error: {e}")
+        _logger.error(f"Error: {e}")
         return -1
 
 
 def remove_prefix(file: DFUFile) -> int:
     """
     Remove TI Stellaris DFU prefix from a binary file.
 
     :param file: DFUFile instance representing the file to be modified.
     :return: 0 on success, -1 on error.
     """
 
     try:
-        logger.info("Remove TI Stellaris prefix")
+        _logger.info("Remove TI Stellaris prefix")
 
         # Get file length
-        file.filep.seek(0, 2)
-        length = file.filep.tell()
-        file.filep.seek(0, 0)
+        file.file_p.seek(0, 2)
+        length = file.file_p.tell()
+        file.file_p.seek(0, 0)
 
         # Read file content
-        data = file.filep.read()
+        data = file.file_p.read()
 
         # Check if the file has enough data to contain the prefix
         if length < 16:
-            logger.error("Error: File does not contain a valid prefix.")
+            _logger.error("Error: File does not contain a valid prefix.")
             return -1
 
         # Truncate the file
-        file.filep.truncate(0)
-        file.filep.seek(0)
+        file.file_p.truncate(0)
+        file.file_p.seek(0)
 
         # Write data without the TI Stellaris prefix
-        file.filep.write(data[16:])
+        file.file_p.write(data[16:])
 
-        logger.info("TI Stellaris prefix removed")
+        _logger.info("TI Stellaris prefix removed")
         return 0
 
     except Exception as e:
-        logger.error(f"Error: {e}")
+        _logger.error(f"Error: {e}")
         return -1
 
 
 def check_prefix(file: DFUFile) -> int:
     """
     Check if a binary file contains a valid TI Stellaris DFU prefix.
 
     :param file: DFUFile instance representing the file to be checked.
     :return: 0 if not a valid prefix, 1 if a valid prefix, -1 on error.
     """
 
     try:
-        logger.info("Check TI Stellaris prefix")
+        _logger.info("Check TI Stellaris prefix")
 
         # Allocate buffer for reading the prefix
         data = bytearray(16)
 
         # Read prefix from the file
-        ret = file.filep.readinto(data)
+        ret = file.file_p.readinto(data)
         if ret < 16:
-            logger.error("Error: Could not read prefix")
+            _logger.error("Error: Could not read prefix")
             return -1
 
         # Check if it's a valid TI Stellaris DFU prefix
         if data[0] != 0x01 or data[1] != 0x00:
-            logger.info("Not a valid TI Stellaris DFU prefix")
+            _logger.info("Not a valid TI Stellaris DFU prefix")
             ret = 0
         else:
-            logger.info("Possible TI Stellaris DFU prefix with the following properties:")
+            _logger.info("Possible TI Stellaris DFU prefix with the following properties:")
             address = 1024 * (data[3] << 8 | data[2])
             payload_length = data[4] | data[5] << 8 | data[6] << 16 | data[7] << 24
-            logger.info(f"Address:        0x{address:08X}")
-            logger.info(f"Payload length: {payload_length}")
+            _logger.info(f"Address:        0x{address:08X}")
+            _logger.info(f"Payload length: {payload_length}")
 
         # Rewind the file
-        file.filep.seek(0)
+        file.file_p.seek(0)
 
         return ret
 
     except Exception as e:
-        logger.error(f"Error: {e}")
+        _logger.error(f"Error: {e}")
         return -1
```

### Comparing `pydfuutil-0.0.2b2/pydfuutil/quirks.py` & `pydfuutil-0.0.2b3/pydfuutil/quirks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Simple quirk system for dfu-util
 (C) 2023 Yaroshenko Dmytro (https://github.com/o-murphy)
 """
 
-VENDOR_OPENMOKO = 0x1d50  # Openmoko Freerunner / GTA02
-VENDOR_FIC = 0x1457  # Openmoko Freerunner / GTA02
+VENDOR_OPENMOKO = 0x1d50  # Openmoko Free-runner / GTA02
+VENDOR_FIC = 0x1457  # Openmoko Free-runner / GTA02
 VENDOR_VOTI = 0x16c0  # OpenPCD Reader
 VENDOR_LEAFLABS = 0x1eaf  # Maple
 PRODUCT_MAPLE3 = 0x0003  # rev 3 and 5
 
 QUIRK_POLLTIMEOUT = 1 << 0
 QUIRK_FORCE_DFU11 = 1 << 1
```

### Comparing `pydfuutil-0.0.2b2/pydfuutil/suffix.py` & `pydfuutil-0.0.2b3/pydfuutil/suffix.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,27 @@
 (C) 2023 Yaroshenko Dmytro (https://github.com/o-murphy)
 """
 
 import argparse
 import os
 import sys
 from enum import IntEnum
+import importlib.metadata
 
-from pydfuutil import __version__, __copyright__
+from pydfuutil import __copyright__
 from pydfuutil import lmdfu
 from pydfuutil.dfu_file import DFUFile, parse_dfu_suffix
-from pydfuutil.logger import get_logger
+from pydfuutil.logger import logger
 
-logger = get_logger("dfu-suffix")
+try:
+    __version__ = importlib.metadata.version("pydfuutil")
+except importlib.metadata.PackageNotFoundError:
+    __version__ = 'UNKNOWN'
+
+_logger = logger.getChild(__name__.rsplit('.', maxsplit=1)[-1])
 
 
 class Mode(IntEnum):
     """DFU suffix operate mode"""
     NONE = 0x1
     ADD = 0x2
     DEL = 0x3
@@ -61,15 +67,15 @@
     ret = parse_dfu_suffix(file)
     if ret > 0:
         print(f"The file {file.name} contains a DFU suffix with the following properties:")
         print(f"BCD device:\t0x{file.bcdDevice:04X}")
         print(f"Product ID:\t0x{file.idProduct:04X}")
         print(f"Vendor ID:\t0x{file.idVendor:04X}")
         print(f"BCD DFU:\t0x{file.bcdDFU:04X}")
-        print(f"Length:\t\t{file.suffixlen}")
+        print(f"Length:\t\t{file.suffix_len}")
         print(f"CRC:\t\t0x{file.dwCRC:08X}")
     return ret
 
 
 def remove_suffix(file: DFUFile) -> int:
     """remove suffix from DFU file"""
     ret: int
@@ -77,21 +83,21 @@
     ret = parse_dfu_suffix(file)
     if ret <= 0:
         return 0
 
     if hasattr(os, 'ftruncate'):
         try:
             with open(file.name, 'r+', encoding='utf-8') as f:
-                f.truncate(file.size - file.suffixlen)
-            logger.info("DFU suffix removed")
+                f.truncate(file.size - file.suffix_len)
+            _logger.info("DFU suffix removed")
         except OSError as e:
-            logger.error(f"Error truncating file: {e}")
+            _logger.error(f"Error truncating file: {e}")
             sys.exit(1)
     else:
-        logger.error("Suffix removal not implemented on this platform")
+        _logger.error("Suffix removal not implemented on this platform")
     return 1
 
 
 def add_suffix(file: DFUFile, pid: int, vid: int, did: int) -> None:
     """Add suffix to DFU file"""
     ret: int
 
@@ -100,20 +106,20 @@
     file.bcdDevice = did
 
     ret = lmdfu.generate_dfu_suffix(file)
     if ret < 0:
         try:
             raise OSError("generate")
         except OSError as e:
-            logger.error(e)
+            _logger.error(e)
             sys.exit(1)
-    logger.info("New DFU suffix added.")
+    _logger.info("New DFU suffix added.")
 
 
-def _get_argparser():
+def _get_arg_parser():
     """Get custom argument parser"""
 
     class CustomHelpFormatter(argparse.HelpFormatter):
         """Custom argument parser formatter"""
 
         def add_argument(self, action):
             if action.dest == 'help':
@@ -132,72 +138,73 @@
 
     parser.add_argument('-V', '--version', action='version',
                         version=f'{parser.prog} " v{__version__} "',
                         help='Print the version number')
 
     group = parser.add_mutually_exclusive_group(required=True)
 
-    group.add_argument('-c', '--check', metavar="<file>",
+    group.add_argument('-c', '--check',
                        const=Mode.CHECK, dest='mode', action='store_const',
                        help='Check DFU suffix of <file>')
-    group.add_argument('-a', '--add', metavar="<file>",
+    group.add_argument('-a', '--add',
                        const=Mode.ADD, dest='mode', action='store_const',
                        help='Add DFU suffix to <file>')
-    group.add_argument('-D', '--delete', metavar="<file>",
+    group.add_argument('-D', '--delete',
                        const=Mode.DEL, dest='mode', action='store_const',
                        help='Delete DFU suffix from <file>')
 
     parser.add_argument('file', action='store', metavar='<file>',
-                        type=argparse.FileType('r+b'),
+                        type=argparse.FileType('r+b'), default=None,
                         help="Target filename")
 
     parser.add_argument('-p', '--pid', action='store', metavar="<productID>",
                         required=False,
                         type=lambda x: int(x, 16), help='Add product ID into DFU suffix in <file>')
     parser.add_argument('-v', '--vid', action='store', metavar="<vendorID>",
                         required=False,
                         type=lambda x: int(x, 16), help='Add vendor ID into DFU suffix in <file>')
     parser.add_argument('-d', '--did', action='store', metavar="<deviceID>",
                         required=False,
                         type=lambda x: int(x, 16), help='Add device ID into DFU suffix in <file>')
-    # parser.add_argument('-S', '--spec', action='store', metavar="<specID>",
-    # required=False, help='Add DFU specification ID into DFU suffix in <file>')
     parser.add_argument('-s', '--stellaris-address', dest='lmdfu_flash_address',
                         metavar="<address>", type=int, help='Specify lmdfu address for LMDFU_ADD')
     parser.add_argument('-T', '--stellaris', dest='lmdfu_mode', action='store_const',
                         const=LmdfuMode.CHECK, help='Set lmdfu mode to LMDFU_CHECK')
 
     return parser
 
 
-def get_args(parser):
+def get_args(parser, argv):
     """parse command line arguments"""
     print_version()
     try:
-        args = parser.parse_args()
-    except Exception as err:
+        args = parser.parse_args(argv)
+    except argparse.ArgumentError as err:
         parser.print_help()
-        logger.error(err)
+        _logger.error(err)
         sys.exit(1)
     return args
 
 
-def main() -> None:
+def main(argv) -> None:
     """main executable"""
-    parser = _get_argparser()
-    args = get_args(parser)
+    if argv[0] == __file__:
+        argv.pop(0)
+
+    parser = _get_arg_parser()
+    args = get_args(parser, argv)
 
     lmdfu_mode = LmdfuMode.NONE
     lmdfu_flash_address: int = 0
     lmdfu_prefix: int = 0
 
     empty = 0xffff
 
     file = DFUFile(args.file.name)
-    file.filep, mode = args.file, args.mode
+    file.file_p, mode = args.file, args.mode
 
     pid = args.pid if args.pid else empty
     vid = args.vid if args.vid else empty
     did = args.did if args.did else empty
 
     if args.lmdfu_flash_address:
         lmdfu_mode, lmdfu_flash_address = LmdfuMode.ADD, args.lmdfu_flash_address
@@ -211,26 +218,26 @@
     if mode != Mode.NONE:
         try:
             if mode == Mode.ADD:
 
                 if check_suffix(file):
                     if lmdfu_prefix:
                         lmdfu.check_prefix(file)
-                    logger.warning("Please remove existing DFU suffix before adding a new one.")
+                    _logger.warning("Please remove existing DFU suffix before adding a new one.")
                     sys.exit(1)
 
                 if lmdfu_mode == LmdfuMode.ADD:
                     if lmdfu.check_prefix(file):
-                        logger.info("Adding new anyway")
+                        _logger.info("Adding new anyway")
                     lmdfu.add_prefix(file, lmdfu_flash_address)
 
                 add_suffix(file, pid, vid, did)
 
             elif mode == Mode.CHECK:
-                # FIXME: could open read-only here
+                # Note: could open read-only here
                 check_suffix(file)
                 if lmdfu_mode == LmdfuMode.CHECK:
                     lmdfu.check_prefix(file)
 
             elif mode == Mode.DEL:
                 if (not remove_suffix(file)
                         and lmdfu_mode == LmdfuMode.DEL
@@ -239,24 +246,24 @@
                     sys.exit(1)
 
             else:
                 parser.print_help()
                 sys.exit(2)
 
             if lmdfu_mode == LmdfuMode.DEL and check_suffix(file):
-                logger.warning(
+                _logger.warning(
                     "DFU suffix exist. "
                     "Remove suffix before using -T or use it with -D to delete suffix")
                 sys.exit(1)
 
             if lmdfu_mode == LmdfuMode.DEL and lmdfu.check_prefix(file):
                 lmdfu.remove_prefix(file)
 
         except Exception as error:
-            logger.error(error)
+            _logger.error(error)
             sys.exit(1)
 
     sys.exit(0)
 
 
 if __name__ == '__main__':
-    main()
+    main(sys.argv)
```

### Comparing `pydfuutil-0.0.2b2/pydfuutil/usb_dfu.py` & `pydfuutil-0.0.2b3/pydfuutil/usb_dfu.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,43 +2,44 @@
 USB Device Firmware Update Implementation for OpenPCD
 Protocol definitions for USB DFU
 (C) 2023 Yaroshenko Dmytro (https://github.com/o-murphy)
 
 This ought to be compliant to the USB DFU Spec 1.0 as available from
 https://www.usb.org/developers/devclass_docs/usbdfu10.pdf
 """
-
+from dataclasses import dataclass
 from enum import IntEnum
 
 import usb.util
-from construct import Int8ul, Struct, Int16ul
 
 
 USB_DT_DFU = 0x21
+USB_DT_DFU_SIZE = 9
+USB_TYPE_DFU = usb.util.CTRL_TYPE_CLASS | usb.util.CTRL_RECIPIENT_INTERFACE
+
 
-class bmAttributes(IntEnum):
-    """Enum of DFU_FUNC_DESCRIPTOR's bmAttributes"""
+class BmAttributes(IntEnum):
+    """Enum of DFU_FUNC_DESCRIPTOR's BmAttributes"""
     USB_DFU_CAN_DOWNLOAD = 0x1
     USB_DFU_CAN_UPLOAD = 0x2
     USB_DFU_MANIFEST_TOL = 0x3
     USB_DFU_WILL_DETACH = 0x4
 
 
-USB_DFU_FUNC_DESCRIPTOR = Struct(
-    bLength=Int8ul,
-    bDescriptorType=Int8ul,
-    bmAttributes=Int8ul,
-    wDetachTimeOut=Int16ul,
-    wTransferSize=Int16ul,
-    bcdDFUVersion=Int16ul,
-)
+# pylint: disable=invalid-name
+@dataclass
+class FuncDescriptor:
+    """USB_DFU_FUNC_DESCRIPTOR's'"""
+    bLength: int = 0
+    bDescriptorType: int = 0
+    bmAttributes: BmAttributes = 0
+    wDetachTimeOut: int = 0
+    wTransferSize: int = 0
+    bcdDFUVersion: int = 0
 
-USB_DT_DFU_SIZE = 9
-
-USB_TYPE_DFU = usb.util.CTRL_TYPE_CLASS | usb.util.CTRL_RECIPIENT_INTERFACE
 
 
 # DFU class-specific requests (Section 3, DFU Rev 1.1)
 class UsbReqDfu(IntEnum):
     """Dfu requests"""
     DETACH = 0x00
     DNLOAD = 0x01
```

### Comparing `pydfuutil-0.0.2b2/pydfuutil.egg-info/PKG-INFO` & `pydfuutil-0.0.2b3/pydfuutil.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydfuutil
-Version: 0.0.2b2
+Version: 0.0.2b3
 Summary: PyDfuUtil - Pure python fork of dfu-util wrappers to libusb
 Author-email: o-murphy <thehelixpg@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -185,18 +185,19 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyusb
 Requires-Dist: libusb-package
-Requires-Dist: rich
 Requires-Dist: construct
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
+Provides-Extra: rich
+Requires-Dist: rich; extra == "rich"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pylint; extra == "test"
 
 # PyDfuUtil - Pure python fork of **[dfu-util](https://github.com/Stefan-Schmidt/dfu-util)** wrappers to **[libusb](https://github.com/libusb/libusb)**
 
 [![PyPI Version](https://img.shields.io/pypi/v/pydfuutil?label=PyPI&logo=pypi)](https://pypi.org/project/pydfuutil/)
```

### Comparing `pydfuutil-0.0.2b2/pyproject.toml` & `pydfuutil-0.0.2b3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pydfuutil"
-
+version = "0.0.2b3"
 authors = [
     { name="o-murphy", email="thehelixpg@gmail.com" },
 ]
 description = "PyDfuUtil - Pure python fork of dfu-util wrappers to libusb"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["dfu_util", "dfu-util", "pydfu", "libusb", "python", "python3"]
@@ -26,41 +26,42 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
-dependencies = ['pyusb', 'libusb-package', 'rich', 'construct']
+dependencies = ['pyusb', 'libusb-package', 'construct']
 
-dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/o-murphy/pydfuutil"
 "Bug Reports" = "https://github.com/o-murphy/pydfuutil/issues"
 "Source" = "https://github.com/o-murphy/pydfuutil"
 
 
 [tool.setuptools]
 py-modules = ["pydfuutil"]
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["pydfuutil*"]
-#exclude = ["*"]
 
 
 [tool.setuptools.dynamic]
 version = {attr = "pydfuutil.__version__"}
 
 
 [project.optional-dependencies]
 build = [
     "build"
 ]
+rich = [
+    "rich"
+]
 test = [
     "pytest",
     "pylint",
 ]
 
 [project.scripts]
 pydfuutil = "pydfuutil.__main__:main"
```

### Comparing `pydfuutil-0.0.2b2/tests/test_dfu.py` & `pydfuutil-0.0.2b3/tests/test_dfu.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.2b2/tests/test_dfu_file.py` & `pydfuutil-0.0.2b3/tests/test_dfu_file.py`

 * *Files identical despite different names*

### Comparing `pydfuutil-0.0.2b2/tests/test_dfu_load.py` & `pydfuutil-0.0.2b3/tests/test_dfu_load.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 import unittest
 from unittest.mock import Mock, patch
 
-from pydfuutil.dfu_load import *
+from pydfuutil import dfu
+from pydfuutil.dfu_load import DFUFile, do_upload, do_dnload
 
 
 class TestDFULoader(unittest.TestCase):
 
     def test_dfu_load_do_upload(self):
         xfer_size = 256
-        file = DFUFile(name='test_file', filep=Mock())  # Provide a mock file object
-        total_size = 1024
+        file = DFUFile(name='test_file', file_p=Mock())  # Provide a mock file object
+        total_size = 4096
 
         dif = Mock()
         dif.upload.return_value = bytes(xfer_size)
         dif.get_status.return_value = total_size
 
-        # Mock filep.write to return the length of the data written
-        with patch.object(file.filep, 'write', return_value=xfer_size) as mock_write:
+        # Mock file_p.write to return the length of the data written
+        with patch.object(file.file_p, 'write', return_value=xfer_size) as mock_write:
             result = do_upload(dif, xfer_size, file, total_size)
 
         # Assertions
         self.assertEqual(result, total_size)  # Assuming total_size bytes are received
 
     def test_dfu_load_do_dnload(self):
 
         xfer_size = 1024
-        result = dfu.StatusData(dfu.Status.OK, 100, dfu.State.DFU_DOWNLOAD_IDLE, 0)
+        result = dfu.StatusRetVal(dfu.Status.OK, 100, dfu.State.DFU_DOWNLOAD_IDLE, 0)
 
         dif = Mock()
         dif.download.return_value = xfer_size
         dif.get_status.return_value = result
 
-        file = DFUFile(name='test_file', filep=Mock(), size=xfer_size, suffixlen=0)
+        file = DFUFile(name='test_file', file_p=Mock(), size=xfer_size, suffix_len=0)
         quirks = 0
-        verbose = True
+        verbose = False
 
-        # Mock filep.readinto to return the length of the data read
-        with patch.object(file.filep, 'readinto', return_value=xfer_size) as mock_readinto:
+        # Mock file_p.readinto to return the length of the data read
+        with patch.object(file.file_p, 'readinto', return_value=xfer_size) as mock_readinto:
             result = do_dnload(dif, xfer_size, file, quirks, verbose)
 
         # Assertions
         self.assertEqual(result, xfer_size)  # Assuming xfer_size bytes are sent
 
 
 if __name__ == '__main__':
```

### Comparing `pydfuutil-0.0.2b2/tests/test_dfuse_mem.py` & `pydfuutil-0.0.2b3/tests/test_dfuse_mem.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from pydfuutil.dfuse_mem import MemSegment, add_segment, find_segment, parse_memory_layout
+from pydfuutil.dfuse_mem import MemSegment, add_segment, parse_memory_layout
 
 
 class TestDfuSeMem(unittest.TestCase):
 
     def test_parse_build(self):
         mem_seq = MemSegment.from_bytes(bytes(12))
         buf = bytes(mem_seq)
@@ -64,34 +64,34 @@
         self.assertNotEqual(seqment_sequence.next.next, None)
         self.assertEqual(seqment_sequence.next.end, 30)
         self.assertEqual(seqment_sequence.next.next.end, 20)
 
     def test_parse_memory_layout(self):
         with self.subTest("Test case 1: Valid input"):
             intf_desc = "@Internal Flash/0x08000000/04*016Kg,01*064Kg,01*128Kg"
-            result = parse_memory_layout(intf_desc, True)
+            result = parse_memory_layout(intf_desc)
             self.assertIsNotNone(result)
             self.assertIsInstance(result, MemSegment)
             self.assertEqual(len(result), 3)
 
         with self.subTest("Test case 2: Empty input"):
             result = parse_memory_layout("")
             self.assertIsNone(result)
 
         with self.subTest("Test case 3: Invalid input with missing name"):
             intf_desc = "/0x1000/1*1024B/04*016Kg"
-            result = parse_memory_layout(intf_desc, True)
+            result = parse_memory_layout(intf_desc)
             self.assertIsNone(result)
 
         with self.subTest("Test case 4: Invalid input with missing address"):
             intf_desc = "@Internal Flash/1*1024B/"
-            result = parse_memory_layout(intf_desc, True)
+            result = parse_memory_layout(intf_desc)
             self.assertIsNone(result)
 
         with self.subTest("Test case 5: Invalid input with missing segment details"):
             intf_desc = "@Internal Flash/0x08000000/"
-            result = parse_memory_layout(intf_desc, True)
+            result = parse_memory_layout(intf_desc)
             self.assertIsNone(result)  # Should return None, as it's invalid
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pydfuutil-0.0.2b2/tests/test_quirks.py` & `pydfuutil-0.0.2b3/tests/test_quirks.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,14 @@
+import logging
 import unittest
 from pydfuutil.quirks import *
+from pydfuutil.logger import logger
+
+logger.setLevel(logging.DEBUG)
+
 
 class TestSetQuirks(unittest.TestCase):
 
     def test_quirk_polltimeout(self):
         self.assertEqual(set_quirks(VENDOR_OPENMOKO, 123, 1), QUIRK_POLLTIMEOUT)
         self.assertEqual(set_quirks(VENDOR_FIC, 456, 1), QUIRK_POLLTIMEOUT)
         self.assertEqual(set_quirks(VENDOR_VOTI, 789, 1), QUIRK_POLLTIMEOUT)
```


# Comparing `tmp/tcconfig-0.8.0.tar.gz` & `tmp/tcconfig-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tcconfig-0.8.0.tar", last modified: Sat Mar 18 09:12:16 2017, max compression
+gzip compressed data, was "dist/tcconfig-0.9.0.tar", last modified: Sat Mar 25 16:18:52 2017, max compression
```

## Comparing `tcconfig-0.8.0.tar` & `tcconfig-0.9.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-03-18 09:12:16.000000 tcconfig-0.8.0/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-03-18 09:12:16.000000 tcconfig-0.8.0/docs/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-03-18 09:12:16.000000 tcconfig-0.8.0/docs/pages/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-03-18 09:12:16.000000 tcconfig-0.8.0/docs/pages/introduction/
--rw-r--r--   0 travis    (1000) travis    (1000)      130 2017-03-18 09:11:47.000000 tcconfig-0.8.0/docs/pages/introduction/summary.txt
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-03-18 09:12:16.000000 tcconfig-0.8.0/requirements/
--rw-r--r--   0 travis    (1000) travis    (1000)       51 2017-03-18 09:11:47.000000 tcconfig-0.8.0/requirements/docs_requirements.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       99 2017-03-18 09:11:47.000000 tcconfig-0.8.0/requirements/requirements.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       41 2017-03-18 09:11:47.000000 tcconfig-0.8.0/requirements/test_requirements.txt
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-03-18 09:12:16.000000 tcconfig-0.8.0/tcconfig/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-03-18 09:12:16.000000 tcconfig-0.8.0/tcconfig/shaper/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-03-18 09:11:47.000000 tcconfig-0.8.0/tcconfig/shaper/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     5404 2017-03-18 09:11:47.000000 tcconfig-0.8.0/tcconfig/shaper/_interface.py
--rw-r--r--   0 travis    (1000) travis    (1000)     7868 2017-03-18 09:11:47.000000 tcconfig-0.8.0/tcconfig/shaper/htb.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4317 2017-03-18 09:11:47.000000 tcconfig-0.8.0/tcconfig/shaper/tbf.py
--rw-r--r--   0 travis    (1000) travis    (1000)      112 2017-03-18 09:11:47.000000 tcconfig-0.8.0/tcconfig/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1984 2017-03-18 09:11:47.000000 tcconfig-0.8.0/tcconfig/_argparse_wrapper.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3023 2017-03-18 09:11:47.000000 tcconfig-0.8.0/tcconfig/_common.py
--rw-r--r--   0 travis    (1000) travis    (1000)      726 2017-03-18 09:11:47.000000 tcconfig-0.8.0/tcconfig/_const.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2052 2017-03-18 09:11:47.000000 tcconfig-0.8.0/tcconfig/_converter.py
--rw-r--r--   0 travis    (1000) travis    (1000)      643 2017-03-18 09:11:47.000000 tcconfig-0.8.0/tcconfig/_error.py
--rw-r--r--   0 travis    (1000) travis    (1000)     5883 2017-03-18 09:11:47.000000 tcconfig-0.8.0/tcconfig/_iptables.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1028 2017-03-18 09:11:47.000000 tcconfig-0.8.0/tcconfig/_logger.py
--rw-r--r--   0 travis    (1000) travis    (1000)      903 2017-03-18 09:11:47.000000 tcconfig-0.8.0/tcconfig/_split_line_list.py
--rw-r--r--   0 travis    (1000) travis    (1000)      281 2017-03-18 09:11:47.000000 tcconfig-0.8.0/tcconfig/_traffic_direction.py
--rw-r--r--   0 travis    (1000) travis    (1000)     9032 2017-03-18 09:11:47.000000 tcconfig-0.8.0/tcconfig/parser.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2327 2017-03-18 09:11:47.000000 tcconfig-0.8.0/tcconfig/tcdel.py
--rw-r--r--   0 travis    (1000) travis    (1000)    10134 2017-03-18 09:11:47.000000 tcconfig-0.8.0/tcconfig/tcset.py
--rw-r--r--   0 travis    (1000) travis    (1000)     7250 2017-03-18 09:11:47.000000 tcconfig-0.8.0/tcconfig/tcshow.py
--rw-r--r--   0 travis    (1000) travis    (1000)    11885 2017-03-18 09:11:47.000000 tcconfig-0.8.0/tcconfig/traffic_control.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-03-18 09:12:16.000000 tcconfig-0.8.0/tcconfig.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)     8876 2017-03-18 09:12:16.000000 tcconfig-0.8.0/tcconfig.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)     1138 2017-03-18 09:12:16.000000 tcconfig-0.8.0/tcconfig.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-03-18 09:12:16.000000 tcconfig-0.8.0/tcconfig.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)      105 2017-03-18 09:12:16.000000 tcconfig-0.8.0/tcconfig.egg-info/entry_points.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       99 2017-03-18 09:12:16.000000 tcconfig-0.8.0/tcconfig.egg-info/requires.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        9 2017-03-18 09:12:16.000000 tcconfig-0.8.0/tcconfig.egg-info/top_level.txt
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-03-18 09:12:16.000000 tcconfig-0.8.0/test/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-03-18 09:11:47.000000 tcconfig-0.8.0/test/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)      561 2017-03-18 09:11:47.000000 tcconfig-0.8.0/test/common.py
--rw-r--r--   0 travis    (1000) travis    (1000)      194 2017-03-18 09:11:47.000000 tcconfig-0.8.0/test/conftest.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1025 2017-03-18 09:11:47.000000 tcconfig-0.8.0/test/test_common.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3147 2017-03-18 09:11:47.000000 tcconfig-0.8.0/test/test_converter.py
--rw-r--r--   0 travis    (1000) travis    (1000)     7822 2017-03-18 09:11:47.000000 tcconfig-0.8.0/test/test_iptables.py
--rw-r--r--   0 travis    (1000) travis    (1000)     5328 2017-03-18 09:11:47.000000 tcconfig-0.8.0/test/test_parser.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3247 2017-03-18 09:11:47.000000 tcconfig-0.8.0/test/test_split_line_list.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3572 2017-03-18 09:11:47.000000 tcconfig-0.8.0/test/test_tcconfig.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1749 2017-03-18 09:11:47.000000 tcconfig-0.8.0/test/test_tcset_config_file.py
--rw-r--r--   0 travis    (1000) travis    (1000)     5197 2017-03-18 09:11:47.000000 tcconfig-0.8.0/test/test_tcset_one.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2677 2017-03-18 09:11:47.000000 tcconfig-0.8.0/test/test_tcset_two.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3066 2017-03-18 09:11:47.000000 tcconfig-0.8.0/test/test_tcshow.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4920 2017-03-18 09:11:47.000000 tcconfig-0.8.0/test/test_traffic_control.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1084 2017-03-18 09:11:47.000000 tcconfig-0.8.0/LICENSE
--rw-r--r--   0 travis    (1000) travis    (1000)      223 2017-03-18 09:11:47.000000 tcconfig-0.8.0/MANIFEST.in
--rw-r--r--   0 travis    (1000) travis    (1000)     5831 2017-03-18 09:11:47.000000 tcconfig-0.8.0/README.rst
--rw-r--r--   0 travis    (1000) travis    (1000)     2461 2017-03-18 09:11:47.000000 tcconfig-0.8.0/setup.py
--rw-r--r--   0 travis    (1000) travis    (1000)      136 2017-03-18 09:11:47.000000 tcconfig-0.8.0/tox.ini
--rw-r--r--   0 travis    (1000) travis    (1000)     8876 2017-03-18 09:12:16.000000 tcconfig-0.8.0/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)      107 2017-03-18 09:12:16.000000 tcconfig-0.8.0/setup.cfg
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-03-25 16:18:52.000000 tcconfig-0.9.0/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-03-25 16:18:52.000000 tcconfig-0.9.0/docs/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-03-25 16:18:52.000000 tcconfig-0.9.0/docs/pages/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-03-25 16:18:52.000000 tcconfig-0.9.0/docs/pages/introduction/
+-rw-r--r--   0 travis    (1000) travis    (1000)      130 2017-03-25 16:18:22.000000 tcconfig-0.9.0/docs/pages/introduction/summary.txt
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-03-25 16:18:52.000000 tcconfig-0.9.0/requirements/
+-rw-r--r--   0 travis    (1000) travis    (1000)       51 2017-03-25 16:18:22.000000 tcconfig-0.9.0/requirements/docs_requirements.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       96 2017-03-25 16:18:22.000000 tcconfig-0.9.0/requirements/requirements.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       41 2017-03-25 16:18:22.000000 tcconfig-0.9.0/requirements/test_requirements.txt
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-03-25 16:18:52.000000 tcconfig-0.9.0/tcconfig/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-03-25 16:18:52.000000 tcconfig-0.9.0/tcconfig/shaper/
+-rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-03-25 16:18:22.000000 tcconfig-0.9.0/tcconfig/shaper/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     5591 2017-03-25 16:18:22.000000 tcconfig-0.9.0/tcconfig/shaper/_interface.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     7977 2017-03-25 16:18:22.000000 tcconfig-0.9.0/tcconfig/shaper/htb.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4407 2017-03-25 16:18:22.000000 tcconfig-0.9.0/tcconfig/shaper/tbf.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      112 2017-03-25 16:18:22.000000 tcconfig-0.9.0/tcconfig/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1984 2017-03-25 16:18:22.000000 tcconfig-0.9.0/tcconfig/_argparse_wrapper.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3824 2017-03-25 16:18:22.000000 tcconfig-0.9.0/tcconfig/_common.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      827 2017-03-25 16:18:22.000000 tcconfig-0.9.0/tcconfig/_const.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2052 2017-03-25 16:18:22.000000 tcconfig-0.9.0/tcconfig/_converter.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      643 2017-03-25 16:18:22.000000 tcconfig-0.9.0/tcconfig/_error.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     6113 2017-03-25 16:18:22.000000 tcconfig-0.9.0/tcconfig/_iptables.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1028 2017-03-25 16:18:22.000000 tcconfig-0.9.0/tcconfig/_logger.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      903 2017-03-25 16:18:22.000000 tcconfig-0.9.0/tcconfig/_split_line_list.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      281 2017-03-25 16:18:22.000000 tcconfig-0.9.0/tcconfig/_traffic_direction.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    12599 2017-03-25 16:18:22.000000 tcconfig-0.9.0/tcconfig/parser.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2335 2017-03-25 16:18:22.000000 tcconfig-0.9.0/tcconfig/tcdel.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    10399 2017-03-25 16:18:22.000000 tcconfig-0.9.0/tcconfig/tcset.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     7993 2017-03-25 16:18:22.000000 tcconfig-0.9.0/tcconfig/tcshow.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    12537 2017-03-25 16:18:22.000000 tcconfig-0.9.0/tcconfig/traffic_control.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-03-25 16:18:52.000000 tcconfig-0.9.0/tcconfig.egg-info/
+-rw-r--r--   0 travis    (1000) travis    (1000)     8876 2017-03-25 16:18:51.000000 tcconfig-0.9.0/tcconfig.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)     1138 2017-03-25 16:18:52.000000 tcconfig-0.9.0/tcconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-03-25 16:18:51.000000 tcconfig-0.9.0/tcconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)      105 2017-03-25 16:18:51.000000 tcconfig-0.9.0/tcconfig.egg-info/entry_points.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)      106 2017-03-25 16:18:51.000000 tcconfig-0.9.0/tcconfig.egg-info/requires.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        9 2017-03-25 16:18:51.000000 tcconfig-0.9.0/tcconfig.egg-info/top_level.txt
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-03-25 16:18:52.000000 tcconfig-0.9.0/test/
+-rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-03-25 16:18:22.000000 tcconfig-0.9.0/test/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      561 2017-03-25 16:18:22.000000 tcconfig-0.9.0/test/common.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      194 2017-03-25 16:18:22.000000 tcconfig-0.9.0/test/conftest.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2593 2017-03-25 16:18:22.000000 tcconfig-0.9.0/test/test_common.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3147 2017-03-25 16:18:22.000000 tcconfig-0.9.0/test/test_converter.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     7599 2017-03-25 16:18:22.000000 tcconfig-0.9.0/test/test_iptables.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     8672 2017-03-25 16:18:22.000000 tcconfig-0.9.0/test/test_parser.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3247 2017-03-25 16:18:22.000000 tcconfig-0.9.0/test/test_split_line_list.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3572 2017-03-25 16:18:22.000000 tcconfig-0.9.0/test/test_tcconfig.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1788 2017-03-25 16:18:22.000000 tcconfig-0.9.0/test/test_tcset_config_file.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     5197 2017-03-25 16:18:22.000000 tcconfig-0.9.0/test/test_tcset_one.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2677 2017-03-25 16:18:22.000000 tcconfig-0.9.0/test/test_tcset_two.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     5757 2017-03-25 16:18:22.000000 tcconfig-0.9.0/test/test_tcshow.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     5854 2017-03-25 16:18:22.000000 tcconfig-0.9.0/test/test_traffic_control.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1084 2017-03-25 16:18:22.000000 tcconfig-0.9.0/LICENSE
+-rw-r--r--   0 travis    (1000) travis    (1000)      223 2017-03-25 16:18:22.000000 tcconfig-0.9.0/MANIFEST.in
+-rw-r--r--   0 travis    (1000) travis    (1000)     5831 2017-03-25 16:18:22.000000 tcconfig-0.9.0/README.rst
+-rw-r--r--   0 travis    (1000) travis    (1000)     2564 2017-03-25 16:18:22.000000 tcconfig-0.9.0/setup.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      139 2017-03-25 16:18:22.000000 tcconfig-0.9.0/tox.ini
+-rw-r--r--   0 travis    (1000) travis    (1000)     8876 2017-03-25 16:18:52.000000 tcconfig-0.9.0/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)      107 2017-03-25 16:18:52.000000 tcconfig-0.9.0/setup.cfg
```

### Comparing `tcconfig-0.8.0/tcconfig/shaper/_interface.py` & `tcconfig-0.9.0/tcconfig/shaper/_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,20 +9,19 @@
 
 import abc
 
 import six
 import subprocrunner
 import typepy
 
-from .._common import run_command_helper
-from .._const import ANYWHERE_NETWORK
-from .._iptables import (
-    IptablesMangleController,
-    IptablesMangleMark
+from .._common import (
+    get_anywhere_network,
+    run_command_helper,
 )
+from .._iptables import IptablesMangleMark
 from .._traffic_direction import TrafficDirection
 
 
 @six.add_metaclass(abc.ABCMeta)
 class ShaperInterface(object):
 
     @abc.abstractproperty
@@ -104,37 +103,40 @@
                 "(dev={:s}, parent={:s}, handle={:s})".format(
                     self._tc_obj.get_tc_device(), parent, handle)))
 
     def add_filter(self):
         command_item_list = [
             "tc filter add",
             self.dev,
-            "protocol ip",
+            "protocol {:s}".format(self._tc_obj.protocol),
             "parent {:s}:".format(self._tc_obj.qdisc_major_id_str),
             "prio 1",
         ]
 
         if self._is_use_iptables():
             command_item_list.append(
                 "handle {:d} fw".format(self._get_unique_mangle_mark_id()))
         else:
             if typepy.is_null_string(self._tc_obj.network):
-                network = ANYWHERE_NETWORK
+                network = get_anywhere_network(self._tc_obj.ip_version)
             else:
                 network = self._tc_obj.network
 
             command_item_list.extend([
                 "u32",
-                "match ip {:s} {:s}".format(
-                    self._get_network_direction_str(), network),
+                "match {:s} {:s} {:s}".format(
+                    self._tc_obj.protocol_match,
+                    self._get_network_direction_str(),
+                    network),
             ])
 
             if self._tc_obj.port is not None:
                 command_item_list.append(
-                    "match ip dport {:d} 0xffff".format(self._tc_obj.port))
+                    "match {:s} dport {:d} 0xffff".format(
+                        self._tc_obj.protocol_match, self._tc_obj.port))
 
         command_item_list.append("flowid {:s}:{:d}".format(
             self._tc_obj.qdisc_major_id_str,
             self.get_qdisc_minor_id()))
 
         return subprocrunner.SubprocessRunner(
             " ".join(command_item_list)).run()
@@ -151,15 +153,15 @@
 
         if self._tc_obj.direction == TrafficDirection.INCOMING:
             return "src"
 
         raise ValueError("unknown direction: {}".format(self.direction))
 
     def _get_unique_mangle_mark_id(self):
-        mark_id = IptablesMangleController.get_unique_mark_id()
+        mark_id = self._tc_obj.iptables_ctrl.get_unique_mark_id()
 
         self.__add_mangle_mark(mark_id)
 
         return mark_id
 
     def __add_mangle_mark(self, mark_id):
         dst_network = None
@@ -172,10 +174,10 @@
             else:
                 src_network = self._tc_obj.src_network
                 chain = "PREROUTING"
         elif self._tc_obj.direction == TrafficDirection.INCOMING:
             src_network = self._tc_obj.network
             chain = "INPUT"
 
-        IptablesMangleController.add(IptablesMangleMark(
-            mark_id=mark_id, source=src_network, destination=dst_network,
-            chain=chain))
+        self._tc_obj.iptables_ctrl.add(IptablesMangleMark(
+            ip_version=self._tc_obj.ip_version, mark_id=mark_id,
+            source=src_network, destination=dst_network, chain=chain))
```

### Comparing `tcconfig-0.8.0/tcconfig/shaper/htb.py` & `tcconfig-0.9.0/tcconfig/shaper/htb.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,16 @@
         self.__qdisc_minor_id = None
         self.__qdisc_minor_id_count = 0
         self.__netem_major_id = None
 
     def get_qdisc_minor_id(self):
         if self.__qdisc_minor_id is None:
             self.__qdisc_minor_id = self.__get_unique_qdisc_minor_id()
+            logger.debug("__get_unique_qdisc_minor_id: {:d}".format(
+                self.__qdisc_minor_id))
 
         return self.__qdisc_minor_id
 
     def get_netem_qdisc_major_id(self, base_id):
         if self.__netem_major_id is None:
             self.__netem_major_id = self.__get_unique_netem_major_id()
```

### Comparing `tcconfig-0.8.0/tcconfig/shaper/tbf.py` & `tcconfig-0.9.0/tcconfig/shaper/tbf.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from __future__ import unicode_literals
 
 from subprocrunner import SubprocessRunner
 import typepy
 
 from .._common import (
     logging_context,
+    get_anywhere_network,
     run_command_helper,
 )
-from .._const import ANYWHERE_NETWORK
 from .._error import EmptyParameterError
 from .._traffic_direction import TrafficDirection
 from ._interface import AbstractShaper
 
 
 class TbfShaper(AbstractShaper):
 
@@ -129,14 +129,15 @@
                 self.get_qdisc_minor_id())
         else:
             flowid = "{:s}:2".format(self._tc_obj.qdisc_major_id_str)
 
         return SubprocessRunner(" ".join([
             "tc filter add",
             self.dev,
-            "protocol ip",
+            "protocol {:s}".format(self._tc_obj.protocol),
             "parent {:s}:".format(self._tc_obj.qdisc_major_id_str),
-            "prio 2 u32 match ip {:s} {:s}".format(
+            "prio 2 u32 match {:s} {:s} {:s}".format(
+                self._tc_obj.protocol,
                 self._get_network_direction_str(),
-                ANYWHERE_NETWORK),
+                get_anywhere_network(self._tc_obj.ip_version)),
             "flowid {:s}".format(flowid),
         ])).run()
```

### Comparing `tcconfig-0.8.0/tcconfig/_argparse_wrapper.py` & `tcconfig-0.9.0/tcconfig/_argparse_wrapper.py`

 * *Files identical despite different names*

### Comparing `tcconfig-0.8.0/tcconfig/_common.py` & `tcconfig-0.9.0/tcconfig/_common.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,67 +8,95 @@
 from __future__ import unicode_literals
 
 import contextlib
 
 import logbook
 import six
 import typepy
-import typepy
 
 import subprocrunner as spr
 
-from ._const import ANYWHERE_NETWORK
+from ._const import Network
 from ._error import NetworkInterfaceNotFoundError
 from ._logger import logger
 
 
 @contextlib.contextmanager
 def logging_context(name):
     logger.debug("|---- {:s}: {:s} -----".format("start", name))
     try:
         yield
     finally:
         logger.debug("----- {:s}: {:s} ----|".format("complete", name))
 
 
+def is_anywhere_network(network, ip_version):
+    try:
+        return network.strip() == get_anywhere_network(ip_version)
+    except AttributeError as e:
+        raise ValueError(e)
+
+
+def get_anywhere_network(ip_version):
+    ip_version_n = typepy.type.Integer(ip_version).try_convert()
+
+    if ip_version_n == 4:
+        return Network.Ipv4.ANYWHERE
+
+    if ip_version_n == 6:
+        return Network.Ipv6.ANYWHERE
+
+    raise ValueError("unknown ip version: {}".format(ip_version))
+
+
 def verify_network_interface(device):
     try:
         import netifaces
     except ImportError:
         return
 
     if device not in netifaces.interfaces():
         raise NetworkInterfaceNotFoundError(
             "network interface not found: {}".format(device))
 
 
-def sanitize_network(network):
+def sanitize_network(network, ip_version):
     """
     :return: Network string
     :rtype: str
     :raises ValueError: if the network string is invalid.
     """
 
     import ipaddress
 
     if typepy.is_null_string(network):
         return ""
 
     if network.lower() == "anywhere":
-        return ANYWHERE_NETWORK
+        return get_anywhere_network(ip_version)
 
     try:
-        ipaddress.IPv4Address(six.text_type(network))
-        return network + "/32"
+        if ip_version == 4:
+            ipaddress.IPv4Address(network)
+            return network + "/32"
+
+        if ip_version == 6:
+            return ipaddress.IPv6Address(network).compressed
     except ipaddress.AddressValueError:
         pass
 
-    ipaddress.IPv4Network(six.text_type(network))  # validate network str
+    # validate network str ---
+
+    if ip_version == 4:
+        return ipaddress.IPv4Network(six.text_type(network)).compressed
+
+    if ip_version == 6:
+        return ipaddress.IPv6Network(six.text_type(network)).compressed
 
-    return network
+    raise ValueError("unexpected ip version: {}".format(ip_version))
 
 
 def run_command_helper(command, error_regexp, message, exception=None):
     if logger.level != logbook.DEBUG:
         spr.set_logger(is_enable=False)
 
     proc = spr.SubprocessRunner(command)
```

### Comparing `tcconfig-0.8.0/tcconfig/_const.py` & `tcconfig-0.9.0/tcconfig/_const.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,21 +4,28 @@
 .. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
 """
 
 from __future__ import absolute_import
 from __future__ import unicode_literals
 
 
-VERSION = "0.8.0"
+VERSION = "0.9.0"
 
-ANYWHERE_NETWORK = "0.0.0.0/0"
 KILO_SIZE = 1000
 LIST_MANGLE_TABLE_COMMAND = "iptables -t mangle --line-numbers -L"
 
 
+class Network(object):
+    class Ipv4(object):
+        ANYWHERE = "0.0.0.0/0"
+
+    class Ipv6(object):
+        ANYWHERE = "::0/0"
+
+
 class Tc(object):
 
     class Subcommand(object):
         CLASS = "class"
         FILTER = "filter"
         QDISC = "qdisc"
         SHOW = "show"
```

### Comparing `tcconfig-0.8.0/tcconfig/_converter.py` & `tcconfig-0.9.0/tcconfig/_converter.py`

 * *Files identical despite different names*

### Comparing `tcconfig-0.8.0/tcconfig/_error.py` & `tcconfig-0.9.0/tcconfig/_error.py`

 * *Files identical despite different names*

### Comparing `tcconfig-0.8.0/tcconfig/_iptables.py` & `tcconfig-0.9.0/tcconfig/_iptables.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 from subprocrunner import SubprocessRunner
 import typepy
 from typepy.type import Integer
 
 from ._common import sanitize_network
 from ._const import (
-    ANYWHERE_NETWORK,
     LIST_MANGLE_TABLE_COMMAND,
+    Network,
 )
 from ._logger import logger
 from ._split_line_list import split_line_list
 
 
 VALID_CHAIN_LIST = ["PREROUTING", "INPUT", "OUTPUT"]
 
@@ -48,20 +48,20 @@
         return self.__mark_id
 
     @property
     def chain(self):
         return self.__chain
 
     def __init__(
-            self, mark_id, source, destination, chain, protocol="all",
-            line_number=None):
+            self, ip_version, mark_id, source, destination, chain,
+            protocol="all", line_number=None):
         self.__line_number = line_number
         self.__mark_id = mark_id
-        self.__source = sanitize_network(source)
-        self.__destination = sanitize_network(destination)
+        self.__source = sanitize_network(source, ip_version)
+        self.__destination = sanitize_network(destination, ip_version)
         self.__protocol = protocol
 
         if chain not in VALID_CHAIN_LIST:
             raise ValueError("invalid chain: {}".format(chain))
 
         self.__chain = chain
 
@@ -118,73 +118,76 @@
         return "iptables -t mangle -D {:s} {}".format(
             self.chain, self.line_number)
 
     @staticmethod
     def __is_valid_srcdst(srcdst):
         return (
             typepy.is_not_null_string(srcdst) and
-            srcdst != ANYWHERE_NETWORK
+            srcdst not in (Network.Ipv4.ANYWHERE, Network.Ipv6.ANYWHERE)
         )
 
 
 class IptablesMangleController(object):
 
     __RE_CHAIN = re.compile(
         "Chain {:s} |Chain {:s} |Chain {:s} ".format(*VALID_CHAIN_LIST))
     __RE_CHAIN_NAME = re.compile(
         "{:s}|{:s}|{:s}".format(*VALID_CHAIN_LIST))
     __MAX_MARK_ID = 0xffffffff
     __MARK_ID_OFFSET = 100
 
-    enable = True
+    @property
+    def enable(self):
+        return self.__enable
 
-    @classmethod
-    def clear(cls):
-        if not cls.enable:
+    def __init__(self, enable, ip_version):
+        self.__enable = enable
+        self.__ip_version = ip_version
+
+    def clear(self):
+        if not self.enable:
             return
 
-        for mangle in cls.parse():
+        for mangle in self.parse():
             proc = SubprocessRunner(mangle.to_delete_command())
             if proc.run() != 0:
                 raise RuntimeError(proc.stderr)
 
-    @classmethod
-    def get_iptables(cls):
+    def get_iptables(self):
         proc = SubprocessRunner(LIST_MANGLE_TABLE_COMMAND)
         if proc.run() != 0:
             raise RuntimeError(proc.stderr)
 
         return proc.stdout
 
-    @classmethod
-    def get_unique_mark_id(cls):
-        mark_id_list = [mangle.mark_id for mangle in cls.parse()]
+    def get_unique_mark_id(self):
+        mark_id_list = [
+            mangle.mark_id for mangle in self.parse()]
         logger.debug("mangle mark list: {}".format(mark_id_list))
 
-        unique_mark_id = 1 + cls.__MARK_ID_OFFSET
-        while unique_mark_id < cls.__MAX_MARK_ID:
+        unique_mark_id = 1 + self.__MARK_ID_OFFSET
+        while unique_mark_id < self.__MAX_MARK_ID:
             if unique_mark_id not in mark_id_list:
                 return unique_mark_id
 
             unique_mark_id += 1
 
         raise RuntimeError("usable mark id not found")
 
-    @classmethod
-    def parse(cls):
-        for block in split_line_list(cls.get_iptables().splitlines()):
+    def parse(self):
+        for block in split_line_list(self.get_iptables().splitlines()):
             if len(block) <= 1:
                 # skip if no entry exists
                 continue
 
-            match = cls.__RE_CHAIN.search(block[0])
+            match = self.__RE_CHAIN.search(block[0])
             if match is None:
                 continue
 
-            chain = cls.__RE_CHAIN_NAME.search(match.group()).group()
+            chain = self.__RE_CHAIN_NAME.search(match.group()).group()
 
             for line in reversed(block[2:]):
                 item_list = line.split()
                 if len(item_list) < 6:
                     continue
 
                 line_number = int(item_list[0])
@@ -198,14 +201,15 @@
                 except ValueError:
                     continue
 
                 if target != "MARK":
                     continue
 
                 yield IptablesMangleMark(
+                    ip_version=self.__ip_version,
                     mark_id=mark, source=source, destination=destination,
                     chain=chain, protocol=protocol, line_number=line_number)
 
     @classmethod
     def add(cls, mangling_mark):
         if not cls.enable:
             return 0
```

### Comparing `tcconfig-0.8.0/tcconfig/_logger.py` & `tcconfig-0.9.0/tcconfig/_logger.py`

 * *Files identical despite different names*

### Comparing `tcconfig-0.8.0/tcconfig/_split_line_list.py` & `tcconfig-0.9.0/tcconfig/_split_line_list.py`

 * *Files identical despite different names*

### Comparing `tcconfig-0.8.0/tcconfig/parser.py` & `tcconfig-0.9.0/tcconfig/parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 .. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
 """
 
 from __future__ import absolute_import
 from __future__ import unicode_literals
 
 import copy
+import ipaddress
 import re
 
 import typepy
 
 import pyparsing as pp
 
 from ._const import Tc
@@ -23,24 +24,34 @@
         return text.decode("ascii")
     except AttributeError:
         return text
 
 
 class TcFilterParser(object):
 
-    class FilterMatchId(object):
+    class FilterMatchIdIpv4(object):
         INCOMING_NETWORK = 12
         OUTGOING_NETWORK = 16
         PORT = 20
 
+    class FilterMatchIdIpv6(object):
+        INCOMING_NETWORK_LIST = [8, 12, 16, 20]
+        OUTGOING_NETWORK_LIST = [24, 28, 32, 36]
+        PORT = 40
+
     __FILTER_FLOWID_PATTERN = (
         pp.Literal("filter parent") +
         pp.SkipTo("flowid", include=True) +
         pp.Word(pp.hexnums + ":")
     )
+    __FILTER_PROTOCOL_PATTERN = (
+        pp.Literal("filter parent") +
+        pp.SkipTo("protocol", include=True) +
+        pp.Word(pp.alphanums)
+    )
     __FILTER_MATCH_PATTERN = (
         pp.Literal("match") +
         pp.Word(pp.alphanums + "/") +
         pp.Literal("at") +
         pp.Word(pp.nums)
     )
     __FILTER_MANGLE_MARK_PATTERN = (
@@ -52,14 +63,18 @@
     )
 
     @property
     def flow_id(self):
         return self.__flow_id
 
     @property
+    def protocol(self):
+        return self.__protocol
+
+    @property
     def filter_network(self):
         return self.__filter_network
 
     @property
     def filter_port(self):
         return self.__filter_port
 
@@ -67,26 +82,35 @@
     def handle(self):
         return self.__handle
 
     @property
     def classid(self):
         return self.__classid
 
-    def __init__(self):
+    def __init__(self, ip_version):
+        self.__ip_version = ip_version
         self.__clear()
 
+        self.__buffer = None
+        self.__parse_idx = 0
+
     def parse_filter(self, text):
         self.__clear()
 
         if typepy.is_null_string(text):
             return []
 
         filter_data_matrix = []
+        self.__buffer = text.splitlines()
+        self.__parse_idx = 0
+
+        while self.__parse_idx < len(self.__buffer):
+            line = self.__buffer[self.__parse_idx].strip()
+            self.__parse_idx += 1
 
-        for line in text.splitlines():
             if typepy.is_null_string(line):
                 continue
 
             try:
                 self.__parse_mangle_mark(line)
             except pp.ParseException:
                 logger.debug("failed to parse mangle: {}".format(line))
@@ -110,15 +134,27 @@
                     self.__parse_flow_id(line)
 
                 continue
             except pp.ParseException:
                 logger.debug("failed to parse flow id: {}".format(line))
 
             try:
-                self.__parse_filter(line)
+                self.__parse_protocol(line)
+                continue
+            except pp.ParseException:
+                logger.debug("failed to parse protocol: {}".format(line))
+
+            try:
+                if self.__ip_version == 4:
+                    self.__parse_filter_ipv4(line)
+                elif self.__ip_version == 6:
+                    self.__parse_filter_ipv6(line)
+                else:
+                    raise ValueError(
+                        "unknown ip version: {}".format(self.__ip_version))
             except pp.ParseException:
                 logger.debug("failed to parse filter: {}".format(line))
 
         if self.flow_id:
             filter_data_matrix.append(self.__get_filter())
 
         return filter_data_matrix
@@ -135,59 +171,127 @@
 
         return re.search("ifb[\d]+", match.group()).group()
 
     def __clear(self):
         self.__flow_id = None
         self.__filter_network = None
         self.__filter_port = None
+        self.__protocol = None
 
         self.__handle = None
         self.__classid = None
 
     def __get_filter(self):
         return copy.deepcopy({
             "flowid": self.flow_id,
             "network": self.filter_network,
             "port": self.filter_port,
+            "protocol": self.protocol
         })
 
     def __parse_flow_id(self, line):
         parsed_list = self.__FILTER_FLOWID_PATTERN.parseString(
             _to_unicode(line.lstrip()))
         self.__flow_id = parsed_list[-1]
         logger.debug("succeed to parse flow id: flow-id={}, line={}".format(
             self.flow_id, line))
 
+    def __parse_protocol(self, line):
+        parsed_list = self.__FILTER_PROTOCOL_PATTERN.parseString(
+            _to_unicode(line.lstrip()))
+        self.__protocol = parsed_list[-1]
+
     def __parse_mangle_mark(self, line):
         parsed_list = self.__FILTER_MANGLE_MARK_PATTERN.parseString(
             _to_unicode(line.lstrip()))
         self.__classid = parsed_list[-1]
         self.__handle = int(u"0" + parsed_list[-3], 16)
         logger.debug(
             "succeed to parse mangle mark: classid={}, handle={}, line={}".format(
                 self.classid, self.handle, line))
 
-    def __parse_filter(self, line):
+    def __parse_filter_line(self, line):
         parsed_list = self.__FILTER_MATCH_PATTERN.parseString(
             _to_unicode(line))
         value_hex, mask_hex = parsed_list[1].split("/")
         match_id = int(parsed_list[3])
 
+        return (value_hex, mask_hex, match_id)
+
+    def __parse_filter_ipv4(self, line):
+        value_hex, mask_hex, match_id = self.__parse_filter_line(line)
+
         if match_id in [
-            self.FilterMatchId.INCOMING_NETWORK,
-            self.FilterMatchId.OUTGOING_NETWORK,
+            self.FilterMatchIdIpv4.INCOMING_NETWORK,
+            self.FilterMatchIdIpv4.OUTGOING_NETWORK,
         ]:
             ipaddr = ".".join([
                 str(int(value_hex[i: i + 2], 16))
                 for i in range(0, len(value_hex), 2)
             ])
             netmask = bin(int(mask_hex, 16)).count("1")
 
             self.__filter_network = "{:s}/{:d}".format(ipaddr, netmask)
-        elif match_id == self.FilterMatchId.PORT:
+        elif match_id == self.FilterMatchIdIpv4.PORT:
+            self.__filter_port = int(value_hex, 16)
+
+        logger.debug(
+            "succeed to parse filter: filter_network={}, filter_port={}, line={}".format(
+                self.filter_network, self.filter_port, line))
+
+    def __parse_filter_ipv6(self, line):
+        netmask = 0
+        value_hex, mask_hex, match_id = self.__parse_filter_line(line)
+
+        octet_list = []
+        octet_len = 4
+
+        if (
+            match_id in self.FilterMatchIdIpv6.INCOMING_NETWORK_LIST or
+            match_id in self.FilterMatchIdIpv6.OUTGOING_NETWORK_LIST
+        ):
+            octet_list.extend([
+                value_hex[i: i + octet_len]
+                for i in range(0, len(value_hex), octet_len)
+            ])
+            netmask += bin(int(mask_hex, 16)).count("1")
+
+            while True:
+                try:
+                    line = self.__buffer[self.__parse_idx].strip()
+                except IndexError:
+                    break
+
+                try:
+                    value_hex, mask_hex, match_id = self.__parse_filter_line(
+                        line)
+                except pp.ParseException:
+                    break
+
+                if (
+                    match_id in self.FilterMatchIdIpv6.INCOMING_NETWORK_LIST or
+                    match_id in self.FilterMatchIdIpv6.OUTGOING_NETWORK_LIST
+                ):
+                    octet_list.extend([
+                        value_hex[i: i + octet_len]
+                        for i in range(0, len(value_hex), octet_len)
+                    ])
+                    netmask += bin(int(mask_hex, 16)).count("1")
+                else:
+                    break
+
+                self.__parse_idx += 1
+
+            while len(octet_list) < 8:
+                octet_list.append("0000")
+
+            self.__filter_network = ipaddress.IPv6Network("{:s}/{:d}".format(
+                ":".join(octet_list), netmask)).compressed
+
+        elif match_id == self.FilterMatchIdIpv6.PORT:
             self.__filter_port = int(value_hex, 16)
 
         logger.debug(
             "succeed to parse filter: filter_network={}, filter_port={}, line={}".format(
                 self.filter_network, self.filter_port, line))
```

### Comparing `tcconfig-0.8.0/tcconfig/tcdel.py` & `tcconfig-0.9.0/tcconfig/tcdel.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
     tc = TrafficControl(options.device)
     if options.log_level == logbook.INFO:
         subprocrunner.set_log_level(logbook.ERROR)
 
     subprocrunner.SubprocessRunner.is_save_history = True
     if options.tc_command_output != TcCoomandOutput.NOT_SET:
-        subprocrunner.SubprocessRunner.is_dry_run = True
+        subprocrunner.SubprocessRunner.is_dry_run_default = True
 
     if options.tc_command_output != TcCoomandOutput.NOT_SET:
         set_logger(False)
 
     try:
         return_code = tc.delete_tc()
     except NetworkInterfaceNotFoundError as e:
```

### Comparing `tcconfig-0.8.0/tcconfig/tcset.py` & `tcconfig-0.9.0/tcconfig/tcset.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 import pyparsing as pp
 
 from ._argparse_wrapper import ArgparseWrapper
 from ._common import write_tc_script
 from ._const import (
     VERSION,
-    ANYWHERE_NETWORK,
+    Network,
     TcCoomandOutput,
 )
 from ._error import (
     ModuleNotFoundError,
     NetworkInterfaceNotFoundError,
 )
 from ._logger import (
@@ -108,14 +108,17 @@
     group.add_argument(
         "--network",
         help="target IP address/network to control traffic")
     group.add_argument(
         "--port", type=int,
         help="target port number to control traffic.")
     group.add_argument(
+        "--ipv6", dest="is_ipv6", action="store_true", default=False,
+        help="apply traffic control to IPv6 packets rather than IPv4.")
+    group.add_argument(
         "--shaping-algo", dest="shaping_algorithm",
         choices=["tbf", "htb"], default="htb",
         help="shaping algorithm. defaults to %(default)s (recommended).")
 
     group = parser.parser.add_argument_group("Routing")
     group.add_argument(
         "--iptables", dest="is_enable_iptables",
@@ -192,15 +195,16 @@
                     ] + [
                         "--{:s}={:s}".format(k, v)
                         for k, v in six.iteritems(filter_table)
                     ]
 
                     try:
                         network = self.__parse_tc_filter_network(tc_filter)
-                        if network != ANYWHERE_NETWORK:
+                        if network not in (
+                                Network.Ipv4.ANYWHERE, Network.Ipv6.ANYWHERE):
                             option_list.append("--network=" + network)
                     except pp.ParseException:
                         pass
 
                     try:
                         port = self.__parse_tc_filter_port(tc_filter)
                         option_list.append("--port=" + port)
@@ -265,29 +269,30 @@
         latency_ms=options.network_latency,
         latency_distro_ms=options.latency_distro_ms,
         packet_loss_rate=options.packet_loss_rate,
         corruption_rate=options.corruption_rate,
         network=options.network,
         src_network=options.src_network,
         port=options.port,
+        is_ipv6=options.is_ipv6,
         is_add_shaper=options.is_add_shaper,
         is_enable_iptables=options.is_enable_iptables,
         shaping_algorithm=options.shaping_algorithm,
         tc_command_output=options.tc_command_output,
     )
 
     try:
         tc.validate()
     except (NetworkInterfaceNotFoundError, ValueError) as e:
         logger.error(str(e))
         return errno.EINVAL
 
     subprocrunner.SubprocessRunner.is_save_history = True
     if options.tc_command_output != TcCoomandOutput.NOT_SET:
-        subprocrunner.SubprocessRunner.is_dry_run = True
+        subprocrunner.SubprocessRunner.is_dry_run_default = True
 
     if options.overwrite:
         if options.log_level == logbook.INFO:
             set_log_level(logbook.ERROR)
 
         try:
             tc.delete_tc()
```

### Comparing `tcconfig-0.8.0/tcconfig/tcshow.py` & `tcconfig-0.9.0/tcconfig/tcshow.py`

 * *Files 11% similar despite different names*

```diff
@@ -52,56 +52,69 @@
 def parse_option():
     parser = ArgparseWrapper(VERSION)
 
     group = parser.parser.add_argument_group("Traffic Control")
     group.add_argument(
         "--device", action="append", required=True,
         help="network device name (e.g. eth0)")
+    group.add_argument(
+        "--ipv6", dest="ip_version", action="store_const",
+        const=6, default=4,
+        help="""
+        Display IPv6 shaping rules.
+        Defaults to show IPv4 shaping rules.
+        """)
 
     return parser.parser.parse_args()
 
 
 class TcShapingRuleParser(object):
 
     @property
     def device(self):
         return self.__device
 
-    def __init__(self, device, logger):
+    def __init__(self, device, ip_version, logger):
         self.__device = device
+        self.__ip_version = ip_version
         self.__logger = logger
 
+        self.__iptables_ctrl = IptablesMangleController(True, ip_version)
+
     def get_tc_parameter(self):
         return {
             self.device: {
                 TrafficDirection.OUTGOING: self.__get_shaping_rule(
                     self.device),
                 TrafficDirection.INCOMING: self.__get_shaping_rule(
                     self.__get_ifb_from_device()),
             },
         }
 
     def __get_ifb_from_device(self):
         filter_runner = SubprocessRunner(
-            "tc filter show dev {:s} root".format(self.device))
+            "tc filter show dev {:s} root".format(self.device), dry_run=False)
         filter_runner.run()
 
-        return TcFilterParser().parse_incoming_device(filter_runner.stdout)
+        return TcFilterParser(self.__ip_version).parse_incoming_device(
+            filter_runner.stdout)
 
     def __get_filter_key(self, filter_param):
         network_format = "network={:s}"
         port_format = "port={:d}"
+        protocol_format = "protocol={:s}"
         key_item_list = []
 
         if Tc.Param.HANDLE in filter_param:
             handle = filter_param.get(Tc.Param.HANDLE)
             Integer(handle).validate()
             handle = int(handle)
 
-            for mangle in IptablesMangleController.parse():
+            # for mangle in IptablesMangleController.parse(self.__ip_version):
+            for mangle in self.__iptables_ctrl.parse():
                 if mangle.mark_id != handle:
                     continue
 
                 key_item_list.append(network_format.format(mangle.destination))
                 if typepy.is_not_null_string(mangle.source):
                     key_item_list.append("source={:s}".format(mangle.source))
                 key_item_list.append("protocol={}".format(mangle.protocol))
@@ -114,14 +127,17 @@
             if typepy.is_not_null_string(network):
                 key_item_list.append(network_format.format(network))
 
             port = filter_param.get(Tc.Param.PORT)
             if Integer(port).is_type():
                 key_item_list.append(port_format.format(port))
 
+            protocol = filter_param.get("protocol")
+            if typepy.is_not_null_string(protocol):
+                key_item_list.append(protocol_format.format(protocol))
         return ", ".join(key_item_list)
 
     def __get_shaping_rule(self, device):
         if typepy.is_null_string(device):
             return {}
 
         class_param_list = self.__parse_tc_class(device)
@@ -184,15 +200,15 @@
             return []
 
         logger.debug("tc qdisc parse result: {}".format(param_list))
 
         return param_list
 
     def __parse_tc_filter(self, device):
-        param_list = list(TcFilterParser().parse_filter(
+        param_list = list(TcFilterParser(self.__ip_version).parse_filter(
             run_tc_show(Tc.Subcommand.FILTER, device)))
         logger.debug("tc filter parse result: {}".format(param_list))
 
         return param_list
 
     def __parse_tc_class(self, device):
         param_list = list(TcClassParser().parse(
@@ -207,25 +223,26 @@
 
     set_log_level(options.log_level)
 
     subprocrunner.Which("tc").verify()
 
     subprocrunner.SubprocessRunner.is_save_history = True
     if options.tc_command_output != TcCoomandOutput.NOT_SET:
-        subprocrunner.SubprocessRunner.is_dry_run = True
+        subprocrunner.SubprocessRunner.is_dry_run_default = True
 
     tc_param = {}
     for device in options.device:
         try:
             verify_network_interface(device)
         except NetworkInterfaceNotFoundError as e:
             logger.debug(str(e))
             continue
 
-        tc_param.update(TcShapingRuleParser(device, logger).get_tc_parameter())
+        tc_param.update(TcShapingRuleParser(
+            device, options.ip_version, logger).get_tc_parameter())
 
     command_history = "\n".join(SubprocessRunner.get_history())
 
     if options.tc_command_output == TcCoomandOutput.STDOUT:
         print(command_history)
         return 0
```

### Comparing `tcconfig-0.8.0/tcconfig/traffic_control.py` & `tcconfig-0.9.0/tcconfig/traffic_control.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import typepy
 from typepy.type import RealNumber
 
 import subprocrunner as spr
 
 from ._common import (
     logging_context,
+    get_anywhere_network,
     sanitize_network,
     verify_network_interface,
     run_command_helper,
 )
 from ._const import (
     KILO_SIZE,
     TcCoomandOutput,
@@ -139,23 +140,39 @@
         return self.__qdisc_major_id
 
     @property
     def qdisc_major_id_str(self):
         return "{:x}".format(self.__qdisc_major_id)
 
     @property
+    def ip_version(self):
+        return 6 if self.__is_ipv6 else 4
+
+    @property
+    def protocol(self):
+        return "ipv6" if self.__is_ipv6 else "ip"
+
+    @property
+    def protocol_match(self):
+        return "ip6" if self.__is_ipv6 else "ip"
+
+    @property
     def tc_command_output(self):
         return self.__tc_command_output
 
+    @property
+    def iptables_ctrl(self):
+        return self.__iptables_ctrl
+
     def __init__(
             self, device,
             direction=None, bandwidth_rate=None,
             latency_ms=None, latency_distro_ms=None,
             packet_loss_rate=None, corruption_rate=None,
-            network=None, port=None,
+            network=None, port=None, is_ipv6=False,
             src_network=None,
             is_add_shaper=False,
             is_enable_iptables=True,
             shaping_algorithm=None,
             tc_command_output=TcCoomandOutput.NOT_SET,
     ):
         self.__device = device
@@ -164,38 +181,41 @@
         self.__latency_ms = latency_ms  # [milliseconds]
         self.__latency_distro_ms = latency_distro_ms  # [milliseconds]
         self.__packet_loss_rate = packet_loss_rate  # [%]
         self.__corruption_rate = corruption_rate  # [%]
         self.__network = network
         self.__src_network = src_network
         self.__port = port
+        self.__is_ipv6 = is_ipv6
         self.__is_add_shaper = is_add_shaper
         self.__is_enable_iptables = is_enable_iptables
         self.__tc_command_output = tc_command_output
 
         self.__qdisc_major_id = self.__get_device_qdisc_major_id()
 
         # bandwidth string [G/M/K bit per second]
         try:
             self.__bandwidth_rate = Humanreadable(
                 bandwidth_rate, kilo_size=KILO_SIZE).to_kilo_value()
         except (TypeError, ValueError):
             self.__bandwidth_rate = None
 
-        IptablesMangleController.enable = is_enable_iptables
+        self.__iptables_ctrl = IptablesMangleController(
+            is_enable_iptables, self.ip_version)
 
         self.__init_shaper(shaping_algorithm)
 
     def validate(self):
         verify_network_interface(self.__device)
         self.__validate_netem_parameter()
         self.__validate_src_network()
 
-        self.__network = sanitize_network(self.network)
-        self.__src_network = sanitize_network(self.src_network)
+        self.__network = sanitize_network(self.network, self.ip_version)
+        self.__src_network = sanitize_network(
+            self.src_network, self.ip_version)
         self.__validate_port()
 
     def __validate_src_network(self):
         if typepy.is_null_string(self.src_network):
             return
 
         if not self.is_enable_iptables:
@@ -216,14 +236,17 @@
             return self.__device
 
         if self.direction == TrafficDirection.INCOMING:
             return self.ifb_device
 
         raise ValueError("unknown direction: " + self.direction)
 
+    def get_anywhere_network(self):
+        return get_anywhere_network(self, )
+
     def get_command_history(self):
         def tc_filter(command):
             if command == LIST_MANGLE_TABLE_COMMAND:
                 return False
 
             if re.search("^tc .* show dev", command):
                 return False
@@ -249,26 +272,27 @@
         with logging_context("delete ingress qdisc"):
             returncode = run_command_helper(
                 "tc qdisc del dev {:s} ingress".format(self.__device),
                 re.compile("|".join([
                     "RTNETLINK answers: Invalid argument",
                     "RTNETLINK answers: No such file or directory",
                 ])),
-                "failed to delete qdisc: no qdisc for incomming packets")
+                "failed to delete qdisc: no qdisc for incoming packets")
             result_list.append(returncode == 0)
 
         with logging_context("delete ifb device"):
             try:
                 result_list.append(self.__delete_ifb_device() == 0)
             except NetworkInterfaceNotFoundError as e:
                 logger.debug(e)
                 result_list.append(False)
 
         with logging_context("delete iptables mangle table entries"):
-            IptablesMangleController.clear()
+            self.iptables_ctrl.clear()
+            # IptablesMangleController.clear()
 
         return any(result_list)
 
     def __init_shaper(self, shaping_algorithm):
         if shaping_algorithm is None:
             self.__shaper = None
             return
@@ -364,15 +388,15 @@
             self.REGEXP_FILE_EXISTS,
             self.EXISTS_MSG_TEMPLATE.format(
                 "failed to add qdisc: ingress qdisc already exists."))
 
         return_code |= spr.SubprocessRunner(" ".join([
             "tc filter add",
             "dev " + self.__device,
-            "parent ffff: protocol ip u32 match u32 0 0",
+            "parent ffff: protocol " + self.protocol + " u32 match u32 0 0",
             "flowid {:x}:".format(self.__get_device_qdisc_major_id()),
             "action mirred egress redirect",
             "dev " + self.ifb_device,
         ])).run()
 
         return return_code
```

### Comparing `tcconfig-0.8.0/tcconfig.egg-info/PKG-INFO` & `tcconfig-0.9.0/tcconfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tcconfig
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Simple tc command wrapper tool. Easy to set up traffic control of network bandwidth/latency/packet-loss to a network interface.
 
 Home-page: https://github.com/thombashi/tcconfig
 Author: Tsuyoshi Hombashi
 Author-email: gogogo.vm@gmail.com
 License: MIT License
 Description: tcconfig
```

### Comparing `tcconfig-0.8.0/tcconfig.egg-info/SOURCES.txt` & `tcconfig-0.9.0/tcconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tcconfig-0.8.0/test/common.py` & `tcconfig-0.9.0/test/common.py`

 * *Files identical despite different names*

### Comparing `tcconfig-0.8.0/test/test_converter.py` & `tcconfig-0.9.0/test/test_converter.py`

 * *Files identical despite different names*

### Comparing `tcconfig-0.8.0/test/test_iptables.py` & `tcconfig-0.9.0/test/test_iptables.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,74 @@
 # encoding: utf-8
 
 """
 .. codeauthor:: Tsuyoshi Hombashi <gogogo.vm@gmail.com>
 """
 
 from __future__ import unicode_literals
+
 import random
 
 import pytest
 from subprocrunner import SubprocessRunner
 
-from tcconfig._iptables import VALID_CHAIN_LIST
-from tcconfig._iptables import IptablesMangleMark
 from tcconfig._iptables import IptablesMangleController
+from tcconfig._iptables import IptablesMangleMark
+from tcconfig._iptables import VALID_CHAIN_LIST
 
 
 _DEF_SRC = "192.168.0.0/24"
 _DEF_DST = "192.168.100.0/24"
 
 
 prerouting_mangle_mark_list = [
     IptablesMangleMark(
+        ip_version=4,
         line_number=1,
         mark_id=1,
         source=_DEF_SRC,
         destination=_DEF_DST,
         chain="PREROUTING",
         protocol="all"
     ),
 ]
 
 input_mangle_mark_list = [
     IptablesMangleMark(
+        ip_version=4,
         line_number=1,
         mark_id=1234,
         source="anywhere",
         destination=_DEF_DST,
         chain="INPUT",
         protocol="all"
     ),
 ]
 
 output_mangle_mark_list = [
     IptablesMangleMark(
+        ip_version=4,
         line_number=1,
         mark_id=12,
         source=_DEF_SRC,
         destination=_DEF_DST,
         chain="OUTPUT",
         protocol="tcp"
     ),
     IptablesMangleMark(
+        ip_version=4,
         line_number=2,
         mark_id=123,
         source=_DEF_SRC,
         destination="anywhere",
         chain="OUTPUT",
         protocol="all"
     ),
     IptablesMangleMark(
+        ip_version=4,
         line_number=3,
         mark_id=12345,
         source="anywhere",
         destination="anywhere",
         chain="OUTPUT",
         protocol="all"
     ),
@@ -77,14 +83,19 @@
 reverse_mangle_mark_list = (
     list(reversed(prerouting_mangle_mark_list)) +
     list(reversed(input_mangle_mark_list)) +
     list(reversed(output_mangle_mark_list))
 )
 
 
+@pytest.fixture
+def iptables_ctrl_ipv4():
+    return IptablesMangleController(True, ip_version=4)
+
+
 class Test_IptablesMangleMark_repr(object):
 
     def test_smoke(self):
         for mangle_mark in mangle_mark_list:
             assert len(str(mangle_mark)) > 0
 
 
@@ -129,14 +140,15 @@
             ],
         ]
     )
     def test_normal(
             self, mark_id, source, destination, chain, protocol, line_number,
             expected):
         mark = IptablesMangleMark(
+            ip_version=4,
             mark_id=mark_id, source=source, destination=destination,
             chain=chain, protocol=protocol, line_number=line_number)
         assert mark.to_append_command() == expected
 
 
 class Test_IptablesMangleMark_to_delete_command(object):
 
@@ -156,14 +168,15 @@
             ],
         ]
     )
     def test_normal(
             self, mark_id, source, destination, chain, protocol, line_number,
             expected):
         mark = IptablesMangleMark(
+            ip_version=4,
             mark_id=mark_id, source=_DEF_SRC, destination=_DEF_DST,
             chain=chain, protocol=protocol, line_number=line_number)
         assert mark.to_delete_command() == expected
 
     @pytest.mark.parametrize(
         [
             "mark_id", "source", "destination", "chain", "protocol", "line_number",
@@ -176,103 +189,79 @@
             ],
         ]
     )
     def test_exception(
             self, mark_id, source, destination, chain, protocol, line_number,
             expected):
         mark = IptablesMangleMark(
+            ip_version=4,
             mark_id=mark_id, source=source, destination=destination,
             chain=chain, protocol=protocol, line_number=line_number)
         with pytest.raises(expected):
             mark.to_delete_command()
 
 
 class Test_IptablesMangleController_get_unique_mark_id(object):
 
-    @classmethod
-    def setup_class(cls):
-        IptablesMangleController.clear()
-
-    @classmethod
-    def teardown_class(cls):
-        IptablesMangleController.clear()
-
     @pytest.mark.xfail
-    def test_normal(self):
+    def test_normal(self, iptables_ctrl_ipv4):
+        iptables_ctrl_ipv4.clear()
+
         for i in range(5):
-            mark_id = IptablesMangleController.get_unique_mark_id()
+            mark_id = iptables_ctrl_ipv4.get_unique_mark_id()
 
             assert mark_id == (i + 101)
 
             mangle_mark = IptablesMangleMark(
+                ip_version=4,
                 mark_id=mark_id, source=_DEF_SRC, destination=_DEF_DST,
                 chain=random.choice(VALID_CHAIN_LIST))
 
-            assert IptablesMangleController.add(mangle_mark) == 0
+            assert iptables_ctrl_ipv4.add(mangle_mark) == 0
 
 
 class Test_IptablesMangleController_add(object):
 
-    @classmethod
-    def setup_class(cls):
-        IptablesMangleController.clear()
-
-    @classmethod
-    def teardown_class(cls):
-        IptablesMangleController.clear()
-
     @pytest.mark.xfail
-    def test_normal(self):
-        initial_len = len(IptablesMangleController.get_iptables())
+    def test_normal(self, iptables_ctrl_ipv4):
+        iptables_ctrl_ipv4.clear()
+        initial_len = len(iptables_ctrl_ipv4.get_iptables())
 
         for mangle_mark in mangle_mark_list:
-            assert IptablesMangleController.add(mangle_mark) == 0
+            assert iptables_ctrl_ipv4.add(mangle_mark) == 0
 
-        assert len(IptablesMangleController.get_iptables()) > initial_len
+        assert len(iptables_ctrl_ipv4.get_iptables()) > initial_len
 
 
 class Test_IptablesMangleController_clear(object):
 
-    @classmethod
-    def setup_class(cls):
-        IptablesMangleController.clear()
-
-    @classmethod
-    def teardown_class(cls):
-        IptablesMangleController.clear()
-
     @pytest.mark.xfail
-    def test_normal(self):
-        initial_len = len(IptablesMangleController.get_iptables())
+    def test_normal(self, iptables_ctrl_ipv4):
+        iptables_ctrl_ipv4.clear()
+
+        initial_len = len(iptables_ctrl_ipv4.get_iptables())
 
         for mangle_mark in mangle_mark_list:
-            assert IptablesMangleController.add(mangle_mark) == 0
+            assert iptables_ctrl_ipv4.add(mangle_mark) == 0
 
-        assert len(IptablesMangleController.get_iptables()) > initial_len
+        assert len(iptables_ctrl_ipv4.get_iptables()) > initial_len
 
-        IptablesMangleController.clear()
+        iptables_ctrl_ipv4.clear()
 
-        assert len(IptablesMangleController.get_iptables()) == initial_len
+        assert len(iptables_ctrl_ipv4.get_iptables()) == initial_len
 
 
 class Test_IptablesMangleController_parse(object):
-
-    @classmethod
-    def setup_class(cls):
-        IptablesMangleController.clear()
-
-    @classmethod
-    def teardown_class(cls):
-        IptablesMangleController.clear()
-
     @pytest.mark.xfail
-    def test_normal(self):
+    def test_normal(self, iptables_ctrl_ipv4):
+        iptables_ctrl_ipv4.clear()
+
         for mangle_mark in mangle_mark_list:
-            assert IptablesMangleController.add(mangle_mark) == 0
+            assert iptables_ctrl_ipv4.add(mangle_mark) == 0
 
         for lhs_mangle, rhs_mangle in zip(
-                IptablesMangleController.parse(), reverse_mangle_mark_list):
+                iptables_ctrl_ipv4.parse(), reverse_mangle_mark_list):
 
             print("lhs: {}".format(lhs_mangle))
             print("rhs: {}".format(rhs_mangle))
 
             assert lhs_mangle == rhs_mangle
```

### Comparing `tcconfig-0.8.0/test/test_parser.py` & `tcconfig-0.9.0/test/test_parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,82 +10,178 @@
 import pytest
 import six
 
 import tcconfig.parser
 
 
 @pytest.fixture
-def filter_parser():
-    return tcconfig.parser.TcFilterParser()
+def filter_parser_ipv4():
+    return tcconfig.parser.TcFilterParser(ip_version=4)
+
+
+@pytest.fixture
+def filter_parser_ipv6():
+    return tcconfig.parser.TcFilterParser(ip_version=6)
 
 
 @pytest.fixture
 def qdisc_parser():
     return tcconfig.parser.TcQdiscParser()
 
 
-class Test_TcFilterParser_parse_filter(object):
+class Test_TcFilterParser_parse_filter_ipv4(object):
 
     @pytest.mark.parametrize(["value", "expected"], [
         [None, []],
         ["", []],
         [
             six.b("""filter parent 1: protocol ip pref 1 u32
 filter parent 1: protocol ip pref 1 u32 fh 801: ht divisor 1
 filter parent 1: protocol ip pref 1 u32 fh 801::800 order 2048 key ht 801 bkt 0 flowid 1:1
   match c0a8000a/ffffffff at 16
 filter parent 1: protocol ip pref 2 u32
 filter parent 1: protocol ip pref 2 u32 fh 800: ht divisor 1
 filter parent 1: protocol ip pref 2 u32 fh 800::800 order 2048 key ht 800 bkt 0 flowid 1:2
   match 00000000/00000000 at 16"""),
             [
-                {'flowid': '1:1', 'network': '192.168.0.10/32', 'port': None},
-                {'flowid': '1:2', 'network': '0.0.0.0/0', 'port': None},
+                {
+                    'flowid': '1:1', 'network': '192.168.0.10/32',
+                    'protocol': 'ip', 'port': None,
+                },
+                {
+                    'flowid': '1:2', 'network': '0.0.0.0/0',
+                    'protocol': None, 'port': None,
+                },
             ],
         ],
         [
             six.b("""filter parent 1: protocol ip pref 1 u32
 filter parent 1: protocol ip pref 1 u32 fh 801: ht divisor 1
 filter parent 1: protocol ip pref 1 u32 fh 801::800 order 2048 key ht 801 bkt 0 flowid 1:1
   match c0a80000/ffffff00 at 16
   match 00000050/0000ffff at 20
 filter parent 1: protocol ip pref 2 u32
 filter parent 1: protocol ip pref 2 u32 fh 800: ht divisor 1
 filter parent 1: protocol ip pref 2 u32 fh 800::800 order 2048 key ht 800 bkt 0 flowid 1:2
   match 00000000/00000000 at 16"""),
             [
-                {'flowid': '1:1', 'network': '192.168.0.0/24', 'port': 80},
-                {'flowid': '1:2', 'network': '0.0.0.0/0', 'port': None},
+                {
+                    'flowid': '1:1', 'network': '192.168.0.0/24',
+                    'protocol': 'ip', 'port': 80,
+                },
+                {
+                    'flowid': '1:2', 'network': '0.0.0.0/0',
+                    'protocol': None, 'port': None,
+                },
             ],
         ],
         [
             six.b("""filter parent 1: protocol ip pref 1 u32
 filter parent 1: protocol ip pref 1 u32 fh 801: ht divisor 1
 filter parent 1: protocol ip pref 1 u32 fh 801::800 order 2048 key ht 801 bkt 0 flowid 1:3
   match c0a8000a/ffffffff at 12
   match 00001f90/0000ffff at 20
 filter parent 1: protocol ip pref 2 u32
 filter parent 1: protocol ip pref 2 u32 fh 800: ht divisor 1
 filter parent 1: protocol ip pref 2 u32 fh 800::800 order 2048 key ht 800 bkt 0 flowid 1:2
   match 00000000/00000000 at 12"""),
             [
-                {'flowid': '1:3', 'network': '192.168.0.10/32', 'port': 8080},
-                {'flowid': '1:2', 'network': '0.0.0.0/0', 'port': None},
+                {
+                    'flowid': '1:3', 'network': '192.168.0.10/32',
+                    'protocol': 'ip', 'port': 8080,
+                },
+                {
+                    'flowid': '1:2', 'network': '0.0.0.0/0',
+                    'protocol': None, 'port': None,
+                },
             ],
         ],
         [
             six.b("""filter parent 1f1c: protocol ip pref 1 fw
 filter parent 1f1c: protocol ip pref 1 fw handle 0x65 classid 1f1c:1"""),
             [
                 {'classid': '1f1c:1', 'handle': 101},
             ],
         ],
     ])
-    def test_normal(self, filter_parser, value, expected):
-        actual = filter_parser.parse_filter(value)
+    def test_normal(self, filter_parser_ipv4, value, expected):
+        actual = filter_parser_ipv4.parse_filter(value)
+
+        print("[expected]\n{}".format(expected))
+        print("\n[actual]\n{}".format(actual))
+
+        assert actual == expected
+
+
+class Test_TcFilterParser_parse_filter_ipv6(object):
+
+    @pytest.mark.parametrize(["value", "expected"], [
+        [None, []],
+        ["", []],
+        [
+            six.b("""filter parent 1f87: protocol ipv6 pref 1 u32
+filter parent 1f87: protocol ipv6 pref 1 u32 fh 800: ht divisor 1
+filter parent 1f87: protocol ipv6 pref 1 u32 fh 800::800 order 2048 key ht 800 bkt 0 flowid 1f87:2
+  match 00000000/ffffffff at 24
+  match 00000000/ffffffff at 28
+  match 00000000/ffffffff at 32
+  match 00000001/ffffffff at 36"""),
+            [
+                {
+                    'flowid': '1f87:2', 'network': '::1/128',
+                    'protocol': 'ipv6', 'port': None,
+                },
+            ]
+        ],
+        [
+            six.b("""filter parent 1f87: protocol ipv6 pref 1 u32
+filter parent 1f87: protocol ipv6 pref 1 u32 fh 800: ht divisor 1
+filter parent 1f87: protocol ipv6 pref 1 u32 fh 800::800 order 2048 key ht 800 bkt 0 flowid 1f87:2
+  match 2001db00/ffffffff at 8
+  match 00000000/ffffffff at 12
+  match 00000000/ffffffff at 16
+  match 00000001/ffffffff at 20"""),
+            [
+                {
+                    'flowid': '1f87:2', 'protocol': 'ipv6',
+                    'network': '2001:db00::1/128', 'port': None
+                }
+            ]
+        ],
+        [
+            six.b("""[/home/GitHubDesktop/tcconfig]# tc filter show dev ens33
+filter parent 1f87: protocol ipv6 pref 1 u32
+filter parent 1f87: protocol ipv6 pref 1 u32 fh 800: ht divisor 1
+filter parent 1f87: protocol ipv6 pref 1 u32 fh 800::800 order 2048 key ht 800 bkt 0 flowid 1f87:2
+  match 2001db00/ffffff00 at 24
+filter parent 1f87: protocol ipv6 pref 1 u32 fh 800::801 order 2049 key ht 800 bkt 0 flowid 1f87:3
+  match 2001db00/ffffffff at 24
+  match 00000000/ffffffff at 28
+  match 00000000/ffffffff at 32
+  match 00000001/ffffffff at 36
+filter parent 1f87: protocol ipv6 pref 1 u32 fh 800::802 order 2050 key ht 800 bkt 0 flowid 1f87:4
+  match 00001f90/0000ffff at 40"""),
+            [
+                {
+                    'flowid': '1f87:2', 'protocol': 'ipv6',
+                    'network': '2001:db00::/24', 'port': None
+                },
+                {
+                    'flowid': '1f87:3', 'protocol': None,
+                    'network': '2001:db00::1/128', 'port': None
+                },
+                {
+                    'flowid': '1f87:4', 'protocol': None,
+                    'network': None, 'port': 8080
+                },
+            ]
+        ],
+    ])
+    def test_normal(self, filter_parser_ipv6, value, expected):
+        actual = filter_parser_ipv6.parse_filter(value)
 
         print("[expected]\n{}".format(expected))
         print("\n[actual]\n{}".format(actual))
 
         assert actual == expected
 
 
@@ -109,16 +205,16 @@
 filter parent ffff: protocol ip pref 49152 u32 fh 800::800 order 2048 key ht 800 bkt 0 flowid 1:
   match 00000000/00000000 at 0
         action order 1: mirred (Egress Redirect to device ifb0) stolen
         index 3795 ref 1 bind 1"""),
             "ifb0",
         ],
     ])
-    def test_normal(self, filter_parser, value, expected):
-        assert filter_parser.parse_incoming_device(value) == expected
+    def test_normal(self, filter_parser_ipv4, value, expected):
+        assert filter_parser_ipv4.parse_incoming_device(value) == expected
 
 
 class Test_TcQdiscParser_parse(object):
 
     @pytest.mark.parametrize(["value", "expected"], [
         [
             six.b("""qdisc htb 1f87: root refcnt 2 r2q 10 default 1 direct_packets_stat 1 direct_qlen 1000
```

### Comparing `tcconfig-0.8.0/test/test_split_line_list.py` & `tcconfig-0.9.0/test/test_split_line_list.py`

 * *Files identical despite different names*

### Comparing `tcconfig-0.8.0/test/test_tcconfig.py` & `tcconfig-0.9.0/test/test_tcconfig.py`

 * *Files identical despite different names*

### Comparing `tcconfig-0.8.0/test/test_tcset_config_file.py` & `tcconfig-0.9.0/test/test_tcset_config_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,51 +16,52 @@
 def device_value(request):
     return request.config.getoption("--device")
 
 
 class Test_tcconfig(object):
 
     @pytest.mark.xfail
-    @pytest.mark.parametrize(["overwrite", "expected"], [
-        ["", 0],
-        ["--overwrite", 0],
+    @pytest.mark.parametrize(["overwrite"], [
+        [""],
+        ["--overwrite"],
     ])
-    def test_config_file(self, tmpdir, device_value, overwrite, expected):
+    def test_config_file_smoke(self, tmpdir, device_value, overwrite):
         if device_value is None:
             pytest.skip("device option is null")
 
         p = tmpdir.join("tcconfig.json")
         config = "{" + '"{:s}"'.format(device_value) + ": {" + """
         "outgoing": {
-            "network=192.168.0.10/32, port=8080": {
+            "network=192.168.0.10/32, port=8080, protocol=ip": {
                 "delay": "10.0",
                 "loss": "0.01",
                 "rate": "250K",
                 "delay-distro": "2.0"
             }
         },
         "incoming": {
-            "network=192.168.10.0/24": {
+            "network=192.168.10.0/24, protocol=ip": {
                 "corrupt": "0.02",
                 "rate": "1500K"
             }
         }
     }
 }
 """
         p.write(config)
 
         device_option = "--device {:s}".format(device_value)
 
         SubprocessRunner("tcdel {:s}".format(device_option)).run()
         command = " ".join(["tcset -f ", str(p), overwrite])
-        assert SubprocessRunner(command).run() == expected
+        SubprocessRunner(command).run()
 
         runner = SubprocessRunner("tcshow {:s}".format(device_option))
         runner.run()
 
-        print("[expected]\n{}".format(config))
-        print("\n[actual]\n{}".format(runner.stdout))
+        print("[expected]\n{}\n".format(config))
+        print("[actual]\n{}\n".format(runner.stdout))
+        print("[stderr]\n{}".format(runner.stderr))
 
         assert json.loads(runner.stdout) == json.loads(config)
 
         SubprocessRunner("tcdel {:s}".format(device_option)).run()
```

### Comparing `tcconfig-0.8.0/test/test_tcset_one.py` & `tcconfig-0.9.0/test/test_tcset_one.py`

 * *Files identical despite different names*

### Comparing `tcconfig-0.8.0/test/test_tcset_two.py` & `tcconfig-0.9.0/test/test_tcset_two.py`

 * *Files identical despite different names*

### Comparing `tcconfig-0.8.0/test/test_tcshow.py` & `tcconfig-0.9.0/test/test_tcshow.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     """
     Tests in this class are not executable on CI services.
     Execute the following command at the local environment to running tests:
       python setup.py test --addopts "--runxfail --device=<test device>"
     """
 
     @pytest.mark.xfail
-    def test_normal(self, device_value):
+    def test_normal_ipv4(self, device_value):
         if device_value is None:
             pytest.skip("device option is null")
 
         device_option = "--device {:s}".format(device_value)
         tcdel_command = "tcdel {:s}".format(device_option)
 
         assert SubprocessRunner(" ".join([
@@ -79,35 +79,129 @@
         expected = "{" + '"{:s}"'.format(device_value) + ": {" + """
         "outgoing": {
             "network=192.168.1.0/24": {
                 "delay": "1.0",
                 "loss": "1",
                 "rate": "100M"
             },
-           "network=192.168.0.10/32, port=8080": {
+           "network=192.168.0.10/32, port=8080, protocol=ip": {
                 "delay": "10.0",
                 "loss": "0.01",
                 "rate": "248",
                 "delay-distro": "2.0"
             }
         },
         "incoming": {
             "network=192.168.11.0/24, port=80": {
                 "delay": "1.0",
                 "loss": "0.02",
                 "rate": "100K"
             },
-            "network=0.0.0.0/0": {
+            "network=0.0.0.0/0, protocol=ip": {
                 "delay": "10.0",
                 "delay-distro": "2.0",
                 "rate": "500K"
             }
         }
     }
 }"""
 
         print("[expected]\n{}".format(expected))
         print("[actual]\n{}".format(runner.stdout))
+
+        assert json.loads(runner.stdout) == json.loads(expected)
+
+        SubprocessRunner(tcdel_command).run()
+
+    @pytest.mark.xfail
+    def test_normal_ipv6(self, device_value):
+        if device_value is None:
+            pytest.skip("device option is null")
+
+        device_option = "--device {:s}".format(device_value)
+        tcdel_command = "tcdel {:s}".format(device_option)
+
+        assert SubprocessRunner(" ".join([
+            "tcset",
+            device_option,
+            "--delay", "10",
+            "--delay-distro", "2",
+            "--loss", "0.01",
+            "--rate", "0.25K",
+            "--network", "::1",
+            "--port", "8080",
+            "--overwrite",
+            "--ipv6",
+        ])).run() == 0
+
+        assert SubprocessRunner(" ".join([
+            "tcset",
+            device_option,
+            "--delay", "1",
+            "--loss", "1",
+            "--rate", "100M",
+            "--network", "2001:db00::0/24",
+            "--add",
+            "--ipv6",
+        ])).run() == 0
+
+        assert SubprocessRunner(" ".join([
+            "tcset",
+            device_option,
+            "--delay", "10",
+            "--delay-distro", "2",
+            "--rate", "500K",
+            "--direction", "incoming",
+            "--ipv6",
+        ])).run() == 0
+
+        assert SubprocessRunner(" ".join([
+            "tcset",
+            device_option,
+            "--delay", "1",
+            "--loss", "0.02",
+            "--rate", "0.1M",
+            "--network", "2001:db00::0/25",
+            "--port", "80",
+            "--direction", "incoming",
+            "--add",
+            "--ipv6",
+        ])).run() == 0
+
+        runner = SubprocessRunner("tcshow {:s} --ipv6".format(device_option))
+        runner.run()
+
+        expected = "{" + '"{:s}"'.format(device_value) + ": {" + """
+        "outgoing": {
+            "network=2001:db00::/24": {
+                "delay": "1.0",
+                "loss": "1",
+                "rate": "100M"
+            },
+            "network=::1/128, port=8080, protocol=ipv6": {
+                "delay": "10.0",
+                "loss": "0.01",
+                "rate": "248",
+                "delay-distro": "2.0"
+            }
+        },
+        "incoming": {
+            "network=2001:db00::/25, port=80": {
+                "delay": "1.0",
+                "loss": "0.02",
+                "rate": "100K"
+            },
+            "protocol=ipv6": {
+                "delay": "10.0",
+                "rate": "500K",
+                "delay-distro": "2.0"
+            }
+        }
+    }
+}"""
+
+        print("[expected]\n{}".format(expected))
+        print("[actual]\n{}".format(runner.stdout))
 
         assert json.loads(runner.stdout) == json.loads(expected)
 
         SubprocessRunner(tcdel_command).run()
```

### Comparing `tcconfig-0.8.0/LICENSE` & `tcconfig-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tcconfig-0.8.0/README.rst` & `tcconfig-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `tcconfig-0.8.0/setup.py` & `tcconfig-0.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 
 with open(os.path.join("docs", "pages", "introduction", "summary.txt")) as f:
     summary = f.read()
 
 with open(os.path.join(REQUIREMENT_DIR, "requirements.txt")) as f:
     install_requires = [line.strip() for line in f if line.strip()]
 
+if sys.version_info.major < 3 or sys.version_info.minor < 4:
+    install_requires.append("ipaddress")
+
 with open(os.path.join(REQUIREMENT_DIR, "test_requirements.txt")) as f:
     tests_require = [line.strip() for line in f if line.strip()]
 
 setuptools.setup(
     name="tcconfig",
     version=tcconfig.VERSION,
     author="Tsuyoshi Hombashi",
```

### Comparing `tcconfig-0.8.0/PKG-INFO` & `tcconfig-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tcconfig
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Simple tc command wrapper tool. Easy to set up traffic control of network bandwidth/latency/packet-loss to a network interface.
 
 Home-page: https://github.com/thombashi/tcconfig
 Author: Tsuyoshi Hombashi
 Author-email: gogogo.vm@gmail.com
 License: MIT License
 Description: tcconfig
```


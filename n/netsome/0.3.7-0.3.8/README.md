# Comparing `tmp/netsome-0.3.7.tar.gz` & `tmp/netsome-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsome-0.3.7.tar", max compression
+gzip compressed data, was "netsome-0.3.8.tar", max compression
```

## Comparing `netsome-0.3.7.tar` & `netsome-0.3.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1286 2024-04-11 18:59:46.819718 netsome-0.3.7/LICENSE
--rw-r--r--   0        0        0      355 2024-04-15 07:10:06.582777 netsome-0.3.7/README.md
--rw-r--r--   0        0        0        0 2024-04-11 18:59:46.820411 netsome-0.3.7/netsome/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 18:59:46.820647 netsome-0.3.7/netsome/_converters/__init__.py
--rw-r--r--   0        0        0      967 2024-04-27 12:52:19.064834 netsome-0.3.7/netsome/_converters/bgp.py
--rw-r--r--   0        0        0      343 2024-04-20 09:23:59.213195 netsome-0.3.7/netsome/_converters/ipv4.py
--rw-r--r--   0        0        0     1057 2024-04-27 12:48:27.358013 netsome-0.3.7/netsome/constants.py
--rw-r--r--   0        0        0      324 2024-04-29 13:55:02.391250 netsome-0.3.7/netsome/types/__init__.py
--rw-r--r--   0        0        0     2219 2024-04-20 09:23:59.214154 netsome-0.3.7/netsome/types/bgp.py
--rw-r--r--   0        0        0     6303 2024-04-29 13:54:24.615586 netsome-0.3.7/netsome/types/ipv4.py
--rw-r--r--   0        0        0     3212 2024-04-28 18:56:11.702930 netsome-0.3.7/netsome/types/mac.py
--rw-r--r--   0        0        0      906 2024-04-20 09:23:59.215917 netsome-0.3.7/netsome/types/vlans.py
--rw-r--r--   0        0        0        0 2024-04-11 18:59:46.824730 netsome-0.3.7/netsome/validators/__init__.py
--rw-r--r--   0        0        0     2016 2024-04-27 12:48:27.359049 netsome-0.3.7/netsome/validators/bgp.py
--rw-r--r--   0        0        0     2112 2024-04-20 09:23:59.217488 netsome-0.3.7/netsome/validators/ipv4.py
--rw-r--r--   0        0        0      512 2024-04-28 18:55:56.209709 netsome-0.3.7/netsome/validators/mac.py
--rw-r--r--   0        0        0      379 2024-04-27 12:48:27.359608 netsome-0.3.7/netsome/validators/vlans.py
--rw-r--r--   0        0        0     1234 2024-04-29 13:56:17.087594 netsome-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 netsome-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1286 2024-04-11 18:59:46.819718 netsome-0.3.8/LICENSE
+-rw-r--r--   0        0        0      355 2024-04-15 07:10:06.582777 netsome-0.3.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 18:59:46.820411 netsome-0.3.8/netsome/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:59:46.820647 netsome-0.3.8/netsome/_converters/__init__.py
+-rw-r--r--   0        0        0      967 2024-04-27 12:52:19.064834 netsome-0.3.8/netsome/_converters/bgp.py
+-rw-r--r--   0        0        0      343 2024-04-20 09:23:59.213195 netsome-0.3.8/netsome/_converters/ipv4.py
+-rw-r--r--   0        0        0     1057 2024-04-27 12:48:27.358013 netsome-0.3.8/netsome/constants.py
+-rw-r--r--   0        0        0      324 2024-04-30 07:23:29.209737 netsome-0.3.8/netsome/types/__init__.py
+-rw-r--r--   0        0        0     2349 2024-05-02 11:03:45.728278 netsome-0.3.8/netsome/types/bgp.py
+-rw-r--r--   0        0        0     6303 2024-05-02 11:03:00.066006 netsome-0.3.8/netsome/types/ipv4.py
+-rw-r--r--   0        0        0     3212 2024-04-28 18:56:11.702930 netsome-0.3.8/netsome/types/mac.py
+-rw-r--r--   0        0        0      906 2024-04-20 09:23:59.215917 netsome-0.3.8/netsome/types/vlans.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:59:46.824730 netsome-0.3.8/netsome/validators/__init__.py
+-rw-r--r--   0        0        0     2016 2024-04-27 12:48:27.359049 netsome-0.3.8/netsome/validators/bgp.py
+-rw-r--r--   0        0        0     2112 2024-04-20 09:23:59.217488 netsome-0.3.8/netsome/validators/ipv4.py
+-rw-r--r--   0        0        0      512 2024-04-28 18:55:56.209709 netsome-0.3.8/netsome/validators/mac.py
+-rw-r--r--   0        0        0      379 2024-04-27 12:48:27.359608 netsome-0.3.8/netsome/validators/vlans.py
+-rw-r--r--   0        0        0     1234 2024-05-02 11:04:09.228242 netsome-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 netsome-0.3.8/PKG-INFO
```

### Comparing `netsome-0.3.7/LICENSE` & `netsome-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `netsome-0.3.7/netsome/_converters/bgp.py` & `netsome-0.3.8/netsome/_converters/bgp.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.7/netsome/constants.py` & `netsome-0.3.8/netsome/constants.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.7/netsome/types/bgp.py` & `netsome-0.3.8/netsome/types/bgp.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,18 @@
     MAX = c.BGP.ASN_MAX
     ORDER_MAX = c.BGP.ASN_ORDER_MAX
 
     def __init__(self, number: int) -> None:
         valids.validate_asplain(number)
         self._number = number
 
+    @property
+    def number(self):
+        return self._number
+
     @classmethod
     def from_asdot(cls, string: str) -> "ASN":
         valids.validate_asdot(string)
         return cls(convs.asdot_to_asplain(string))
 
     @classmethod
     def from_asdotplus(cls, string: str) -> "ASN":
@@ -55,14 +59,18 @@
 
 
 class Community:
     def __init__(self, number: int) -> None:
         valids.validate_asplain(number)
         self._number = number
 
+    @property
+    def number(self):
+        return self._number
+
     @classmethod
     def from_str(cls, value: str) -> "Community":
         valids.validate_community(value)
         return cls(convs.community_to_asplain(value))
 
     def __eq__(self, other: t.Any) -> bool:
         return isinstance(other, self.__class__) and (self._number == other._number)
```

### Comparing `netsome-0.3.7/netsome/types/ipv4.py` & `netsome-0.3.8/netsome/types/ipv4.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.7/netsome/types/mac.py` & `netsome-0.3.8/netsome/types/mac.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.7/netsome/types/vlans.py` & `netsome-0.3.8/netsome/types/vlans.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.7/netsome/validators/bgp.py` & `netsome-0.3.8/netsome/validators/bgp.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.7/netsome/validators/ipv4.py` & `netsome-0.3.8/netsome/validators/ipv4.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.7/netsome/validators/mac.py` & `netsome-0.3.8/netsome/validators/mac.py`

 * *Files identical despite different names*

### Comparing `netsome-0.3.7/pyproject.toml` & `netsome-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ]
 description = "The one and only library to make your network code handsome"
 keywords = ["library", "network"]
 license = "X11 License Distribution Modification Variant"
 name = "netsome"
 readme = "README.md"
 repository = "https://github.com/kuderr/netsome"
-version = "0.3.7"
+version = "0.3.8"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
 poethepoet = "^0.25.0"
 pytest = "^8.1.1"
```

### Comparing `netsome-0.3.7/PKG-INFO` & `netsome-0.3.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsome
-Version: 0.3.7
+Version: 0.3.8
 Summary: The one and only library to make your network code handsome
 Home-page: https://github.com/kuderr/netsome
 License: X11-distribute-modifications-variant
 Keywords: library,network
 Author: kuderr
 Author-email: dakudryavcev@gmail.com
 Requires-Python: >=3.10,<4.0
```


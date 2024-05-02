# Comparing `tmp/SymLinkDB-0.4.8.tar.gz` & `tmp/SymLinkDB-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SymLinkDB-0.4.8.tar", last modified: Fri Apr 19 09:23:08 2024, max compression
+gzip compressed data, was "SymLinkDB-0.4.9.tar", last modified: Fri Apr 19 11:22:53 2024, max compression
```

## Comparing `SymLinkDB-0.4.8.tar` & `SymLinkDB-0.4.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 09:23:08.778354 SymLinkDB-0.4.8/
--rw-rw-rw-   0        0        0    36975 2024-04-19 09:23:08.777322 SymLinkDB-0.4.8/PKG-INFO
--rw-rw-rw-   0        0        0    30649 2024-03-26 07:32:05.000000 SymLinkDB-0.4.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 09:23:08.754661 SymLinkDB-0.4.8/SymLinkDB/
--rw-rw-rw-   0        0        0    47762 2024-04-19 09:18:37.000000 SymLinkDB-0.4.8/SymLinkDB/__init__.py
--rw-rw-rw-   0        0        0     2374 2024-02-06 06:01:21.000000 SymLinkDB-0.4.8/SymLinkDB/document_code.py
-drwxrwxrwx   0        0        0        0 2024-04-19 09:23:08.740136 SymLinkDB-0.4.8/SymLinkDB/parts/
-drwxrwxrwx   0        0        0        0 2024-04-19 09:23:08.772308 SymLinkDB-0.4.8/SymLinkDB/parts/cfd_backend/
--rw-rw-rw-   0        0        0     3680 2024-04-19 09:20:12.000000 SymLinkDB-0.4.8/SymLinkDB/parts/cfd_backend/__init__.py
--rw-rw-rw-   0        0        0      799 2024-03-26 07:32:05.000000 SymLinkDB-0.4.8/SymLinkDB/parts/cfd_backend/test.py
-drwxrwxrwx   0        0        0        0 2024-04-19 09:23:08.775318 SymLinkDB-0.4.8/SymLinkDB/parts/memory_backend/
--rw-rw-rw-   0        0        0     2453 2024-03-03 05:14:03.000000 SymLinkDB-0.4.8/SymLinkDB/parts/memory_backend/__init__.py
--rw-rw-rw-   0        0        0      744 2024-02-06 06:01:21.000000 SymLinkDB-0.4.8/SymLinkDB/parts/memory_backend/test.py
--rw-rw-rw-   0        0        0    11537 2024-04-19 02:36:35.000000 SymLinkDB-0.4.8/SymLinkDB/test.py
-drwxrwxrwx   0        0        0        0 2024-04-19 09:23:08.769708 SymLinkDB-0.4.8/SymLinkDB.egg-info/
--rw-rw-rw-   0        0        0    36975 2024-04-19 09:23:08.000000 SymLinkDB-0.4.8/SymLinkDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2024-04-19 09:23:08.000000 SymLinkDB-0.4.8/SymLinkDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 09:23:08.000000 SymLinkDB-0.4.8/SymLinkDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2024-04-19 09:23:08.000000 SymLinkDB-0.4.8/SymLinkDB.egg-info/requires.txt
--rw-rw-rw-   0        0        0       69 2024-04-19 09:23:08.000000 SymLinkDB-0.4.8/SymLinkDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 09:23:08.778354 SymLinkDB-0.4.8/setup.cfg
--rw-rw-rw-   0        0        0      893 2024-04-19 09:22:48.000000 SymLinkDB-0.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:22:53.834959 SymLinkDB-0.4.9/
+-rw-rw-rw-   0        0        0    36975 2024-04-19 11:22:53.834959 SymLinkDB-0.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0    30649 2024-03-26 07:32:05.000000 SymLinkDB-0.4.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 11:22:53.810827 SymLinkDB-0.4.9/SymLinkDB/
+-rw-rw-rw-   0        0        0    47762 2024-04-19 09:18:37.000000 SymLinkDB-0.4.9/SymLinkDB/__init__.py
+-rw-rw-rw-   0        0        0     2374 2024-02-06 06:01:21.000000 SymLinkDB-0.4.9/SymLinkDB/document_code.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:22:53.794553 SymLinkDB-0.4.9/SymLinkDB/parts/
+drwxrwxrwx   0        0        0        0 2024-04-19 11:22:53.834959 SymLinkDB-0.4.9/SymLinkDB/parts/cfd_backend/
+-rw-rw-rw-   0        0        0     3680 2024-04-19 09:46:57.000000 SymLinkDB-0.4.9/SymLinkDB/parts/cfd_backend/__init__.py
+-rw-rw-rw-   0        0        0      799 2024-03-26 07:32:05.000000 SymLinkDB-0.4.9/SymLinkDB/parts/cfd_backend/test.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:22:53.834959 SymLinkDB-0.4.9/SymLinkDB/parts/memory_backend/
+-rw-rw-rw-   0        0        0     2453 2024-03-03 05:14:03.000000 SymLinkDB-0.4.9/SymLinkDB/parts/memory_backend/__init__.py
+-rw-rw-rw-   0        0        0      744 2024-02-06 06:01:21.000000 SymLinkDB-0.4.9/SymLinkDB/parts/memory_backend/test.py
+-rw-rw-rw-   0        0        0    11537 2024-04-19 02:36:35.000000 SymLinkDB-0.4.9/SymLinkDB/test.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:22:53.826949 SymLinkDB-0.4.9/SymLinkDB.egg-info/
+-rw-rw-rw-   0        0        0    36975 2024-04-19 11:22:53.000000 SymLinkDB-0.4.9/SymLinkDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2024-04-19 11:22:53.000000 SymLinkDB-0.4.9/SymLinkDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 11:22:53.000000 SymLinkDB-0.4.9/SymLinkDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2024-04-19 11:22:53.000000 SymLinkDB-0.4.9/SymLinkDB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       69 2024-04-19 11:22:53.000000 SymLinkDB-0.4.9/SymLinkDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 11:22:53.834959 SymLinkDB-0.4.9/setup.cfg
+-rw-rw-rw-   0        0        0      893 2024-04-19 11:22:49.000000 SymLinkDB-0.4.9/setup.py
```

### Comparing `SymLinkDB-0.4.8/PKG-INFO` & `SymLinkDB-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SymLinkDB
-Version: 0.4.8
+Version: 0.4.9
 Summary: A graph database characterized by bidirectional links. It allows for intuitive design of data relationships.
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: - The explanations in English, Simplified Chinese, and Spanish are provided below.
         - 下面提供了英语、简体中文和西班牙语的说明。
```

### Comparing `SymLinkDB-0.4.8/README.md` & `SymLinkDB-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.8/SymLinkDB/__init__.py` & `SymLinkDB-0.4.9/SymLinkDB/__init__.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.8/SymLinkDB/document_code.py` & `SymLinkDB-0.4.9/SymLinkDB/document_code.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.8/SymLinkDB/parts/cfd_backend/__init__.py` & `SymLinkDB-0.4.9/SymLinkDB/parts/cfd_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.8/SymLinkDB/parts/cfd_backend/test.py` & `SymLinkDB-0.4.9/SymLinkDB/parts/cfd_backend/test.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.8/SymLinkDB/parts/memory_backend/__init__.py` & `SymLinkDB-0.4.9/SymLinkDB/parts/memory_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.8/SymLinkDB/parts/memory_backend/test.py` & `SymLinkDB-0.4.9/SymLinkDB/parts/memory_backend/test.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.8/SymLinkDB/test.py` & `SymLinkDB-0.4.9/SymLinkDB/test.py`

 * *Files identical despite different names*

### Comparing `SymLinkDB-0.4.8/SymLinkDB.egg-info/PKG-INFO` & `SymLinkDB-0.4.9/SymLinkDB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SymLinkDB
-Version: 0.4.8
+Version: 0.4.9
 Summary: A graph database characterized by bidirectional links. It allows for intuitive design of data relationships.
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: - The explanations in English, Simplified Chinese, and Spanish are provided below.
         - 下面提供了英语、简体中文和西班牙语的说明。
```

### Comparing `SymLinkDB-0.4.8/setup.py` & `SymLinkDB-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 00000080: 205b 657a 7069 705d 0d0a 7769 7468 2065   [ezpip]..with e
 00000090: 7a70 6970 2e70 6163 6b61 6765 7228 6465  zpip.packager(de
 000000a0: 7665 6c6f 705f 6469 7220 3d20 222e 2f5f  velop_dir = "./_
 000000b0: 6465 7665 6c6f 705f 5379 6d4c 696e 6b44  develop_SymLinkD
 000000c0: 422f 2229 2061 7320 703a 0d0a 0973 6574  B/") as p:...set
 000000d0: 7570 280d 0a09 096e 616d 6520 3d20 2253  up(....name = "S
 000000e0: 796d 4c69 6e6b 4442 222c 0d0a 0909 7665  ymLinkDB",....ve
-000000f0: 7273 696f 6e20 3d20 2230 2e34 2e38 222c  rsion = "0.4.8",
+000000f0: 7273 696f 6e20 3d20 2230 2e34 2e39 222c  rsion = "0.4.9",
 00000100: 0d0a 0909 6465 7363 7269 7074 696f 6e20  ....description 
 00000110: 3d20 2241 2067 7261 7068 2064 6174 6162  = "A graph datab
 00000120: 6173 6520 6368 6172 6163 7465 7269 7a65  ase characterize
 00000130: 6420 6279 2062 6964 6972 6563 7469 6f6e  d by bidirection
 00000140: 616c 206c 696e 6b73 2e20 4974 2061 6c6c  al links. It all
 00000150: 6f77 7320 666f 7220 696e 7475 6974 6976  ows for intuitiv
 00000160: 6520 6465 7369 676e 206f 6620 6461 7461  e design of data
@@ -33,15 +33,15 @@
 00000200: 732c 0d0a 0909 696e 7374 616c 6c5f 7265  s,....install_re
 00000210: 7175 6972 6573 203d 205b 2265 7a70 6970  quires = ["ezpip
 00000220: 222c 2022 736f 7574 3e3d 312e 322e 3122  ", "sout>=1.2.1"
 00000230: 2c20 2272 656c 7061 7468 222c 2022 736c  , "relpath", "sl
 00000240: 696d 2d69 643e 3d30 2e30 2e32 222c 2022  im-id>=0.0.2", "
 00000250: 6669 6573 3e3d 312e 342e 3022 2c20 2243  fies>=1.4.0", "C
 00000260: 6163 6865 6446 696c 6544 6963 3e3d 302e  achedFileDic>=0.
-00000270: 322e 3122 5d2c 0d0a 0909 6c6f 6e67 5f64  2.1"],....long_d
+00000270: 322e 3222 5d2c 0d0a 0909 6c6f 6e67 5f64  2.2"],....long_d
 00000280: 6573 6372 6970 7469 6f6e 203d 2070 2e6c  escription = p.l
 00000290: 6f6e 675f 6465 7363 7269 7074 696f 6e2c  ong_description,
 000002a0: 0d0a 0909 6c6f 6e67 5f64 6573 6372 6970  ....long_descrip
 000002b0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
 000002c0: 6520 3d20 2274 6578 742f 6d61 726b 646f  e = "text/markdo
 000002d0: 776e 222c 0d0a 0909 6c69 6365 6e73 6520  wn",....license 
 000002e0: 3d20 2243 4330 2076 312e 3022 2c0d 0a09  = "CC0 v1.0",...
```


# Comparing `tmp/itwingstestsprojectnn-0.3.tar.gz` & `tmp/itwingstestsprojectnn-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itwingstestsprojectnn-0.3.tar", last modified: Thu May  2 13:03:42 2024, max compression
+gzip compressed data, was "itwingstestsprojectnn-0.4.tar", last modified: Thu May  2 15:21:15 2024, max compression
```

## Comparing `itwingstestsprojectnn-0.3.tar` & `itwingstestsprojectnn-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 13:03:42.943703 itwingstestsprojectnn-0.3/
--rw-rw-rw-   0        0        0        0 2021-07-31 02:25:56.000000 itwingstestsprojectnn-0.3/LICENSE
--rw-rw-rw-   0        0        0      393 2024-05-02 13:03:42.943703 itwingstestsprojectnn-0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-02 11:00:34.000000 itwingstestsprojectnn-0.3/README.md
--rw-rw-rw-   0        0        0      103 2021-07-31 02:25:56.000000 itwingstestsprojectnn-0.3/pyproject.toml
--rw-rw-rw-   0        0        0      533 2024-05-02 13:03:42.949709 itwingstestsprojectnn-0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-02 13:03:42.885744 itwingstestsprojectnn-0.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-02 13:03:42.942703 itwingstestsprojectnn-0.3/src/itwingstestsprojectnn.egg-info/
--rw-rw-rw-   0        0        0      393 2024-05-02 13:03:42.000000 itwingstestsprojectnn-0.3/src/itwingstestsprojectnn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2024-05-02 13:03:42.000000 itwingstestsprojectnn-0.3/src/itwingstestsprojectnn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 13:03:42.000000 itwingstestsprojectnn-0.3/src/itwingstestsprojectnn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-02 13:03:42.000000 itwingstestsprojectnn-0.3/src/itwingstestsprojectnn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-02 13:03:42.939705 itwingstestsprojectnn-0.3/src/mymodule/
--rw-rw-rw-   0        0        0        0 2024-05-02 06:46:40.000000 itwingstestsprojectnn-0.3/src/mymodule/__init__.py
--rw-rw-rw-   0        0        0     4347 2024-05-02 08:29:07.000000 itwingstestsprojectnn-0.3/src/mymodule/config.py
--rw-rw-rw-   0        0        0     3775 2024-05-02 13:02:56.000000 itwingstestsprojectnn-0.3/src/mymodule/main.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:21:15.635196 itwingstestsprojectnn-0.4/
+-rw-rw-rw-   0        0        0        0 2021-07-31 02:25:56.000000 itwingstestsprojectnn-0.4/LICENSE
+-rw-rw-rw-   0        0        0      393 2024-05-02 15:21:15.635196 itwingstestsprojectnn-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-02 11:00:34.000000 itwingstestsprojectnn-0.4/README.md
+-rw-rw-rw-   0        0        0      103 2021-07-31 02:25:56.000000 itwingstestsprojectnn-0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      533 2024-05-02 15:21:15.648191 itwingstestsprojectnn-0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-02 15:21:15.515264 itwingstestsprojectnn-0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-02 15:21:15.634195 itwingstestsprojectnn-0.4/src/itwingstestsprojectnn.egg-info/
+-rw-rw-rw-   0        0        0      393 2024-05-02 15:21:15.000000 itwingstestsprojectnn-0.4/src/itwingstestsprojectnn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2024-05-02 15:21:15.000000 itwingstestsprojectnn-0.4/src/itwingstestsprojectnn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 15:21:15.000000 itwingstestsprojectnn-0.4/src/itwingstestsprojectnn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 15:21:15.000000 itwingstestsprojectnn-0.4/src/itwingstestsprojectnn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 15:21:15.623204 itwingstestsprojectnn-0.4/src/mymodule/
+-rw-rw-rw-   0        0        0        0 2024-05-02 06:46:40.000000 itwingstestsprojectnn-0.4/src/mymodule/__init__.py
+-rw-rw-rw-   0        0        0     4347 2024-05-02 08:29:07.000000 itwingstestsprojectnn-0.4/src/mymodule/config.py
+-rw-rw-rw-   0        0        0     8792 2024-05-02 15:20:48.000000 itwingstestsprojectnn-0.4/src/mymodule/main.py
```

### Comparing `itwingstestsprojectnn-0.3/setup.cfg` & `itwingstestsprojectnn-0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 7477 696e 6773 7465 7374 7370   = itwingstestsp
 00000020: 726f 6a65 6374 6e6e 0d0a 7665 7273 696f  rojectnn..versio
-00000030: 6e20 3d20 302e 330d 0a61 7574 686f 7220  n = 0.3..author 
+00000030: 6e20 3d20 302e 340d 0a61 7574 686f 7220  n = 0.4..author 
 00000040: 3d20 4d61 7961 6e6b 0d0a 6175 7468 6f72  = Mayank..author
 00000050: 5f65 6d61 696c 203d 206d 6179 616e 6b74  _email = mayankt
 00000060: 696d 6261 6469 6140 676d 6169 6c2e 636f  imbadia@gmail.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2041 2073 6d61 6c6c 2065 7861 6d70 6c65   A small example
 00000090: 2070 6163 6b61 6765 0d0a 6c6f 6e67 5f64   package..long_d
 000000a0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
```

### Comparing `itwingstestsprojectnn-0.3/src/mymodule/config.py` & `itwingstestsprojectnn-0.4/src/mymodule/config.py`

 * *Files identical despite different names*


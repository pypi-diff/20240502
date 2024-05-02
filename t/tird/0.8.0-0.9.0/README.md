# Comparing `tmp/tird-0.8.0.tar.gz` & `tmp/tird-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tird-0.8.0.tar", last modified: Mon Feb 26 14:04:36 2024, max compression
+gzip compressed data, was "tird-0.9.0.tar", last modified: Wed Mar 27 15:35:33 2024, max compression
```

## Comparing `tird-0.8.0.tar` & `tird-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-26 14:04:36.492523 tird-0.8.0/
--rw-r--r--   0 user      (1000) user      (1000)     7152 2024-02-26 14:04:36.492523 tird-0.8.0/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     5174 2024-02-26 14:03:59.000000 tird-0.8.0/README.md
--rw-r--r--   0 user      (1000) user      (1000)       38 2024-02-26 14:04:36.492523 tird-0.8.0/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     1472 2024-02-25 09:30:19.000000 tird-0.8.0/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-26 14:04:36.488523 tird-0.8.0/tird/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-03-21 16:33:02.000000 tird-0.8.0/tird/__init__.py
--rwxr-xr-x   0 user      (1000) user      (1000)    54966 2024-02-25 13:19:09.000000 tird-0.8.0/tird/tird.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-26 14:04:36.492523 tird-0.8.0/tird.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     7152 2024-02-26 14:04:36.000000 tird-0.8.0/tird.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      218 2024-02-26 14:04:36.000000 tird-0.8.0/tird.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2024-02-26 14:04:36.000000 tird-0.8.0/tird.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       41 2024-02-26 14:04:36.000000 tird-0.8.0/tird.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)       35 2024-02-26 14:04:36.000000 tird-0.8.0/tird.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        5 2024-02-26 14:04:36.000000 tird-0.8.0/tird.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-03-27 15:35:33.013051 tird-0.9.0/
+-rw-r--r--   0 user      (1000) user      (1000)     7002 2024-03-27 15:35:33.009051 tird-0.9.0/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     5040 2024-03-27 15:34:41.000000 tird-0.9.0/README.md
+-rw-r--r--   0 user      (1000) user      (1000)       38 2024-03-27 15:35:33.013051 tird-0.9.0/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     1472 2024-03-27 15:20:56.000000 tird-0.9.0/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-03-27 15:35:33.009051 tird-0.9.0/tird/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-03-21 16:33:02.000000 tird-0.9.0/tird/__init__.py
+-rwxr-xr-x   0 user      (1000) user      (1000)    55527 2024-03-27 15:20:56.000000 tird-0.9.0/tird/tird.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-03-27 15:35:33.009051 tird-0.9.0/tird.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     7002 2024-03-27 15:35:32.000000 tird-0.9.0/tird.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      218 2024-03-27 15:35:32.000000 tird-0.9.0/tird.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-03-27 15:35:32.000000 tird-0.9.0/tird.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       41 2024-03-27 15:35:32.000000 tird-0.9.0/tird.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)       35 2024-03-27 15:35:32.000000 tird-0.9.0/tird.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        5 2024-03-27 15:35:32.000000 tird-0.9.0/tird.egg-info/top_level.txt
```

### Comparing `tird-0.8.0/PKG-INFO` & `tird-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tird
-Version: 0.8.0
+Version: 0.9.0
 Summary: A tool for writing random bytes, encrypting file contents, and hiding encrypted data
 Home-page: https://github.com/hakavlad/tird
 Author: Alexey Avramov
 Author-email: hakavlad@gmail.com
 License: CC0
 Project-URL: Homepage, https://github.com/hakavlad/tird
 Project-URL: Bug Tracker, https://github.com/hakavlad/tird/issues
@@ -13,16 +13,14 @@
         
         # tird
         
         `tird` *(an acronym for "this is random data")* is a tool for writing random bytes, encrypting file contents, and hiding encrypted data.
         
         `tird` can create files with random data, overwrite file contents with random data, encrypt file contents and comments, hide encrypted data among random data, minimize metadata leakage, and can provide some forms of [plausible deniability](https://en.wikipedia.org/wiki/Plausible_deniability#Use_in_cryptography).
         
-        `tird` aims to provide a stable encryption format for long-term data storage using modern and standardized cryptographic primitives.
-        
         ![screenshot: MENU](https://i.imgur.com/cZX73zg.png)
         
         ## Goals
         
         - Providing protection for individual files, including:
           - symmetric encryption;
           - reducing metadata leakage;
```

### Comparing `tird-0.8.0/README.md` & `tird-0.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 # tird
 
 `tird` *(an acronym for "this is random data")* is a tool for writing random bytes, encrypting file contents, and hiding encrypted data.
 
 `tird` can create files with random data, overwrite file contents with random data, encrypt file contents and comments, hide encrypted data among random data, minimize metadata leakage, and can provide some forms of [plausible deniability](https://en.wikipedia.org/wiki/Plausible_deniability#Use_in_cryptography).
 
-`tird` aims to provide a stable encryption format for long-term data storage using modern and standardized cryptographic primitives.
-
 ![screenshot: MENU](https://i.imgur.com/cZX73zg.png)
 
 ## Goals
 
 - Providing protection for individual files, including:
   - symmetric encryption;
   - reducing metadata leakage;
```

### Comparing `tird-0.8.0/setup.py` & `tird-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
     with open('README.md', 'r') as file:
         return file.read()
 
 
 NAME = 'tird'
-VERSION = '0.8.0'
+VERSION = '0.9.0'
 
 setup(
     name=NAME,
     version=VERSION,
     license='CC0',
     author='Alexey Avramov',
     author_email='hakavlad@gmail.com',
```

### Comparing `tird-0.8.0/tird/tird.py` & `tird-0.9.0/tird/tird.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,17 @@
         print(f'{ERR}E: {e}{RES}')
         return None
 
 
 def seek_pos(f: Any, offset: int, whence: int = 0) -> bool:
     """
     """
+    if DEBUG:
+        print(f'{ITA}D: move to position {offset} in {f}{RES}')
+
     try:
         f.seek(offset, whence)
         return True
     except OSError as e:
         print(f'{ERR}E: {e}{RES}')
         return False
 
@@ -676,15 +679,15 @@
         cur_pos: int = iod['i'].tell()
 
         if action == 3:
             new_pos: int = i_size - SALTS_HALF_SIZE
         else:  # 7
             new_pos = final_pos - SALTS_HALF_SIZE
 
-        # jump to the beginning of footer_salt
+        # move to the beginning of footer_salt
         if not seek_pos(iod['i'], new_pos):
             return False
 
         if DEBUG:
             print(f'{ITA}D: current position: before footer_salt{RES}')
             print_positions()
 
@@ -1148,17 +1151,21 @@
               f'{round(written_sum / data_size * 100, 1)}% in '
               f'{round(t, 1)}s{RES}')
 
 
 def print_positions() -> None:
     """
     """
-    i: int = iod['i'].tell()
     o: int = iod['o'].tell()
-    print(f'{ITA}D: current pointer positions: if={i}, of={o}{RES}')
+
+    if 'i' in iod:
+        i: int = iod['i'].tell()
+        print(f'{ITA}D: current positions: if={i}, of={o}{RES}')
+    else:
+        print(f'{ITA}D: current position: of={o}{RES}')
 
 
 # #############################################################################
 
 
 def cryptoembed(action: int) -> bool:
     """
@@ -1713,18 +1720,29 @@
 
     return ok
 
 
 def embed_processor(action: int, init_pos: int, message_size: int) -> bool:
     """
     """
-    print(f'{ITA}I: reading, writing...{RES}')
+    if DEBUG:
+        print_positions()
 
-    if not seek_pos(iod['o'], init_pos):
-        return False
+    # seek init_pos in the container
+    if action == 4:
+        if not seek_pos(iod['o'], init_pos):
+            return False
+    else:  # 5
+        if not seek_pos(iod['i'], init_pos):
+            return False
+
+    if DEBUG:
+        print_positions()
+
+    print(f'{ITA}I: reading, writing...{RES}')
 
     ho: Any = blake2b(digest_size=EMBED_DIGEST_SIZE)
 
     t_start: float = monotonic()
     t_last_print: float = t_start
 
     w_sum: int = 0
@@ -1758,14 +1776,17 @@
         if not write_data(i_data):
             return False
 
         ho.update(i_data)
 
         w_sum += len(i_data)
 
+    if DEBUG:
+        print_positions()
+
     progress(w_sum, message_size, t_start)
 
     if action == 4:
         print(f'{ITA}I: fsyncing...{RES}')
         t0: float = monotonic()
 
         if not fsync_data():
@@ -1890,17 +1911,23 @@
 
     return ok
 
 
 def wiper_processor(init_pos: int, data_size: int) -> bool:
     """
     """
+    if DEBUG:
+        print_positions()
+
     if not seek_pos(iod['o'], init_pos):
         return False
 
+    if DEBUG:
+        print_positions()
+
     print(f'{ITA}I: writing...{RES}')
 
     t_start: float = monotonic()
     t_last_print: float = t_start
 
     w_sum: int = 0
 
@@ -1923,14 +1950,17 @@
         chunk = urandom(rem_size)
 
         if not write_data(chunk):
             return False
 
         w_sum += len(chunk)
 
+    if DEBUG:
+        print_positions()
+
     progress(w_sum, data_size, t_start)
 
     print(f'{ITA}I: fsyncing...{RES}')
     t0: float = monotonic()
 
     if not fsync_data():
         return False
@@ -2028,15 +2058,15 @@
 elif argv[1:] == ['-d'] or argv[1:] == ['--debug']:
     DEBUG = True
 else:
     print(f'{ERR}E: invalid command line options: {argv[1:]}{RES}')
     exit(1)
 
 
-VERSION: str = '0.8.0'
+VERSION: str = '0.9.0'
 
 INFO: str = f"""{ITA}I: tird v{VERSION}
     A tool for writing random bytes,
     encrypting file contents,
     and hiding encrypted data.
     Homepage: https://github.com/hakavlad/tird{RES}"""
```

### Comparing `tird-0.8.0/tird.egg-info/PKG-INFO` & `tird-0.9.0/tird.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tird
-Version: 0.8.0
+Version: 0.9.0
 Summary: A tool for writing random bytes, encrypting file contents, and hiding encrypted data
 Home-page: https://github.com/hakavlad/tird
 Author: Alexey Avramov
 Author-email: hakavlad@gmail.com
 License: CC0
 Project-URL: Homepage, https://github.com/hakavlad/tird
 Project-URL: Bug Tracker, https://github.com/hakavlad/tird/issues
@@ -13,16 +13,14 @@
         
         # tird
         
         `tird` *(an acronym for "this is random data")* is a tool for writing random bytes, encrypting file contents, and hiding encrypted data.
         
         `tird` can create files with random data, overwrite file contents with random data, encrypt file contents and comments, hide encrypted data among random data, minimize metadata leakage, and can provide some forms of [plausible deniability](https://en.wikipedia.org/wiki/Plausible_deniability#Use_in_cryptography).
         
-        `tird` aims to provide a stable encryption format for long-term data storage using modern and standardized cryptographic primitives.
-        
         ![screenshot: MENU](https://i.imgur.com/cZX73zg.png)
         
         ## Goals
         
         - Providing protection for individual files, including:
           - symmetric encryption;
           - reducing metadata leakage;
```


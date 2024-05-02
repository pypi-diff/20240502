# Comparing `tmp/tdh-twitch-utils-1.7.1.tar.gz` & `tmp/tdh_twitch_utils-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdh-twitch-utils-1.7.1.tar", last modified: Mon Dec 25 01:12:08 2023, max compression
+gzip compressed data, was "tdh_twitch_utils-1.7.2.tar", last modified: Thu May  2 17:44:25 2024, max compression
```

## Comparing `tdh-twitch-utils-1.7.1.tar` & `tdh_twitch_utils-1.7.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 01:12:08.588222 tdh-twitch-utils-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35140 2023-12-25 01:11:54.000000 tdh-twitch-utils-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2023-12-25 01:12:08.588222 tdh-twitch-utils-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4920 2023-12-25 01:11:54.000000 tdh-twitch-utils-1.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-25 01:12:08.588222 tdh-twitch-utils-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-12-25 01:11:54.000000 tdh-twitch-utils-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 01:12:08.588222 tdh-twitch-utils-1.7.1/tdh_twitch_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2023-12-25 01:12:08.000000 tdh-twitch-utils-1.7.1/tdh_twitch_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      474 2023-12-25 01:12:08.000000 tdh-twitch-utils-1.7.1/tdh_twitch_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-25 01:12:08.000000 tdh-twitch-utils-1.7.1/tdh_twitch_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-25 01:12:08.000000 tdh-twitch-utils-1.7.1/tdh_twitch_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2023-12-25 01:12:08.000000 tdh-twitch-utils-1.7.1/tdh_twitch_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-25 01:12:08.000000 tdh-twitch-utils-1.7.1/tdh_twitch_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 01:12:08.588222 tdh-twitch-utils-1.7.1/twitch_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2023-12-25 01:11:54.000000 tdh-twitch-utils-1.7.1/twitch_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-25 01:11:54.000000 tdh-twitch-utils-1.7.1/twitch_utils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2023-12-25 01:11:54.000000 tdh-twitch-utils-1.7.1/twitch_utils/clip.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6464 2023-12-25 01:11:54.000000 tdh-twitch-utils-1.7.1/twitch_utils/concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2023-12-25 01:11:54.000000 tdh-twitch-utils-1.7.1/twitch_utils/mute.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6225 2023-12-25 01:11:54.000000 tdh-twitch-utils-1.7.1/twitch_utils/offset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12646 2023-12-25 01:11:54.000000 tdh-twitch-utils-1.7.1/twitch_utils/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2023-12-25 01:11:54.000000 tdh-twitch-utils-1.7.1/twitch_utils/twitch.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-25 01:11:54.000000 tdh-twitch-utils-1.7.1/twitch_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:44:25.607510 tdh_twitch_utils-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35140 2024-05-02 17:44:17.000000 tdh_twitch_utils-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-05-02 17:44:25.607510 tdh_twitch_utils-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-05-02 17:44:17.000000 tdh_twitch_utils-1.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 17:44:25.607510 tdh_twitch_utils-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-02 17:44:17.000000 tdh_twitch_utils-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:44:25.607510 tdh_twitch_utils-1.7.2/tdh_twitch_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-05-02 17:44:25.000000 tdh_twitch_utils-1.7.2/tdh_twitch_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-02 17:44:25.000000 tdh_twitch_utils-1.7.2/tdh_twitch_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:44:25.000000 tdh_twitch_utils-1.7.2/tdh_twitch_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-02 17:44:25.000000 tdh_twitch_utils-1.7.2/tdh_twitch_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-02 17:44:25.000000 tdh_twitch_utils-1.7.2/tdh_twitch_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 17:44:25.000000 tdh_twitch_utils-1.7.2/tdh_twitch_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:44:25.607510 tdh_twitch_utils-1.7.2/twitch_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-02 17:44:17.000000 tdh_twitch_utils-1.7.2/twitch_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-02 17:44:17.000000 tdh_twitch_utils-1.7.2/twitch_utils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-02 17:44:17.000000 tdh_twitch_utils-1.7.2/twitch_utils/clip.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6464 2024-05-02 17:44:17.000000 tdh_twitch_utils-1.7.2/twitch_utils/concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-02 17:44:17.000000 tdh_twitch_utils-1.7.2/twitch_utils/mute.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6225 2024-05-02 17:44:17.000000 tdh_twitch_utils-1.7.2/twitch_utils/offset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12646 2024-05-02 17:44:17.000000 tdh_twitch_utils-1.7.2/twitch_utils/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-05-02 17:44:17.000000 tdh_twitch_utils-1.7.2/twitch_utils/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-02 17:44:17.000000 tdh_twitch_utils-1.7.2/twitch_utils/utils.py
```

### Comparing `tdh-twitch-utils-1.7.1/LICENSE` & `tdh_twitch_utils-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tdh-twitch-utils-1.7.1/PKG-INFO` & `tdh_twitch_utils-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdh-twitch-utils
-Version: 1.7.1
+Version: 1.7.2
 Summary: Record, concatenate and synchronize Twitch live streams
 Home-page: https://github.com/TheDrHax/Twitch-Utils
 Author: Dmitry Karikh
 Author-email: the.dr.hax@gmail.com
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `tdh-twitch-utils-1.7.1/README.md` & `tdh_twitch_utils-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `tdh-twitch-utils-1.7.1/setup.py` & `tdh_twitch_utils-1.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 }
 
 EXTRAS['all'] = list(itertools.chain.from_iterable(EXTRAS.values()))
 
 
 setup(
     name='tdh-twitch-utils',
-    version='1.7.1',
+    version='1.7.2',
 
     author='Dmitry Karikh',
     author_email='the.dr.hax@gmail.com',
 
     description='Record, concatenate and synchronize Twitch live streams',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `tdh-twitch-utils-1.7.1/tdh_twitch_utils.egg-info/PKG-INFO` & `tdh_twitch_utils-1.7.2/tdh_twitch_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdh-twitch-utils
-Version: 1.7.1
+Version: 1.7.2
 Summary: Record, concatenate and synchronize Twitch live streams
 Home-page: https://github.com/TheDrHax/Twitch-Utils
 Author: Dmitry Karikh
 Author-email: the.dr.hax@gmail.com
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `tdh-twitch-utils-1.7.1/twitch_utils/__init__.py` & `tdh_twitch_utils-1.7.2/twitch_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tdh-twitch-utils-1.7.1/twitch_utils/clip.py` & `tdh_twitch_utils-1.7.2/twitch_utils/clip.py`

 * *Files identical despite different names*

### Comparing `tdh-twitch-utils-1.7.1/twitch_utils/concat.py` & `tdh_twitch_utils-1.7.2/twitch_utils/concat.py`

 * *Files identical despite different names*

### Comparing `tdh-twitch-utils-1.7.1/twitch_utils/mute.py` & `tdh_twitch_utils-1.7.2/twitch_utils/mute.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 The main purpose of this script is to remove automated Content-ID claims from
 the video on YouTube. YouTube displays exact time ranges for every claim.
 
 Timestamp format: [[HH:]MM:]SS[.MMM]
 Time range format: START~END
 
 Options:
-  -o <file>   Name of the output file.
-  --inverse   Remove voice instead of music.
-  --pass <n>  Number of passes for each time range. [default: 1]
+  -o <file>    Name of the output file.
+  --inverse    Remove voice instead of music.
+  --pass <n>   Number of passes for each time range. [default: 1]
+  --chunk <s>  Split ranges into smaller chunks (in seconds). [default: 300]
 """
 
 import os
 import sys
 
 from docopt import docopt
 from subprocess import run
@@ -46,23 +47,24 @@
     fi = Clip(args['<input>'])
     fo = args['-o']
     ranges = list(tuple(ptime(t) for t in range.split('~'))
                   for range in args['<range>'])
 
     loader = AudioAdapter.default()
     sample_rate = 44100
+    chunk_size = float(args['--chunk'])
     separator = Separator('spleeter:2stems')
 
     new_ranges = []
     for r in ranges:
         start, end = r
         
-        while end - start > 300:
-            new_ranges.append((start, start + 300))
-            start += 300
+        while end - start > chunk_size:
+            new_ranges.append((start, start + chunk_size))
+            start += chunk_size
         
         new_ranges.append((start, end))
 
     ranges = new_ranges
     segments = {}
 
     for start, end in ranges:
```

### Comparing `tdh-twitch-utils-1.7.1/twitch_utils/offset.py` & `tdh_twitch_utils-1.7.2/twitch_utils/offset.py`

 * *Files identical despite different names*

### Comparing `tdh-twitch-utils-1.7.1/twitch_utils/record.py` & `tdh_twitch_utils-1.7.2/twitch_utils/record.py`

 * *Files identical despite different names*

### Comparing `tdh-twitch-utils-1.7.1/twitch_utils/twitch.py` & `tdh_twitch_utils-1.7.2/twitch_utils/twitch.py`

 * *Files identical despite different names*


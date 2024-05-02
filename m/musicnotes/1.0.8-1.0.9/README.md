# Comparing `tmp/musicnotes-1.0.8.tar.gz` & `tmp/musicnotes-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicnotes-1.0.8.tar", last modified: Thu May  2 02:35:20 2024, max compression
+gzip compressed data, was "musicnotes-1.0.9.tar", last modified: Thu May  2 02:39:52 2024, max compression
```

## Comparing `musicnotes-1.0.8.tar` & `musicnotes-1.0.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 02:35:20.222208 musicnotes-1.0.8/
--rw-rw-rw-   0        0        0     1132 2024-05-01 23:52:07.000000 musicnotes-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     4161 2024-05-02 02:35:20.220211 musicnotes-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3091 2024-05-02 00:50:49.000000 musicnotes-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 02:35:20.147564 musicnotes-1.0.8/musicnotes/
--rw-rw-rw-   0        0        0       29 2024-05-02 02:08:52.000000 musicnotes-1.0.8/musicnotes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 02:35:20.140045 musicnotes-1.0.8/musicnotes/assets/
-drwxrwxrwx   0        0        0        0 2024-05-02 02:35:20.217209 musicnotes-1.0.8/musicnotes/assets/piano/
--rw-rw-rw-   0        0        0    21509 2024-05-01 19:10:16.000000 musicnotes-1.0.8/musicnotes/assets/piano/highA#piano.mp3
--rw-rw-rw-   0        0        0    25883 2024-05-01 19:11:10.000000 musicnotes-1.0.8/musicnotes/assets/piano/highApiano.mp3
--rw-rw-rw-   0        0        0    23536 2024-05-01 19:11:45.000000 musicnotes-1.0.8/musicnotes/assets/piano/highBpiano.mp3
--rw-rw-rw-   0        0        0    24789 2024-05-01 19:12:24.000000 musicnotes-1.0.8/musicnotes/assets/piano/highC#piano.mp3
--rw-rw-rw-   0        0        0    24060 2024-05-01 19:12:55.000000 musicnotes-1.0.8/musicnotes/assets/piano/highCpiano.mp3
--rw-rw-rw-   0        0        0    25258 2024-05-01 19:13:29.000000 musicnotes-1.0.8/musicnotes/assets/piano/highD#piano.mp3
--rw-rw-rw-   0        0        0    24789 2024-05-01 19:14:36.000000 musicnotes-1.0.8/musicnotes/assets/piano/highDpiano.mp3
--rw-rw-rw-   0        0        0    26456 2024-05-01 19:14:59.000000 musicnotes-1.0.8/musicnotes/assets/piano/highEpiano.mp3
--rw-rw-rw-   0        0        0    25204 2024-05-01 19:15:40.000000 musicnotes-1.0.8/musicnotes/assets/piano/highF#piano.mp3
--rw-rw-rw-   0        0        0    24994 2024-05-01 19:16:09.000000 musicnotes-1.0.8/musicnotes/assets/piano/highFpiano.mp3
--rw-rw-rw-   0        0        0    27558 2024-05-01 19:16:53.000000 musicnotes-1.0.8/musicnotes/assets/piano/highG#piano.mp3
--rw-rw-rw-   0        0        0    24787 2024-05-01 19:17:25.000000 musicnotes-1.0.8/musicnotes/assets/piano/highGpiano.mp3
--rw-rw-rw-   0        0        0    25050 2024-05-01 20:32:07.000000 musicnotes-1.0.8/musicnotes/assets/piano/lowA#piano.mp3
--rw-rw-rw-   0        0        0    33704 2024-05-01 20:32:58.000000 musicnotes-1.0.8/musicnotes/assets/piano/lowApiano.mp3
--rw-rw-rw-   0        0        0    30966 2024-05-01 20:33:22.000000 musicnotes-1.0.8/musicnotes/assets/piano/lowBpiano.mp3
--rw-rw-rw-   0        0        0    33028 2024-05-01 20:34:23.000000 musicnotes-1.0.8/musicnotes/assets/piano/lowC#piano.mp3
--rw-rw-rw-   0        0        0    32768 2024-05-01 20:34:57.000000 musicnotes-1.0.8/musicnotes/assets/piano/lowCpiano.mp3
--rw-rw-rw-   0        0        0    32507 2024-05-01 20:36:28.000000 musicnotes-1.0.8/musicnotes/assets/piano/lowDpiano.mp3
--rw-rw-rw-   0        0        0    34332 2024-05-01 20:36:54.000000 musicnotes-1.0.8/musicnotes/assets/piano/lowEpiano.mp3
--rw-rw-rw-   0        0        0    25884 2024-05-01 20:37:40.000000 musicnotes-1.0.8/musicnotes/assets/piano/lowF#piano.mp3
--rw-rw-rw-   0        0        0    24736 2024-05-01 20:38:10.000000 musicnotes-1.0.8/musicnotes/assets/piano/lowFpiano.mp3
--rw-rw-rw-   0        0        0    25624 2024-05-01 20:38:45.000000 musicnotes-1.0.8/musicnotes/assets/piano/lowG#piano.mp3
--rw-rw-rw-   0        0        0    26455 2024-05-01 20:39:13.000000 musicnotes-1.0.8/musicnotes/assets/piano/lowGpiano.mp3
--rw-rw-rw-   0        0        0    33291 2024-05-01 20:35:54.000000 musicnotes-1.0.8/musicnotes/assets/piano/lowd#piano.mp3
--rw-rw-rw-   0        0        0    17540 2024-05-01 20:39:50.000000 musicnotes-1.0.8/musicnotes/assets/piano/midA#piano.mp3
--rw-rw-rw-   0        0        0    19526 2024-05-01 20:40:19.000000 musicnotes-1.0.8/musicnotes/assets/piano/midApiano.mp3
--rw-rw-rw-   0        0        0    17360 2024-05-01 20:40:47.000000 musicnotes-1.0.8/musicnotes/assets/piano/midBpiano.mp3
--rw-rw-rw-   0        0        0    25363 2024-05-01 20:41:57.000000 musicnotes-1.0.8/musicnotes/assets/piano/midC#piano.mp3
--rw-rw-rw-   0        0        0    18116 2024-05-01 20:42:25.000000 musicnotes-1.0.8/musicnotes/assets/piano/midCpiano.mp3
--rw-rw-rw-   0        0        0    18012 2024-05-01 20:42:51.000000 musicnotes-1.0.8/musicnotes/assets/piano/midD#piano.mp3
--rw-rw-rw-   0        0        0    18586 2024-05-01 20:43:30.000000 musicnotes-1.0.8/musicnotes/assets/piano/midDpiano.mp3
--rw-rw-rw-   0        0        0    17489 2024-05-01 20:44:05.000000 musicnotes-1.0.8/musicnotes/assets/piano/midEpiano.mp3
--rw-rw-rw-   0        0        0    17749 2024-05-01 20:44:36.000000 musicnotes-1.0.8/musicnotes/assets/piano/midF#piano.mp3
--rw-rw-rw-   0        0        0    18116 2024-05-01 20:44:59.000000 musicnotes-1.0.8/musicnotes/assets/piano/midFpiano.mp3
--rw-rw-rw-   0        0        0    18583 2024-05-01 20:45:22.000000 musicnotes-1.0.8/musicnotes/assets/piano/midG#piano.mp3
--rw-rw-rw-   0        0        0    18115 2024-05-01 20:45:56.000000 musicnotes-1.0.8/musicnotes/assets/piano/midGpiano.mp3
--rw-rw-rw-   0        0        0     1211 2024-05-02 02:08:56.000000 musicnotes-1.0.8/musicnotes/musicnotes.py
--rw-rw-rw-   0        0        0     7194 2024-05-02 02:01:15.000000 musicnotes-1.0.8/musicnotes/sound.py
-drwxrwxrwx   0        0        0        0 2024-05-02 02:35:20.219212 musicnotes-1.0.8/musicnotes.egg-info/
--rw-rw-rw-   0        0        0     4161 2024-05-02 02:35:20.000000 musicnotes-1.0.8/musicnotes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1625 2024-05-02 02:35:20.000000 musicnotes-1.0.8/musicnotes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 02:35:20.000000 musicnotes-1.0.8/musicnotes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-02 02:35:20.000000 musicnotes-1.0.8/musicnotes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 02:35:20.223209 musicnotes-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1429 2024-05-02 02:35:04.000000 musicnotes-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 02:39:52.339806 musicnotes-1.0.9/
+-rw-rw-rw-   0        0        0     1132 2024-05-01 23:52:07.000000 musicnotes-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     4161 2024-05-02 02:39:52.337809 musicnotes-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3091 2024-05-02 00:50:49.000000 musicnotes-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 02:39:52.275285 musicnotes-1.0.9/musicnotes/
+-rw-rw-rw-   0        0        0       29 2024-05-02 02:08:52.000000 musicnotes-1.0.9/musicnotes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 02:39:52.269286 musicnotes-1.0.9/musicnotes/assets/
+drwxrwxrwx   0        0        0        0 2024-05-02 02:39:52.335804 musicnotes-1.0.9/musicnotes/assets/piano/
+-rw-rw-rw-   0        0        0    21509 2024-05-01 19:10:16.000000 musicnotes-1.0.9/musicnotes/assets/piano/highA#piano.mp3
+-rw-rw-rw-   0        0        0    25883 2024-05-01 19:11:10.000000 musicnotes-1.0.9/musicnotes/assets/piano/highApiano.mp3
+-rw-rw-rw-   0        0        0    23536 2024-05-01 19:11:45.000000 musicnotes-1.0.9/musicnotes/assets/piano/highBpiano.mp3
+-rw-rw-rw-   0        0        0    24789 2024-05-01 19:12:24.000000 musicnotes-1.0.9/musicnotes/assets/piano/highC#piano.mp3
+-rw-rw-rw-   0        0        0    24060 2024-05-01 19:12:55.000000 musicnotes-1.0.9/musicnotes/assets/piano/highCpiano.mp3
+-rw-rw-rw-   0        0        0    25258 2024-05-01 19:13:29.000000 musicnotes-1.0.9/musicnotes/assets/piano/highD#piano.mp3
+-rw-rw-rw-   0        0        0    24789 2024-05-01 19:14:36.000000 musicnotes-1.0.9/musicnotes/assets/piano/highDpiano.mp3
+-rw-rw-rw-   0        0        0    26456 2024-05-01 19:14:59.000000 musicnotes-1.0.9/musicnotes/assets/piano/highEpiano.mp3
+-rw-rw-rw-   0        0        0    25204 2024-05-01 19:15:40.000000 musicnotes-1.0.9/musicnotes/assets/piano/highF#piano.mp3
+-rw-rw-rw-   0        0        0    24994 2024-05-01 19:16:09.000000 musicnotes-1.0.9/musicnotes/assets/piano/highFpiano.mp3
+-rw-rw-rw-   0        0        0    27558 2024-05-01 19:16:53.000000 musicnotes-1.0.9/musicnotes/assets/piano/highG#piano.mp3
+-rw-rw-rw-   0        0        0    24787 2024-05-01 19:17:25.000000 musicnotes-1.0.9/musicnotes/assets/piano/highGpiano.mp3
+-rw-rw-rw-   0        0        0    25050 2024-05-01 20:32:07.000000 musicnotes-1.0.9/musicnotes/assets/piano/lowA#piano.mp3
+-rw-rw-rw-   0        0        0    33704 2024-05-01 20:32:58.000000 musicnotes-1.0.9/musicnotes/assets/piano/lowApiano.mp3
+-rw-rw-rw-   0        0        0    30966 2024-05-01 20:33:22.000000 musicnotes-1.0.9/musicnotes/assets/piano/lowBpiano.mp3
+-rw-rw-rw-   0        0        0    33028 2024-05-01 20:34:23.000000 musicnotes-1.0.9/musicnotes/assets/piano/lowC#piano.mp3
+-rw-rw-rw-   0        0        0    32768 2024-05-01 20:34:57.000000 musicnotes-1.0.9/musicnotes/assets/piano/lowCpiano.mp3
+-rw-rw-rw-   0        0        0    32507 2024-05-01 20:36:28.000000 musicnotes-1.0.9/musicnotes/assets/piano/lowDpiano.mp3
+-rw-rw-rw-   0        0        0    34332 2024-05-01 20:36:54.000000 musicnotes-1.0.9/musicnotes/assets/piano/lowEpiano.mp3
+-rw-rw-rw-   0        0        0    25884 2024-05-01 20:37:40.000000 musicnotes-1.0.9/musicnotes/assets/piano/lowF#piano.mp3
+-rw-rw-rw-   0        0        0    24736 2024-05-01 20:38:10.000000 musicnotes-1.0.9/musicnotes/assets/piano/lowFpiano.mp3
+-rw-rw-rw-   0        0        0    25624 2024-05-01 20:38:45.000000 musicnotes-1.0.9/musicnotes/assets/piano/lowG#piano.mp3
+-rw-rw-rw-   0        0        0    26455 2024-05-01 20:39:13.000000 musicnotes-1.0.9/musicnotes/assets/piano/lowGpiano.mp3
+-rw-rw-rw-   0        0        0    33291 2024-05-01 20:35:54.000000 musicnotes-1.0.9/musicnotes/assets/piano/lowd#piano.mp3
+-rw-rw-rw-   0        0        0    17540 2024-05-01 20:39:50.000000 musicnotes-1.0.9/musicnotes/assets/piano/midA#piano.mp3
+-rw-rw-rw-   0        0        0    19526 2024-05-01 20:40:19.000000 musicnotes-1.0.9/musicnotes/assets/piano/midApiano.mp3
+-rw-rw-rw-   0        0        0    17360 2024-05-01 20:40:47.000000 musicnotes-1.0.9/musicnotes/assets/piano/midBpiano.mp3
+-rw-rw-rw-   0        0        0    25363 2024-05-01 20:41:57.000000 musicnotes-1.0.9/musicnotes/assets/piano/midC#piano.mp3
+-rw-rw-rw-   0        0        0    18116 2024-05-01 20:42:25.000000 musicnotes-1.0.9/musicnotes/assets/piano/midCpiano.mp3
+-rw-rw-rw-   0        0        0    18012 2024-05-01 20:42:51.000000 musicnotes-1.0.9/musicnotes/assets/piano/midD#piano.mp3
+-rw-rw-rw-   0        0        0    18586 2024-05-01 20:43:30.000000 musicnotes-1.0.9/musicnotes/assets/piano/midDpiano.mp3
+-rw-rw-rw-   0        0        0    17489 2024-05-01 20:44:05.000000 musicnotes-1.0.9/musicnotes/assets/piano/midEpiano.mp3
+-rw-rw-rw-   0        0        0    17749 2024-05-01 20:44:36.000000 musicnotes-1.0.9/musicnotes/assets/piano/midF#piano.mp3
+-rw-rw-rw-   0        0        0    18116 2024-05-01 20:44:59.000000 musicnotes-1.0.9/musicnotes/assets/piano/midFpiano.mp3
+-rw-rw-rw-   0        0        0    18583 2024-05-01 20:45:22.000000 musicnotes-1.0.9/musicnotes/assets/piano/midG#piano.mp3
+-rw-rw-rw-   0        0        0    18115 2024-05-01 20:45:56.000000 musicnotes-1.0.9/musicnotes/assets/piano/midGpiano.mp3
+-rw-rw-rw-   0        0        0     1238 2024-05-02 02:39:08.000000 musicnotes-1.0.9/musicnotes/musicnotes.py
+-rw-rw-rw-   0        0        0     7194 2024-05-02 02:01:15.000000 musicnotes-1.0.9/musicnotes/sound.py
+drwxrwxrwx   0        0        0        0 2024-05-02 02:39:52.336805 musicnotes-1.0.9/musicnotes.egg-info/
+-rw-rw-rw-   0        0        0     4161 2024-05-02 02:39:52.000000 musicnotes-1.0.9/musicnotes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1625 2024-05-02 02:39:52.000000 musicnotes-1.0.9/musicnotes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 02:39:52.000000 musicnotes-1.0.9/musicnotes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-02 02:39:52.000000 musicnotes-1.0.9/musicnotes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 02:39:52.339806 musicnotes-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1429 2024-05-02 02:39:34.000000 musicnotes-1.0.9/setup.py
```

### Comparing `musicnotes-1.0.8/LICENSE` & `musicnotes-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/PKG-INFO` & `musicnotes-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicnotes
-Version: 1.0.8
+Version: 1.0.9
 Summary: Play music notes in your Python scripts with ease.
 Home-page: https://github.com/must108/musicnotes
 Author: Mustaeen Ahmed
 Author-email: contact@mustaeen.dev
 License: MIT
 Keywords: sound,music,mp3,wave,wav,media,song,play,audio,notes,music notes,melody
 Classifier: Intended Audience :: Developers
```

### Comparing `musicnotes-1.0.8/README.md` & `musicnotes-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/highA#piano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/highA#piano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/highApiano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/highApiano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/highBpiano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/highBpiano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/highC#piano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/highC#piano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/highCpiano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/highCpiano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/highD#piano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/highD#piano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/highDpiano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/highDpiano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/highEpiano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/highEpiano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/highF#piano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/highF#piano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/highFpiano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/highFpiano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/highG#piano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/highG#piano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/highGpiano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/highGpiano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/lowA#piano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/lowA#piano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/lowApiano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/lowApiano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/lowBpiano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/lowBpiano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/lowC#piano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/lowC#piano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/lowCpiano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/lowCpiano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/lowDpiano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/lowDpiano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/lowEpiano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/lowEpiano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/lowF#piano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/lowF#piano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/lowFpiano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/lowFpiano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/lowG#piano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/lowG#piano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/lowGpiano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/lowGpiano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/lowd#piano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/lowd#piano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/midA#piano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/midA#piano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/midApiano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/midApiano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/midBpiano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/midBpiano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/midC#piano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/midC#piano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/midCpiano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/midCpiano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/midD#piano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/midD#piano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/midDpiano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/midDpiano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/midEpiano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/midEpiano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/midF#piano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/midF#piano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/midFpiano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/midFpiano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/midG#piano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/midG#piano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/assets/piano/midGpiano.mp3` & `musicnotes-1.0.9/musicnotes/assets/piano/midGpiano.mp3`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes/musicnotes.py` & `musicnotes-1.0.9/musicnotes/musicnotes.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,12 +22,12 @@
                 
             play(note, pitch, '#')
         else:
             play(note, pitch)
             
 def play(note, pitch, sym = ''): # for drier code
     if pitch == 'low':
-        soundPlayer('./assets/piano/' + 'low' + note + sym + 'piano.mp3', block = True)
+        soundPlayer('musicnotes/assets/piano/' + 'low' + note + sym + 'piano.mp3', block = True)
     elif pitch == 'mid':
-        soundPlayer('./assets/piano/' + 'mid' + note + sym + 'piano.mp3', block = True)
+        soundPlayer('musicnotes/assets/piano/' + 'mid' + note + sym + 'piano.mp3', block = True)
     elif pitch == 'high':
-        soundPlayer('./assets/piano/' + 'high' + note + sym + 'piano.mp3', block = True)
+        soundPlayer('musicnotes/assets/piano/' + 'high' + note + sym + 'piano.mp3', block = True)
```

### Comparing `musicnotes-1.0.8/musicnotes/sound.py` & `musicnotes-1.0.9/musicnotes/sound.py`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/musicnotes.egg-info/PKG-INFO` & `musicnotes-1.0.9/musicnotes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicnotes
-Version: 1.0.8
+Version: 1.0.9
 Summary: Play music notes in your Python scripts with ease.
 Home-page: https://github.com/must108/musicnotes
 Author: Mustaeen Ahmed
 Author-email: contact@mustaeen.dev
 License: MIT
 Keywords: sound,music,mp3,wave,wav,media,song,play,audio,notes,music notes,melody
 Classifier: Intended Audience :: Developers
```

### Comparing `musicnotes-1.0.8/musicnotes.egg-info/SOURCES.txt` & `musicnotes-1.0.9/musicnotes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.8/setup.py` & `musicnotes-1.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', encoding = 'utf-8') as f:
     long_description = f.read()
 
 setup (
     name = 'musicnotes',
-    version = '1.0.8',
+    version = '1.0.9',
     description = 'Play music notes in your Python scripts with ease.',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/must108/musicnotes',
     author = 'Mustaeen Ahmed',
     author_email = 'contact@mustaeen.dev',
     license = 'MIT',
```


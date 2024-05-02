# Comparing `tmp/musicnotes-1.0.5.tar.gz` & `tmp/musicnotes-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicnotes-1.0.5.tar", last modified: Thu May  2 02:09:25 2024, max compression
+gzip compressed data, was "musicnotes-1.0.6.tar", last modified: Thu May  2 02:14:47 2024, max compression
```

## Comparing `musicnotes-1.0.5.tar` & `musicnotes-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 02:09:25.758968 musicnotes-1.0.5/
--rw-rw-rw-   0        0        0     1132 2024-05-01 23:52:07.000000 musicnotes-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     4161 2024-05-02 02:09:25.756971 musicnotes-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3091 2024-05-02 00:50:49.000000 musicnotes-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 02:09:25.749452 musicnotes-1.0.5/musicnotes/
--rw-rw-rw-   0        0        0       29 2024-05-02 02:08:52.000000 musicnotes-1.0.5/musicnotes/__init__.py
--rw-rw-rw-   0        0        0     1211 2024-05-02 02:08:56.000000 musicnotes-1.0.5/musicnotes/musicnotes.py
--rw-rw-rw-   0        0        0     7194 2024-05-02 02:01:15.000000 musicnotes-1.0.5/musicnotes/sound.py
-drwxrwxrwx   0        0        0        0 2024-05-02 02:09:25.755971 musicnotes-1.0.5/musicnotes.egg-info/
--rw-rw-rw-   0        0        0     4161 2024-05-02 02:09:25.000000 musicnotes-1.0.5/musicnotes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2024-05-02 02:09:25.000000 musicnotes-1.0.5/musicnotes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 02:09:25.000000 musicnotes-1.0.5/musicnotes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-02 02:09:25.000000 musicnotes-1.0.5/musicnotes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 02:09:25.759967 musicnotes-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1351 2024-05-02 02:09:09.000000 musicnotes-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 02:14:47.503848 musicnotes-1.0.6/
+-rw-rw-rw-   0        0        0     1132 2024-05-01 23:52:07.000000 musicnotes-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     4161 2024-05-02 02:14:47.501853 musicnotes-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3091 2024-05-02 00:50:49.000000 musicnotes-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 02:14:47.495109 musicnotes-1.0.6/musicnotes/
+-rw-rw-rw-   0        0        0       29 2024-05-02 02:08:52.000000 musicnotes-1.0.6/musicnotes/__init__.py
+-rw-rw-rw-   0        0        0     1211 2024-05-02 02:08:56.000000 musicnotes-1.0.6/musicnotes/musicnotes.py
+-rw-rw-rw-   0        0        0     7194 2024-05-02 02:01:15.000000 musicnotes-1.0.6/musicnotes/sound.py
+drwxrwxrwx   0        0        0        0 2024-05-02 02:14:47.500850 musicnotes-1.0.6/musicnotes.egg-info/
+-rw-rw-rw-   0        0        0     4161 2024-05-02 02:14:47.000000 musicnotes-1.0.6/musicnotes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2024-05-02 02:14:47.000000 musicnotes-1.0.6/musicnotes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 02:14:47.000000 musicnotes-1.0.6/musicnotes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-02 02:14:47.000000 musicnotes-1.0.6/musicnotes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 02:14:47.503848 musicnotes-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1422 2024-05-02 02:14:32.000000 musicnotes-1.0.6/setup.py
```

### Comparing `musicnotes-1.0.5/LICENSE` & `musicnotes-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.5/PKG-INFO` & `musicnotes-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicnotes
-Version: 1.0.5
+Version: 1.0.6
 Summary: Play music notes in your Python scripts with ease.
 Home-page: https://github.com/must108/musicnotes
 Author: Mustaeen Ahmed
 Author-email: contact@mustaeen.dev
 License: MIT
 Keywords: sound,music,mp3,wave,wav,media,song,play,audio,notes,music notes,melody
 Classifier: Intended Audience :: Developers
```

### Comparing `musicnotes-1.0.5/README.md` & `musicnotes-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.5/musicnotes/musicnotes.py` & `musicnotes-1.0.6/musicnotes/musicnotes.py`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.5/musicnotes/sound.py` & `musicnotes-1.0.6/musicnotes/sound.py`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.5/musicnotes.egg-info/PKG-INFO` & `musicnotes-1.0.6/musicnotes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicnotes
-Version: 1.0.5
+Version: 1.0.6
 Summary: Play music notes in your Python scripts with ease.
 Home-page: https://github.com/must108/musicnotes
 Author: Mustaeen Ahmed
 Author-email: contact@mustaeen.dev
 License: MIT
 Keywords: sound,music,mp3,wave,wav,media,song,play,audio,notes,music notes,melody
 Classifier: Intended Audience :: Developers
```

### Comparing `musicnotes-1.0.5/setup.py` & `musicnotes-1.0.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', encoding = 'utf-8') as f:
     long_description = f.read()
 
 setup (
     name = 'musicnotes',
-    version = '1.0.5',
+    version = '1.0.6',
     description = 'Play music notes in your Python scripts with ease.',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/must108/musicnotes',
     author = 'Mustaeen Ahmed',
     author_email = 'contact@mustaeen.dev',
     license = 'MIT',
@@ -25,9 +25,12 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',   
         'Topic :: Multimedia :: Sound/Audio :: MIDI',
         'Topic :: Multimedia :: Sound/Audio :: Players',
         'Topic :: Multimedia :: Sound/Audio :: Players :: MP3',
     ],
-    packages = ['musicnotes']
+    packages = ['musicnotes'],
+    package_data = {
+        'musicnotes': ['media/*.mp3'],
+    },
 )
```


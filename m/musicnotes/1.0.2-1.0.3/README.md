# Comparing `tmp/musicnotes-1.0.2.tar.gz` & `tmp/musicnotes-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicnotes-1.0.2.tar", last modified: Thu May  2 01:22:47 2024, max compression
+gzip compressed data, was "musicnotes-1.0.3.tar", last modified: Thu May  2 01:48:37 2024, max compression
```

## Comparing `musicnotes-1.0.2.tar` & `musicnotes-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 01:22:47.676878 musicnotes-1.0.2/
--rw-rw-rw-   0        0        0     1132 2024-05-01 23:52:07.000000 musicnotes-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     4686 2024-05-02 01:22:47.674366 musicnotes-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3091 2024-05-02 00:50:49.000000 musicnotes-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 01:22:47.669490 musicnotes-1.0.2/musicnotes.egg-info/
--rw-rw-rw-   0        0        0     4686 2024-05-02 01:22:47.000000 musicnotes-1.0.2/musicnotes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2024-05-02 01:22:47.000000 musicnotes-1.0.2/musicnotes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 01:22:47.000000 musicnotes-1.0.2/musicnotes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-02 01:22:47.000000 musicnotes-1.0.2/musicnotes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1210 2024-05-02 00:00:06.000000 musicnotes-1.0.2/musicnotes.py
--rw-rw-rw-   0        0        0       42 2024-05-02 01:22:47.676878 musicnotes-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1939 2024-05-02 01:21:38.000000 musicnotes-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 01:48:37.614380 musicnotes-1.0.3/
+-rw-rw-rw-   0        0        0     1132 2024-05-01 23:52:07.000000 musicnotes-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4686 2024-05-02 01:48:36.976807 musicnotes-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3091 2024-05-02 00:50:49.000000 musicnotes-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 01:48:36.975808 musicnotes-1.0.3/musicnotes.egg-info/
+-rw-rw-rw-   0        0        0     4686 2024-05-02 01:48:36.000000 musicnotes-1.0.3/musicnotes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2024-05-02 01:48:36.000000 musicnotes-1.0.3/musicnotes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 01:48:36.000000 musicnotes-1.0.3/musicnotes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-02 01:48:36.000000 musicnotes-1.0.3/musicnotes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1210 2024-05-02 00:00:06.000000 musicnotes-1.0.3/musicnotes.py
+-rw-rw-rw-   0        0        0       42 2024-05-02 01:48:37.615383 musicnotes-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1939 2024-05-02 01:48:31.000000 musicnotes-1.0.3/setup.py
```

### Comparing `musicnotes-1.0.2/LICENSE` & `musicnotes-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.2/PKG-INFO` & `musicnotes-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicnotes
-Version: 1.0.2
+Version: 1.0.3
 Summary: Play music notes in your Python scripts with ease.
 Home-page: https://github.com/must108/musicnotes
 Author: Mustaeen Ahmed
 Author-email: contact@mustaeen.dev
 License: MIT
 Keywords: sound,music,mp3,wave,wav,media,song,play,audio,notes,music notes,melody
 Classifier: Intended Audience :: Developers
```

### Comparing `musicnotes-1.0.2/README.md` & `musicnotes-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.2/musicnotes.egg-info/PKG-INFO` & `musicnotes-1.0.3/musicnotes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicnotes
-Version: 1.0.2
+Version: 1.0.3
 Summary: Play music notes in your Python scripts with ease.
 Home-page: https://github.com/must108/musicnotes
 Author: Mustaeen Ahmed
 Author-email: contact@mustaeen.dev
 License: MIT
 Keywords: sound,music,mp3,wave,wav,media,song,play,audio,notes,music notes,melody
 Classifier: Intended Audience :: Developers
```

### Comparing `musicnotes-1.0.2/musicnotes.py` & `musicnotes-1.0.3/musicnotes.py`

 * *Files identical despite different names*

### Comparing `musicnotes-1.0.2/setup.py` & `musicnotes-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = abspath(dirname(getsource(lambda: 0)))
 
 with open(join(here, 'README.md'), encoding = 'utf-8') as f:
     desc = f.read()
 
 setup (
     name = 'musicnotes',
-    version = '1.0.2',
+    version = '1.0.3',
     description = 'Play music notes in your Python scripts with ease.',
     long_description = desc,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/must108/musicnotes',
     author = 'Mustaeen Ahmed',
     author_email = 'contact@mustaeen.dev',
     license = 'MIT',
```

